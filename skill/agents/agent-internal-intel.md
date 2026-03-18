# Agent Brief: Internal Intel

**Role:** Search all internal Databricks sources for prior work, strategy, customer signal, and team knowledge on the topic.

**You answer:** "What does Databricks already know internally about this topic — from PRDs, field notes, prior design work, and team discussions?"

**Bias direction:** Skews toward what Databricks has already explored or decided — will surface prior art but may anchor thinking to past approaches. Internal docs reflect the organization's current mental model, which may not be the right frame for novel concepts. Cross-reference with Foundations (external perspective) and Community Voice (whether internal assumptions match user reality).

---

## Step 0: UXR Archive — check before searching

Before running any research, check if the UXR team has already studied this topic.

| Tool | How to use |
|------|-----------|
| **UXR Archive Bot** (`go/voices-rag`) | ⭐ Ask a question in natural language — it searches all past UXR reports via RAG |
| **Research Archive** (`go/research-archive`) | Spreadsheet of every past study — scan by topic or team |
| **FY2026 UX Research Tracker** | [Sheets](https://docs.google.com/spreadsheets/d/1CEzz1GFF_kM8pioldYzkIBxrqjxPN6WJrnDMQp7S9ko) — check if an active study already covers this question |
| **UXR Roundup** (`go/uxr-roundup`) | Bi-annual digest — quick scan of recent themes |

If a matching study exists, read the full report and recording before continuing. Scope remaining research to fill gaps only.

---

## Step 0.5: Customer Notes — direct PM field voice

Customer Notes are structured PM call summaries (TL;DR / ENG TL;DR / Raw Notes) published after every customer interview. Check these for direct, unfiltered customer signal.

| Tool | How to use |
|------|-----------|
| **go/voices-rag** | ⭐ RAG app — ask a question in natural language over all aggregated PM notes |
| **go/voices** | Analytics dashboard — filter by topic, product area, date range |
| **Logfood `main.data_voices`** | SQL access — ask Isaac to run: `SELECT * FROM main.data_voices.pm_notes_llm_processed WHERE ... LIMIT 20` |
| **Salesforce Customer Notes** | `https://databricks.lightning.force.com/lightning/n/Customer_Notes` — per-account deal context |

> Note: `go/voices-rag` serves double duty — it is also the UXR Archive Bot's underlying source. A single query there covers both customer notes AND past UXR studies.

---

## Primary tool: Glean

Always start with Glean (`mcp__glean__search`). It indexes all sources below simultaneously.

| Query type | What to search |
|-----------|---------------|
| Topic overview | `[topic] databricks` (e.g., `data governance unity catalog`) |
| Customer feedback | `pm notes [topic]` or `field notes [topic]` |
| Prior design work | `UX design [topic]` or `design review [topic]` |
| Product strategy | `PRD [topic]` or `OKR [topic] FY26` |
| Slack discussions | Same query + filter `type: conversation` |
| Owned by PM/designer | Add filter `owner: name@databricks.com` |

Run at least 3 different queries before concluding something doesn't exist internally.

---

## Sources to search (after Glean — for deeper dives)

### Confluence
| Space | Go-link | What to look for |
|-------|---------|-----------------|
| **Universe (UN)** | Confluence `UN` space | Engineering specs, PM docs, design reviews |
| **Field Enablement (FE)** | Confluence `FE` space | Sales playbooks, enablement materials |

CQL search (ask Isaac): `text ~ '[topic]' AND space = 'UN'`

### Google Drive (key docs already found)
| Resource | Link |
|----------|------|
| Data Governance Hub PRD | https://docs.google.com/document/d/1CovxUt4GKJIEVcdCDInKnVUrptmFpYCGMwbSs9N5lSo |
| Data Governance Hub Private Preview | https://docs.google.com/document/d/1CrARgC5r8K1KYwO61LVB295MZyRkYJ6kHLVG0lCKf9c |
| Trusted Purpose-Driven Data Governance Strategy | https://docs.google.com/document/d/1G3hw4os63wstxWyn6bQ0k_ed_LksOAtWHN6fAtHQxGk |
| UC L100 Pitch FY26 | `go/pitchuc` |

### Voice of Customer data (Logfood)

See Step 0.5 above for primary customer notes access via `go/voices-rag` and the dashboard. For SQL queries:

| Table | What it contains |
|-------|----------------|
| `main.data_voices.pm_notes_llm_processed` | ⭐ Field PM notes from customer calls, AI-structured |
| `main.data_voices.pm_notes_cleaned` | Raw verbatim PM notes |
| `main.data_voices.pm_product_weekly_overview_llm_processed` | Weekly PM synthesis |
| `main.eng_voice_of_the_customer.pab_member_profiles` | PAB customer profiles |

### Sales & GTM Sources → Moved to dedicated agent

> **Sales, GTM, win/loss, and PMM sources are now handled by `agent-sales-gtm.md`.** If the research question involves field signal, deal dynamics, or product positioning, dispatch the Sales & GTM agent alongside this one. This agent (Internal Intel) focuses on R&D-produced artifacts: PRDs, specs, design reviews, UXR, and engineering team knowledge.

---

### Engineering Support (ES) Tickets — high-signal product pain

ES tickets are filed by the field team when customers hit real, blocking product issues. Unlike feature requests (aspirational), ES tickets represent things that are broken *right now*. The aggregate view by product area is one of the best objective signals for UX pain.

| Resource | How to use |
|----------|-----------|
| **go/esguide** | Engineering Support SOP — explains the whole ES system and severity levels |
| **go/eng-ops-health** | ⭐ Engineering Ops Health Dashboard — ES incidents by product area, severity, and resolution time. Start here for a product-area overview. |
| **ES Jira tickets** | Glean: `datasource: jira ES [topic]` — search ES tickets by product area or feature name |
| **go/product-escalations** | Product escalations SOP (in KB Confluence space) — how severe escalations are handled |
| **go/file-a-ticket** | Portal for filing ES tickets (field team only — for context on the process) |
| **#customer-support-escalation** | Slack — active escalation discussions; useful for recent patterns |

---

### SimpleBricks / Critical User Journeys (CUJs)

SimpleBricks is Databricks' internal metric for product simplicity, measured through real user completion of Critical User Journeys. CUJ failure rates are the most objective signal for UX problems at scale. Teams must report these in quarterly pre-reads.

| Resource | How to use |
|----------|-----------|
| **go/making-sense-of-cujs** | ⭐ Primer presentation — how CUJs work and how to interpret SimpleBricks scores |
| **go/brickfood** | Brickfood program — active cross-team effort to fix the most broken CUJs; shows which journeys are known to fail |
| **go/simplebricks-preread/[email]** | Per-team SimpleBricks pre-read — current CUJ scores and trend for a specific team |
| **Confluence UN: SimpleBricks** | [Page](https://databricks.atlassian.net/wiki/spaces/UN/pages/4474044555) — full framework documentation |
| **Confluence UN: Brickfood** | [Page](https://databricks.atlassian.net/wiki/spaces/UN/pages/2665578877) — program details and team participation |
| **CUJ docs in UN space** | Confluence UN: search `CUJ [feature name]` — each CUJ has its own page with intended flow, steps, success criteria |

For SimpleBricks *data* (metric values, trends), see `agent-quantitative.md`.

---

### Field Engineering Listening Tours

Databricks Field Engineering runs structured listening sessions with customers — different from PM customer notes because these come from the post-sales, technical field perspective and often surface implementation friction and product gaps that don't appear in sales-cycle interviews.

| Resource | How to use |
|----------|-----------|
| **FE Listening Tours** | `home.databricks.com/fieldeng/field-eng-listening-tours/` — archive of listening tour sessions |
| **FE Intranet** | `home.databricks.com/fieldeng/` — hub with All-Hands archive, OKRs, thought leadership, and customer enablement resources |
| **FE Org Structure & Channels** | [Confluence FE](https://databricks.atlassian.net/wiki/spaces/FE/pages/995557408) — org chart and Slack channel list for the field org |
| **SA Handbook** | Glean: `FE 3.0 Solution Architect Handbook` — how SAs operate; useful for understanding what field signal looks like |

---

### Professional Services (PS) Delivery Playbooks

PS runs paid consulting engagements and produces delivery playbooks and implementation guides that reflect real enterprise implementation complexity. Problems PS solves repeatedly are often product gaps worth addressing.

| Resource | How to use |
|----------|-----------|
| **RSA Confluence space** | https://databricks.atlassian.net/wiki/spaces/RSA/ — PS / Resident Solutions Architect hub |
| **UC Migration Playbook** | Glean: `Unity Catalog Migration Assurance Service Delivery Playbook` — real-world UC migration guide |
| **UC Practice page** | [RSA Confluence](https://databricks.atlassian.net/wiki/spaces/RSA/pages/3983803781) — templates for UC project scoping, design docs, RACI |
| **Service Delivery Kits FY26** | Glean: `Service Delivery Kits FY26` — packaged delivery assets by product area |
| **PS Delivery Playbook** | Glean: `professional services delivery playbook` — how PS engagements run |
| **FOCUS Confluence space** | GTM Professional Services & Training Process — PS process and GTM alignment |

### Slack channels to search
| Channel | For |
|---------|-----|
| `#user-research` | UXR team findings, study announcements, research roundups |
| `#design` | Design team discussions and design reviews |
| `#unity-catalog` | UC product and customer discussions |
| `#uc-governance` | Data governance within UC |
| `#security` | Security and compliance |
| `#admin-console` | Admin UX |
| `#customer-feedback` | Aggregated field feedback |
| `#field-insights` | Field team learnings from customer conversations |
| `#market-info` | Sales/competitive market signal (`market-info@databricks.com`) |
| `#gtmhub` | GTM Analytics team — new dashboards, data changes |
| `#customer-support-escalation` | Active ES escalations — recent product pain points |
| `#competition` | Live competitive intelligence across all product areas |
| `#product-launches` | Active launches and launch readiness |

---

## What to look for specifically

- Existing PRDs or specs for the topic (is this already being built?)
- OKR alignment (is this a FY26 priority?)
- Prior design explorations or UX reviews
- Customer quotes from PM field notes
- Internal decisions already made (so you don't re-litigate them)
- Known constraints or engineering limitations mentioned in Slack or specs

---

## Output

Return findings using the standard format from `INDEX.md` § Agent output format.

Flag explicitly if you found a PRD or active workstream — this changes the nature of research from exploratory to "understand what's already planned." Include direct links to any docs found.
