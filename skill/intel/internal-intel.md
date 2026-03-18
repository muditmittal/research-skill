# Internal Intel — Internal Sources

All internal Databricks sources for product research. Always start with Glean — it searches everything simultaneously.

> For topic-specific Databricks product docs see `intel/governance-intel.md`. For external sources see `intel/external-intel.md`.

---

## Glean — Start Here

`go/glean` or via `mcp__glean__search`

| What you need | Query |
|--------------|-------|
| Any product topic | `data governance unity catalog` |
| Customer feedback on a feature | `pm notes [feature name]` |
| Prior design work | `UX design [feature name]` |
| Competitive analysis | `competitive analysis [competitor]` |
| PMM messaging | `messaging framework [product]` |
| Slack discussions | query + filter `type: conversation` |

---

## Key Go-Links

| Go-link | What it is |
|---------|-----------|
| `go/glean` | Internal search — start here |
| `go/voices-rag` | ⭐ RAG agent over all PM customer notes |
| `go/voices` | Customer notes analytics dashboard |
| `go/compete` | All competitive battlecards and analyses |
| `go/uxr` | UX research archive hub |
| `go/research-archive` | Every past UXR study (spreadsheet) |
| `go/hub` | GTM analytics — pipeline, consumption, account health |
| `go/customerinsights` | Customer usage by DBR type per week |
| `go/eng-ops-health` | ES ticket volume by product area |
| `go/making-sense-of-cujs` | CUJ primer — read before SimpleBricks work |
| `go/brickfood` | Active program to fix broken CUJs |
| `go/simplebricks-preread/<email>` | Your team's CUJ scorecard |
| `go/tko-decks` | TKO product positioning decks (annual, FE-facing) |
| `go/pm-access` / `go/cuj-access` | Hands-on access to competitor products |

---

## Confluence Spaces

Use CQL: `text ~ '[topic]' AND space = 'UN'`

| Space | Name | What's there |
|-------|------|-------------|
| `UN` | **Universe** | ⭐ Engineering specs, PRDs, design reviews, CUJ docs, roadmapping |
| `FE` | **Field Engineering** | Sales playbooks, competitive SME, presales skills |
| `CI` | **Competitive Intelligence** | All battlecards, analyses, newsletters (`go/compete`) |
| `RSA` | **Professional Services** | PS delivery playbooks, UC migration guides |
| `devrel` | **Developer Relations** | DevX talks, advocacy content |
| `KB` | **Knowledge Base** | Product escalation SOPs (`go/product-escalations`) |
| `FOCUS` | **GTM / PS Process** | GTM Professional Services and field alignment |

---

## Slack Channels

| Channel | Topic |
|---------|-------|
| `#unity-catalog` | UC product discussions, field questions, feature gaps |
| `#uc-governance` | Data governance within UC |
| `#security` | Security features, compliance |
| `#admin-console` | Admin UX, workspace/account console |
| `#competition` | Live competitive intelligence, all product areas |
| `#design` | Product design team |
| `#user-research` | Customer interviews, research synthesis |
| `#field-insights` | Field team learnings from customers |
| `#tko-fy27` | Technical Kickoff announcements and Q&A |
| `#customer-support-escalation` | High-priority customer escalations |
| `#market-info` | Sales/competitive market signal |

---

## Customer Notes & Voice of Customer

`go/voices-rag` (RAG) · `go/voices` (dashboard) · Logfood: `main.data_voices`

| # | Tool | Notes |
|---|------|-------|
| 1 | **go/voices-rag** | ⭐ Ask NL questions — answers from all PM notes |
| 2 | **go/voices** | Dashboard — filter by topic, product area, date |
| 3 | **Logfood: `main.data_voices`** | SQL access: `pm_notes_llm_processed` (structured) and `pm_notes_cleaned` (verbatim) |
| 4 | **Salesforce Customer Notes** | Per-opportunity deal-level context |

---

## Logfood Quick Reference

**Full schema list:** `intel/db-data.md` · **Workspace:** `central-logfood-prodtools-azure-westus`

| Table | What it answers |
|-------|----------------|
| `main.data_product_features.workspace_metrics` | Feature usage per workspace |
| `main.data_voices.pm_notes_llm_processed` | PM field notes, AI-structured |
| `main.eng_data_gov_ds.workspace_data_governance_metrics_agg` | Governance feature usage per workspace |
| `main.eng_ui_observability.agg_traces_30d` | UI interaction traces, 30-day |
| `main.metric_store.okr_fy26_report_metric_snapshot_latest_post_processed` | FY26 OKR metrics incl. SimpleBricks/CUJ scores |
| `main.gtm_silver` | Accounts, pipeline, consumption, competitor tagging |
| `main.it_sfdc_silver` | SFDC proxy — opportunity, account, win/loss |
| `system.billing.usage` | Cloud cost and DBU consumption |
| `system.access.audit` | All user actions |

---

## Sales & GTM

| Resource | Where | Notes |
|----------|-------|-------|
| **Sales Portal** | `home.databricks.com/sales/` | All sales resources by product area |
| **BrickBites** | `home.databricks.com/sales/field-performance/brickbites/` | ⭐ AE videos on competitive wins — real customer scenarios |
| **Win/Loss Tracker** | Glean: `Compete Review ASQ Win/Loss Tracker` | Quarterly deal-level competitive log |
| **GTM Hub** | `go/hub` | Pipeline, consumption, account health |
| **Customer Insights** | `go/customerinsights` | Usage by DBR type per customer per week |
| **GTM Account Research agent** | [Glean agent](https://databricks.glean.com/chat/agents/ca615183421141d3adc47079a9225bae) | AI agent for account context |
| `#field-insights` | Slack | Field learnings from customer conversations |
| **FE Listening Tours** | `home.databricks.com/fieldeng/field-eng-listening-tours/` | Published summaries from FE listening sessions |

---

## UXR Archive

| Resource | Where | Notes |
|----------|-------|-------|
| **Archive Bot** | [Glean agent](https://databricks.glean.com/chat/agents/cc38959446e84292bc2608f33d3cb779) | ⭐ AI agent over full UXR archive — check before starting any new research |
| **UXR hub** | `go/uxr` | Archive, templates, methods |
| **Research Archive spreadsheet** | `go/research-archive` | Every completed study with report and recording links |
| **FY26 Research Tracker** | [Sheets](https://docs.google.com/spreadsheets/d/1CEzz1GFF_kM8pioldYzkIBxrqjxPN6WJrnDMQp7S9ko) | Active studies — team, topic, method, status |
| **Study plan template** | `go/newstudyplan` | Copy before starting any research project |

---

## PMM Sources

| Resource | Where | Notes |
|----------|-------|-------|
| **TKO Decks** | `go/tko-decks` | ⭐ Field-facing product positioning; single best artifact for how PMM pitches a feature |
| **Positioning & Messaging** | Glean: `messaging framework [product]` | Official narrative: target customer, problem, differentiators |
| **CKO Content** | `go/cko` | Company Kickoff — FY priorities |
| **Launch Briefs** | Glean: `launch brief [feature]` | Per-feature GTM artifacts, tier, messaging, date |

---

## ES Tickets & SimpleBricks

| Resource | Where | Notes |
|----------|-------|-------|
| **Eng Ops Health Dashboard** | `go/eng-ops-health` | ⭐ ES ticket volume by product area — spot pain concentration |
| **ES Jira** | Jira: project = ES | Direct ticket access — read customer-reported symptoms |
| **Making Sense of CUJs** | `go/making-sense-of-cujs` | ⭐ CUJ primer — read first |
| **Brickfood** | `go/brickfood` | Active program to fix broken CUJs |
| **SimpleBricks scorecard** | `go/simplebricks-preread/<email>` | CUJ completion rates for your team |

---

## Key Strategy & Roadmap Docs

| Resource | Link | Notes |
|----------|------|-------|
| **Data Governance Hub PRD** | [Google Doc](https://docs.google.com/document/d/1CovxUt4GKJIEVcdCDInKnVUrptmFpYCGMwbSs9N5lSo) | Primary PRD for governance area |
| **UC L100 Pitch FY26** | `go/pitchuc` | UC positioning and messaging deck |
| **OKRs / Roadmap** | Glean: `OKR FY26 governance` | Multiple docs — search Glean |

---

## Topic Quick-Start

| Topic | First stop | Key Logfood table |
|-------|-----------|-------------------|
| **Data Governance** | `go/uc/compete` → Data Governance battlecard | `main.eng_data_gov_ds.workspace_data_governance_metrics_agg` |
| **AI Governance** | `intel/governance-intel.md` § AI Governance | `main.eng_foundation_model_api` → `system.ai` |
| **Cost Governance** | `intel/governance-intel.md` § Cost Governance | `system.billing.usage` |
| **Performance Governance** | `intel/governance-intel.md` § Performance Governance | `main.eng_dbsql_performance` |
| **Security & Compliance** | `intel/governance-intel.md` § Security | `system.access.audit` |
| **Admin Console** | `intel/governance-intel.md` § Admin Console | `main.data_product_features.workspace_metrics` |
| **Customer context** | `go/customerinsights` → `go/hub` | `main.gtm_silver` |
| **Win/loss** | BrickBites + Win/Loss Tracker | `main.it_sfdc_silver` |

---

*Last updated: March 2026. Companion: `intel/governance-intel.md` · `intel/external-intel.md` · `intel/db-data.md`*
