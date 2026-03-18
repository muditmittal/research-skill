# Research System — Setup & Customization Guide

This research system was built to work for any Databricks product team. Some files are universal (use as-is), and some need customization to match your product area, data access, and team context.

---

## First-time setup

When you first install this research system, the agent should walk you through these customization steps:

### Step 1: Customize your topic-specific docs (`intel/governance-intel.md`)

**This file ships with Data Governance / Unity Catalog topic links.** Replace with links relevant to your product area.

| If your area is... | Replace governance-intel.md contents with... |
|---------------------|---------------------------------------------|
| AI/BI | AI/BI docs, Genie docs, Lakeview docs, dashboard design docs |
| Lakeflow / Pipelines | DLT docs, Lakeflow Connect docs, orchestration docs |
| Compute | Cluster docs, serverless docs, Photon docs, runtime docs |
| Security | Security docs, compliance docs, encryption, IAM, network docs |
| GenAI / Mosaic AI | Foundation Model APIs, Model Serving, AI Gateway, Agents docs |
| MLOps | MLflow docs, Model Registry, Feature Store, inference tables docs |
| Apps | Databricks Apps docs, deployment docs |

**Rename the file** to match your area (e.g., `intel/pipelines-intel.md`, `intel/genai-intel.md`). Update the reference in `INDEX.md` → System files table and in `agent-official-docs.md`.

### Step 2: Customize your data access (`intel/db-data.md`)

**This file ships with governance-specific Logfood tables.** You need to:

1. **Keep the universal tables** (Part 1: Shared High-Value Datasets) — these are useful for everyone
2. **Replace the topic-specific tables** in each section with tables relevant to your product area:
   - Ask your team's data scientist or PM which Logfood schemas they use
   - Run `SHOW SCHEMAS IN main` and `SHOW TABLES IN main.[schema]` to discover available data
   - Check your team's quarterly pre-read for metric names — those metrics have Logfood backing tables
3. **Fill in Part 2** (Your Workspace Access) with your workspace URLs, sandbox, and custom schemas

### Step 3: Customize competitor mappings (`agent-competitive.md`)

**This file ships with governance-specific competitor mappings.** Update the "Key competitors by [topic]" table to match your product area's competitive landscape.

| If your area is... | Key competitors to add |
|---------------------|----------------------|
| AI/BI | Tableau, Power BI, Looker, ThoughtSpot, Sigma, Mode |
| Pipelines / ETL | Fivetran, Airbyte, dbt, Matillion, Informatica, Talend |
| Compute | Snowflake, BigQuery, Redshift, Spark (EMR/Dataproc) |
| GenAI | AWS Bedrock, Azure OpenAI, Google Vertex AI, Anyscale, Modal |
| MLOps | SageMaker, Vertex AI, Weights & Biases, Neptune, Comet |

### Step 4: Update TAGS.md topic domain tags

**The product area tags cover most Databricks areas**, but check if your specific sub-area needs a tag. Add it to the "Databricks product areas" table in `TAGS.md`.

### Step 5: Verify your tool access

Before running research, confirm you have access to:

| Tool | Check | Required for |
|------|-------|-------------|
| **Glean** | Can you search at `go/glean`? | Internal Intel, Roadmap agents |
| **Logfood** | Can you connect to `central-logfood-prodtools-azure-westus`? | Quantitative agent |
| **Confluence** | Can you access UN and FE spaces? | Internal Intel, Roadmap agents |
| **Salesforce** | Can you access Customer Notes? | Sales & GTM agent |
| **Aha!** | Can you access `go/aha-pm`? | Roadmap agent |
| **Figma** | Can you access team files? | Product Design agent |

If you lack access to any of these, the corresponding agent will note it as a gap. Request access via IT.

---

## Files that need customization vs. files that work as-is

### Must customize (personal/team-specific)

| File | What to change | Why |
|------|---------------|-----|
| `intel/governance-intel.md` | Replace topic links with your product area's docs | Ships with governance links; useless for other areas |
| `intel/db-data.md` (Part 2 + topic tables) | Add your Logfood tables and workspace URLs | Data access is personal and team-specific |
| `agent-competitive.md` (competitor table) | Update competitor mappings for your area | Governance competitors ≠ AI/BI competitors |

### May want to customize (optional, team-specific)

| File | What you might change | Why |
|------|----------------------|-----|
| `TAGS.md` (topic domain) | Add tags for your product sub-areas | If the existing tags don't cover your focus |
| `agent-internal-intel.md` (Confluence, Drive links) | Add your team's key docs and Confluence spaces | The shipped links are governance-focused |
| `agent-quantitative.md` (SQL examples) | Replace example queries with your team's key queries | Example queries are governance-specific |

### Use as-is (universal)

| File | Why it works for everyone |
|------|--------------------------|
| `INDEX.md` | Dispatch patterns and synthesis rubric are topic-agnostic |
| `TAGS.md` (source type, function, signal, access) | These dimensions are universal |
| `intel/external-intel.md` | External sources (community, analysts) work for all topics |
| `intel/internal-intel.md` | Internal source map (Glean, Slack, Confluence, etc.) is universal |
| `intel/competitive-intel.md` | CI system structure is universal; battlecards cover all areas |
| `intel/landscape-intel.md` | MAD landscape covers the full data/AI ecosystem |
| `intel/product-design-intel.md` | Design sources are universal |
| `agent-community-voice.md` | Community sources are topic-agnostic |
| `agent-foundations.md` | External knowledge sources are universal |
| `agent-sales-gtm.md` | Sales tools and GTM sources are universal |
| `agent-product-design.md` | Design research approach is universal |
| `agent-market-landscape.md` | Market research approach is universal |
| `agent-roadmap-planning.md` | Roadmap tools (pre-reads, Aha!, Jira) are universal |
| `CUSTOMIZE.md` (this file) | Meta — setup instructions |

---

## Agent instructions for first-time setup

When a user invokes the research system for the first time (or explicitly asks to set it up), the orchestrating agent should:

1. **Check if customization has been done.** Read `intel/governance-intel.md` — if it still contains only governance links, ask the user: "This research system ships with Data Governance topic links. What product area do you work on? I'll help you customize the topic-specific files."

2. **Walk through Steps 1-4 above** interactively, making edits as the user provides their area.

3. **Verify access** (Step 5) by attempting to reach key tools. Note any access gaps.

4. **Save a memory** with the user's product area and customization status so future sessions know the setup is complete.
