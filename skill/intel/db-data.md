# Data Access — Databricks Internal Datasets

A two-part guide. **Part 1** covers shared high-value schemas that any Databricks researcher (designer, PM, analyst) would use. **Part 2** is a per-user section — fill in your own workspace credentials and custom schemas.

Tags: `#r-and-d` `#high-signal` `#internal` `#requires-access`

---

## Part 1 — Shared high-value datasets

These schemas are available in the central Logfood workspace and are the most useful for product design and research work across any product area.

**Central workspace:** `central-logfood-prodtools-azure-westus`
All queries run via Isaac using `mcp__databricks-v2__execute_parameterized_sql`.

---

### `main.data_product_features` — Feature adoption metrics
**Primary signal for "is anyone using what was designed?"**

| Table | What it answers |
|-------|----------------|
| `workspace_metrics` | Feature usage per workspace — filter by `feature_name` |
| `user_metrics` | Per-user feature usage |
| `customer_metrics` | Per-customer rollup |
| `account_metrics` | Account-level rollup |

---

### `main.data_voices` — Voice of customer (AI-processed PM notes)
**Primary source for qualitative customer insights and direct field signal.**

| Table | What it answers |
|-------|----------------|
| `pm_notes_llm_processed` | ⭐ PM field notes from customer calls, AI-structured with tags and themes |
| `pm_notes_cleaned` | Raw verbatim note text |
| `pm_notes_llm_processed_rag_selection` | RAG-indexed version (backs `go/voices-rag`) |
| `pm_product_weekly_overview_llm_processed` | Weekly PM synthesis across all notes |

Access via dashboard: `go/voices` | RAG app: `go/voices-rag`

---

### `main.eng_voice_of_the_customer` — Product Advisory Board (PAB)

| Table | What it answers |
|-------|----------------|
| `pab_member_profiles` | PAB customer profiles — useful for outreach targeting |
| `fy_25_pab_members` | Current PAB member list |

---

### `main.eng_ui_observability` — UI interaction and funnel data
**Analytics for measuring UX flows, funnel behavior, and interaction patterns.**

| Table | What it answers |
|-------|----------------|
| `agg_traces_30d` | 30-day aggregated UI interaction traces |
| `adhoc_funnel_sankey_metrics` | Funnel flow and drop-off analysis |
| `traces` | Raw UI interaction traces (high volume — filter carefully) |
| `ui_benchmarks_v2` | UI performance benchmarks |

---

### `main.eng_data_gov_ds` — Governance feature adoption signals

| Table | What it answers |
|-------|----------------|
| `workspace_data_governance_metrics_agg` | Governance feature usage per workspace |
| `unity_catalog_customer_metric_daily` | Daily UC metrics per customer |
| `workspace_unity_catalog_metrics_agg` | UC adoption rollup |
| `uc_okr_fy26_ds_forecast` | FY26 OKR forecasts for governance area |

---

### `main.eng_data_gov_obs` — Deep governance telemetry
300+ tables of Unity Catalog internals. Engineering-focused but useful for real usage patterns at scale.

| Table | What it answers |
|-------|----------------|
| `customer_traffic_last_30_days` | Customer API traffic to governance services |
| `privilege_counts_latest_snapshot` | Access control and permission usage patterns |
| `child_counts_latest_snapshot` | How many catalogs/schemas/tables customers have |

---

### `main.eng_aibi` — AI/BI (Genie / Lakeview) usage

| Table | What it answers |
|-------|----------------|
| `lakeview_usage_breakdown` | Dashboard usage detail |
| `lakeview_usage_customer_rollup` | Per-customer Lakeview usage |
| `dbone_metrics_v2` | Databricks One product metrics |
| `mobile_metrics` | Mobile app usage |

---

### `main.metric_store` — OKRs and product simplicity metrics

| Table | What it answers |
|-------|----------------|
| `fct_customer_insights_dbr_type_weekly` | Weekly customer usage by DBR type (backs `go/customerinsights`) |
| `okr_fy26_report_metric_snapshot_latest_post_processed` | FY26 OKR metrics — includes SimpleBricks / CUJ scores |

---

### `main.gtm_silver` + GTM tables — Sales and account context

| Table | What it answers |
|-------|----------------|
| `main.gtm_silver` | ⭐ Curated GTM tables — accounts, pipeline, consumption, competitor tagging |
| `main.gtm_consumption_silver.account_platform_consumption_daily` | Daily DBU consumption per account |
| `main.it_sfdc_silver` | SFDC proxy — opportunity, account, win/loss (no SFDC access needed) |

Visual exploration: `go/customerinsights` / `go/hub`

---

### `system.*` — Standard Unity Catalog system tables

| Schema | What it answers |
|--------|----------------|
| `system.billing` | Cloud cost and DBU consumption |
| `system.compute` | Cluster and warehouse usage |
| `system.ai` | AI/ML workload data |
| `system.access.audit` | All user actions (if audit logging enabled) |
| `system.data_quality_monitoring` | DQM metrics |

---

## Part 2 — Your workspace access

> **How to use:** Fill in your own workspace details below. Copy this section and personalize it. This is what makes the research system work for you specifically — the shared schemas above work for everyone, but your workspace URL, personal sandbox, and any custom schemas you have access to belong here.

---

### My primary workspace

```
Workspace name: [fill in]
URL: [fill in — e.g., https://adb-XXXX.YY.azuredatabricks.net]
Status: [Connected / Browse only / Write access]
```

### My personal sandbox

```
Catalog: [fill in — e.g., users.your_name or home_your_name]
Schema: [fill in]
Notes: [e.g., "safe to write intermediate tables here"]
```

### Dogfood / staging workspace (if applicable)

```
URL: [fill in — e.g., https://dogfood.staging.databricks.com]
Org ID: [fill in]
Access level: [browse / write / TBD]
```

### Custom schemas I have access to

| Schema | What it contains | Notes |
|--------|-----------------|-------|
| [fill in] | [fill in] | [fill in] |

### Go-links I use frequently

| Go-link | What it is |
|---------|-----------|
| [fill in] | [fill in] |

---

*Part 1 is shared and maintained centrally. Part 2 is yours — keep it updated as your access changes. Used by: `agents/agent-quantitative.md`. Companion: `intel/internal-intel.md` § Logfood Quick Reference.*
