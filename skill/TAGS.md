# Research Tags — Shared Taxonomy

Use these tags consistently across all research files, agent outputs, and synthesis docs. Tags help agents cross-reference findings, apply the trust hierarchy, and let humans scan results quickly.

Apply tags inline after a finding: `Unity Catalog privilege counts grew 40% QoQ` → `#unity-catalog #adoption #high-signal #r-and-d`

---

## 1. Source Type — what kind of artifact is this?

| Tag | Artifact type |
|-----|---------------|
| `#prd` | Product Requirements Document |
| `#roadmap` | Roadmap doc, quarterly pre-read, or planning artifact |
| `#okr` | OKR or goal-tracking document |
| `#gtm-plan` | Go-to-market plan or launch plan |
| `#launch-brief` | Launch brief or NPI (New Product Introduction) doc |
| `#messaging-framework` | Positioning & messaging framework |
| `#battlecard` | Competitive battlecard |
| `#customer-notes` | PM field notes from customer calls |
| `#uxr-report` | UX research study or synthesis report |
| `#nps-csat` | NPS or CSAT survey results |
| `#es-ticket` | Engineering Support ticket (customer-reported bug or issue) |
| `#cuj` | Critical User Journey definition or SimpleBricks score |
| `#playbook` | Sales or delivery playbook |
| `#enablement` | Training or enablement content |
| `#blog` | Blog post or external article |
| `#analysis` | Internal analysis or synthesis doc |
| `#wiki` | Confluence or intranet page |
| `#academic` | Peer-reviewed paper, conference proceeding, or academic survey |
| `#standard` | Industry standard or specification (W3C, ISO, DMBOK, OpenLineage, etc.) |
| `#design-pattern` | UX pattern, interaction model, or design system reference |
| `#ux-benchmark` | Usability benchmark, heuristic evaluation, or NNGroup guideline |

---

## 2. Business Function — who produced it?

| Tag | Function |
|-----|----------|
| `#r-and-d` | Product / Engineering (R&D) |
| `#pmm` | Product Marketing |
| `#uxr` | UX Research |
| `#design` | Product Design |
| `#field-eng` | Field Engineering (pre-sales SAs, post-sales DSAs) |
| `#cse` | Customer Success Engineering |
| `#pro-services` | Professional Services (PS / RSA) |
| `#sales` | Sales / Account Executives |
| `#devrel` | Developer Relations |
| `#academy` | Databricks Academy / Learning & Enablement |
| `#partner` | Partner ecosystem (ISV, SI, cloud partner) |
| `#community` | External user community (public forums, Reddit, Ideas Portal) |
| `#legal` | Legal, compliance, or regulatory teams |
| `#finance` | Finance, pricing, or business analytics |
| `#academic` | External academic or research institution |

---

## 3. Signal Quality — how much to trust this?

These map directly to the trust hierarchy in `INDEX.md`. When two findings conflict, `#high-signal` beats `#opinion-based`.

| Tag | Meaning |
|-----|---------|
| `#high-signal` | Quantitative data or direct customer quote — highest authority |
| `#primary-source` | Official docs, shipped feature, or public commitment |
| `#field-signal` | PM notes, ES tickets, BrickBites — direct from customer interactions |
| `#canonical` | Widely-cited academic paper, industry standard, or foundational text — high authority for definitional questions |
| `#lagging` | External analyst report; typically 6–18 months behind current state |
| `#opinion-based` | Blog, community post, or practitioner take; useful for trends, low authority |
| `#requires-access` | Source exists but needs special permissions (SFDC, partner portal, etc.) |

---

## 4. Topic Domain — what product area or theme?

### Databricks product areas

| Tag | Area |
|-----|------|
| `#unity-catalog` | Unity Catalog, data governance, lineage, access control, Delta Sharing |
| `#ai-bi` | AI/BI, Genie, Lakeview dashboards |
| `#lakeflow` | Lakeflow Pipelines, DLT, Lakeflow Connect (ingestion) |
| `#lakebase` | Lakebase (OLTP / operational database) |
| `#compute` | Clusters, serverless, Photon, runtimes, DBR |
| `#security` | Security, compliance, encryption, network, IAM |
| `#admin-console` | Account console, workspace admin, identity management |
| `#mlops` | MLflow, Model Registry, Feature Store, inference tables |
| `#genai` | GenAI, Foundation Model APIs, Mosaic AI, agents, RAG |
| `#data-sharing` | Delta Sharing, Lakehouse Federation, external data access |
| `#apps` | Databricks Apps |
| `#notebooks` | Notebooks, collaborative editing, notebook workflows |
| `#sql` | Databricks SQL, SQL warehouse, SQL editor, query history |
| `#streaming` | Structured Streaming, real-time data, Delta Live Tables streaming |
| `#marketplace` | Databricks Marketplace, data products, data exchange |
| `#workflows` | Databricks Workflows, Jobs, orchestration, scheduling |
| `#developer-experience` | SDKs, CLI, REST APIs, Terraform, IDE integrations |
| `#delta-lake` | Delta Lake, table format, liquid clustering, optimizations |
| `#collaboration` | Shared workspaces, comments, reviews, multi-user workflows |
| `#cost` | Cost governance, billing, budgets, DBU pricing, consumption |
| `#performance` | Query performance, cluster tuning, Photon, benchmarks |
| `#platform` | Cross-cutting platform topics, workspace config, account architecture |

### Research themes

| Tag | Theme |
|-----|-------|
| `#adoption` | Feature adoption, usage rates, onboarding patterns |
| `#simplicity` | Product simplicity, CUJ completion, UX friction, discoverability |
| `#competitive` | Competitor comparison or positioning |
| `#market` | Market landscape, analyst views, ecosystem mapping |
| `#customer-voice` | Direct customer feedback, verbatim quotes, pain points |
| `#product-gap` | Known missing feature or unmet customer need |
| `#roadmap-signal` | Active or planned work on this topic |
| `#win-loss` | Deal win/loss dynamics and competitive objections |
| `#foundations` | Foundational concept, academic definition, or industry standard |
| `#design-implication` | Finding with direct UX/product design consequence |
| `#ux-pattern` | Interaction pattern, competitor UX, or design system reference |
| `#trend` | Temporal signal — growing, declining, or inflecting |
| `#ecosystem` | Partner, ISV, or integration ecosystem dynamics |
| `#regulatory` | Legal, compliance, or regulatory requirement |
| `#migration` | Migration path, upgrade friction, backwards compatibility |
| `#pricing` | Pricing model, cost structure, or monetization pattern |

---

## 5. Access Level — who can see this?

| Tag | Meaning |
|-----|---------|
| `#public` | Publicly available (docs, blog, community forum) |
| `#internal` | Internal to Databricks employees (Glean, Confluence, Drive) |
| `#field-only` | Restricted to Field / Sales org (Sales Portal, FE intranet) |
| `#partner-only` | Partner portal only (partners.databricks.com) |

---

## How to use

Tag each key finding in agent output with source type + function + signal quality. In synthesis, `#high-signal #r-and-d` beats `#opinion-based #community` — document resolutions in the Conflicts Resolved table. Intel files (`intel/competitive-intel.md`, `intel/landscape-intel.md`, `intel/db-data.md`) use this taxonomy to tag sources.
