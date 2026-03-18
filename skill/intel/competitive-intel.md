# Competitive Intelligence — Internal Resources & Playbook

A self-contained guide for anyone at Databricks doing competitive research. Covers where to find CI resources, how to answer common question types, and how to stay current.

Tags: `#competitive` `#internal` `#battlecard` `#pmm` `#field-eng`

---

## Where to go first

| Resource | Link | What's there |
|----------|------|-------------|
| **Main hub** | `go/compete` | All battlecards, analyses, newsletters, competitor matrix — start here |
| **GenAI compete** | `go/genai/compete` | GenAI-specific competitive content |
| **Snowflake compete** | `go/snowflake/compete` | Everything vs Snowflake |
| **Fabric compete** | `go/fabric/compete` | Everything vs Microsoft Fabric |
| **GCP compete** | `go/gcp/compete` | Everything vs Google Cloud |
| **UC compete guide** | `go/uc/compete` | Unity Catalog-specific compete playbook |
| **DWH battlecard** | `go/dwh/battle` | Data warehousing use case battlecard |
| **Benchmarks** | `go/competitive/benchmarks` | Performance benchmark data |
| **Newsletter archive** | `go/competitive/newsletter` | Periodic CI updates from the CI team |
| **Competitor product access** | `go/pm-access` / `go/cuj-access` | Get hands-on access to competitor products |
| **Slack** | `#competition` | Live discussion, field questions, competitive news |
| **Contact** | `competitive-intelligence@databricks.com` | CI team direct |

---

## How to answer common CI question types

### "How do we compare to [competitor] on [topic]?"
1. Start at `go/compete` → find the platform battlecard for that competitor
2. Find the use-case battlecard for the topic (e.g., Data Governance, AI/BI)
3. Check for recent deep-dive analysis docs (Confluence CI space → Analyses)
4. Glean: `competitive analysis [competitor] [topic]` — filter `datasource: gdrive` or `datasource: confluence`
5. Check `go/competitive/newsletter` for anything in the past 6 months

### "Why are we winning or losing deals against [competitor]?"
1. Win/Loss Tracker: Glean `Compete Review ASQ Win/Loss Tracker` — quarterly deal-level log
2. SFDC Compete360 fields: Salesforce → Opportunity → Compete360 (requires SFDC access)
3. BrickBites: `home.databricks.com/sales/field-performance/brickbites/` — AE videos on specific competitive wins
4. `#competition` Slack — search for competitor name; field team often surfaces real objections

### "What is [competitor] building / recently shipped?"
1. `go/compete` → Updates/Events section — competitor earnings calls, conference announcements, launches
2. Glean: `[competitor] product announcement [year]` or `[competitor] launch [feature]`
3. `go/competitive/newsletter` — CI team tracks this on a rolling basis
4. External: competitor docs, release notes, and blog posts (search directly)

### "Who are all the players in [market segment]?"
→ Delegate to the **Market Landscape agent** (`intel/landscape-intel.md`). The MAD landscape (~1,200 companies) covers every player in data/AI/ML. Use it to find niche players that battlecards miss.

### "What is the competitive positioning for a design review?"
1. Get the relevant use-case battlecard for messaging frames and competitive differentiators
2. Read the PMM messaging framework if it exists: Glean `messaging framework [product]`
3. `go/tko-decks` — TKO product positioning notes capture how the field is trained to position vs competitors

---

## Battlecard inventory

### Platform battlecards (whole platform vs Databricks)

| Competitor | Link | Notes |
|-----------|------|-------|
| **Snowflake** | [Google Slides](https://docs.google.com/presentation/d/1fjrioZbSvkRnffwXhli2jlW5yBeLF-z-KFKRj2OrdHs) | Includes data governance section |
| **Microsoft Fabric** | [Google Slides](https://docs.google.com/presentation/d/1CXH_Pe03xydM_-AL3-qOh1lkf53JHYBQqqXFZrklzmY) | "Fabric won't offer enterprise data governance for the foreseeable future" |
| **BigQuery** | [Google Slides](https://docs.google.com/presentation/d/1kLuLKjNNel3Fgx8vYyZSbkZZNLkORVkHlND0l5sBf5M) | See also `go/competitive/benchmarks` |
| **Amazon Bedrock** | (Confluence CI space) | GenAI-focused |

### Use case battlecards (specific product areas)

| Use Case | Link | Key competitors |
|----------|------|----------------|
| **Data Governance** ⭐ | [Google Slides](https://docs.google.com/presentation/d/1CY3jIPHi4D9WQ2pIwBRG4oK-WHTjoayp0Uz311ctA4c) | Fabric/Purview · AWS Glue/LakeFormation · Snowflake Horizon · Snowflake Polaris · GCP Dataplex/BigLake |
| **AI/BI** | [Google Slides](https://docs.google.com/presentation/d/1BjvbDBlHd7ZdHJHUmwD24UqMysP_57vHQQTc8DXe0P8) | (updated version at `go/aibi/battle`) |
| **DWH** | [Google Slides](https://docs.google.com/presentation/d/1-P7kEMdUUEIjUPIuSeSDGfA-XLFkEh_G-qtfSGx_WFQ) | Data warehousing use cases |
| **Lakeflow Pipelines** | [Google Slides](https://docs.google.com/presentation/d/1mrGr8NvTO_eTNAVYYAEp0jVl3MxzDLXjAsW6y2SpxfI) | (`go/pipelines/battle`) |
| **Lakeflow Connect** | [Google Slides](https://docs.google.com/presentation/d/1nwIeEXqhoSa_HSP4NraOyoYiR_76RxXRr-DVGCEmb6Y) | Data ingestion (`go/connect/battle`) |
| **Lakebase** | [Google Slides](https://docs.google.com/presentation/d/1R784FiroNX0it0IU3ITtSt7IBX4MVXr3o7JkXdyDeE4) | OLTP/database use cases |
| **Databricks Apps** | `home.databricks.com` | Updated Jan 2026 |
| **Vector Search** | (Confluence CI space) | Vector Search deals |
| **Polaris Catalog** | [Google Slides](https://docs.google.com/presentation/d/1u97b0sFC5N1FRaEBbhMp5RPDAX5-Nt1HcyPLr5VK_ZE) | Snowflake's open catalog vs Unity Catalog |

---

## Deep-dive competitive analyses

| Analysis | Link | Topic |
|----------|------|-------|
| **Snowflake FY25 Product Strategy** | [Google Doc](https://docs.google.com/document/d/1DEpkUe2ERUMF_OcQTPPOJh8sLXUJDQpWyjAn89LP_1w) | Snowflake investor day, June 2024 |
| **GCP BigQuery ML/GenAI Capabilities** | [Google Doc](https://docs.google.com/document/d/1mRWFjD33aXcxwB4vs3QHDE_axmbZefZsO20sUqgHQzI) | BigQuery AI/ML feature analysis |
| **AWS S3 Tables** | [Google Doc](https://docs.google.com/document/d/1X_1WnjO3FBh3JDiAxErKkXK_BhMZd8HjpMUOmDfJw8o) | AWS S3 Tables (vs Delta Lake) |
| **Orchestration Triggers** | [Google Doc](https://docs.google.com/document/d/1IohY45Y3YhiSCbom6mL1c1nYcmGQh-XTgW5pnNuCazA) | Dagster · Prefect · Airflow · Azure Data Factory · Snowflake |
| **Cloud Competitive Analysis Report** | [Google Doc](https://docs.google.com/document/d/1aVg-5JK9wXmPcsHWvVRl_aYCTY_4QTS4kTA_L6eNPgo) | Databricks vs Snowflake vs BigQuery pricing |
| **Competitive Performance Benchmarks** | [Google Slides](https://docs.google.com/presentation/d/1tUkvYDHNvWwQ1FFDvovt17TuN8vfJKlMxvxWHfAeNc) | BigQuery, Snowflake benchmarks |
| **FY26 Industry Data Intelligence Outcome Maps** | [Google Slides](https://docs.google.com/presentation/d/1kSzA3vRVpys3K4mZr2G5rw3orI8efXQ4jHMvLAL5WJs) | CI by industry vertical |
| **Unity Catalog Compete Guide** | [Google Doc](https://docs.google.com/document/d/14Uy0la7nzL1AY3JkHdqLMIZL0P-UOc2qKKD_-rojdnw) | UC positioning vs competitors |

---

## Confluence CI Space structure

The `CI` Confluence space at `go/compete` is organized as:
- **Battlecards** — all battlecards with competitor tags and dates
- **Analyses** — deep-dive docs per competitor or topic
- **Updates/Events** — earnings calls, product launches, conference events
- **Newsletters** — periodic CI digests
- **Competitive assets** — all downloadable assets

---

## Key competitors by product area

### Data Governance (most relevant for UC / governance design work)
| Competitor | Product | Key differentiator vs UC |
|-----------|---------|--------------------------|
| **Microsoft** | Fabric / OneLake / Purview | Fabric lacks enterprise governance depth |
| **Snowflake** | Horizon (governance) + Polaris (open catalog) | Polaris is open-source Apache Iceberg catalog |
| **AWS** | Glue Data Catalog + LakeFormation | AWS-native but siloed |
| **Google** | Dataplex + BigLake | Tightly coupled to GCP |

### AI/BI
| Competitor | Product |
|-----------|---------|
| Microsoft | Power BI / Fabric |
| Snowflake | Cortex Analyst |
| Google | Looker / BigQuery Studio |

### Orchestration / Pipelines
Dagster · Prefect · Airflow · Azure Data Factory · dbt Cloud · Snowflake Tasks

### GenAI Platform
AWS Bedrock · Azure AI · Google Vertex AI

---

## Staying current

- **Weekly:** `#competition` Slack — live questions and news
- **Newsletter:** `go/competitive/newsletter` — periodic CI team digest
- **Earnings events:** CI Confluence space → Updates/Events section
- **Contact:** `competitive-intelligence@databricks.com`

---

*Companion: `intel/landscape-intel.md` for broader ecosystem mapping beyond direct competitors. For win/loss data see also `agents/agent-sales-gtm.md`.*
