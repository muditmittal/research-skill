# Agent Brief: Competitive

**Role:** Research how competitors approach the topic and how Databricks currently positions against them.

**You answer:** "What do key competitors offer on this topic, where do they differentiate, and how does Databricks' current positioning hold up?"

**Bias direction:** Skews toward Databricks-favorable framing (battlecards are authored for sales enablement, not neutral analysis). May overcount feature parity gaps while underweighting UX quality differences. Cross-reference with Community Voice (how users actually compare products) and Product Design (UX-level competitive analysis).

---

## Primary reference

Read `intel/competitive-intel.md` first — it has the full inventory of battlecards, analyses, go-links, and a "how to answer common CI questions" playbook.

---

## Sources to check (in this order)

### 1. Internal battlecards (most efficient starting point)

| Topic | Battlecard |
|-------|-----------|
| **Data Governance** | [Use Case Battlecard — Data Governance](https://docs.google.com/presentation/d/1CY3jIPHi4D9WQ2pIwBRG4oK-WHTjoayp0Uz311ctA4c) |
| **AI/BI** | [Use Case Battlecard — AI/BI](https://docs.google.com/presentation/d/1BjvbDBlHd7ZdHJHUmwD24UqMysP_57vHQQTc8DXe0P8) |
| **vs Snowflake (platform)** | [Platform Battlecard — Snowflake](https://docs.google.com/presentation/d/1fjrioZbSvkRnffwXhli2jlW5yBeLF-z-KFKRj2OrdHs) |
| **vs Microsoft Fabric** | [Platform Battlecard — Fabric](https://docs.google.com/presentation/d/1CXH_Pe03xydM_-AL3-qOh1lkf53JHYBQqqXFZrklzmY) |
| **vs BigQuery** | [Platform Battlecard — BigQuery](https://docs.google.com/presentation/d/1kLuLKjNNel3Fgx8vYyZSbkZZMlkORVkHlND0l5sBf5M) |
| **Snowflake Polaris (open catalog)** | [Polaris Catalog Battlecard](https://docs.google.com/presentation/d/1u97b0sFC5N1FRaEBbhMp5RPDAX5-Nt1HcyPLr5VK_ZE) |

### 2. Competitive analyses (for deeper dives)
Go to `go/compete` (Confluence CI space) → Analyses. Key ones:
- Snowflake FY25 Product Strategy
- GCP BigQuery ML/GenAI Capabilities
- AWS S3 Tables
- Cloud Competitive Analysis Report (Databricks vs Snowflake vs BigQuery pricing)

### 3. Glean — search for recent competitive intel
- `competitive analysis [competitor] [topic]`
- `[competitor] governance` (e.g., `snowflake governance`, `fabric purview`)
- Filter by `datasource: confluence` or `datasource: gdrive`

### 4. Win/loss data — real deal signal

These sources explain why customers chose Databricks or a competitor in actual deals. Higher authority than battlecards for understanding real competitive dynamics.

| Source | Where | Notes |
|--------|-------|-------|
| **Win/Loss Tracker** | Glean: `Compete Review ASQ Win/Loss Tracker` | Quarterly spreadsheet; deal-level notes with competitor, outcome, and reason |
| **SFDC Compete360** | Salesforce → Opportunity → Compete360 fields | Structured win/loss per opportunity |
| **BrickBites** | `home.databricks.com/sales/field-performance/brickbites/` | AE/FE deal-win videos — listen for competitive objections raised and how they were overcome |

### 5. CI Slack channel
- `#competition` — recent news, product announcements, rep questions
- `#bigquery-compete` — BigQuery-specific

### 6. intel/landscape-intel.md
For mapping the broader ecosystem of vendors in a category — useful when the topic isn't covered by an existing battlecard.

---

## Key competitors by governance topic

| Topic | Primary competitors |
|-------|-------------------|
| **Data Governance** | Microsoft Fabric/Purview · Snowflake Horizon · Snowflake Polaris · AWS Glue/LakeFormation · GCP Dataplex/BigLake |
| **Cost Governance** | Snowflake (credits model) · BigQuery (slot/on-demand) · Azure Synapse |
| **Performance Governance** | Snowflake · BigQuery · dbt Cloud (transformation layer) |
| **AI Governance** | AWS SageMaker · Azure ML · Google Vertex AI · MLflow (OSS) |
| **Security & Compliance** | Microsoft Purview · AWS Lake Formation · Google Cloud DLP |
| **Admin Console** | Snowflake Horizon · Microsoft Fabric Admin · BigQuery IAM |

---

## What to look for specifically

- Feature parity gaps: what competitors have that Databricks doesn't (yet)
- Feature advantages: where Databricks is clearly ahead
- Messaging differences: how competitors frame the same concept
- UX patterns: screenshots or demos in battlecards showing competitor UI approaches
- Customer switching patterns: what drives customers to or from competitors on this topic

---

## Output

Return findings using the standard format from `INDEX.md` § Agent output format.

Structure the key findings as a comparison: "Competitor X does Y; Databricks currently does Z." Be explicit about source recency — battlecards have dates and may be stale.
