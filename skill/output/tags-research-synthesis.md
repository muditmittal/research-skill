# Research: Tags in Databricks — Deep Dive Across 8 Subtopics for Governance Hub Design

**2026-03-17 · Full Coverage · 10 agents consulted**

```
/research We have Tags that are account level concept, but they live
in Workspace UI today. We want to make them available at Account level
in the new GovHub which is being built to serve account-level needs
and it sits inside of Account Console.

Help me understand everything related to Tags feature, its usage by
customers, feature plans, what users like about them and what they
complain about. What are things we can possibly improve in the short term.

I want to leverage this research to figure out where we can take Tags
in the long term and build a perspective on how Tags would be similar
or different than Domains which are also built on the same tags foundation.

Subtopics: 1. discovery vs governed, 2. system vs customer-defined,
3. Tag propagation, 4. Tag inheritance, 5. Required tags, 6. Tags vs
Domains, 7. Tag permissions, 8. Data Tags vs Cost Tags.
```

---

## Executive Summary

**Tags are Databricks' most cross-cutting governance primitive — touching access control, cost management, compliance, discovery, and now AI grounding — yet they suffer from a fragmented architecture, an authoring bottleneck, and an identity crisis between discovery and governance.**

The data tells a clear story: 29% of workspaces use tags, with **97% of traffic being reads and only 91 workspaces writing any tags** out of 1,695 active. Tags are consumed broadly but authored by almost nobody. This 37:1 read-to-write ratio — and the fact that **94.6% of tag-using workspaces never write a single tag** — signals that the authoring UX is the bottleneck, not demand. Meanwhile, **131.6M tag assignments exist** across metastores (32.7M securable-level + 98.8M column-level), confirming tags are a foundational primitive at massive scale.

Three major inflections are happening simultaneously: **(1) Governed Tags GA** (mid-March 2026, bundled with ABAC + PII Classification), **(2) "Unified Tagging" as an FY27 Big Rock** ("tag as a primitive" for all Databricks products), and **(3) Account-level tag management in Governance Hub** (targeting DAIS, May 2026). Meanwhile, **Snowflake shipped automatic tag propagation through lineage in May 2025** — a capability Databricks has in development but hasn't shipped.

**The eight subtopics resolve as follows:**

1. **Discovery vs Governed** — Two tiers are the right model (industry consensus). Visual differentiation (lock icon + restricted palette for governed) rather than separate surfaces.
2. **System vs Customer-Defined** — System tags need distinct visual treatment (Databricks badge) and must be excluded from customer-facing admin views (Gov Hub PRD already flags this).
3. **Tag Propagation** — Opt-in propagation is the right default (Foundations agent). Sensitivity/governance tags should propagate; discovery tags should not. PRD exists, Jira EDC-913 in progress.
4. **Tag Inheritance** — Currently ABAC-only and never reaches columns. Literature says: parent-to-child default, explicit override breaks the chain, warn users when overriding.
5. **Required Tags** — Strong customer demand (GDPR compliance, cost allocation). Databricks is first to support required tags on data assets natively via Tag Policies. Keep mandatory set minimal (sensitivity + ownership).
6. **Tags vs Domains** — Domains ARE governed tags with special UI. Tags are cross-cutting facets; domains are structural hierarchy. Don't nest tags inside domains.
7. **Tag Permissions** — Two-layer model (object-level APPLY TAG + governed-tag-level ASSIGN). ES tickets show intermittent PERMISSION_DENIED bugs via dbt. Nike wants fine-grained control.
8. **Data Tags vs Cost Tags** — Two separate systems today (UC tags vs compute/billing tags). Convergence planned but not shipped. 8 customers left serverless preview over this gap.

**Confidence: High.** 10 of 10 agents returned substantive findings. Quantitative data, internal PRDs, competitive analysis, standards, and field signal all converge.

---

## Coverage Confidence

**Coverage: Full** — 10 of 10 agents returned substantive findings.

| Agent | Confidence | Key contribution |
|-------|------------|-----------------|
| Official Docs | High | Complete capability inventory, all 8 subtopics from docs, limits and gaps |
| Community Voice | Medium | IaC/programmatic tagging pain, orphaned tags, tag inconsistency at scale |
| Internal Intel | High | 7+ PRDs, ES tickets, customer notes, Sev0 tag search bug, 30 internal docs |
| Quantitative | High | 30% adoption, 79/21 read/write split, 49 write workspaces, 1.2M tag capsule clicks |
| Competitive | High | 8-dimension matrix across 7 competitors, Snowflake lineage propagation advantage |
| Product Design | High | 5 interaction patterns, Snowflake lineage tag UX benchmark, ABAC sentence builder |
| Roadmap | High | Governed Tags GA imminent, Unified Tagging FY27 Big Rock, DAIS Gov Hub target |
| Foundations | Medium-High | Hybrid taxonomy model, SKOS standard, opt-in propagation, minimal mandatory tags |
| Sales & GTM | Medium | 8 customers left serverless preview, Tag Policies P1, Purview sync blocker |
| Market Landscape | High | AI classification trend, regulatory drivers, cost tag convergence, buy-over-build |

**Dimension gaps:** None.

---

## Key Themes

### Theme 1: Tags have an authoring crisis — consumed by many, created by almost nobody

The quantitative data is unambiguous:

- **1,695 workspaces** have tag API traffic (29% of all workspaces) [Quantitative — verified]
- **97.4% of tag transactions are reads**, 2.6% writes — a 37:1 ratio [Quantitative — corrected from earlier 79/21 claim which included false-positive staging RPCs]
- **Only 91 workspaces** write any tags (49 column-level, 71 table-level, with overlap) [Quantitative — verified]
- **94.6% of tag-using workspaces are read-only** — they never write a single tag [Quantitative — corrected from earlier 46% claim]
- **131.6M tag assignments exist** across metastores (32.7M securable-level + 98.8M column-level) [Quantitative — new finding]
- **142K "add tag" button clicks** per month in UI — the actual human authoring signal [Quantitative — new finding]
- **200K governance tag page visits** per month [Quantitative — verified]

Internal Intel confirms: "Tags are mandatory for all objects to make it easier for GDPR auditing" (customer notes), but the tooling for tag creation is SQL-only or API-only for governed tags. Community Voice adds: Terraform users waited over a year for tag support; DAB tagging for schemas/volumes is still an open request.

**Design implication:** The #1 short-term improvement is making tag authoring dramatically easier — bulk tagging UI, AI-suggested tags, and better IaC support. The consumption experience is already working (200K page views/month); the production side is broken. The 8.67% error rate on column-level tag writes (`UpdateTagSubentityAssignments`) means nearly 1 in 11 write attempts fails — a usability signal worth investigating.

### Theme 2: Three systems masquerading as one — UC tags, cost tags, and system tags need unification

Today, Databricks has three separate tag systems:

| System | Attached to | Stored in | Used for |
|--------|------------|-----------|----------|
| UC tags (standard + governed) | Data assets (catalogs, schemas, tables, columns) | Unity Catalog metadata | Discovery, classification, ABAC |
| Compute/billing tags | Clusters, SQL warehouses, jobs, serverless workloads | system.billing.usage | Cost attribution, chargeback, budgets |
| System tags | UC assets (predefined by Databricks) | Unity Catalog metadata | Data classification (PII), certification, deprecation |

These systems have different limits (50 UC tags per object vs 20 compute tags), different character restrictions, different propagation rules, and different APIs. [Official Docs]

The "Unified Tagging" FY27 Big Rock aims to resolve this: "tag as a primitive to support various tag-like products across Databricks." [Roadmap] But today, customers wanting end-to-end governance (tag a table as `cost_center=marketing` AND have that flow to billing) must navigate both systems. **8 customers left the serverless preview** because they couldn't enforce cost tags. [Sales & GTM]

**Design implication:** The Governance Hub should present a unified tag management surface even if the underlying systems remain separate for now. Users should not need to know which tag system they're interacting with.

### Theme 3: Tag propagation is the most-requested missing capability — and Snowflake already shipped it

Multiple independent signals converge:

- **65 Aha! votes** for tag propagation [Roadmap]
- **Dedicated PRD** exists: "[PRD] Tag Propagation for UC tables" [Internal Intel]
- **Jira EDC-913** actively in progress; aligned with Matei and leadership [Roadmap]
- **Snowflake shipped automatic tag propagation through lineage in May 2025** — tags auto-apply to CTAS, views, materialized views [Competitive]
- **Customer YipitData** specifically asked for "tag inheritance across workflows (bronze-to-gold)" [Internal Intel]
- **Foundations literature**: propagation should be opt-in, not automatic; governance tags should propagate, discovery tags should not; transformation-aware propagation is unsolved [Foundations]

**Design implication:** Tag propagation is the highest-impact feature to ship alongside the Governance Hub. The design should follow the opt-in model: admins configure which governed tags propagate, with visual indicators in lineage views showing propagated vs directly-applied tags (Snowflake's dashed/yellow border pattern).

### Theme 4: Domains ARE governed tags — but users won't understand this without careful IA

The internal architecture is clear: "We will reuse existing Governed Tags and create a Domain management console that can direct which Governed Tags are Domains. Governed Tags marked as Domains will receive unique UI treatment." [Internal Intel, Roadmap]

But from a user mental model perspective, tags and domains serve fundamentally different purposes:

| | Tags | Domains |
|---|---|---|
| **Purpose** | Cross-cutting classification (sensitivity, cost center, data quality tier) | Business-aligned ownership grouping (Marketing Data, Finance Data) |
| **Cardinality** | Many tags per asset | One primary domain per asset |
| **Access control** | Drive ABAC policies | No access control function |
| **Navigation** | Filter/facet | Browse hierarchy |
| **Foundation** | Standard: Tags = any key-value; Governed: Tags = controlled vocabulary | Governed tags with special UI designation |

Foundations literature supports this separation: "hierarchy for governance/browsing (domains), flat tags for cross-cutting concerns (tags)" [Foundations]. Product Design concurs: "Do NOT nest tags inside domains — allow tags to be scoped via configuration." [Product Design]

**Design implication:** In the Governance Hub, domains and tags should be sibling concepts in the navigation — not nested. The fact that domains are implemented as governed tags is an implementation detail that should be invisible to users.

---

## Subtopic Deep Dives

### Subtopic 1: Discovery Tags vs Governed Tags

**Current state:** Two tiers exist. Standard (discovery) tags are free-form key-value pairs any user with `APPLY TAG` can set. Governed tags have tag policies with restricted values, permission controls, and ABAC integration. Governed tags GA mid-March 2026. [Official Docs]

**Competitive context:** Two-tier systems are the emerging enterprise standard — Snowflake (object tags + classification tags), Purview (sensitivity labels + enterprise keywords), Atlan (classifications + tags), Collibra (classifications + tags). [Competitive]

**What the literature says:** Hybrid model (controlled vocabulary backbone + folksonomy intake) is the consensus best practice. Users should be able to suggest tags that get promoted into the governed vocabulary through a review process. [Foundations]

**Community signal:** No widespread confusion yet (governed tags still in preview), but the risk grows as adoption increases. One Medium author noted the "engineering" vs "eng" problem — exactly what governed tags solve. [Community Voice]

**Design recommendation:** Visually differentiate with a lock icon for governed tags and an open tag icon for discovery tags. In typeahead, show governed tags first with a "Governed" badge. Allow discovery tags to be "promoted" to governed through a steward workflow.

### Subtopic 2: System Tags vs Customer-Defined Tags

**Current state:** System tags are a special subset of governed tags predefined by Databricks (wrench icon). Keys and values cannot be modified or deleted. Used primarily for automated data classification (`class.*` tags). Customer-defined governed tags appear with a lock icon. [Official Docs]

**Known issue:** Gov Hub PRD flags: "Need to exclude system tags (LakehouseMonitoringId) from custom_tag Account-view" — system tags pollute customer-facing views. [Internal Intel]

**Design recommendation:** Three-tier visual treatment: (1) system tags with Databricks logo badge (immutable, auto-applied), (2) customer governed tags with lock icon (admin-controlled), (3) discovery tags with open tag icon (user-created). System tags should be filterable/hideable in admin views.

### Subtopic 3: Tag Propagation

**Current state:** Tags do NOT physically propagate to child or downstream objects. ABAC policy evaluation performs runtime inheritance (catalog/schema tags apply to children), but this is not visible in INFORMATION_SCHEMA or search. Lineage-based propagation is not shipped. [Official Docs]

**In development:** Tag Propagation PRD exists. Jira EDC-913 in progress. Lineage-based propagation (DDISC-8765) is open but not started. [Roadmap]

**Competitive benchmark:** Snowflake shipped automatic tag propagation through lineage in May 2025 — tags auto-apply to CTAS, views, materialized views with ON_CONFLICT collision handling. [Competitive]

**What the literature says:** Propagation should be opt-in. Governance/sensitivity tags should propagate; discovery tags should not. Transformation-aware propagation (knowing when PII is removed by aggregation) is unsolved. Deletion should cascade. [Foundations]

**Customer demand:** YipitData wants bronze-to-gold propagation. Data Classification team wants propagation for `class.*` tags (XTA-10920). [Internal Intel]

**Design recommendation:** Per-tag propagation toggle in governed tag settings ("Propagate this tag through lineage: On/Off"). Visual indicators in lineage view: solid badge = directly applied, dashed badge = propagated. Override option: "This asset inherited tag X from [source] — Keep / Remove."

### Subtopic 4: Tag Inheritance

**Current state:** "Implicit tag inheritance occurs when evaluating ABAC policies only. Tag inheritance doesn't apply generally." Catalog/schema tags inherit to children for ABAC. Never inherits to columns. [Official Docs]

**What the literature says:** Inheritance flows downward by default. Override stops the chain. Explicit overrides should warn users. Not all metadata should inherit — governance tags yes, discovery tags no. [Foundations]

**Customer feedback:** YipitData wants catalog/schema-level tags to appear on all children. The current ABAC-only inheritance is confusing — users expect tags set on a catalog to be visible on its tables in search and INFORMATION_SCHEMA. [Internal Intel]

**Design recommendation:** Expand inheritance beyond ABAC. When a governed tag is set on a catalog or schema, it should be visible (as "inherited") on child objects in Catalog Explorer and INFORMATION_SCHEMA. Use visual distinction: "Inherited from [parent]" badge. Allow override at child level with a warning.

### Subtopic 5: Required Tags

**Current state:** No native support for mandatory tags on UC data assets. Required tagging exists only for compute resources (cluster policies, AWS IAM, serverless budget policies). Tag Policies (Private Preview, targeting DAIS) will add enforcement. [Official Docs, Roadmap]

**Customer demand:** "Tags are mandatory for all objects to make it easier for GDPR auditing" (customer notes). 8 customers left serverless preview over missing tag enforcement. "Customers expect every query to carry required tags (e.g., cost center)." [Internal Intel, Sales & GTM]

**Competitive context:** Databricks will be first to support required tags on data assets natively. Snowflake lacks this. AWS (SCPs + Tag Policies) and Azure (Azure Policy with Deny/Modify) support it at infra level. Purview uses mandatory sensitivity labels. [Competitive]

**What the literature says:** Keep mandatory tags minimal — sensitivity + ownership at creation. Seamless UX is the #1 adoption factor. Use default values and grace periods rather than hard blocks at creation. [Foundations]

**Design recommendation:** Required tags should appear inline during asset creation (not as a post-creation gate). Provide default values for common required tags. Allow a grace period option: "Tag within 7 days" with escalating reminders rather than hard blocks. Start with 2-3 required tags maximum.

### Subtopic 6: Tags vs Domains

**Current state:** Domains are governed tags with special UI designation. Domains provide business-aligned discovery grouping (cross-catalog). Tags provide granular key-value classification for search, ABAC, and cost. Domains do not drive access control. [Official Docs, Roadmap]

**Internal architecture:** "[PRD] Domains: Using Governed Tags for Business-Centric Data Discovery" — assigning to a domain requires ASSIGN TAG + APPLY TAG permissions. Domains get unique treatment in Discover page, Search, Catalog Explorer. [Internal Intel]

**Design recommendation:** Present as sibling navigation items in Governance Hub ("Tags" and "Domains" as separate sections). The underlying governed tag implementation is invisible to users. Domains appear in left-nav/breadcrumbs as the structural hierarchy. Tags appear as cross-cutting facets in search/filter.

### Subtopic 7: Tag Permissions

**Current state:** Two-layer model. Object level: `APPLY TAG` + `USE SCHEMA` + `USE CATALOG`. Governed tag level: `CREATE`, `MANAGE`, `ASSIGN` at account or individual tag scope. [Official Docs]

**Known issues:** ES-1727597 (Avant) — intermittent PERMISSION_DENIED errors when dbt runs ALTER TABLE SET TAGS for governed tags. Nike wants "ability to control which users or groups have permissions to apply/remove a specific tag assignment." [Internal Intel]

**Competitive context:** Snowflake centralizes with TAG_ADMIN role. AWS LF delegates tag creation. Purview scopes via label policies. [Competitive]

**Design recommendation:** Permission management should be part of the governed tag definition flow in Governance Hub (not a separate surface). When creating a governed tag, the admin sets: allowed values, who can assign, and which assets it applies to — all in one flow.

### Subtopic 8: Data Tags vs Cost Tags

**Current state:** Two separate systems. UC governed tags on data assets; custom/usage tags on compute resources. Different limits (50 vs 20), different character restrictions, different APIs, different propagation. Convergence planned ("governed tags will integrate with serverless budget policies") but not shipped. [Official Docs]

**Customer impact:** 8 customers left serverless preview. Finance teams require tag-based chargeback as a prerequisite for serverless adoption. [Sales & GTM]

**Roadmap:** "Unified Tagging" FY27 Big Rock. Tag syntax change CM doc filed to allow ":" in tag keys (unification step). Query Tags PRD mentions future integration. [Roadmap, Internal Intel]

**Design recommendation:** In the Governance Hub, present cost and data tags in a unified view with a "Type" filter (Governance / Cost / System). Behind the scenes, bridge the systems via the Unified Tagging initiative. Short-term: surface cost tag usage alongside UC tag usage in the Gov Hub dashboard.

---

## Conflicts Resolved

| Conflict | Agent A | Agent B | Resolution |
|----------|---------|---------|------------|
| Should tags auto-propagate? | Community Voice: users want automatic propagation | Foundations: propagation should be opt-in | **Opt-in is correct** (trust hierarchy: standards > community requests). Auto-propagation causes metadata sprawl. Per-tag toggle is the right UX. |
| Required tags: hard block or grace period? | Sales & GTM: customers want enforcement (8 left preview) | Foundations: seamless UX is #1 factor; use defaults and grace periods | **Both are right for different contexts.** Cost tags on compute = hard block (finance needs it). Governance tags on data assets = grace period with escalation. Let admins configure per-tag. |
| Tag inheritance: ABAC-only or general? | Official Docs: inheritance is ABAC-only today | Customer notes: expect catalog tags visible on child tables | **General inheritance is the right direction** (Quantitative data: users browse 72.5M table views/month and expect to see inherited context). ABAC-only is a V1 limitation, not a design choice. |
| Domains: same as tags or different concept? | Roadmap/Internal Intel: domains ARE governed tags technically | Product Design/Foundations: domains and tags serve different user needs | **Present as different concepts, share the infrastructure.** Users need structural hierarchy (domains) AND cross-cutting facets (tags). Implementation detail ≠ user model. |

---

## Gaps That Remain

1. **No UXR study on tag authoring friction.** We know 46% of tag-using workspaces never write — but we don't know why. Is it permissions? UX? Lack of awareness? Need user research. [Internal Intel]
2. **No tag coverage metrics.** We can count API calls but not "% of assets with at least one tag" or "% of assets with all required tags." This metric is essential for the Gov Hub dashboard. [Quantitative]
3. **Transformation-aware propagation is unsolved.** When a PII column is aggregated (removing PII), should the PII tag propagate to the aggregate table? No platform has solved this. [Foundations]
4. **Cross-platform tag interop undefined.** How do tags translate when data moves between Databricks, Snowflake, and Purview? Philips 66 specifically needs UC ↔ Purview tag sync. [Sales & GTM, Competitive]
5. **Ideas Portal vote counts inaccessible.** Cannot quantify community demand for specific tag features. [Community Voice]
6. **AI classification accuracy benchmarks missing.** No independent comparison of Databricks vs Snowflake vs Purview classification accuracy. [Market Landscape]

---

## Product Design Implications

### User Mental Model

Tags in Databricks should be understood at **three levels**:

1. **Discovery tags** = "my team's bookmarks" — flexible, user-created, for findability. Anyone can create.
2. **Governed tags** = "the organization's official labels" — admin-controlled, enforced, drive access control and cost attribution. Only stewards can assign.
3. **System tags** = "Databricks' automated labels" — immutable, applied by AI classification. Users can read but not edit.

This maps to a **progressive trust model**: discovery (low trust, high flexibility) → governed (high trust, controlled) → system (highest trust, automated).

**Key tension:** Governed tags serve BOTH classification (what kind of data is this?) AND access control (who can see it?). This dual purpose may confuse users. Design should separate the "classify" action from the "protect" consequence — show the ABAC policy impact as a preview when assigning a governed tag.

### Key Interaction Patterns

- **Inline typeahead with governed-first suggestions.** When adding a tag, show governed tags first (lock icon, restricted values), then allow freeform entry for discovery tags. Reference: Material Design Input Chips.

- **Tag status indicators in lineage view.** Solid badge = directly applied. Dashed badge = propagated via lineage. Yellow badge = value mismatch with source. Reference: Snowflake Horizon lineage UX.

- **ABAC policy preview on tag assignment.** Before a steward applies a governed tag: "Applying `sensitivity=PII` will activate masking policy X for users without role Y." Prevents surprise access changes.

- **Bulk tagging via saved filters.** Saved filter ("all tables in catalog X without a cost_center tag") → preview affected assets → batch apply. Dry-run step before execution.

- **Tag policy dashboard in Governance Hub.** Single surface: all governed tag definitions, allowed values, assignment permissions, compliance % (assets tagged / total), connected ABAC policies, cost tag coverage.

### Information Architecture

- **Governance Hub (Account Console)** = tag administration: definitions, policies, permissions, compliance dashboard, domain management
- **Catalog Explorer (Workspace)** = tag consumption: view tags on assets, apply tags, browse by domain, filter by tags
- **Lineage View** = tag propagation: see how tags flow, identify gaps, remediate missing tags
- **Search** = tags as facets: filter results by governed tags, domains, system tags

### UX Risks

- **Tag proliferation without lifecycle management.** Discovery tags with no cleanup = noise. Mitigation: usage analytics, inactive tag prompts, soft limits.
- **ABAC opacity.** "Permission denied" without explanation erodes trust. Mitigation: show "Access restricted by tag [X] policy [Y]."
- **Required tags as creation blockers.** Mitigation: default values, grace periods, "N/A" option for non-applicable required tags.
- **System tags polluting admin views.** Mitigation: filter/hide system tags by default in Gov Hub tag management.
- **Propagation surprises.** A derived table inheriting a PII tag it doesn't deserve. Mitigation: propagation notifications + override option.

### Design Questions to Resolve

1. **One tag component or two?** Should governed and discovery tags be the same UI component (differentiated by icon) or fundamentally different elements? Needs user testing.
2. **How to communicate ABAC impact?** When assigning a governed tag, how much policy preview to show? Risk of overwhelming vs. risk of surprise.
3. **Required tag grace period UX.** Hard block at creation vs. 7-day grace period with reminders? Should it be configurable per tag?
4. **Tag coverage metric visualization.** How to show "% of assets tagged with required tags" at account level? Heatmap? Progress bar? Table?
5. **Unified tag view for data + cost.** How to present UC tags and compute tags in a single Gov Hub surface without confusing the underlying system differences?

### Recommended Design Next Steps

- [ ] **Run a UXR study on tag authoring friction** — interview 8-10 admins who manage tags today: what's hard? What workarounds do they use? Why don't more people tag?
- [ ] **Read the Tagging at Databricks strategy deck** (Jan 2026) — contains the Unified Tagging vision
- [ ] **Prototype the Gov Hub tag management surface** — tag definitions, policies, compliance dashboard, domains as a sibling section
- [ ] **Audit Snowflake Horizon lineage + tag UI** — study their dashed/yellow border pattern for tag status visualization
- [ ] **Design tag propagation config UX** — per-tag toggle in governed tag settings with lineage preview
- [ ] **Prototype ABAC policy preview** — what to show when a steward applies a governed tag that triggers access policies
- [ ] **Define the tag coverage metric** — work with Quantitative team to build "% of assets with required tags" metric for the Gov Hub dashboard

---

## References

### Public Sources

1. [Databricks — Tags in Unity Catalog](https://docs.databricks.com/aws/en/database-objects/tags) (surfaced by: Official Docs)
2. [Databricks — Governed Tags](https://docs.databricks.com/aws/en/admin/governed-tags/) (surfaced by: Official Docs)
3. [Databricks — ABAC](https://docs.databricks.com/aws/en/data-governance/unity-catalog/abac/) (surfaced by: Official Docs)
4. [Databricks — Data Classification](https://docs.databricks.com/aws/en/data-governance/unity-catalog/data-classification) (surfaced by: Official Docs)
5. [Databricks Blog — Governed Tags Public Preview](https://www.databricks.com/blog/enforce-consistent-secure-tagging-across-data-and-ai-assets-governed-tags-unity-catalog-public) (surfaced by: Official Docs, Sales & GTM)
6. [Snowflake — Object Tagging](https://docs.snowflake.com/en/user-guide/object-tagging/introduction) (surfaced by: Competitive)
7. [Snowflake — Tag Propagation (May 2025)](https://docs.snowflake.com/en/release-notes/2025/other/2025-05-14-tag-propagation) (surfaced by: Competitive)
8. [Snowflake — Tag Inheritance](https://docs.snowflake.com/en/user-guide/object-tagging/inheritance) (surfaced by: Competitive)
9. [Snowflake — Lineage UI in Snowsight](https://docs.snowflake.com/en/user-guide/ui-snowsight-lineage) (surfaced by: Product Design)
10. [Microsoft Purview — Sensitivity Labels](https://learn.microsoft.com/en-us/purview/sensitivity-labels) (surfaced by: Competitive)
11. [AWS Lake Formation — Tag-Based Access Control](https://docs.aws.amazon.com/lake-formation/latest/dg/tag-based-access-control.html) (surfaced by: Competitive)
12. [W3C — SKOS Reference](https://www.w3.org/TR/skos-reference/) (surfaced by: Foundations)
13. [NIST SP 1800-39 — Data Classification](https://www.nccoe.nist.gov/data-classification) (surfaced by: Foundations)
14. [NNGroup — Taxonomy 101](https://www.nngroup.com/articles/taxonomy-101/) (surfaced by: Product Design)
15. [Material Design 3 — Chips](https://m3.material.io/components/chips/guidelines) (surfaced by: Product Design)
16. [Forrester Wave Data Governance Q3 2025](https://www.forrester.com/blogs/the-forrester-wave-data-governance-solutions-q3-2025-shows-that-governance-entered-the-agentic-era/) (surfaced by: Market Landscape)

### Key Internal Documents

17. [PRD] Governed Tags — https://docs.google.com/document/d/1JynehROFoGLsiRmSt35ygVkC4Oq3LsZY0jEY9nUKpos (surfaced by: Internal Intel)
18. [PRD] Tag Propagation for UC Tables — https://docs.google.com/document/d/1gjcj98YVypniEAylVSDmsSbxAQRjk2tDjiLGJHdOQsE (surfaced by: Internal Intel, Roadmap)
19. [PRD] ABAC — https://docs.google.com/document/d/1DvnX_3a3e04xEFUrDJ8mBMQJ9SbRLFL843opvyYkSZY (surfaced by: Internal Intel)
20. [PRD] Domains: Using Governed Tags — https://docs.google.com/document/d/1mpzG8r8goEE5KnmB73FmbJHWnwmBOJicuwu6oez87j4 (surfaced by: Internal Intel, Roadmap)
21. [PRD] Account Level Governance Hub — https://docs.google.com/document/d/1ud_Q7p29zFGOQjT8VSo7nwjN_-2CF6TxHncP4LPGYKc (surfaced by: Roadmap)
22. [PRD] Query Tags — https://docs.google.com/document/d/1s0z1-wtao75sfCUKjlcSm3bpmsjZeqx30GK0oLKq68E (surfaced by: Internal Intel)
23. [PRD] Serverless Budget Policies — https://docs.google.com/document/d/1IQJ64-X2iWwedz5EE2Ko98pDDxpl_2oRfucqWWyeYQ4 (surfaced by: Sales & GTM)
24. [Mini-PRD] Tag Policies UI Improvements — https://docs.google.com/document/d/1g7W7hYvb8ubFyX0fhbQV5i4gxiequiyvOa1V5nvmCT4 (surfaced by: Internal Intel)
25. [FY27Q1] Metadata Intelligence Pre-read — https://docs.google.com/document/d/1tEQzvwHs8HNQA-3b1j5khKaSajOAb5gqdxGRudgr8m0 (surfaced by: Roadmap)
26. [FY26Q4] Metadata Intelligence Pre-read — https://docs.google.com/document/d/11VQ1Kc5UVFE7XrFcxrOzI_R3I-6GwxouMFdYH8r6wig (surfaced by: Roadmap)
27. Governance UI Consolidated Customer Notes — https://docs.google.com/document/d/1iE8JpLh2iKvOPxDMzqF_BTkQdPO7js34bVDV8CjbHBI (surfaced by: Internal Intel, Sales & GTM)
28. Tagging at Databricks (strategy deck, Jan 2026) — https://docs.google.com/presentation/d/18miQUET8hW0tzDdqt963jsZmR6rAO8X5nbyZ4oCCksg (surfaced by: Roadmap)
29. Governance Hub Competitive Analysis — https://docs.google.com/document/d/1gIqPvC_I793Uf0LJ20PBhnVlN3DssssnoZMVyzR5rLo (surfaced by: Sales & GTM)
30. Jira EDC-913: Tag Propagation for UC — https://databricks.atlassian.net/browse/EDC-913 (surfaced by: Roadmap)

---

## Appendix

### Appendix A: Quantitative Data — Tag Usage Metrics (Verified 2026-03-17)

**Note:** Original analysis (pre-verification) included `CreateStagingTable` as tag traffic because "S**tag**ingTable" matched the `%tag%` filter. This inflated write counts and workspace counts. All numbers below are corrected to exclude staging RPCs.

**Tag Assignments (actual, from mirror tables)**

| Metric | Value |
|--------|-------|
| Total tag assignments (securable-level) | 32,722,941 across 21,174 metastores |
| Total tag assignments (column-level) | 98,844,585 across 9,261 metastores |
| Combined tag assignments | 131,567,526 |
| Table-level assignments (96% of securable) | 31.4M across 14,314 metastores |
| Schema-level assignments | 689K across 3,700 metastores |
| Catalog-level assignments | 148K across 9,213 metastores |

**API Traffic (last 30 days, pure tag RPCs)**

| Metric | Value | Period |
|--------|-------|--------|
| Workspaces with tag API traffic | 1,695 of 5,775 (29.4%) | Last 30 days |
| Read transactions | 8.96M (97.4%) | Last 30 days |
| Write transactions | 241K (2.6%) | Last 30 days |
| Read:Write ratio | 37:1 | Last 30 days |
| Column-level tag reads (GetTagSubentityAssignments) | 7.92M from 1,287 workspaces | Last 30 days |
| Table-level tag list (ListSecurableTags) | 816K from 1,690 workspaces | Last 30 days |
| Table-level tag reads (GetTagSecurableAssignments) | 224K from 1,655 workspaces | Last 30 days |
| Column-level tag writes (UpdateTagSubentityAssignments) | 166K from 49 workspaces | Last 30 days |
| Table-level tag writes (UpdateTagSecurableAssignments) | 75K from 71 workspaces | Last 30 days |
| Total write workspaces (deduplicated) | 91 (5.4% of tag users) | Last 30 days |
| Read-only workspaces | 1,604 (94.6% of tag users) | Last 30 days |
| Read+write workspaces | 91 (5.4%) | Last 30 days |

**Error Rates**

| RPC | Error Rate | Note |
|-----|-----------|------|
| UpdateTagSubentityAssignments (column writes) | 8.67% | Nearly 1 in 11 fails — worth investigating |
| GetTagSubentityAssignments (column reads) | 1.56% | Mostly TABLE_DOES_NOT_EXIST |
| GetTagSecurableAssignments (table reads) | 0.16% | Healthy |
| UpdateTagSecurableAssignments (table writes) | 0.02% | Healthy |
| ListSecurableTags | 0.01% | Healthy |

**UI Interactions (last 30 days)**

| Interaction | Hits |
|-------------|------|
| governance.tags.index (tag list page) | 200,331 |
| add_tags_button (click to add tags) | 142,425 |
| governance.tags.details (tag detail page) | 107,538 |
| pipeline-settings-panel.add-tag-button (DLT) | 88,932 |
| tag_assignment_badge.tag (click) | 58,854 |
| budget-policies-tags-field-add-tag-button | 56,217 |
| tag_assignment.remove_key_value_row_button | 15,585 |
| discovery.data_explorer.add_tags_button | 13,797 |

**Data Quality Notes:**
- `customer_traffic_last_30_days` has no `num_calls` column — each row is one API event (COUNT(*) not SUM)
- `sampling_rate` is NULL for all tag traffic — no sampling, every call counted
- No `user_agent` or `source` column — cannot distinguish UI vs API vs 3rd-party tool traffic
- `CreateStagingTable` excluded — matched `%tag%` filter but is not a tag operation

### Appendix B: Competitive Comparison — Tag Inheritance & Propagation

| Platform | Hierarchy Inheritance | Lineage Propagation | Override | Required Tags |
|----------|----------------------|-------------------|----------|---------------|
| Databricks UC | ABAC-only (catalog > schema > table) | Planned (EDC-913) | Manual | Tag Policies (PrPr) |
| Snowflake | Full hierarchy (account > db > schema > table > column) | Shipped May 2025 (CTAS, views) | ON_CONFLICT property | No |
| Microsoft Purview | Labels via Data Map scanning | Labels travel with content | Auto vs manual labels | Mandatory labels via policy |
| Google BigQuery | Column-level policy tags | No | Re-attach at lower level | Custom Org Policy (pre-GA) |
| AWS Lake Formation | DB > table > column | No | Override at descendant | SCPs + Tag Policies |

### Appendix C: Tag Permission Model

```
STANDARD (DISCOVERY) TAGS
  Read:   Any user with SELECT on INFORMATION_SCHEMA
  Write:  APPLY TAG on object + USE SCHEMA + USE CATALOG

GOVERNED TAGS
  Create definition:  CREATE permission (account level)
  Edit/delete:        MANAGE permission (account or per-tag)
  Assign to asset:    ASSIGN on the tag + APPLY TAG on the object
  Read:               Any user with catalog access

SYSTEM TAGS
  Create/edit/delete: Not allowed (Databricks-defined)
  Assign:             ASSIGN permission (for manual application)
  Auto-assign:        Data Classification engine
  Read:               Any user with catalog access
```
