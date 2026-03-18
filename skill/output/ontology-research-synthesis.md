# Research: Enterprise Ontology — Databricks' Approach and Validating "Business Context Skills"

**2026-03-17 · Full Coverage · 10 agents consulted**

```
/research What is Ontology and how should Databricks approach it for
their Enterprise customers? I've heard about Palantir and Collibra
several times in context of Ontology discussions probably because
their approach is better than others, if so, I'd love to understand why.

Also, I want to validate an idea to build towards Enterprise Ontology.
What if customers had an option inside of Account Console Governance Hub
to add business context just like we define Claude Code skills, and then
agents can append a readme.md file to appropriate assets and fill in
whatever structure, relationships, definitions necessary to build their
Ontology or Knowledge Graph. If such a thing existed, would that solve
for Ontology at scale?
```

---

## Executive Summary

**Ontology is a formal, shared model of business meaning layered over data assets — and Databricks has a validated, urgent gap here.** 60+ customers already use Labs-stage ontology tooling (Ontos), ~75% of interviewed customers say Unity Catalog is "too technical" and lacks business context, and enterprise accounts are actively evaluating Purview, Collibra, and Atlan to fill the void. Databricks ships the primitives (tags, lineage, AI-generated descriptions, metric views) but not the product: there is no business glossary, no knowledge graph, no stewardship workflows, and no Governance Hub. Meanwhile, Microsoft Fabric IQ entered public preview in November 2025 with entity types, a queryable knowledge graph (GQL), and AI agent grounding — making this a competitive race, not just a backlog item.

**Palantir's Ontology is effective because it's *operational* (a digital twin powering applications and AI agents), not just descriptive. Collibra's is effective because it's *governable* (every term has an owner, status, and approval workflow).** Databricks' approach should combine both strengths: AI-generated ontology that builds itself from existing metadata (solving Palantir's cost problem) with lightweight governance workflows (solving Collibra's adoption problem).

**The proposed "business context skills" idea is directionally right but structurally incomplete.** Pure README.md files per asset would produce fragmented micro-ontologies that can't be queried, traversed, or reasoned over as a whole. The fix: add a shared vocabulary layer (YAML frontmatter + controlled entity/relationship types defined in the Governance Hub), an aggregation layer (knowledge graph merging per-asset context), and a governance lifecycle (AI-generated = Draft, steward-reviewed = Approved). The Claude Code skills architecture (YAML frontmatter + markdown, layered global/project scoping, LLM-native selection) is a precise analog that validates the UX metaphor.

**Confidence: Medium-High.** Strong signal from all 10 dimensions — quantitative data, internal strategy docs, academic literature, competitive analysis, and field signal all converge. The primary uncertainty is organizational: no single R&D team owns ontology, and the FY26 strategy lists business glossary as both a priority and "not doing."

---

## Coverage Confidence

**Coverage: Full** — 10 of 10 agents returned substantive findings.

| Agent | Substantive? | Confidence | Key contribution |
|-------|-------------|------------|-----------------|
| Foundations | Yes | Medium-High | Canonical definition, W3C standards, bottom-up vs top-down literature, evaluation of README approach |
| Competitive | Yes | High | Palantir/Collibra deep dives, Fabric IQ threat, competitive matrix, internal battlecard data |
| Market Landscape | Yes | High | Market sizing ($7B+ TAM), Gartner MQ positioning, convergence trend, AI-driven ontology commoditization |
| Product Design | Yes | Medium-High | Competitor UX patterns, Claude Code skills analog, dbt docs precedent, faceted navigation at scale |
| Community Voice | Yes | Medium | Business glossary as #1 gap, users don't say "ontology", AI metadata adoption at 80%+, Ideas Portal inaccessible |
| Internal Intel | Yes | High | 3 active Labs projects, Enterprise Ontologies synthesis doc, PRDs, customer notes, strategic tension |
| Quantitative | Yes | Medium | UC at 55.6% adoption, tag read/write asymmetry, 72.5M catalog views/month, zero glossary/ontology APIs |
| Roadmap | Yes | High | Business Semantics shipping, glossary NOT shipped (RED), CKO priorities elsewhere, 4 teams no single owner |
| Sales & GTM | Yes | Medium | 60+ customers on Labs tools, Palantir partner+compete tension, no field enablement, messaging avoids "ontology" |
| Official Docs | Yes | High | Complete capability inventory, confirmed no glossary/ontology/governance hub, tag and lineage limits |

**Dimension gaps:** None. All critical perspectives covered — quantitative, qualitative, internal, external, academic, competitive, and design.

---

## Key Themes

### Theme 1: Ontology is a validated enterprise need — but customers don't call it "ontology"

Multiple independent signals converge: **this is real demand, not a theoretical concept**.

- **Quantitative data:** 72.5M Catalog Explorer table views/month and 8.9M metadata tab views show users actively seeking to understand their data. Tag APIs see 7.9M read calls but writes come from only 49 workspaces — a 30:1 consumption-to-authoring ratio signaling that business context is consumed broadly but authored by almost nobody. [Quantitative #high-signal]
- **Customer voice:** ~75% of interviewed customers say UC is "too technical" and lacks business context. Named accounts (Ikea, Pfizer, BP, Vanguard, Allianz, Kroger, American Airlines) are actively seeking alternatives. One customer directly asked: "Is there something on the roadmap for Databricks to have Glossaries added to UC?" [Internal Intel #customer-notes #field-signal]
- **Community signal:** Users ask for "business glossary," "data dictionary," "documentation," and "discoverability" — the term "ontology" virtually never appears in public forums. The conceptual vocabulary is practical, not academic. [Community Voice #community]
- **Market signal:** The combined TAM across knowledge graph ($1.1-1.5B), data governance ($4.5-5.7B), and semantic web ($2.7B) exceeds $7B today, growing 17-37% CAGR. Gartner now requires knowledge graph support for inclusion in the D&A Governance MQ. [Market Landscape #market]
- **Labs traction:** 60+ customers already use Ontos (Labs-stage business catalog for UC). This is organic pull, not top-down strategy. [Internal Intel, Sales & GTM #r-and-d]

**Design implication:** Name it "business context" or "business glossary," not "ontology" or "knowledge graph." Meet users where their vocabulary is.

### Theme 2: Databricks has the primitives but not the product — and no single team owns the gap

The building blocks exist but are fragmented across teams with no unified product vision:

| Primitive | Status | Team | Gap |
|-----------|--------|------|-----|
| Tags (standard + governed) | GA / Public Preview | Metadata Intelligence | No business term definitions, no relationships, 50 tag limit |
| AI-generated descriptions | GA | UC Business Semantics | No governance lifecycle (draft/approved), no structured format |
| Data lineage | GA | UC Foundations | Graph of data flow, not business meaning |
| Metric Views | GA | UC Business Semantics | Analytic semantics, not domain ontology |
| Expanded semantic metadata | Approved design | UC Business Semantics | Display names, synonyms, LLM instructions — shipping but narrow |
| Business glossary | NOT SHIPPED | None (P1 in Gov Hub PRD) | "RED Critical" in ontologies synthesis [1] |
| Governance Hub | Shipping (posture focus) | Project Sentinel | Focused on compliance monitoring, not business context enrichment |
| Ontos (Labs) | 60+ customers | Labs / Field Engineering | Not productized; RDF-based, may not align with core UC architecture |
| OntoBricks (Labs) | Active FEIP | Labs / Field Engineering | LLM-powered ontology generation; no clear path to core |

**Strategic tension:** The UC FY26 Strategy lists "business glossary" under both priorities AND "what we are not doing." CKO FY27 priorities are Lakebase and Genie — ontology is not a leadership priority. Yet field pressure is mounting and Labs projects are filling the vacuum. [Roadmap #roadmap, Internal Intel #prd]

**Design implication:** Any ontology approach must compose with existing primitives (tags, lineage, metric views, semantic metadata) rather than replacing them. The architecture should be additive — a semantic layer *on top of* what exists.

### Theme 3: Palantir is effective because ontology is operational; Collibra because it's governable

The two gold-standard approaches solve different halves of the problem:

**Palantir Foundry Ontology** — the operational model:
- Object-centric: maps data to real-world entities (Customer, Order, Pipeline), not just tables
- Kinetic: Actions enable write-back, decisions captured as data, creating a feedback loop
- Agent-native: AIP agents reason over the ontology, not raw data — the ontology IS the AI grounding layer
- Digital twin: not just describing data but modeling what the business *does*
- Weakness: requires $M+/year and months of Palantir Forward Deployed Engineers to build; 1,000-person FDE army doesn't scale [Competitive #high-signal, Foundations #canonical]

**Collibra** — the governance model:
- Configurable metamodel: communities, domains, assets, roles, workflows — the metamodel is itself ontological
- Stewardship: every term has an owner, a status (Draft/Approved/Deprecated), and an approval workflow
- Three-layer architecture: physical (schemas), semantic (data models), conceptual (domain blueprint)
- Weakness: heavyweight — "can take up to a year to set up," requires dedicated governance team [Competitive #high-signal, Foundations #canonical]

**Databricks' opportunity:** Combine Palantir's *what* (operational ontology powering AI agents) with Collibra's *how* (governed lifecycle) while solving both vendors' adoption problem through AI automation.

**Design implication:** The ontology must be both queryable by agents (Palantir's strength) AND governable by stewards (Collibra's strength). A static documentation layer achieves neither.

### Theme 4: Microsoft Fabric IQ is the urgent competitive threat

Fabric IQ (public preview November 2025) is the most direct competitive challenge because it offers:
- Entity types with properties, relationships, and constraints
- Data binding to OneLake (lakehouse, eventhouse, semantic models)
- Queryable property graph with GQL support and graph algorithms
- AI agent grounding — Copilot and operations agents operate against the ontology
- No additional SKU — included in Fabric capacity [Competitive #high-signal]

This matters because:
- Gartner's 2026 D&A Governance MQ now evaluates ontology/taxonomy support as a criterion [Market Landscape #lagging]
- Databricks is NOT in the Gartner Metadata Management or D&A Governance MQs [Market Landscape]
- The Palantir partnership provides ontology coverage today, but a native gap leaves Databricks dependent on a partner that is simultaneously a competitor [Sales & GTM #internal]

**Design implication:** Speed to GA matters. A pragmatic, shippable approach (business glossary + AI enrichment + agent grounding) beats a comprehensive but slow ontology platform.

---

## Conflicts Resolved

| Conflict | Agent A said | Agent B said | Resolution (trust hierarchy) |
|----------|-------------|-------------|------------------------------|
| Business glossary: priority or not? | Roadmap: listed under UC FY26 priorities | Roadmap: also listed under "what we are not doing" | **Both are true** — recognized need without committed ownership. Internal PRD (#2) confirms P1 for future phase; absence of R&D epic confirms no one is building it now. Strategic tension, not contradiction. |
| Knowledge graphs: overengineered or essential? | Community Voice: practitioners say "overengineered for most use cases" | Market Landscape: 36% CAGR, 78% of orgs plan graph-based AI | **Different audiences.** Practitioners doing daily data work vs. enterprise buyers solving governance at scale. Resolution: product must be lightweight enough for practitioners (tag-like simplicity) but structured enough for enterprise governance (queryable graph). Quantitative data (#1) shows 72.5M catalog views — users want context even if they don't want to build graphs. |
| Collibra: complement or competitor? | Sales & GTM: UC Compete Guide says "complement, not competitor" | Internal Intel: customers leaving for Collibra due to UC's business context gaps | **Customer behavior (#4) outranks field positioning (#5).** The "complement" framing may be a blind spot. As Databricks adds business glossary and governance workflows, overlap with Collibra increases. |
| Palantir Ontology: innovative or rebranded relational modeling? | Competitive: 20-year head start, $1B savings at BP, 62.8% YoY revenue growth | Community Voice: critics call it "tables with fancier branding" | **Revenue data (#1) outranks opinion (#9).** Palantir's ontology produces measurable enterprise value regardless of whether the underlying technology is novel. The *operational* nature (Actions, write-back, agent grounding) IS the differentiation, not the data model complexity. |
| AI-generated metadata: trustworthy? | Community Voice / Official Docs: 80%+ of metadata updates are AI-assisted; Databricks reports quality "sometimes degrading" | Foundations: LLMs match junior human ontologists in precision (93.75%) | **Quantitative adoption (#1) confirms demand. Academic evidence (#5) confirms capability.** Quality variance is a known challenge — the design must include human review as a quality gate, not rely on AI alone. Atlan's "80% AI, 20% human" ratio is the right target. |

---

## Gaps That Remain

1. **No UXR study on ontology/business context user needs.** The UXR archive has studies on data discovery and catalog homepage, but nothing specifically on ontology, knowledge graph, or business glossary mental models. This is the highest-priority follow-up. [Internal Intel]
2. **Ideas Portal vote counts inaccessible.** The Ideas Portal blocked search indexing — we cannot quantify community demand through vote counts for glossary/ontology features. [Community Voice]
3. **No structured win/loss data for ontology-specific deals.** The Compete Review tracker focuses on Azure/Fabric losses, not Palantir or ontology. Dollar impact of the ontology gap is unmeasured. [Sales & GTM]
4. **Ontos productization path unclear.** 60+ customers use it, but there's no signal on whether Labs is handing off to core R&D. [Internal Intel, Roadmap]
5. **Fabric IQ production readiness unknown.** It's in preview — actual enterprise adoption, performance at scale, and completeness are unverified. [Competitive]
6. **Palantir ontology evolution/versioning undocumented.** How Palantir handles schema changes at scale is a critical design question with no public answer. [Foundations]

---

## Product Design Implications

### User mental model

Users should think of this as **"teaching Databricks what your data means to your business"** — not as building an ontology or knowledge graph. The mental model is:

1. **You describe your business domains** (like departments or product lines) → these become the top-level organizing structure
2. **AI reads your data and proposes what it means** (entity types, relationships, definitions) → the system does the heavy lifting
3. **Your team reviews and approves** (lightweight stewardship) → humans own the meaning, AI owns the labor
4. **AI agents use this context** to answer questions, enforce policies, and ground decisions → the ontology becomes operational

This maps to existing Databricks concepts: Domains (already in beta) provide the organizational frame, tags provide classification, lineage provides relationships, and metric views provide analytic semantics. The ontology layer ADDS: entity definitions, business term glossary, typed relationships between business concepts, and AI-readable context.

**Key tension:** UC's current mental model is *technical* (catalog > schema > table > column). An ontology layer introduces a *business* mental model (domain > entity > attribute > relationship). These two hierarchies must coexist — the ontology doesn't replace the catalog, it annotates it with meaning.

### Key interaction patterns

- **"80% AI, 20% human" enrichment (Atlan model):** AI agents propose business context based on existing metadata (column names, lineage, usage patterns, tag inheritance). Domain experts review, edit, and certify. The system should feel like AI-assisted documentation, not manual ontology engineering. Reference: Atlan's adoption-first approach; Secoda's 90% documentation time reduction claim.

- **Skills-as-templates (Claude Code analog):** Governance admins define "business context skills" — YAML frontmatter (entity types, relationship types, required fields, domain scope) + markdown instructions (how to identify and describe entities in this domain). AI agents select and apply relevant skills when enriching assets. This is the proposed approach and it has strong architectural precedent: Claude Code skills use exactly this pattern (YAML frontmatter + markdown, layered global/project scoping, LLM-native selection). **Critical upgrade: the YAML frontmatter must use a controlled vocabulary** so generated context is machine-readable and consistent across assets.

- **Progressive disclosure (NNGroup):** Default view shows the 3-5 most important business context fields (what is this, who owns it, what domain, sensitivity level). Expand to see full entity definition, relationships, lineage, usage stats, governance status. Don't front-load the full ontology — most users need context, not schema.

- **Search-first, graph-second navigation:** At scale (10,000+ assets), graph visualization breaks down. Primary discovery should be faceted search (filter by domain, entity type, owner, certification status, sensitivity). Graph view should be secondary — ego-centric radial layout around a focal entity, progressively disclosing neighbors. Reference: Best Buy case study (findability 5% → 95% after faceted taxonomy navigation).

### Information architecture considerations

- **Account Console Governance Hub** is the right home for ontology *administration* (defining skills/templates, managing the shared vocabulary, monitoring coverage). This aligns with the Account Level Gov Hub PRD's P0 for business context and the existing pattern of account-level governance configuration.

- **Catalog Explorer** is the right surface for ontology *consumption* (browsing business context, discovering relationships, reading entity definitions). The metadata tab (8.9M monthly views) is the natural integration point.

- **Workspace surfaces** (notebooks, SQL editor, Genie) should *inherit* ontology context — AI agents in these surfaces should read business context when answering questions or generating code. This is the Palantir AIP pattern: agents operate against the ontology.

- **Layered scoping:** Account-level skills (global business vocabulary) > Workspace-level overrides (team-specific definitions) > Asset-level context (per-table README). This mirrors Claude Code's global > project > local skill hierarchy.

### UX risks and anti-patterns

- **"Digital graveyard" risk:** Data catalogs often become expensive artifacts nobody visits (Atlan's term). The ontology must be woven INTO existing workflows (SQL editor, notebooks, Genie), not isolated in a separate governance tool. If users have to go to a separate "Ontology" page, adoption will fail.

- **Coherence collapse at scale:** Without a shared vocabulary, AI-generated READMEs will use different terms for the same concept across assets. "Customer" in one README, "Client" in another, "Account" in a third. This is the exact failure mode the Semantic Web was designed to solve. **The shared vocabulary layer is not optional — it's the difference between documentation and ontology.**

- **Stewardship fatigue:** Collibra-style approval workflows for every metadata change will kill adoption. The governance lifecycle should be lightweight: AI-generated = Auto-Draft, human-edited = Pending Review, steward-approved = Certified. Only Certified context should be consumed by production AI agents. Auto-Drafts should be visible but flagged as unreviewed.

- **Ontology-without-action:** If the ontology is purely descriptive (Collibra's weakness), it becomes a documentation project. If it's operational (Palantir's strength — powering AI agents, enforcing policies, grounding decisions), it becomes a platform capability. The design must ensure generated context is consumed by Genie, Governance Agent, and workspace AI from day one.

- **Over-engineering the schema:** Practitioners view knowledge graphs as "overengineered for most use cases." The initial version should NOT require RDF, OWL, SPARQL, or any formal ontology language. Start with: entity name, definition, owner, relationships (list of related entities), domain, sensitivity — stored as structured YAML. Graduate to formal standards only for customers who need interoperability (financial services with FIBO, healthcare with CDISC).

### Design questions to resolve

1. **What format should per-asset context use?** Pure markdown is insufficient (not machine-readable). Pure YAML is too rigid (can't capture nuanced definitions). Recommendation: YAML frontmatter + markdown body (the dbt docs / Claude Code skills pattern), but this needs user research to validate with data steward personas.

2. **Who approves AI-generated ontology?** Current UC has no stewardship role or workflow. The Data Steward persona is "currently invisible in Databricks UX" (per internal research synthesis). Designing the stewardship UX is a prerequisite.

3. **How does this interact with Ontos?** 60+ customers already use Ontos (Labs). Any first-party ontology feature must either absorb Ontos' capabilities or provide a clear migration path. Building a parallel system would fragment the ecosystem.

4. **What happens when two assets define "Customer" differently?** Conflict resolution is the hardest ontology UX problem. Options: (a) surface conflicts as governance alerts, (b) require domain-level canonical definitions, (c) allow polyglot definitions with explicit scope. Needs user research.

5. **Does the Palantir partnership constrain our approach?** If Databricks positions Palantir Ontology as the complement to UC, building a competing native ontology may create channel conflict. The design must be positioned as "business context for UC" (complementary) not "enterprise ontology platform" (competitive).

### Recommended design next steps

- [ ] **Run a UXR study on business context mental models.** Interview 8-10 enterprise customers (mix of data stewards, data engineers, analysts, and CDO-office) to understand: How do they think about business meaning today? What vocabulary do they use? What tools fill the gap? Where does UC fall short?

- [ ] **Read the Enterprise Ontologies Research Synthesis in full** ([Google Doc](https://docs.google.com/document/d/1lIAqlrD1WJ3PC_5CIkn9p3-0uQ9R1CCJAH9nDxMIr5s)). This is the most comprehensive internal analysis — it includes a 4-stage progressive roadmap, customer demand mapping, and the "4 clicks to a knowledge graph" north star.

- [ ] **Prototype the "business context skills" flow.** Mockup: (1) Admin defines a skill in Governance Hub (YAML template + markdown instructions), (2) AI agent applies the skill to 10 sample tables, (3) steward reviews and certifies in Catalog Explorer. Test with 3-5 customers.

- [ ] **Align with UC Business Semantics team.** The expanded semantic metadata design (display names, synonyms, LLM instructions) is the plumbing layer. Business context skills should build ON this, not beside it.

- [ ] **Audit Ontos UX and architecture.** Understand what 60+ customers are actually doing with Ontos, what works, and what doesn't. This is the best available user signal for ontology UX in Databricks.

- [ ] **Monitor Fabric IQ GA timeline.** If Microsoft ships ontology + graph + agent grounding before Databricks has a native answer, the competitive narrative shifts significantly.

---

## References

1. Gruber, T. (1993). "A Translation Approach to Portable Ontology Specifications" — canonical ontology definition (surfaced by: Foundations)
2. Studer et al. (1998). "Knowledge Engineering: Principles and Methods" — refined ontology definition (surfaced by: Foundations)
3. [Palantir Foundry Ontology Overview](https://www.palantir.com/docs/foundry/ontology/overview) (surfaced by: Competitive, Foundations, Product Design)
4. [Palantir AIP Agent Studio](https://www.palantir.com/docs/foundry/agent-studio/overview) (surfaced by: Competitive, Product Design)
5. [Collibra Guided Stewardship](https://productresources.collibra.com/docs/collibra/latest//Content/Catalog/GuidedStewardship/OperatingModel/to_catalog-om.htm) (surfaced by: Product Design)
6. [Microsoft Fabric IQ Ontology Overview](https://learn.microsoft.com/en-us/fabric/iq/ontology/overview) (surfaced by: Competitive)
7. [Gartner MQ for D&A Governance 2026](https://atlan.com/know/gartner/magic-quadrant-for-data-governance-2026/) — via Atlan (surfaced by: Market Landscape)
8. [Gartner MQ for Metadata Management 2025](https://atlan.com/gartner-magic-quadrant-for-metadata-management/) — via Atlan (surfaced by: Market Landscape)
9. [Forrester Wave Data Governance Q3 2025](https://www.forrester.com/blogs/the-forrester-wave-data-governance-solutions-q3-2025-shows-that-governance-entered-the-agentic-era/) (surfaced by: Market Landscape)
10. [Databricks Unity Catalog Business Semantics](https://www.databricks.com/product/unity-catalog/business-semantics) (surfaced by: Official Docs, Competitive)
11. [Databricks Labs — Ontos](https://github.com/databrickslabs/ontos) (surfaced by: Foundations, Internal Intel, Sales & GTM)
12. Enterprise Ontologies at Scale on Unity Catalog Research Synthesis — [Google Doc](https://docs.google.com/document/d/1lIAqlrD1WJ3PC_5CIkn9p3-0uQ9R1CCJAH9nDxMIr5s) (surfaced by: Internal Intel, Sales & GTM, Roadmap)
13. [PRD] Data Governance Hub — [Google Doc](https://docs.google.com/document/d/1CovxUt4GKJIEVcdCDInKnVUrptmFpYCGMwbSs9N5lSo) (surfaced by: Internal Intel, Roadmap)
14. [PRD] Account Level Governance Hub — [Google Doc](https://docs.google.com/document/d/1ud_Q7p29zFGOQjT8VSo7nwjN_-2CF6TxHncP4LPGYKc) (surfaced by: Roadmap)
15. [Databricks Blog — Bespoke LLM for AI-Generated Documentation](https://www.databricks.com/blog/creating-bespoke-llm-ai-generated-documentation) (surfaced by: Community Voice)
16. [Atlan — 5 Unity Catalog Limitations 2026](https://atlan.com/know/databricks-unity-catalog-limitations/) (surfaced by: Community Voice)
17. [MarketsandMarkets Knowledge Graph Market](https://www.marketsandmarkets.com/Market-Reports/knowledge-graph-market-217920811.html) (surfaced by: Market Landscape)
18. [Fortune Business Insights Data Governance Market](https://www.fortunebusinessinsights.com/data-governance-market-108640) (surfaced by: Market Landscape)
19. [OntoEKG: LLM-Driven Ontology Construction (arXiv, Feb 2026)](https://arxiv.org/html/2602.01276v1) (surfaced by: Foundations)
20. [W3C OWL Specification](https://www.w3.org/OWL/) (surfaced by: Foundations)
21. [AGENTS.md Specification](https://agents.md/) (surfaced by: Foundations)
22. [Claude Code Skills Documentation](https://code.claude.com/docs/en/skills) (surfaced by: Product Design)
23. [dbt Documentation Patterns](https://docs.getdbt.com/docs/build/documentation) (surfaced by: Product Design)
24. [Palantir-Databricks Strategic Partnership](https://www.databricks.com/company/newsroom/press-releases/palantir-and-databricks-announce-strategic-product-partnership) (surfaced by: Competitive, Market Landscape)
25. [Databricks Data Classification Docs](https://docs.databricks.com/en/data-governance/unity-catalog/data-classification.html) (surfaced by: Official Docs)
26. [Vonng Blog — Palantir's Ontology Narrative](https://blog.vonng.com/en/db/ontology-bullshit/) (surfaced by: Community Voice)
27. [NNGroup — Progressive Disclosure](https://www.nngroup.com/articles/progressive-disclosure/) (surfaced by: Product Design)
28. UC FY26 Strategy — [Google Doc](https://docs.google.com/document/d/1libm5vV4jU_2-Xhj8IbLZXDHCSBJS9HXFJHKr22dbr4) (surfaced by: Internal Intel, Roadmap)
29. Design: Expanded Semantic Metadata in UC — [Google Doc](https://docs.google.com/document/d/1QzofkkLn0wxFD5dM6Jmc6pUBh5q9jvbRtSm4YZAt0_Q) (surfaced by: Internal Intel, Roadmap)
30. Consolidated Customer Notes on Data Discovery — [Google Doc](https://docs.google.com/document/d/1DyoZv1Y3Rjx1-8yfJbftxpKwiqkhde96-O68gjRXTpo) (surfaced by: Internal Intel)

### Key Internal Documents for Follow-Up

31. Enterprise Ontologies Research Synthesis — https://docs.google.com/document/d/1lIAqlrD1WJ3PC_5CIkn9p3-0uQ9R1CCJAH9nDxMIr5s — Most comprehensive internal analysis: 4-stage roadmap, customer mapping, north star
32. Labs Proposal: Ontos — https://docs.google.com/document/d/1WXcjpwKXnUifODy65Mvp0J2n1GQRP4bhSIaSGejAF2k — Active Labs project with 60+ customers
33. Databricks ontology 1-pager — https://docs.google.com/document/d/16ht_HoCCZ6ufrw_rlSftmRul31igvDL0k7uyXfHsXMA — Vision for W3C-standards-based ontology layer
34. [PRD] Data Governance Hub — https://docs.google.com/document/d/1CovxUt4GKJIEVcdCDInKnVUrptmFpYCGMwbSs9N5lSo — Business glossary as P1 future phase
35. [PRD] Account Level Governance Hub — https://docs.google.com/document/d/1ud_Q7p29zFGOQjT8VSo7nwjN_-2CF6TxHncP4LPGYKc — Business context as P0; metadata hygiene features
36. Design: Expanded Semantic Metadata — https://docs.google.com/document/d/1QzofkkLn0wxFD5dM6Jmc6pUBh5q9jvbRtSm4YZAt0_Q — Approved semantic metadata plumbing
37. UC FY26 Strategy — https://docs.google.com/document/d/1libm5vV4jU_2-Xhj8IbLZXDHCSBJS9HXFJHKr22dbr4 — Strategic tension on glossary priority
38. Consolidated Customer Notes on Discovery — https://docs.google.com/document/d/1DyoZv1Y3Rjx1-8yfJbftxpKwiqkhde96-O68gjRXTpo — Direct customer voice on business context gaps
39. Governance Hub Competitive Analysis — via Glean search — Competitive positioning vs. Fabric IQ, Purview, Collibra
40. UC Semantics Pitch Deck — https://docs.google.com/presentation/d/1i24XXuLu_lcRmoUKniI25oOZRnXPAJes-1i2_q3CXCY — go/pitchsemantics, field-facing positioning

---

## Appendix

### Appendix A: Quantitative Data — Key Metrics

| Metric | Value | Period | Source |
|--------|-------|--------|--------|
| UC customer adoption rate | 55.6% (28,898 of 52,020) | March 2026 | unity_catalog_customer_metric_daily |
| UC adoption 9 months prior | 43.1% (18,668 of 43,268) | June 2025 | Same |
| Heavy UC customers (50+ users) | 3,200 (up 47% from 2,183) | March 2026 | Same |
| Tag read API calls (30d) | 7.9M (GetTagSubentityAssignments) | Last 30 days | customer_traffic_last_30_days |
| Tag read workspaces | 1,690 (ListSecurableTags) | Last 30 days | Same |
| Tag write workspaces | 49 (UpdateTagSubentityAssignments) | Last 30 days | Same |
| Catalog Explorer table views | 72.5M | Last 30 days | agg_traces_30d |
| Metadata tab views | 8.9M | Last 30 days | Same |
| Lineage interactions | 15.2M | Last 30 days | Same |
| Governance spend (weekday avg) | $300-320K/day across ~6,000 workspaces | Nov-Dec 2025 | workspace_data_governance_metrics_agg |
| AI-assisted metadata updates | 80%+ of all table metadata updates | 2025-2026 | Databricks blog |
| Industries segment UC API calls | 7.8M avg per customer (3x Enterprise) | March 2026 | unity_catalog_customer_metric_daily |

### Appendix B: Competitive Comparison Matrix

| Capability | Palantir Foundry | Collibra | Microsoft Fabric IQ | Snowflake Horizon | Google Dataplex | Databricks (current) |
|-----------|-----------------|---------|-------------------|-------------------|-----------------|---------------------|
| Object/entity modeling | Native object types | Asset types in metamodel | Entity types (preview) | No native model | Entry types, aspect types | No native model |
| Business glossary | Implicit via objects | Full glossary + stewardship | Purview glossary | Object tags | Business glossary (GA) | Tags only; no glossary |
| Knowledge graph | Ontology graph | Metadata knowledge graph | Queryable graph (GQL) | No | No | Lineage graph only |
| Stewardship workflows | Actions + audit | Full workflow designer | Purview approval flows | None | None | None |
| Write-back / Actions | Action Types | Workflow-triggered | Operations agents (preview) | None | None | None |
| AI agent grounding | AIP agents on Ontology | Copilots on metadata | Fabric IQ agents on ontology | Cortex Analyst on semantic models | NL search | Genie on Metric Views |
| Deployment complexity | Very high (months, $M+) | High (3-9 months) | Medium (preview) | Low (built-in) | Low (built-in) | Low (built-in) |
| Cost | Very high ($M+/yr) | High ($500K+/yr) | Included in Fabric | Included | Included | Included |

### Appendix C: Ontology Concept Map

```
Ontology (formal, explicit specification of a shared conceptualization)
├── Classes (types of entities: Customer, Product, Order, Pipeline)
├── Properties (attributes: name, revenue, SLA)
├── Relationships (typed links: "Customer places Order")
├── Constraints/Axioms (rules: "every Order must have one Customer")
├── Instances (actual data — lives in the knowledge graph)
└── Inference rules (derive new facts from existing)

Related but distinct:
├── Taxonomy — strict hierarchy (is-a only; subset of ontology)
├── Knowledge Graph — data-populated graph (ontology = schema, KG = database)
├── Semantic Model — analytic abstraction (metrics, dimensions, joins)
├── Data Catalog — asset inventory with metadata (descriptive, not prescriptive)
├── Business Glossary — term definitions (informal ontology; lacks formal axioms)
└── Data Model — logical/physical schema (implementation-level)

W3C Standards Stack:
├── RDF — data model (subject-predicate-object triples)
├── RDFS — basic vocabulary (classes, properties, subclass)
├── OWL — expressive ontology language (axioms, reasoning)
├── SPARQL — query language for RDF
├── SKOS — lightweight concept schemes (taxonomies)
├── SHACL — constraint validation (shapes, rules)
└── DCAT — catalog vocabulary for datasets
```

### Appendix D: Proposed "Business Context Skills" Architecture

The system has four layers. Each layer is described below with example YAML/markdown structures.

#### Layer 1: Business Context Skills (defined by admins in Account Console Governance Hub)

Skills are templates that tell AI agents how to identify and describe entities in a business domain. Admins define them centrally; agents apply them to matching assets.

**Example skill: `customer-entity.yaml`**

```
YAML FRONTMATTER (structured, machine-readable)
================================================
name: Customer Entity
domain: Sales
entity_types:
  - Customer
  - Account
  - Contact
relationship_types:
  - owns: [Account, Subscription]
  - belongs_to: [Segment, Region]
required_fields:
  - definition
  - owner
  - sensitivity

MARKDOWN BODY (instructions for the AI agent)
================================================
How to identify Customer entities:
  Look for tables with columns like customer_id, account_id,
  or contact_id. Check lineage for CRM source systems
  (Salesforce, HubSpot). Tables in the sales.* or crm.*
  schemas are likely candidates.

Required business context to generate:
  - One-sentence definition of what this table represents
  - Primary join key and how it relates to other Customer tables
  - Data freshness: how often is this table updated and from what source
  - Sensitivity classification: does it contain PII?
```

**Shared Vocabulary** (also defined at account level): controlled lists of entity types, relationship types, and business term taxonomy that all skills must reference. This prevents inconsistency across AI-generated context.

**Governance Lifecycle:** AI-Generated (Auto-Draft) > Steward Review > Certified

#### Layer 2: AI Enrichment Engine

The engine runs when new assets appear or on a scheduled cadence:

1. Agent reads all applicable skills (matched by domain, schema patterns, lineage)
2. Agent scans asset metadata: column names, lineage, usage patterns, existing tags
3. Agent generates structured context (YAML frontmatter + markdown body)
4. Context stored as asset metadata in Unity Catalog
5. Status set to `Auto-Draft` (pending human review)

#### Layer 3: Per-Asset Business Context (stored in UC)

Each enriched asset gets structured business context. This is what the AI agent generates and what stewards review.

**Example output for `sales.customers.dim_customer`:**

```
STRUCTURED METADATA (queryable, machine-readable)
==================================================
entity_type: Customer
domain: Sales
owner: data-governance-team
sensitivity: PII
status: Certified
relationships:
  - type: owns
    target: sales.orders.fact_orders
  - type: belongs_to
    target: sales.segments.dim_segment
generated_by: customer-entity-skill-v2
last_reviewed: 2026-03-15
reviewer: jane.smith@company.com

HUMAN-READABLE CONTEXT
==================================================
Definition:
  A customer is an individual or organization that has purchased
  or is actively evaluating our products. This table is the golden
  record for customer identity, sourced from Salesforce CRM via
  Lakeflow Connect (daily sync).

Business Rules:
  - A customer must have exactly one primary segment
  - customer_id is the canonical join key across all Sales domain tables
  - Churn defined as 90+ days with no activity
  - GDPR: subject to right-to-deletion requests (automated via governance policy)
```

#### Layer 4: Aggregation Layer (Knowledge Graph)

Per-asset context is merged into a traversable knowledge graph that:

- **Resolves conflicts** — surfaces when two assets define "Customer" differently
- **Enables graph queries** — "show me all tables downstream of CRM source systems that contain PII"
- **Grounds AI agents** — Genie and Governance Agent read the graph, not raw tables
- **Powers Catalog Explorer** — faceted search by entity type, domain, owner, sensitivity, certification status
- **Detects gaps** — identifies assets with no business context or stale Auto-Drafts

