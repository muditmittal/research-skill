# Market Intel — MAD Ecosystem & Company Catalog

The data, AI, and ML vendor ecosystem based on the MAD (Machine Learning, AI & Data) landscape by Matt Turck / FirstMark. This file contains the complete ecosystem guide and the full ~1,200 company catalog.

Tags: `#market` `#competitive` `#public` `#analysis`

---

## MAD Sources

| Source | URL | Notes |
|--------|-----|-------|
| **2025 interactive** | https://mad.firstmark.com/ | Canonical 2025 categories and companies |
| **2024 landscape** | https://firstmark.com/story/the-2024-mad-landscape/ | Full 2024 list and analysis |
| **2024 PDF** | https://mattturck.com/landscape/mad2024.pdf | Downloadable reference |
| **2023** | https://api.mattturck.com/mad2023/ | Prior year for trend comparison |

---

## How to Query

Ask Isaac to read or filter this file:
- "Which companies are tagged `governance` and are Public or Series D+?"
- "Show all companies in the `ai-dev` and `agents` categories"
- "List all companies in the Storage-Lakehouse subsection with Relevance = High"

---

## External Analyst Sources

| Analyst | How to search | Best for |
|---------|--------------|---------|
| **Gartner** | `Gartner Magic Quadrant [category] 2025` | Quadrant positioning; enterprise buyer lens |
| **Forrester** | `Forrester Wave [category] Databricks` | Enterprise platform evaluations |
| **IDC** | `IDC market share data governance 2025` | Market sizing, growth rates |
| **Benn Stancil** | https://benn.substack.com/ | Market direction, governance culture |
| **Locally Optimistic** | https://locallyoptimistic.com/ | Analytics and governance trends |
| **Martin Fowler** | https://martinfowler.com/ | Data mesh, architecture patterns |

---

## Supplementary Analysis Files

Past MAD landscape analyses are in `archive/`:
- `archive/MAD-LANDSCAPE-ANALYSIS.md` — category trends, consolidation patterns, emerging players
- `archive/MAD-LANDSCAPE-MULTI-VOICE-SYNTHESIS.md` — multi-perspective analyst synthesis

These reflect the landscape at a point in time. For current state, re-run analysis against the catalog below.

---

*Used by: `agents/agent-market-landscape.md`. Companion: `intel/competitive-intel.md` for Databricks-specific positioning.*

---

**Column key:**

| Column | Purpose |
|--------|--------|
| **Product** | Company or product name (matches MAD). |
| **Link** | Homepage or product URL (fill from [mad.firstmark.com](https://mad.firstmark.com) or company site). |
| **Relevance** | For our research: `High` / `Medium` / `Low` / `TBD`. |
| **Stage** | Funding/listing: Seed / Series A / Series B / Series C / Series D+ / Public / Subsidiary / OSS. |
| **Tags** | Lifecycle tags (see taxonomy below); comma-separated. |
| **Notes** | What they do well and what stands out vs competitors (1–2 sentences). |
| **MAD** | Year(s) on landscape: 2025, 2024, 2023. |

**Data & AI lifecycle tags (apply all that apply):**

| Tag | Meaning |
|-----|--------|
| `ingestion` | Ingest data from sources into storage or pipelines. |
| `transformation` | Transform, model, or curate data (e.g. dbt, ETL). |
| `orchestration` | Schedule, coordinate, or run workflows/jobs. |
| `storage` | Store data (object, block, file). |
| `storage-lakehouse` | Lakehouse or multi-format table storage (Delta, Iceberg, Hudi). |
| `storage-warehouse` | Data warehouse or analytical SQL store. |
| `storage-vector` | Vector or embedding store for AI/RAG. |
| `streaming` | Event streaming, messaging, or real-time pipelines. |
| `governance` | Data governance, policy, or compliance. |
| `catalog` | Metadata, catalog, lineage, or discovery. |
| `quality` | Data quality, validation, or observability. |
| `observability` | Monitoring, alerting, or ops observability. |
| `security-privacy` | Security, privacy, or access control. |
| `compute` | Compute, runtimes, or execution (e.g. serverless, K8s). |
| `analytics` | Analytics, reporting, or BI. |
| `bi` | Business intelligence or dashboards. |
| `semantic-layer` | Metrics, semantic layer, or unified definitions. |
| `product-analytics` | Product or behavioral analytics. |
| `ml-ops` | MLOps, experiment tracking, or model deployment. |
| `ai-dev` | AI/LLM app development, frameworks, or tooling. |
| `agents` | Agents, tool use, or autonomous AI. |
| `enterprise-ai` | Enterprise AI platform or GenAI at scale. |
| `data-sources` | Data sources, APIs, or enrichment. |
| `marketplace` | Data or model marketplace. |
| `consulting` | Consulting or professional services. |
| `unstructured-etl` | Unstructured or vector ETL / document processing. |
| `integration` | iPaaS, application integration, or CDP. |

---
## Analytics

### BI & Analytics Platforms

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Analytics](https://www.zoho.com/analytics/) | [↗](https://www.zoho.com/analytics/) | Medium | TBD | bi, analytics | Self-service BI and analytics platform; part of Zoho suite (private, profitable). | 2025 |
| [Athena Intelligence](https://www.athenaintel.com/) | [↗](https://www.athenaintel.com/) | High | Seed | analytics, bi, enterprise-ai, agents | AI-native analytics platform (Olympus) with 24/7 Enterprise AI Data Analyst; Seed 2024, $6M 2026. | 2025 |
| [AWS QuickSight](https://aws.amazon.com/quicksuite/quicksight/) | [↗](https://aws.amazon.com/quicksuite/quicksight/) | High | Subsidiary | bi, analytics, enterprise-ai | AWS AI-powered BI: NL queries, dashboards, embedded analytics, 40+ integrations. | 2025 |
| [Databricks LakehouseIQ](https://www.databricks.com/product/lakehouseiq) | [↗](https://www.databricks.com/product/lakehouseiq) | High | Series D+ | bi, analytics, enterprise-ai | NL to SQL and insights on lakehouse. | 2025 |
| [Domo](https://www.domo.com/) | [↗](https://www.domo.com/) | High | Public | bi, analytics, integration | Cloud BI and data platform (NASDAQ); dashboards, integration, AI agentic solutions. | 2025 |
| [Google Looker](https://looker.com/) | [↗](https://looker.com/) | High | Subsidiary | bi, semantic-layer, analytics | BI and semantic layer; part of Google Cloud. | 2025 |
| [Google Looker + Gemini](https://www.looker.com/) | [↗](https://www.looker.com/) | High | Subsidiary | bi, semantic-layer, analytics, enterprise-ai | Gemini in Looker for conversational analytics and natural-language insights (GA 2025). | 2025 |
| [Hex](https://hex.tech/) | [↗](https://hex.tech/) | High | Series C | analytics, bi | Collaborative analytics and data science; integrates Snowflake, Databricks, dbt; $70M Series C (2025). | 2025 |
| [Julius](https://julius.ai/) | [↗](https://julius.ai/) | High | Seed | analytics, bi, enterprise-ai, ai-dev | AI data analyst, NL over data; 2M+ users, Seed $10M (2025); used in Harvard course. | 2025 |
| [Microsoft Power BI](https://powerbi.microsoft.com/) | [↗](https://powerbi.microsoft.com/) | High | Subsidiary | bi, analytics | Market share leader; DAX and DirectLake. | 2025 |
| [Microsoft Power BI + Copilot](https://powerbi.microsoft.com/en-us/) | [↗](https://powerbi.microsoft.com/en-us/) | High | Subsidiary | bi, analytics, enterprise-ai | Copilot for Power BI GA 2024; NL report creation, summarization, and data exploration. | 2025 |
| [Omni](https://www.exploreomni.com/) | [↗](https://www.exploreomni.com/) | TBD | TBD | analytics, bi | — | 2025 |
| [Oracle Analytics Cloud](https://www.oracle.com/analytics/) | [↗](https://www.oracle.com/analytics/) | High | Subsidiary | bi, analytics | Cloud-native analytics with NL, ML, and OCI integration; Gartner Leader 2025. | 2025 |
| [Qlik Staige](https://www.qlik.com/us/) | [↗](https://www.qlik.com/us/) | High | TBD | bi, analytics, enterprise-ai | Qlik’s AI suite for data foundations and Insight Advisor; Qlik private (PE-owned). | 2025 |
| [Salesforce CRM Analytics](https://www.salesforce.com/analytics/crm/) | [↗](https://www.salesforce.com/analytics/crm/) | High | Subsidiary | bi, analytics, product-analytics | CRM-native analytics and Einstein; part of Salesforce. | 2025 |
| [SAP Analytics Cloud](https://www.sap.com/products/data-cloud/cloud-analytics.html) | [↗](https://www.sap.com/products/data-cloud/cloud-analytics.html) | High | Subsidiary | bi, analytics | BI, planning, and predictive; Joule copilot; part of SAP BTP. | 2025 |
| [Sigma Computing](https://www.sigmacomputing.com/) | [↗](https://www.sigmacomputing.com/) | High | Series D | bi, analytics | Cloud-native BI, Snowflake-native; $200M Series D (2024). | 2025 |
| [Snowflake Cortex Analyst](https://www.snowflake.com/) | [↗](https://www.snowflake.com/) | High | Public | bi, analytics, enterprise-ai | NL analytics on Snowflake data; part of Snowflake (public). | 2025 |
| [Strategy](https://www.microstrategy.com/en) | [↗](https://www.microstrategy.com/en) | High | Public | bi, analytics, semantic-layer | Strategy One and Mosaic universal semantic layer; rebrand from MicroStrategy, NASDAQ MSTR. | 2025 |
| [Tableau](https://www.tableau.com/) | [↗](https://www.tableau.com/) | High | Subsidiary | bi, analytics | BI and visualization; owned by Salesforce. | 2025 |
| [TextQL](https://textql.com/) | [↗](https://textql.com/) | Medium | Seed | analytics, bi, semantic-layer, ai-dev | AI analyst Ana, NL over data and Slack; Seed $4.1M (2024). | 2025 |
| [ThoughtSpot](https://www.thoughtspot.com/) | [↗](https://www.thoughtspot.com/) | High | Series D+ | bi, analytics, ai-dev | Search and AI-driven analytics. | 2025 |
| [Wisdom AI](https://www.wisdom.ai/) | [↗](https://www.wisdom.ai/) | TBD | TBD | analytics, bi | — | 2025 |
| [Zoho](https://www.zoho.com/analytics/) | [↗](https://www.zoho.com/analytics/) | Medium | TBD | bi, analytics | Self-service BI; Zoho Corp private, no separate funding. | 2025 |

### Experimentation & Causal

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [ABTasty](https://www.abtasty.com/) | [↗](https://www.abtasty.com/) | Medium | Series C | product-analytics | Digital experience optimization, A/B testing, personalization; $64M raised. | 2025 |
| [Adobe Target](https://business.adobe.com/products/target.html) | [↗](https://business.adobe.com/products/target.html) | High | Subsidiary | product-analytics | A/B testing and personalization; part of Adobe Experience Cloud. | 2025 |
| [Amplitude Experiment](https://amplitude.com/amplitude-experiment) | [↗](https://amplitude.com/amplitude-experiment) | High | Public | product-analytics, analytics | Part of Amplitude Digital Optimization System; NASDAQ AMPL. | 2025 |
| [Ax](https://github.com/facebook/Ax) | [↗](https://github.com/facebook/Ax) | Medium | OSS | ml-ops, analytics | Meta’s adaptive experimentation and Bayesian optimization; GitHub facebook/Ax. | 2025 |
| [CausalML](https://github.com/uber/causalml) | [↗](https://github.com/uber/causalml) | Medium | OSS | analytics | Uber’s causal inference and uplift modeling; GitHub uber/causalml. | 2025 |
| [Conductrics](https://www.conductrics.com/) | [↗](https://www.conductrics.com/) | Low | Seed | product-analytics | A/B testing, ML personalization, surveys; ~$330K seed. | 2025 |
| [Convert](https://www.convert.com/) | [↗](https://www.convert.com/) | Low | TBD | product-analytics | A/B testing platform; bootstrapped, no disclosed VC. | 2025 |
| [Datadog Eppo](https://www.geteppo.com/) | [↗](https://www.geteppo.com/) | High | Subsidiary | product-analytics | Eppo by Datadog; warehouse-native experimentation and feature flags, acquired 2025. | 2025 |
| [Google Cloud Vizier](https://cloud.google.com/vertex-ai/docs/vizier/overview) | [↗](https://cloud.google.com/vertex-ai/docs/vizier/overview) | Medium | Subsidiary | ml-ops, compute | Vertex AI hyperparameter tuning and black-box optimization. | 2025 |
| [Kameleoon](https://www.kameleoon.com/) | [↗](https://www.kameleoon.com/) | Medium | Series A | product-analytics | AI-driven personalization and experimentation; €5M Series A, 500+ European customers. | 2025 |
| [Microsoft DoWhy](https://www.microsoft.com/en-us/research/project/dowhy/) | [↗](https://www.microsoft.com/en-us/research/project/dowhy/) | Medium | OSS | analytics | Microsoft Research causal inference library; py-why/dowhy, MIT. | 2025 |
| [Microsoft EconML](https://www.microsoft.com/en-us/research/project/econml/) | [↗](https://www.microsoft.com/en-us/research/project/econml/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Mixpanel Experiment](https://mixpanel.com/platform/experiments/) | [↗](https://mixpanel.com/platform/experiments/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Monetate SiteSpect](https://monetate.com/) | [↗](https://monetate.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [OpenAI Statsig](https://www.statsig.com/) | [↗](https://www.statsig.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Optimizely](https://www.optimizely.com/) | [↗](https://www.optimizely.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [PyMC](https://github.com/pymc-devs/pymc) | [↗](https://github.com/pymc-devs/pymc) | TBD | TBD | (see taxonomy) | — | 2025 |
| [VWO](https://vwo.com/) | [↗](https://vwo.com/) | TBD | TBD | (see taxonomy) | — | 2025 |

### Headless / Embedded BI & Semantic Layer

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Atscale](https://www.atscale.com/) | [↗](https://www.atscale.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Cube](https://cube.dev/) | [↗](https://cube.dev/) | TBD | Series B | semantic-layer, analytics | — | 2025 |
| [dbt Labs MetricFlow](https://docs.getdbt.com/docs/build/about-metricflow) | [↗](https://docs.getdbt.com/docs/build/about-metricflow) | TBD | TBD | (see taxonomy) | — | 2025 |
| [dbt Labs Semantic Layer](https://www.getdbt.com/product/semantic-layer) | [↗](https://www.getdbt.com/product/semantic-layer) | TBD | Series D+ | semantic-layer, transformation | — | 2025 |
| [Equals](https://equals.app/) | [↗](https://equals.app/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [GoodData](https://www.gooddata.com/) | [↗](https://www.gooddata.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Google LookML](https://docs.cloud.google.com/looker/docs/what-is-lookml) | [↗](https://docs.cloud.google.com/looker/docs/what-is-lookml) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Lightdash](https://www.lightdash.com/) | [↗](https://www.lightdash.com/) | TBD | Series A | bi, semantic-layer | — | 2025 |
| [Luzmo](https://www.luzmo.com/) | [↗](https://www.luzmo.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Metabase](https://www.metabase.com/) | [↗](https://www.metabase.com/) | TBD | Series B | bi, semantic-layer | Open-source BI; self-hosted and cloud. | 2025 |
| [Mozart Data](https://www.mozartdata.com/) | [↗](https://www.mozartdata.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Preset](https://preset.io/) | [↗](https://preset.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Rill](https://www.rilldata.com/) | [↗](https://www.rilldata.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Trace Metric Trees](https://www.hellotrace.io/) | [↗](https://www.hellotrace.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Zenlytic](https://www.zenlytic.com/) | [↗](https://www.zenlytic.com/) | TBD | TBD | (see taxonomy) | — | 2025 |

### Product Analytics

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Amplitude](https://amplitude.com/) | [↗](https://amplitude.com/) | TBD | Public | product-analytics, analytics | — | 2025 |
| [Avo](https://www.avo.app/) | [↗](https://www.avo.app/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Contentsquare](https://contentsquare.com/) | [↗](https://contentsquare.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Fullstory](https://www.fullstory.com/) | [↗](https://www.fullstory.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Gainsight](https://www.gainsight.com/) | [↗](https://www.gainsight.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Glassbox](https://www.glassbox.com/) | [↗](https://www.glassbox.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Heap](https://heap.io/) | [↗](https://heap.io/) | TBD | Subsidiary | product-analytics, analytics | — | 2025 |
| [Kubit](https://kubit.ai/) | [↗](https://kubit.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Logrocket](https://logrocket.com/) | [↗](https://logrocket.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Loops](https://www.getloops.ai/) | [↗](https://www.getloops.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Mixpanel](https://mixpanel.com/) | [↗](https://mixpanel.com/) | TBD | Public | product-analytics, analytics | — | 2025 |
| [mparticle analytics](https://www.mparticle.com/) | [↗](https://www.mparticle.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Pendo](https://www.pendo.io/) | [↗](https://www.pendo.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [PostHog](https://posthog.com/) | [↗](https://posthog.com/) | High | Series D+ | product-analytics, analytics | Open-source product analytics, session replay, feature flags, experiments, and data warehouse integration. Raised $75M Series E at $1.4B valuation (2025); all-in-one developer platform. | 2025 |
| [Quantum Metric](https://www.quantummetric.com/) | [↗](https://www.quantummetric.com/) | High | Series B | product-analytics, analytics | Continuous product design (CPD) platform using real-time customer data for digital experience analytics. $200M Series B at $1B+ valuation (2021); enterprise retail, travel, telecom. | 2025 |
| [Sprig](https://sprig.com/) | [↗](https://sprig.com/) | Medium | Series C | product-analytics | Product research platform: in-product surveys, concept testing, usability testing with AI-powered analysis. $90M total (Series C 2022); a16z, Accel backed. | 2025 |
| [Synerise](https://www.synerise.com/) | [↗](https://www.synerise.com/) | High | Series B | analytics, product-analytics | AI-first behavioral CDP with real-time analytics, personalization, and automated decisions. Poland-based; EIB €25M financing (2025), $23M Series B; 1B+ AI decisions daily. | 2025 |
| [Whatfix](https://whatfix.com/) | [↗](https://whatfix.com/) | Medium | Series D+ | product-analytics | Digital adoption platform: in-app guidance and training for enterprise software. $125M Series E (2024), ~$900M valuation; Warburg Pincus, SoftBank. | 2025 |

## Applications — Enterprise

### Automation & Operations (Agentic RPA)

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AWS Q Business](https://aws.amazon.com/q/business/) | [↗](https://aws.amazon.com/q/business/) | High | Subsidiary | agents, enterprise-ai | AWS GenAI for business: RAG, document Q&A, and connectors to enterprise data. Part of Amazon Web Services; integrates with S3, SharePoint, Salesforce. | 2025 |
| [Celonis Process Intellligence + AI](https://www.celonis.com/) | [↗](https://www.celonis.com/) | High | Series D+ | analytics, orchestration | Process mining and execution management; process intelligence and AI for operations. $13B valuation, $1B Series D (2022); Germany/NYC. | 2025 |
| [Distyl](https://distyl.ai/) | [↗](https://distyl.ai/) | High | Series B | agents, enterprise-ai | Enterprise AI platform with 'Distillery' agent for core operations automation. $175M Series B at $1.8B valuation (2025); 100% production record, Fortune 500 customers. | 2025 |
| [Google Workspace (Gemini) Automations](https://workspace.google.com/blog/product-announcements/new-ai-drives-business-results) | [↗](https://workspace.google.com/blog/product-announcements/new-ai-drives-business-results) | High | Subsidiary | agents, enterprise-ai | Gemini in Google Workspace for writing, summarization, and workflow automation. Part of Google; drives business results via AI in Docs, Sheets, Gmail. | 2025 |
| [HyperScience](https://hyperscience.com/) | [↗](https://hyperscience.com/) | High | Series D | unstructured-etl, agents | Intelligent document processing (IDP) and back-office automation via Hypercell. $80M Series D (2020); FedRAMP High, 99.5% accuracy; Gartner IDP leader. | 2025 |
| [Kognitos](https://www.kognitos.com/) | [↗](https://www.kognitos.com/) | High | Series B | agents, enterprise-ai | Conversational automation: natural language to automate processes (NLPA). $25M Series B (2025), $51M total; banking and healthcare focus. | 2025 |
| [Microsoft Power Automate + Copilot](https://www.microsoft.com/en/power-platform/products/power-automate) | [↗](https://www.microsoft.com/en/power-platform/products/power-automate) | High | Subsidiary | integration, agents | Low-code automation and Copilot for flows, RPA, and process apps. Part of Microsoft Power Platform; broad enterprise adoption. | 2025 |
| [OpenAI Automations](https://openai.com/business/) | [↗](https://openai.com/business/) | High | TBD | agents, enterprise-ai | OpenAI business offerings for automation and assistant use cases. Model provider; enterprise APIs and ChatGPT-driven workflows. | 2025 |
| [Orby AI](https://www.orby.ai/) | [↗](https://www.orby.ai/) | High | Series A | agents, enterprise-ai | 'Large action model' (LAM) for generative process automation from observed workflows. $30M Series A (2024); NEA, Wing, WndrCo; finance, HR, operations. | 2025 |
| [Rossum](https://rossum.ai/) | [↗](https://rossum.ai/) | High | Series A | unstructured-etl | AI document processing for B2B: invoices, POs, cognitive data capture. $100M Series A (2021), General Catalyst; 150+ clients including Bosch, Siemens. | 2025 |
| [Sema4.ai](https://sema4.ai/) | [↗](https://sema4.ai/) | High | Series A | agents, enterprise-ai | Full-stack enterprise AI agent platform; runs natively on Snowflake. $55.5M total (Benchmark, Mayfield, Snowflake Ventures); SAFE AI agents. | 2025 |
| [Servicenow Automation Engine](https://www.servicenow.com/platform/now-assist.html) | [↗](https://www.servicenow.com/platform/now-assist.html) | High | Public | agents, enterprise-ai | Now Assist: GenAI for ITSM, customer service, HR, and workflows on Now Platform. ServiceNow is public (NYSE); broad enterprise footprint. | 2025 |
| [Sola](https://www.sola.ai/) | [↗](https://www.sola.ai/) | High | Series A | agents, enterprise-ai | AI-native back-office automation with self-healing agents; record once, no code. $17.5M Series A (2025), a16z; Fortune 100, AmLaw 100 customers. | 2025 |
| [Thread AI](https://www.threadai.com/) | [↗](https://www.threadai.com/) | High | Series A | agents, enterprise-ai | Composable AI infrastructure (Lemma) for enterprise workflows; ex-Palantir leadership. $20M Series A (2025), Greycroft; 70% faster process response in early customers. | 2025 |
| [UiPath Autopilot](https://www.uipath.com/) | [↗](https://www.uipath.com/) | High | Public | agents, enterprise-ai | RPA leader; Autopilot adds GenAI for discovery and automation. IPO 2021 (PATH); 8,000+ customers, $600M+ revenue at IPO. | 2025 |
| [Workato](https://www.workato.com/) | [↗](https://www.workato.com/) | High | Series D+ | integration, orchestration | Enterprise automation and integration platform; 7,000+ customers. $200M Series E at $5.7B valuation (2021); Battery, Insight, Tiger. | 2025 |
| [Zapier AI Actions](https://zapier.com/) | [↗](https://zapier.com/) | High | TBD | integration | No-code workflow automation and AI actions across 7,000+ apps. Bootstrapped to $5B valuation (2021); profitable, minimal primary funding. | 2025 |
| [Zeta Labs](https://www.zetalabs.ai/) | [↗](https://www.zetalabs.ai/) | Medium | Seed | agents, ai-dev | JACE autonomous AI agent for complex browser-based tasks; AWA-1 model. $2.9M pre-seed (2024); Daniel Gross, Nat Friedman. | 2025 |

### Customer Experience & Support Agents

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Ada](https://www.ada.cx/) | [↗](https://www.ada.cx/) | High | Series C | agents | Automated customer experience (ACX) platform; no-code conversational AI for support. $130M Series C at $1.2B (2021); Zoom, Meta, Square; 1.5B+ interactions (2020). | 2025 |
| [Agency](https://www.agency.inc/) | [↗](https://www.agency.inc/) | High | Series A | agents | B2B customer success AI agent (Kai); scheduling, onboarding, call prep. $20M Series A (Menlo, Sequoia, Snowflake Ventures, Databricks Ventures). | 2025 |
| [Decagon](https://decagon.ai/) | [↗](https://decagon.ai/) | High | Series D+ | agents | AI concierge for customer support across chat, email, voice; 80%+ deflection. $250M Series D at $4.5B (2026); Avis, Block, Affirm, Chime, Deutsche Telekom. | 2025 |
| [Forethought](https://forethought.ai/) | [↗](https://forethought.ai/) | High | Subsidiary | agents | AI-powered customer service; Agatha for case deflection and resolution. Acquired by Zendesk (March 2026); had raised $115M (Series C $65M). | 2025 |
| [Giga](https://giga.ai/) | [↗](https://giga.ai/) | High | Series A | agents | Voice AI for enterprise customer support; 60–98% resolution, <2 weeks deploy. $61M Series A (2025), Redpoint; DoorDash, 99 languages. | 2025 |
| [Gorgias](https://www.gorgias.com/) | [↗](https://www.gorgias.com/) | High | Series C | agents | Ecommerce CX and AI Agent (GPT-4o) for support tickets and actions. $29M Series C-2 (2024); 15,000+ brands, 500M+ tickets; Shopify ecosystem. | 2025 |
| [Intercom](https://www.intercom.com/) | [↗](https://www.intercom.com/) | High | Series D | agents | Conversational support and Fin AI; messaging and help center. ~$1.3B valuation, $240M raised; $343M revenue (2024), 25% growth. | 2025 |
| [Kore.ai](https://kore.ai/) | [↗](https://kore.ai/) | High | Series D | agents | Enterprise conversational and GenAI platform; virtual assistants, 450M interactions/day. $150M Series D (2024), NVIDIA, FTV; PNC, AT&T, Cigna, Airbus. | 2025 |
| [Maven AGI](https://www.mavenagi.com/) | [↗](https://www.mavenagi.com/) | High | Series B | agents | GenAI customer support with enterprise search + GPT-4; 93% autonomous resolution. $50M Series B (2025), $78M total; TripAdvisor, HubSpot, ClickUp. | 2025 |
| [Observe.ai](https://www.observe.ai/) | [↗](https://www.observe.ai/) | High | Series C | agents, analytics | Contact center AI: speech, NLP, real-time coaching and QA. $125M Series C (2022), SoftBank, Zoom; 150% YoY ARR growth. | 2025 |
| [Parloa](https://www.parloa.com/) | [↗](https://www.parloa.com/) | High | Series D+ | agents | Voice-first conversational AI for customer service (AMP platform). $350M Series D at $3B (2026); Allianz, Booking, Swiss Life, SAP; 1B+ interactions. | 2025 |
| [Poly.ai](https://poly.ai/) | [↗](https://poly.ai/) | High | Series D | agents | Human-like voice agents for enterprise calls; 100+ customers, 45 languages. $86M Series D (2025), $750M valuation; Marriott, PG&E, UniCredit, NVIDIA-backed. | 2025 |
| [Salesforce Service Cloud Einstein](https://www.salesforce.com/analytics/crm/) | [↗](https://www.salesforce.com/analytics/crm/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Servicenow Now Assist](https://www.servicenow.com/platform/now-assist.html) | [↗](https://www.servicenow.com/platform/now-assist.html) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Sierra AI](https://sierra.ai/) | [↗](https://sierra.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Wonderful](https://www.wonderful.ai/) | [↗](https://www.wonderful.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Yellow.ai](https://yellow.ai/) | [↗](https://yellow.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Zendesk](https://www.zendesk.com/) | [↗](https://www.zendesk.com/) | TBD | TBD | (see taxonomy) | — | 2025 |

### FinOps & Risk

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Abstract](https://www.abstract.us/) | [↗](https://www.abstract.us/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Alloy](https://www.alloy.com/) | [↗](https://www.alloy.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Brex](https://mad.firstmark.com/brex.com) | [↗](https://mad.firstmark.com/brex.com) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Campfire](https://meetcampfire.com/) | [↗](https://meetcampfire.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Doss](https://www.doss.com/) | [↗](https://www.doss.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Drata](https://drata.com/) | [↗](https://drata.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [GoodDay](https://www.gooddaysoftware.com/) | [↗](https://www.gooddaysoftware.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Greenboard](https://greenboard.com/) | [↗](https://greenboard.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Highbeam](https://www.highbeam.com/) | [↗](https://www.highbeam.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Modern Treasury](https://www.moderntreasury.com/) | [↗](https://www.moderntreasury.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Norm AI](https://www.norm.ai/) | [↗](https://www.norm.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Pigment](https://www.gopigment.com/) | [↗](https://www.gopigment.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Ramp](https://mad.firstmark.com/ramp.com) | [↗](https://mad.firstmark.com/ramp.com) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Rillet](https://www.rillet.com/) | [↗](https://www.rillet.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Riskified](https://www.riskified.com/) | [↗](https://www.riskified.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Secureframe](https://secureframe.com/) | [↗](https://secureframe.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [SentiLink](https://www.sentilink.com/) | [↗](https://www.sentilink.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Stripe Radar](https://stripe.com/radar) | [↗](https://stripe.com/radar) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Unit21](https://www.unit21.ai/) | [↗](https://www.unit21.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Vanta](https://www.vanta.com/) | [↗](https://www.vanta.com/) | TBD | TBD | (see taxonomy) | — | 2025 |

### Human Capital & Talent

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Ashby](https://www.ashbyhq.com/) | [↗](https://www.ashbyhq.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Beamery](https://beamery.com/) | [↗](https://beamery.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Converzai](https://www.converzai.com/) | [↗](https://www.converzai.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Deel](https://www.deel.com/) | [↗](https://www.deel.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [eightfold.ai](https://eightfold.ai/) | [↗](https://eightfold.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Gloat](https://gloat.com/) | [↗](https://gloat.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Juicebox](https://juicebox.ai/) | [↗](https://juicebox.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Mercor](https://mercor.com/) | [↗](https://mercor.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Micro1](https://www.micro1.ai/) | [↗](https://www.micro1.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Paradox](https://www.paradox.ai/) | [↗](https://www.paradox.ai/) | Medium | Subsidiary | enterprise-ai, analytics, integration, agents | Conversational AI recruiting and HR platform (Olivia); automates screening, scheduling, onboarding. Raised $200M Series C (2021); Workday agreed to acquire Paradox. | 2025 |
| [Seekout](https://www.seekout.com/ssd) | [↗](https://www.seekout.com/ssd) | Medium | Series D+ | analytics, enterprise-ai, data-sources, integration | Talent intelligence and recruiting platform with diversity and workforce analytics; used for sourcing and talent data. | 2025 |
| [Tezi](https://tezi.ai/) | [↗](https://tezi.ai/) | Medium | Seed | enterprise-ai, agents, integration | Autonomous AI recruiter (Max) for sourcing, screening, scheduling; $9M seed (2024) from 8VC and Audacious. Early-stage agentic HR tech. | 2025 |
| [Visier](https://www.visier.com/) | [↗](https://www.visier.com/) | High | Series D+ | analytics, bi, enterprise-ai, product-analytics | People analytics and workforce intelligence platform; $125M Series E (2021), unicorn. Strong data/analytics angle for HR data. | 2025 |
| [Workday HiredScore](https://www.workday.com/en-us/products/talent-management/ai-recruiting.html) | [↗](https://www.workday.com/en-us/products/talent-management/ai-recruiting.html) | Medium | Subsidiary | enterprise-ai, analytics, integration | Workday acquired HiredScore (Aug 2024); AI-powered talent orchestration for recruiting and internal mobility, integrated with Workday Skills Cloud. | 2025 |
| [Workera](https://workera.ai/) | [↗](https://workera.ai/) | Medium | Series D+ | analytics, enterprise-ai, quality | AI-powered skills assessments and workforce upskilling analytics; supports data-driven talent and learning decisions. | 2025 |

### Legal AI

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Cicero](https://www.cicerotech.ai/) | [↗](https://www.cicerotech.ai/) | Medium | Series B | enterprise-ai, analytics, unstructured-etl, governance | AI litigation matter analysis: pleading analysis, chronologies, evidence coding. ~$103M total funding; Series B (2025). Document-heavy legal data workflows. | 2025 |
| [Clio](https://www.clio.com/) | [↗](https://www.clio.com/) | Medium | Series D+ | enterprise-ai, analytics, integration | Legal practice management and client intake; established legal tech with analytics and workflow automation for law firms. | 2025 |
| [Darrow](https://www.darrow.ai/) | [↗](https://www.darrow.ai/) | Medium | Series D+ | enterprise-ai, analytics, data-sources | Legal AI for litigation intelligence and case discovery; uses data and AI to surface litigation opportunities and evidence. | 2025 |
| [DoNotPay](https://donotpay.com/) | [↗](https://donotpay.com/) | Low | Series D+ | enterprise-ai, agents, integration | Consumer and SMB legal chatbot for disputes and paperwork; profitable, ~$26.6M raised. Later-stage VC; limited enterprise data relevance. | 2025 |
| [Draftwise](https://www.draftwise.com/) | [↗](https://www.draftwise.com/) | Medium | Series D+ | enterprise-ai, unstructured-etl, integration | Contract drafting and negotiation AI for law firms and legal teams; document-centric legal workflow automation. | 2025 |
| [Eve](https://www.eve.legal/) | [↗](https://www.eve.legal/) | Medium | Series D+ | enterprise-ai, analytics, integration | Legal workflow and matter management with AI-assisted research and analytics for law firms. | 2025 |
| [EvenUp](https://www.evenuplaw.com/) | [↗](https://www.evenuplaw.com/) | Medium | Series D+ | enterprise-ai, analytics, quality | AI for personal injury and mass torts: case valuation, document analysis, and outcome prediction; data-driven legal analytics. | 2025 |
| [Everlaw](https://www.everlaw.com/) | [↗](https://www.everlaw.com/) | Medium | Series D+ | enterprise-ai, analytics, unstructured-etl, governance | Cloud eDiscovery and litigation platform with AI for search, review, and case analytics; document and data management for legal. | 2025 |
| [Evisort](https://www.evisort.com/) | [↗](https://www.evisort.com/) | Medium | Series D+ | enterprise-ai, catalog, governance, unstructured-etl | Contract lifecycle management and AI contract analysis; contract repository and analytics for legal and procurement. | 2025 |
| [Harvey](https://www.harvey.ai/) | [↗](https://www.harvey.ai/) | Medium | Series D+ | enterprise-ai, agents, analytics | Generative AI for law firms: research, drafting, and matter analysis; well-funded legal AI vendor with enterprise adoption. | 2025 |
| [Ironclad AI Assist](https://support.ironcladapp.com/hc/en-us/articles/13740722454935-AI-Assist-Overview) | [↗](https://support.ironcladapp.com/hc/en-us/articles/13740722454935-AI-Assist-Overview) | Medium | Series D+ | enterprise-ai, governance, integration | AI assist within Ironclad’s contract lifecycle platform for drafting, negotiation, and compliance; part of established CLM product. | 2025 |
| [Ivo](https://www.ivo.ai/) | [↗](https://www.ivo.ai/) | Medium | Series D+ | enterprise-ai, analytics, integration | Legal AI for contract and matter workflow; supports legal ops and in-house teams with automation and insights. | 2025 |
| [Legora](https://www.leya.law/) | [↗](https://www.leya.law/) | Medium | Series D+ | enterprise-ai, agents, integration | Legal AI assistant (Leya) for research and workflow; agentic legal tech for law firms and legal teams. | 2025 |
| [LexisNexis Lexis+ AI](https://www.lexisnexis.com/en-us/products/lexis-plus-ai.page) | [↗](https://www.lexisnexis.com/en-us/products/lexis-plus-ai.page) | Medium | Series D+ | enterprise-ai, data-sources, analytics, catalog | Lexis+ AI adds generative AI on top of LexisNexis legal research and data; enterprise incumbent with large legal content catalog. | 2025 |
| [Luminance](https://www.luminance.com/) | [↗](https://www.luminance.com/) | Medium | Series C | enterprise-ai, governance, unstructured-etl | Legal AI for contract generation, negotiation, and analysis; $75M Series C (Feb 2025), total raised >$115M. 700+ organizations, 70+ countries. | 2025 |
| [Robin AI](https://www.robinai.com/) | [↗](https://www.robinai.com/) | Medium | Series B | enterprise-ai, agents, unstructured-etl | Gen AI contract copilot (Word add-in); $26M Series B (Jan 2024) plus $25M follow-on. Hybrid Claude + proprietary contract data; 4x customer growth. | 2025 |
| [Spellbook](https://www.spellbook.legal/) | [↗](https://www.spellbook.legal/) | Medium | Series D+ | enterprise-ai, integration | Contract drafting and review AI integrated with Word and contract workflows for law firms and legal teams. | 2025 |
| [Thomson Reuters CoCounsel](https://www.thomsonreuters.com/en/cocounsel) | [↗](https://www.thomsonreuters.com/en/cocounsel) | Medium | Series D+ | enterprise-ai, data-sources, analytics, catalog | TR’s legal AI assistant built on Westlaw and other TR content; enterprise legal research and workflow with generative AI. | 2025 |
| [vlex Vincent AI](https://vlex.com/vincent-ai) | [↗](https://vlex.com/vincent-ai) | Medium | Series D+ | enterprise-ai, data-sources, analytics | vLex Vincent AI adds generative AI to vLex legal research and global legal data; research and drafting for law firms. | 2025 |

### Sales & Marketing AI (GTM)

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [11x](https://www.11x.ai/) | [↗](https://www.11x.ai/) | Medium | Series B | enterprise-ai, agents, integration, product-analytics | AI SDRs (e.g. Alice, Jordan) for outbound and phone; $50M Series B (Nov 2024) a16z, ~$10M ARR. Digital workers for sales automation. | 2025 |
| [6sense](https://6sense.com/) | [↗](https://6sense.com/) | High | Series D+ | analytics, product-analytics, enterprise-ai, data-sources | Revenue orchestration and ABM platform; account intelligence, intent, and predictive analytics. Strong data/analytics relevance for GTM. | 2025 |
| [Actively AI](https://www.actively.ai/) | [↗](https://www.actively.ai/) | Medium | Series D+ | enterprise-ai, analytics, integration | AI for sales and marketing execution; GTM automation and analytics for revenue teams. | 2025 |
| [AirOps](https://www.airops.com/) | [↗](https://www.airops.com/) | Medium | Series D+ | enterprise-ai, agents, integration | AI workflows and agents for GTM and ops; no-code automation connecting data and tools for sales and marketing. | 2025 |
| [Apollo](https://www.apollo.io/) | [↗](https://www.apollo.io/) | High | Series D+ | data-sources, analytics, product-analytics, integration | Sales intelligence and engagement platform; contact and account data, sequencing, and analytics. Central GTM data and activation layer. | 2025 |
| [Bluefish](https://www.bluefishai.com/) | [↗](https://www.bluefishai.com/) | Medium | Series D+ | enterprise-ai, analytics, integration | AI for B2B sales and marketing; pipeline and engagement analytics and automation for revenue teams. | 2025 |
| [Clay](https://www.clay.com/) | [↗](https://www.clay.com/) | High | Series D+ | data-sources, integration, analytics, enterprise-ai | Data enrichment and lead generation platform; aggregates and enriches contact/company data and integrates with sales tools. Data-centric GTM stack. | 2025 |
| [Collective[i]](https://www.collectivei.com/) | [↗](https://www.collectivei.com/) | Medium | Series D+ | analytics, enterprise-ai, product-analytics | Predictive sales intelligence and revenue analytics; AI for forecasting and pipeline optimization for sales teams. | 2025 |
| [Cresta](https://cresta.com/) | [↗](https://cresta.com/) | Medium | Series D+ | enterprise-ai, analytics, observability | AI for contact center and sales conversations; real-time guidance, coaching, and conversation analytics for revenue and support. | 2025 |
| [Databook](https://trydatabook.com/) | [↗](https://trydatabook.com/) | Medium | Series D+ | analytics, product-analytics, enterprise-ai | Revenue intelligence and sales execution; financial and buying-signal data for strategic accounts and deal intelligence. | 2025 |
| [Evertune](https://www.evertune.ai/) | [↗](https://www.evertune.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Firsthand](https://www.firsthand.ai/) | [↗](https://www.firsthand.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Gong](https://www.gong.io/) | [↗](https://www.gong.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [HubSpot](https://www.hubspot.com/) | [↗](https://www.hubspot.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Momentum](https://www.momentum.io/) | [↗](https://www.momentum.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Outreach](https://www.outreach.io/) | [↗](https://www.outreach.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Profound](https://www.tryprofound.com/) | [↗](https://www.tryprofound.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Regie.ai](https://www.regie.ai/) | [↗](https://www.regie.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Salesloft](https://salesloft.com/) | [↗](https://salesloft.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Unify](https://www.unifygtm.com/) | [↗](https://www.unifygtm.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Vendelux](https://vendelux.com/) | [↗](https://vendelux.com/) | TBD | TBD | (see taxonomy) | — | 2025 |

## Applications — Horizontal

### 3D / Animation / Gaming

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Adobe Substance 3D](https://www.adobe.com/products/substance3d.html) | [↗](https://www.adobe.com/products/substance3d.html) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Anything World](https://anything.world/) | [↗](https://anything.world/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Artificial Agency](https://www.artificial.agency/) | [↗](https://www.artificial.agency/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Decart AI](https://decart.ai/) | [↗](https://decart.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Inworld](https://www.inworld.ai/) | [↗](https://www.inworld.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Kaedim](https://www.kaedim3d.com/) | [↗](https://www.kaedim3d.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Luma AI Genie 3D](https://lumalabs.ai/) | [↗](https://lumalabs.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Move](https://www.move.ai/) | [↗](https://www.move.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [NVIDIA Omniverse](https://www.nvidia.com/en-us/omniverse/) | [↗](https://www.nvidia.com/en-us/omniverse/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Physna](https://www.physna.com/) | [↗](https://www.physna.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Plask](https://plask.ai/en-US) | [↗](https://plask.ai/en-US) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Spline](https://spline.design/) | [↗](https://spline.design/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Unity Muse](https://muse.unity.com/) | [↗](https://muse.unity.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [World Labs](https://www.worldlabs.ai/) | [↗](https://www.worldlabs.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Yellow](https://yellow3d.com/) | [↗](https://yellow3d.com/) | TBD | TBD | (see taxonomy) | — | 2025 |

### Audio & Voice Agents

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AssemblyAI](https://www.assemblyai.com/) | [↗](https://www.assemblyai.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Bland AI](https://www.bland.ai/) | [↗](https://www.bland.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Cartesia](https://cartesia.ai/) | [↗](https://cartesia.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Daily](https://www.daily.co/) | [↗](https://www.daily.co/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [DeepGram](https://deepgram.com/) | [↗](https://deepgram.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Eleven Labs](https://beta.elevenlabs.io/) | [↗](https://beta.elevenlabs.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Hume AI](https://hume.ai/) | [↗](https://hume.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [LiveKit](https://livekit.io/) | [↗](https://livekit.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [OpenAI Realtime API](https://platform.openai.com/docs/api-reference/realtime) | [↗](https://platform.openai.com/docs/api-reference/realtime) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Resemble.ai](https://www.resemble.ai/) | [↗](https://www.resemble.ai/) | Medium | Series A | agents, ai-dev, enterprise-ai | Voice cloning and synthetic voice API for developers and enterprises. B2B focus; fits voice agents and content creation pipelines. | 2025 |
| [Retell AI](https://www.retellai.com/) | [↗](https://www.retellai.com/) | Medium | Series B | agents, ai-dev, enterprise-ai | Conversational voice AI platform for building phone and voice agents. Low-latency, developer-focused; relevant for contact center and voice UX. | 2025 |
| [Sanas](https://www.sanas.ai/) | [↗](https://www.sanas.ai/) | Low | Series B | agents, enterprise-ai | Real-time accent conversion and voice normalization for calls. Niche for communication clarity; limited data-platform overlap. | 2025 |
| [Sesame](https://www.sesame.com/) | [↗](https://www.sesame.com/) | Medium | Series B | agents, ai-dev, enterprise-ai | Conversational voice AI from Oculus co-founders; raised $250M Series B (Oct 2025). CSM model for low-latency, emotional voice; targeting glasses and apps. | 2025 |
| [Sindarin](https://www.sindarin.tech/) | [↗](https://www.sindarin.tech/) | Low | TBD | agents, ai-dev | Voice AI / speech technology company. Limited public footprint for data/AI infrastructure relevance. | 2025 |
| [Suno](https://www.suno.ai/) | [↗](https://www.suno.ai/) | Low | Series B | ai-dev, agents | AI music generation for consumers and creators. Creative/app layer; minimal direct data or ML-infrastructure relevance. | 2025 |
| [Synthflow](https://synthflow.ai/) | [↗](https://synthflow.ai/) | Medium | Seed | agents, ai-dev, enterprise-ai | No-code voice AI for building conversational agents and voice bots. Targets SMBs and use cases like lead qualification. | 2025 |
| [Vapi](https://vapi.ai/) | [↗](https://vapi.ai/) | Medium | Series A | agents, ai-dev, enterprise-ai | Voice agent platform and API for phone and in-app voice assistants. Developer-centric; relevant for voice-first product and contact center AI. | 2025 |
| [Voicemod](https://www.voicemod.net/) | [↗](https://www.voicemod.net/) | Low | Series A | agents, ai-dev | Real-time voice changer and soundboard for streaming and gaming. Consumer/creator focus; little data/AI infrastructure overlap. | 2025 |

### Code AI & Agents

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [All Hands](https://www.all-hands.dev/) | [↗](https://www.all-hands.dev/) | Low | TBD | ai-dev, agents | Engineering management and alignment tooling. Adjacent to dev workflows; not core data or ML platform. | 2025 |
| [Augment](https://www.augmentcode.com/) | [↗](https://www.augmentcode.com/) | High | Series B | ai-dev, agents, enterprise-ai | Enterprise AI coding assistant (formerly Codeium). Full codebase-aware agent; relevant for developer productivity and secure, governed code gen. | 2025 |
| [AWS Q Developer](https://aws.amazon.com/codewhisperer/) | [↗](https://aws.amazon.com/codewhisperer/) | High | Subsidiary | ai-dev, agents, enterprise-ai, integration | Amazon’s AI developer assistant (CodeWhisperer / Q). Deep integration with AWS; part of broader data and dev ecosystem. | 2025 |
| [Claude Code](https://www.anthropic.com/claude-code) | [↗](https://www.anthropic.com/claude-code) | High | Subsidiary | ai-dev, agents, enterprise-ai | Anthropic’s coding agent and CLI. Tied to Claude models; relevant for code gen and tool use in data/ML workflows. | 2025 |
| [Cline](https://cline.bot/) | [↗](https://cline.bot/) | Medium | OSS | ai-dev, agents | Open-source VS Code extension for AI coding. Community-driven; fits dev and scripting workflows that touch data pipelines. | 2025 |
| [CodeRabbit](https://www.coderabbit.ai/) | [↗](https://www.coderabbit.ai/) | Medium | Series A | ai-dev, agents, quality, enterprise-ai | AI-powered code review in PRs. Improves code quality and security; relevant for data/ML code quality in platform teams. | 2025 |
| [Cognition](https://cognition.ai/) | [↗](https://cognition.ai/) | High | Series B | ai-dev, agents, enterprise-ai | Cognition Labs; Devin autonomous coding agent. High profile in AI dev tools; relevant for automation of data/ML engineering tasks. | 2025 |
| [Continue](https://www.continue.dev/) | [↗](https://www.continue.dev/) | Medium | OSS | ai-dev, agents | Open-source AI coding assistant for IDEs. Local and multi-model; used in data and scripting workflows. | 2025 |
| [Cursor](https://cursor.sh/) | [↗](https://cursor.sh/) | High | Series B | ai-dev, agents, enterprise-ai | AI-first code editor built on VS Code. Central to modern AI-assisted development and data/ML codebases. | 2025 |
| [Diffblue](https://www.diffblue.com/) | [↗](https://www.diffblue.com/) | Medium | Series B | ai-dev, quality, enterprise-ai | AI-generated unit tests (Cover). Improves code quality and coverage; applicable to data and service code. | 2025 |
| [Factory](https://www.factory.ai/) | [↗](https://www.factory.ai/) | Low | TBD | ai-dev, consulting | Software delivery and engineering services. Consulting/outsourcing; tangential to data/AI product landscape. | 2025 |
| [GitHub Copilot](https://github.com/features/copilot) | [↗](https://github.com/features/copilot) | High | Subsidiary | ai-dev, agents, enterprise-ai, integration | Microsoft’s AI pair programmer in GitHub/IDE. Default choice for many teams; integrates with repos and CI used in data pipelines. | 2025 |
| [Google Gemini CLI](https://docs.cloud.google.com/gemini/docs/codeassist/gemini-cli) | [↗](https://docs.cloud.google.com/gemini/docs/codeassist/gemini-cli) | High | Subsidiary | ai-dev, agents, enterprise-ai, integration | Google’s CLI and code-assist powered by Gemini. Part of Google Cloud and developer ecosystem for data and apps. | 2025 |
| [Graphite](https://graphite.dev/) | [↗](https://graphite.dev/) | Low | Series A | ai-dev | Stacked diffs and code review workflow. Developer tooling; not data or ML-specific. | 2025 |
| [Greptile](https://www.greptile.com/) | [↗](https://www.greptile.com/) | Medium | Seed | ai-dev, agents, enterprise-ai | AI codebase understanding and Q&A. Helps onboard and reason over repos; useful for data/ML codebases. | 2025 |
| [Jetbrains](https://www.jetbrains.com/) | [↗](https://www.jetbrains.com/) | Medium | Series D+ | ai-dev, integration | IDE vendor (IntelliJ, PyCharm, etc.) with AI features. Widely used for data and backend development; not primarily an AI company. | 2025 |
| [Kilo Code](https://kilocode.ai/) | [↗](https://kilocode.ai/) | Low | TBD | ai-dev | Early-stage or niche code AI product. Limited visibility for data/AI landscape classification. | 2025 |
| [Lovable](https://lovable.dev/) | [↗](https://lovable.dev/) | Low | Series A | ai-dev, agents | AI app builder (formerly GPT Engineer). Targets fast UI/app creation; consumer and SMB, not data infrastructure. | 2025 |
| [Magic](https://magic.dev/) | [↗](https://magic.dev/) | Medium | Series A | ai-dev, agents, enterprise-ai | AI-powered code generation and editing. Targets production codebases; relevant for app and backend development including data services. | 2025 |
| [OpenAI GPT-5 Codex](https://platform.openai.com/docs/models/gpt-5-codex) | [↗](https://platform.openai.com/docs/models/gpt-5-codex) | High | Subsidiary | ai-dev, agents, enterprise-ai | OpenAI’s code-focused model/product. Part of platform API used for code gen and tool use in data/ML pipelines. | 2025 |
| [Qodo](https://www.qodo.ai/) | [↗](https://www.qodo.ai/) | Low | TBD | ai-dev | Code AI or dev tool. Limited public info for stage and data/AI relevance. | 2025 |
| [Replit](https://replit.com/) | [↗](https://replit.com/) | Medium | Series B | ai-dev, agents, compute, integration | Browser-based IDE and hosted runtimes with AI. Used for education and prototyping; can run data/ML experiments and scripts. | 2025 |
| [Roo Code](https://roocode.com/) | [↗](https://roocode.com/) | Low | TBD | ai-dev | Code AI product. Limited public information for classification. | 2025 |
| [Sourcegraph Cody](https://sourcegraph.com/cody) | [↗](https://sourcegraph.com/cody) | High | Series D+ | ai-dev, agents, enterprise-ai, catalog | Sourcegraph’s AI coding assistant with codebase search. Strong fit for large repos and code discovery; catalog-like value for code. | 2025 |
| [StackBlitz](https://bolt.new/) | [↗](https://bolt.new/) | Low | Series A | ai-dev, compute | Web-based dev environment (WebContainers) and Bolt. Front-end and fullstack focus; minimal direct data/AI infrastructure role. | 2025 |
| [Vercel v0](https://v0.dev/) | [↗](https://v0.dev/) | Medium | Subsidiary | ai-dev, agents | Vercel’s AI-powered UI generator. Speeds front-end and design-to-code; tangential to data platform but part of modern app stack. | 2025 |
| [Windsurf](https://windsurf.com/) | [↗](https://windsurf.com/) | Medium | TBD | ai-dev, agents, enterprise-ai | AI-native code editor by Codeium; focuses on in-IDE coding assistance and agentic workflows. Fits data/AI landscape as developer tooling for AI-augmented engineering. | 2025 |
| [Zed](https://zed.dev/) | [↗](https://zed.dev/) | Medium | Series B | ai-dev, agents, enterprise-ai | High-performance open-source editor in Rust; raised $32M Series B (Sequoia, Aug 2025). Building collaborative AI coding and DeltaDB for contextual code conversations. | 2025 |

### Media Generation

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Adobe Firefly](https://www.adobe.com/products/firefly.html) | [↗](https://www.adobe.com/products/firefly.html) | Medium | Series D+ | enterprise-ai, integration | Adobe's gen AI for imaging, video, and design; Firefly Services and Custom Models target enterprises with brand-safe, indemnified generation. 12B+ generations; used by major brands. | 2025 |
| [Black Forest Labs](https://blackforestlabs.ai/) | [↗](https://blackforestlabs.ai/) | Medium | Series D+ | enterprise-ai | Creator of Flux image models; powers consumer and pro image generation. Relevant to data/AI landscape as model provider for media pipelines and integrations. | 2025 |
| [Canva Magic Studio](https://www.canva.com/) | [↗](https://www.canva.com/) | Medium | Series D+ | enterprise-ai, integration | Canva's AI design and media tools (Magic Studio) for SMB and prosumer. Broad adoption; tangential to data stack but part of enterprise content workflows. | 2025 |
| [Figma AI](https://www.figma.com/) | [↗](https://www.figma.com/) | Medium | Series D+ | enterprise-ai, ai-dev, integration | Figma's AI features for design and dev handoff; ties design to code. Relevant for product/design data and design-system governance in data/AI contexts. | 2025 |
| [Google DeepMind Veo 3](https://deepmind.google/technologies/veo/veo-2/) | [↗](https://deepmind.google/technologies/veo/veo-2/) | High | Series D+ | enterprise-ai, compute | Google DeepMind's video generation model (Veo 2/3); part of Google's AI stack and cloud/Vertex offerings. Direct relevance to AI infrastructure and media pipelines. | 2025 |
| [Hedra](https://www.hedra.com/) | [↗](https://www.hedra.com/) | Low | TBD | enterprise-ai | Character-based video and avatar generation. Niche for data/AI landscape; applicable where synthetic video or avatars are part of content pipelines. | 2025 |
| [HeyGen](https://www.heygen.com/) | [↗](https://www.heygen.com/) | Medium | Series D+ | enterprise-ai | AI avatar and video generation for marketing and L&D. Relevant for enterprise content and training workflows that consume or produce video at scale. | 2025 |
| [Higgsfield](https://higgsfield.ai/) | [↗](https://higgsfield.ai/) | Low | TBD | enterprise-ai | AI video and media generation startup. Early-stage; relevance to data/AI landscape is through potential future enterprise or API use. | 2025 |
| [Kling AI](https://www.klingai.com/global/) | [↗](https://www.klingai.com/global/) | Medium | Series D+ | enterprise-ai | Kuaishou-backed video generation (Kling). Significant in APAC; relevant for global media-gen landscape and video pipeline integrations. | 2025 |
| [Luma AI](https://lumalabs.ai/) | [↗](https://lumalabs.ai/) | Medium | Series D+ | enterprise-ai | Luma Dream Machine and related models for video and 3D. Growing adoption; relevant for creative and synthetic media in data/AI workflows. | 2025 |
| [Midjourney](https://midjourney.com/home/?callbackUrl=%2Fapp%2F) | [↗](https://midjourney.com/home/?callbackUrl=%2Fapp%2F) | Medium | TBD | enterprise-ai | Leading consumer/prosumer image generation; limited enterprise API. Influential in gen AI adoption; indirect relevance to data/AI tooling and content pipelines. | 2025 |
| [Mirage](https://mirage.app/) | [↗](https://mirage.app/) | Low | TBD | enterprise-ai | AI media generation app. Early or niche; relevance to data/AI landscape is through media-gen ecosystem only. | 2025 |
| [Moonvalley](https://www.moonvalley.com/) | [↗](https://www.moonvalley.com/) | Low | TBD | enterprise-ai | AI video generation product. Smaller player in video-gen space; tangential to core data/AI stack unless used in content pipelines. | 2025 |
| [OpenAI Sora 2](https://openai.com/sora) | [↗](https://openai.com/sora) | High | Series D+ | enterprise-ai, compute | OpenAI's flagship video model; available via API and in ChatGPT. Core to AI infrastructure landscape and enterprise media-gen adoption. | 2025 |
| [PhotoRoom](https://www.photoroom.com/) | [↗](https://www.photoroom.com/) | Low | Series D+ | enterprise-ai | AI photo editing and background generation; strong in e-commerce. Relevance is through brand and product imagery in data-driven workflows. | 2025 |
| [Pika](https://pika.art/home) | [↗](https://pika.art/home) | Medium | Series D+ | enterprise-ai | AI video generation (Pika Labs); popular consumer and pro tool. Part of media-gen landscape; enterprise relevance depends on API and integrations. | 2025 |
| [Runway](https://runwayml.com/) | [↗](https://runwayml.com/) | High | Series D+ | enterprise-ai, ml-ops, integration | Runway Gen-3 and tools for video and image; used in film and marketing. Strong enterprise and API traction; relevant for creative AI and media pipelines. | 2025 |
| [Stability.ai](https://stability.ai/) | [↗](https://stability.ai/) | High | Series D+ | enterprise-ai, ml-ops | Stable Diffusion and open models; API and on-prem options. Key for open and controllable media gen in data/AI and ML pipelines. | 2025 |
| [Synthesia](https://www.synthesia.io/) | [↗](https://www.synthesia.io/) | Medium | Series D+ | enterprise-ai | AI avatar and video for training and comms. Enterprise-focused; relevant where L&D and internal content are part of knowledge and analytics workflows. | 2025 |

### Text, Docs & Knowledge Agents

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Anthropic Claude](https://www.anthropic.com/news/claude-3-family) | [↗](https://www.anthropic.com/news/claude-3-family) | High | Series D+ | agents, enterprise-ai, compute | Leading foundation model and API; $30B Series G (2026), $14B ARR. Core to data/AI stack for agents, RAG, and enterprise AI deployments. | 2025 |
| [Coda](https://coda.io/) | [↗](https://coda.io/) | Medium | Series D+ | enterprise-ai, integration, analytics | Doc-database hybrid with blocks and automations; AI for docs and workflows. Relevant for knowledge bases and lightweight data apps in data/AI ecosystems. | 2025 |
| [Dust](https://dust.tt/) | [↗](https://dust.tt/) | High | TBD | agents, enterprise-ai, catalog, integration | AI assistant and agent platform that connects to company data and tools. Direct relevance for enterprise search, knowledge, and data-aware agents. | 2025 |
| [Fathom](https://www.fathom.ai/) | [↗](https://www.fathom.ai/) | Medium | Series D+ | enterprise-ai, integration | Meeting assistant for notes and summaries. Relevant where meeting intelligence feeds into knowledge bases and analytics in data/AI workflows. | 2025 |
| [Fireflies](https://fireflies.ai/) | [↗](https://fireflies.ai/) | Medium | Series D+ | enterprise-ai, integration | Meeting transcription and AI summaries. Fits data/AI landscape as a source of unstructured meeting data and downstream analytics. | 2025 |
| [Glean](https://www.glean.com/) | [↗](https://www.glean.com/) | High | Series D+ | enterprise-ai, catalog, agents, integration | Enterprise search and knowledge discovery across apps and data. Direct relevance for data discovery, governance, and agent-ready knowledge layers. | 2025 |
| [Google Workspace Gemini](https://workspace.google.com/blog/product-announcements/new-ai-drives-business-results) | [↗](https://workspace.google.com/blog/product-announcements/new-ai-drives-business-results) | High | Series D+ | agents, enterprise-ai, integration | Gemini in Gmail, Drive, Docs, Sheets; core to Google's enterprise AI. Relevant for productivity data, governance, and integration with data/BI tools. | 2025 |
| [Granola](https://www.granola.ai/) | [↗](https://www.granola.ai/) | Medium | TBD | agents, enterprise-ai | AI for meetings and async work. Relevance to data/AI is through meeting and collaboration data feeding knowledge and analytics. | 2025 |
| [Guru](https://www.getguru.com/) | [↗](https://www.getguru.com/) | Medium | Series D+ | enterprise-ai, catalog, integration | Knowledge management and wiki with AI; used for internal knowledge. Fits data/AI landscape as structured knowledge source and potential agent backend. | 2025 |
| [Jasper](https://www.jasper.ai/) | [↗](https://www.jasper.ai/) | Medium | Series D+ | enterprise-ai, agents, integration | AI marketing and content platform; brand voice and campaigns. Relevant for content and campaign data in analytics and governance workflows. | 2025 |
| [Lindy](https://www.lindy.ai/) | [↗](https://www.lindy.ai/) | Medium | TBD | agents, enterprise-ai, integration | AI agent platform for tasks and workflows. Relevance to data/AI is through automation and integration with data sources and tools. | 2025 |
| [Manus](https://manus.im/) | [↗](https://manus.im/) | Low | TBD | agents, enterprise-ai | AI assistant/productivity tool. Niche for data/AI landscape unless used as agent layer on top of data or knowledge systems. | 2025 |
| [Microsoft Copilot](https://copilot.microsoft.com/) | [↗](https://copilot.microsoft.com/) | High | Series D+ | agents, enterprise-ai, integration, governance | Copilot across M365, Windows, and Azure; central to Microsoft's AI strategy. Core for enterprise AI, data governance, and integration with data/BI stack. | 2025 |
| [Notion AI](https://www.notion.com/product/ai) | [↗](https://www.notion.com/product/ai) | High | Series D+ | enterprise-ai, agents, catalog, integration | Notion's AI search, writing, and knowledge agent; $11B valuation, 50%+ AI revenue. Strong relevance for knowledge bases and data-aware productivity in data/AI ecosystems. | 2025 |
| [OpenAI ChatGPT](https://openai.com/blog/chatgpt/) | [↗](https://openai.com/blog/chatgpt/) | Medium | Series D+ | analytics, product-analytics, ai-dev, agents, enterprise-ai, security-privacy | Consumer and enterprise LLM application with workspace analytics, native data analysis (tables, charts, Python), and file integrations; relevance is application-layer rather than core data infrastructure. | 2025 |
| [Perplexity](https://www.perplexity.ai/) | [↗](https://www.perplexity.ai/) | Medium | Series D+ | analytics, ai-dev, agents, enterprise-ai, data-sources, integration, security-privacy | Enterprise AI search with internal knowledge search, org file uploads, and connectors (Drive, OneDrive, SharePoint); combines external and internal data for cited answers. | 2025 |
| [Sana](https://sanalabs.com/) | [↗](https://sanalabs.com/) | Medium | Series D+ | analytics, ai-dev, agents, enterprise-ai, product-analytics | AI-native learning platform (Sana Learn) and enterprise automation (Sana agents); includes live dashboards and company knowledge access; now part of Workday. | 2025 |
| [Writer](https://writer.com/) | [↗](https://writer.com/) | Medium | Series D+ | orchestration, ai-dev, agents, enterprise-ai, integration, governance | Enterprise AI platform with Knowledge Graph for company data sources, agentic workflows, and connectors; emphasizes factual accuracy and brand governance. | 2025 |
| [You](https://you.com/) | [↗](https://you.com/) | High | Series D+ | ai-dev, agents, enterprise-ai, data-sources, integration, storage-vector | AI search infrastructure: Web Search API, Research API, Contents API, and vertical indexes for RAG/agents; private RAG with vectorized indexing and multi-model LLM support. | 2025 |

## Applications — Industry

### Aerospace, Defense & Govtech

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Anduril](https://www.anduril.com/) | [↗](https://www.anduril.com/) | Medium | Series D+ | orchestration, streaming, compute, analytics, ml-ops, enterprise-ai, integration | Lattice platform integrates sensor and battlefield data with AI-driven analysis; SDK and APIs for data flow and edge processing; defense-focused, not general data landscape. | 2025 |
| [Boom](https://boomsupersonic.com/) | [↗](https://boomsupersonic.com/) | Low | Series D+ | (see taxonomy) | Supersonic aircraft manufacturer; no material data platform or analytics product for the data landscape. | 2025 |
| [CHAOS Industries](https://www.chaosinc.com/) | [↗](https://www.chaosinc.com/) | Low | TBD | (see taxonomy) | Defense technology company; no significant data platform or analytics offering in the canonical data landscape. | 2025 |
| [Echodyne](https://www.echodyne.com/) | [↗](https://www.echodyne.com/) | Low | Series D+ | (see taxonomy) | Radar hardware and systems; sensor provider rather than data platform or analytics software. | 2025 |
| [Epirus](https://www.epirusinc.com/) | [↗](https://www.epirusinc.com/) | Low | Series D+ | (see taxonomy) | Directed-energy and counter-drone systems; hardware/defense focus with no data platform relevance. | 2025 |
| [Hadrian](https://www.hadrian.co/) | [↗](https://www.hadrian.co/) | Low | Series D+ | (see taxonomy) | Defense manufacturing and factory automation; not a data or analytics platform. | 2025 |
| [Harmattan AI](https://www.harmattan.ai/) | [↗](https://www.harmattan.ai/) | Low | TBD | (see taxonomy) | Defense AI company; no public data platform or analytics product in the data landscape taxonomy. | 2025 |
| [Helsing](https://helsing.ai/) | [↗](https://helsing.ai/) | Medium | Series D+ | analytics, ml-ops, enterprise-ai | Defense AI software for military platforms; data and AI at the edge; vertical defense focus rather than general data infrastructure. | 2025 |
| [Kela](https://kelasys.com/) | [↗](https://kelasys.com/) | Low | TBD | (see taxonomy) | Kelasys (Kela) appears defense/industry focused; no clear data platform or analytics product in public positioning. | 2025 |
| [Mach Industries](https://mach.industries/) | [↗](https://mach.industries/) | Low | TBD | (see taxonomy) | Defense hardware and systems; not a data or analytics platform. | 2025 |
| [Neros](https://www.neros.tech/) | [↗](https://www.neros.tech/) | Low | TBD | (see taxonomy) | Defense technology; no material data platform or analytics offering for the data landscape. | 2025 |
| [Palantir](https://www.palantir.com/) | [↗](https://www.palantir.com/) | High | Series D+ | ingestion, transformation, orchestration, storage, governance, catalog, analytics, bi, ml-ops, enterprise-ai, integration, security-privacy | Foundry is a full-stack data platform: connectivity, ontology, analytics (Fusion, Code Workbook, Quiver), lineage, and governance; Gotham serves government/defense; core to the data landscape. | 2025 |
| [Primer](https://primer.ai/) | [↗](https://primer.ai/) | High | Series D+ | ingestion, transformation, analytics, ml-ops, unstructured-etl, catalog, governance | NLP and text analytics platform: Primer Engines (NER, relation extraction, summarization) and Enterprise Platform for unstructured data at scale with provenance; defense and intelligence use cases. | 2025 |
| [Rebellion](https://rebelliondefense.com/) | [↗](https://rebelliondefense.com/) | Medium | Series D+ | streaming, analytics, ml-ops, integration | SensorOS with PRISM sensor fusion (40+ feeds, 16k+ objects) and IRIS console; real-time tracking and analytics; defense-focused data fusion, not general data platform. | 2025 |
| [Saronic](https://www.saronic.com/) | [↗](https://www.saronic.com/) | Low | Series D+ | (see taxonomy) | Autonomous maritime vessels; hardware and autonomy, not a data or analytics platform. | 2025 |
| [Shield AI](https://shield.ai/) | [↗](https://shield.ai/) | Low | Series D+ | (see taxonomy) | Autonomous drones and V-BAT; robotics and autonomy focus, not a data platform or analytics product. | 2025 |
| [Skydio](https://www.skydio.com/) | [↗](https://www.skydio.com/) | Low | Series D+ | (see taxonomy) | Autonomous drones and computer vision; hardware/robotics, not data infrastructure or analytics. | 2025 |
| [Tycho AI](https://www.tycho.ai/) | [↗](https://www.tycho.ai/) | Low | TBD | (see taxonomy) | Defense AI; no public data platform or analytics offering in the data landscape. | 2025 |
| [Vannevar Labs](https://www.vannevarlabs.com/) | [↗](https://www.vannevarlabs.com/) | Medium | Series D+ | analytics, ml-ops, unstructured-etl, enterprise-ai | Defense AI for NLP, open-source intelligence scanning, and report generation; data and AI for intel workflows, not general data platform. | 2025 |

### Finance

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Anrok](https://www.anrok.com/) | [↗](https://www.anrok.com/) | Low | Series D+ | (see taxonomy) | Sales tax compliance software; vertical finops, not a data platform or analytics infrastructure. | 2025 |
| [Auquan](https://www.auquan.com/) | [↗](https://www.auquan.com/) | Medium | TBD | analytics, data-sources, integration | ESG and financial data/analytics; data-sources and integration angle for the data landscape. | 2025 |
| [Basis](https://www.getbasis.ai/) | [↗](https://www.getbasis.ai/) | Low | Series D+ | agents, enterprise-ai | AI agents for accounting workflows (tax, audit, advisory); execution automation, not a data platform or analytics infrastructure. | 2025 |
| [Endex](https://endex.ai/) | [↗](https://endex.ai/) | Low | TBD | (see taxonomy) | Finance/endex.ai; insufficient public detail to assign data-platform relevance; assumed application-layer. | 2025 |
| [Farsight AI](https://www.farsight-ai.com/) | [↗](https://www.farsight-ai.com/) | Low | TBD | (see taxonomy) | Financial AI; no clear data platform or analytics infrastructure in public positioning. | 2025 |
| [Hebbia](https://www.hebbia.com/) | [↗](https://www.hebbia.com/) | High | Series D+ | ingestion, analytics, ai-dev, agents, enterprise-ai, unstructured-etl, storage-vector | Enterprise document analysis and search; proprietary IR over large doc sets, multi-step workflows, full citation; finance/legal use cases; strong data-landscape relevance. | 2025 |
| [Kensho](https://kensho.com/) | [↗](https://kensho.com/) | High | Series D+ | analytics, data-sources, integration, governance, enterprise-ai | S&P Global division; Kensho LLM-ready API exposes structured financial data to LLMs with grounding and audit trails; data-sources and analytics for the data landscape. | 2025 |
| [Klarity](https://www.klarity.ai/) | [↗](https://www.klarity.ai/) | Low | Series D+ | ai-dev, unstructured-etl | AI contract review and revenue workflows; document automation, not a general data platform. | 2025 |
| [ModelML](https://www.modelml.com/) | [↗](https://www.modelml.com/) | Low | TBD | (see taxonomy) | Finance-focused; no clear data platform or analytics infrastructure in public positioning. | 2025 |
| [Modern Treasury](https://www.moderntreasury.com/) | [↗](https://www.moderntreasury.com/) | Medium | Series D+ | storage, analytics, integration, governance | Payments infrastructure with transaction and ledger data, reporting, and retention; data model and APIs support downstream analytics and reconciliation. | 2025 |
| [Noetica](https://noetica.ai/) | [↗](https://noetica.ai/) | Low | TBD | (see taxonomy) | Finance AI; no clear data platform or analytics product in public positioning. | 2025 |
| [Numeric](https://www.numeric.io/) | [↗](https://www.numeric.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Ocrolus](https://www.ocrolus.com/) | [↗](https://www.ocrolus.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [OpenEnvoy](https://www.openenvoy.com/) | [↗](https://www.openenvoy.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Rogo](https://rogo.ai/) | [↗](https://rogo.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Tabs](https://tabs.inc/) | [↗](https://tabs.inc/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Taktile](https://www.taktile.com/) | [↗](https://www.taktile.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Vic.ai](https://www.vic.ai/) | [↗](https://www.vic.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |

### Healthcare & Life Sciences

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Abridge](https://www.abridge.com/) | [↗](https://www.abridge.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Alaffia Health](https://www.alaffia.ai/) | [↗](https://www.alaffia.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Ambience](https://www.ambiencehealthcare.com/) | [↗](https://www.ambiencehealthcare.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Anterior](https://www.anterior.com/) | [↗](https://www.anterior.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Benchling](https://www.benchling.com/) | [↗](https://www.benchling.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Chai Discovery](https://www.chaidiscovery.com/) | [↗](https://www.chaidiscovery.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Corti](https://www.corti.ai/) | [↗](https://www.corti.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Evolutionary Scale](https://www.evolutionaryscale.ai/) | [↗](https://www.evolutionaryscale.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Freenome](https://www.freenome.com/) | [↗](https://www.freenome.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Hippocratic AI](https://www.hippocraticai.com/) | [↗](https://www.hippocraticai.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Insitro](https://www.insitro.com/) | [↗](https://www.insitro.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Latent Labs](https://www.latentlabs.com/) | [↗](https://www.latentlabs.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Nabla](https://www.nabla.com/) | [↗](https://www.nabla.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [OpenEvidence](https://www.openevidence.com/) | [↗](https://www.openevidence.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Owkin](https://owkin.com/) | [↗](https://owkin.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Recursion](https://www.recursion.com/) | [↗](https://www.recursion.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Tempus](https://www.tempus.com/) | [↗](https://www.tempus.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Tennr](https://www.tennr.com/) | [↗](https://www.tennr.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Viz.ai](https://www.viz.ai/) | [↗](https://www.viz.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |

### Robotics, Autonomy & Industrial

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [1x](https://www.1x.tech/) | [↗](https://www.1x.tech/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Applied Intuition](https://www.appliedintuition.com/) | [↗](https://www.appliedintuition.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Apptronik](https://apptronik.com/) | [↗](https://apptronik.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Aurora](https://aurora.tech/) | [↗](https://aurora.tech/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Bright Machines](https://www.brightmachines.com/) | [↗](https://www.brightmachines.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Cobot](https://www.co.bot/) | [↗](https://www.co.bot/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Covariant](https://covariant.ai/) | [↗](https://covariant.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Exodigo](https://www.exodigo.com/) | [↗](https://www.exodigo.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Figure](https://www.figure.ai/) | [↗](https://www.figure.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Flexion](https://www.flexion.ai/) | [↗](https://www.flexion.ai/) | Low | Series A | ml-ops, ai-dev, enterprise-ai | Series A ($50M, 2025). Builds AI autonomy platform for humanoid robots; relevance to data landscape is limited to ML/AI tooling rather than data platforms or governance. | 2025 |
| [Genesis AI](https://genesis-ai.company/) | [↗](https://genesis-ai.company/) | Low | Seed | ml-ops, ai-dev, compute | Seed ($105M, 2025). Physical AI research lab building universal robotics foundation model and simulation; tangential to data infrastructure and governance. | 2025 |
| [Intrinsic](https://www.intrinsic.ai/) | [↗](https://www.intrinsic.ai/) | Low | Subsidiary | ai-dev, enterprise-ai, integration | Alphabet/Google subsidiary (joined Google 2026). Industrial robotics software (Flowstate); low direct relevance to data platforms or data governance. | 2025 |
| [Nuro](https://www.nuro.ai/) | [↗](https://www.nuro.ai/) | Low | TBD | ai-dev, enterprise-ai, compute | Series E ($203M, 2025), $6B valuation. Autonomous delivery and Nuro Driver; data/ML for autonomy, not a data platform vendor. | 2025 |
| [Physical Intelligence](https://www.physicalintelligence.company/) | [↗](https://www.physicalintelligence.company/) | Low | Series B | ml-ops, ai-dev, enterprise-ai | $400M round (2024), $2.4B valuation. General-purpose robot AI (π0); minimal overlap with data landscape or governance. | 2025 |
| [Sanctuary AI](https://www.sanctuary.ai/) | [↗](https://www.sanctuary.ai/) | Low | TBD | ai-dev, enterprise-ai | General-purpose humanoid robotics; relevance to data platforms and governance is low. | 2025 |
| [Skild AI](https://www.skild.ai/) | [↗](https://www.skild.ai/) | Low | Series C | ml-ops, ai-dev, enterprise-ai, compute | Series C ($1.4B, 2026), $14B+ valuation. Omni-bodied robotics foundation model (Skild Brain); not a data infrastructure or governance vendor. | 2025 |
| [Telekinesis](https://telekinesis.ai/) | [↗](https://telekinesis.ai/) | Low | TBD | ai-dev, enterprise-ai | Robotics/AI company; stage and data-landscape relevance unclear; treated as low relevance for governance and data platforms. | 2025 |
| [Tesla](https://www.tesla.com/) | [↗](https://www.tesla.com/) | Medium | Public | ai-dev, enterprise-ai, compute, analytics | Public. Heavy use of data and ML for autonomy and energy; relevant as data/ML practitioner and scale, not as a data platform or governance vendor. | 2025 |

## Data & AI Consulting

### Data & AI Consulting

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Accenture](https://www.accenture.com/) | [↗](https://www.accenture.com/) | High | Public | consulting, governance, analytics, integration, ml-ops | Major system integrator for data, AI, and cloud; strong in data strategy, governance, and implementation across the data landscape. | 2025 |
| [Artefact](https://www.artefact.com/) | [↗](https://www.artefact.com/) | High | TBD | consulting, analytics, governance, bi, ml-ops | Global data and AI consultancy (Cinven majority, 2025); 1,700+ employees, strong in analytics and AI implementation. | 2025 |
| [BCG X](https://www.bcg.com/bcg-x) | [↗](https://www.bcg.com/bcg-x) | High | Subsidiary | consulting, analytics, governance, ml-ops, enterprise-ai | BCG tech build and digital ventures arm; data, AI, and analytics consulting with implementation and product build. | 2025 |
| [BCGX](https://www.bcg.com/x) | [↗](https://www.bcg.com/x) | High | Subsidiary | consulting, analytics, governance, ml-ops, enterprise-ai | Same entity as BCG X (alternate URL); BCG's digital and data/AI build and consulting subsidiary. | 2025 |
| [BlueOrange](https://blueorange.digital/) | [↗](https://blueorange.digital/) | Medium | TBD | consulting, analytics, integration | Data and digital consultancy; stage unknown; relevant for analytics and integration work within the data landscape. | 2025 |
| [Brooklyn Data Co](https://brooklyndata.co/) | [↗](https://brooklyndata.co/) | High | TBD | consulting, transformation, orchestration, storage, analytics | Data engineering and analytics consultancy; stage not publicly disclosed; relevant for modern data stack and analytics implementations. | 2025 |
| [Bytecode IO](https://bytecode.io/) | [↗](https://bytecode.io/) | Medium | TBD | consulting, integration, transformation | Data/engineering consultancy; stage unknown; relevant for data engineering and integration engagements. | 2025 |
| [DAS42](https://das42.com/) | [↗](https://das42.com/) | High | TBD | consulting, storage-warehouse, governance, analytics, bi | Snowflake Premier Partner; data strategy, migration, governance, and analytics; strong in media, telco, and consumer tech. | 2025 |
| [Data & AI Consulting](https://brooklyndata.co/) | [↗](https://brooklyndata.co/) | High | TBD | consulting, analytics, transformation | Generic section label linking to Brooklyn Data Co; same relevance and focus as Brooklyn Data Co. | 2025 |
| [Data Root Labs](https://datarootlabs.com/) | [↗](https://datarootlabs.com/) | Medium | TBD | consulting, transformation, orchestration, analytics | Data engineering and analytics consultancy; stage unknown; relevant for data pipelines and analytics implementations. | 2025 |
| [Deeper Insights](https://deeperinsights.com/) | [↗](https://deeperinsights.com/) | Medium | TBD | consulting, analytics, ml-ops, bi | UK data and AI consultancy; stage unknown; relevant for analytics and ML/AI delivery. | 2025 |
| [Deloitte AI Institute](https://www2.deloitte.com/ai) | [↗](https://www2.deloitte.com/ai) | High | Subsidiary | consulting, governance, analytics, ml-ops, enterprise-ai | Deloitte's AI research and advisory arm; strong in AI strategy, governance, and enterprise data/AI programs. | 2025 |
| [EY Consulting Services](https://www.ey.com/en_us/consulting/analytics-consulting-services) | [↗](https://www.ey.com/en_us/consulting/analytics-consulting-services) | High | Subsidiary | consulting, governance, analytics, bi, security-privacy | EY analytics and AI consulting; part of global EY organization; relevant for data strategy, governance, and analytics. | 2025 |
| [Fractal](https://fractal.ai/) | [↗](https://fractal.ai/) | High | Public | consulting, analytics, bi, ml-ops, enterprise-ai | Public (listed). AI and analytics consulting; Cogentiq, Crux Intelligence; strong in CPG, retail, financial services, and healthcare. | 2025 |
| [IBM AI Consulting](https://www.ibm.com/consulting/artificial-intelligence) | [↗](https://www.ibm.com/consulting/artificial-intelligence) | High | Subsidiary | consulting, governance, ml-ops, enterprise-ai, integration | IBM's AI and data consulting practice; relevant for enterprise AI, governance, and integration with IBM stack. | 2025 |
| [KPMG Lighthouse](https://advisory-marketing.us.kpmg.com/lighthouse/index.html) | [↗](https://advisory-marketing.us.kpmg.com/lighthouse/index.html) | High | Subsidiary | consulting, governance, analytics, ml-ops, enterprise-ai | KPMG's data, analytics, and AI practice; relevant for data strategy, governance, and AI adoption. | 2025 |
| [Latentview](https://www.latentview.com/) | [↗](https://www.latentview.com/) | High | Public | consulting, analytics, bi, data-sources, integration | Public (NSE/BSE). Digital and data analytics firm; data engineering, predictive analytics, and BI; strong growth and global delivery. | 2025 |
| [LeewayHertz](https://www.leewayhertz.com/) | [↗](https://www.leewayhertz.com/) | Medium | TBD | consulting, ml-ops, ai-dev, integration | Software development and AI/blockchain consultancy; relevant for AI/ML build and integration, less focused on core data platform governance. | 2025 |
| [Meru](https://wearemeru.com/) | [↗](https://wearemeru.com/) | Medium | TBD | consulting, analytics, integration | Data and analytics consultancy; stage unknown; relevant for analytics and data integration projects. | 2025 |
| [phData](https://www.phdata.io/) | [↗](https://www.phdata.io/) | High | TBD | consulting, data-sources, storage-lakehouse, transformation, governance | PE-backed (Gryphon, 2024). Large Databricks and Snowflake partner; data engineering, migration, and data platform implementation; high relevance to data landscape. | 2025 |
| [pwc](https://www.pwc.com/us/en.html) | [↗](https://www.pwc.com/us/en.html) | High | Public | consulting, governance, analytics, security-privacy, enterprise-ai | Big Four firm; data, analytics, and AI advisory; strong in governance, risk, and compliance in the data space. | 2025 |
| [Quantiphi](https://quantiphi.com/) | [↗](https://quantiphi.com/) | High | Series A | consulting, ml-ops, analytics, ai-dev, integration | Series A ($20M, 2019). Applied AI and big data services; Google ML partner; relevant for ML/AI and analytics implementations. | 2025 |
| [QuantumBlack (McKinsey)](https://www.mckinsey.com/capabilities/quantumblack) | [↗](https://www.mckinsey.com/capabilities/quantumblack) | High | Subsidiary | consulting, analytics, ml-ops, governance, enterprise-ai | McKinsey's AI and analytics arm; strategy through implementation; strong in data governance and AI at scale. | 2025 |
| [QuantumBlack AI by McKinsey](https://www.mckinsey.com/capabilities/quantumblack/how-we-help-clients) | [↗](https://www.mckinsey.com/capabilities/quantumblack/how-we-help-clients) | High | Subsidiary | consulting, analytics, ml-ops, governance, enterprise-ai | Same as QuantumBlack (McKinsey); alternate URL; McKinsey's AI and advanced analytics capability. | 2025 |
| [Seattle Data Guy](https://www.seattledataguy.com/) | [↗](https://www.seattledataguy.com/) | Medium | TBD | consulting, analytics, transformation | Boutique data consulting; stage unknown; relevant for data engineering and analytics in smaller or mid-market contexts. | 2025 |
| [Slalom](https://www.slalom.com/) | [↗](https://www.slalom.com/) | High | TBD | consulting, analytics, governance, integration, bi | Large private consulting firm (12,000+); data, cloud, and AI practice; relevant for enterprise data and analytics programs. | 2025 |
| [Thoughtworks](https://www.thoughtworks.com/) | [↗](https://www.thoughtworks.com/) | High | TBD | consulting, analytics, enterprise-ai | Global technology consultancy; taken private by Apax in Nov 2024 ($1.75B). Strong in data strategy, design, and engineering for enterprise. | 2025 |
| [Tiger Analytics](https://www.tigeranalytics.com/) | [↗](https://www.tigeranalytics.com/) | High | TBD | consulting, analytics, ml-ops, enterprise-ai | Bootstrapped full-stack AI and analytics services firm (~$750M revenue, 5K+ employees). Serves Fortune 1000 with data science and ML delivery. | 2025 |
| [Tredence](https://www.tredence.com/) | [↗](https://www.tredence.com/) | High | Series B | consulting, analytics, enterprise-ai | Raised $175M Series B (Advent, 2022). ~3,500 employees; focuses on prescriptive revenue growth management (RGM) and AI agents. | 2025 |
| [Tribe.ai](https://www.tribe.ai/) | [↗](https://www.tribe.ai/) | Medium | Seed | consulting, ai-dev, enterprise-ai | Raised $3.25M seed (Jul 2024) after six years bootstrapped. Network of 500+ AI engineers; helps enterprises build AI products. | 2025 |
| [ZS Associates](https://www.zs.com/solutions/artificial-intelligence-and-analytics) | [↗](https://www.zs.com/solutions/artificial-intelligence-and-analytics) | High | TBD | consulting, analytics, enterprise-ai | Large private consultancy (~13K employees) since 1983. AI and analytics solutions for commercial and strategy use cases. | 2025 |

## Data Sources & APIs

### Company / People / Entity Enrichment

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Apollo](https://www.apollo.io/) | [↗](https://www.apollo.io/) | High | Series C | data-sources, integration | B2B contact and company data platform; $110M Series C (2022), ~$900M valuation. 224M+ contacts with sales engagement tools. | 2025 |
| [Builtwith](https://builtwith.com/) | [↗](https://builtwith.com/) | Medium | TBD | data-sources | Technology stack and website profiling data. Used for technographic enrichment and lead intelligence. | 2025 |
| [Clay](https://www.clay.com/) | [↗](https://www.clay.com/) | High | TBD | data-sources, integration | Data enrichment and workflow platform that aggregates multiple B2B data providers. Popular for sales and marketing enrichment pipelines. | 2025 |
| [Clearbit by Hubspot](https://clearbit.com/) | [↗](https://clearbit.com/) | High | Subsidiary | data-sources, integration | Acquired by HubSpot (Dec 2023). B2B company and contact data APIs; 20M companies, 500M decision-makers, real-time enrichment. | 2025 |
| [Cognism](https://www.cognism.com/) | [↗](https://www.cognism.com/) | High | TBD | data-sources, integration | B2B sales intelligence with strong GDPR-safe coverage for EMEA. Competes with ZoomInfo and Apollo in contact and intent data. | 2025 |
| [Crunchbase](https://www.crunchbase.com/) | [↗](https://www.crunchbase.com/) | High | TBD | data-sources, marketplace | Company, funding, and people data platform. Key source for startup and venture data; used for prospecting and market research. | 2025 |
| [Diffbot](https://www.diffbot.com/) | [↗](https://www.diffbot.com/) | Medium | TBD | data-sources, unstructured-etl | AI-powered web data extraction and knowledge graph; 246M+ organizations. Used for structured extraction from web pages. | 2025 |
| [HG Insights](https://hginsights.com/) | [↗](https://hginsights.com/) | High | Series B | data-sources, analytics | Tech intelligence and revenue growth platform; $20M+ raised, Series B. Used by many Fortune 500 for GTM and spend intelligence. | 2025 |
| [IPInfo](https://ipinfo.io/) | [↗](https://ipinfo.io/) | Medium | TBD | data-sources | IP geolocation and company data APIs. Used for enrichment, fraud, and routing use cases. | 2025 |
| [OpenCorporates](https://opencorporates.com/) | [↗](https://opencorporates.com/) | High | TBD | data-sources | Largest open database of companies (220M+ in 140+ jurisdictions) from official registries. Bulk/commercial access is paid. | 2025 |
| [People Data Labs](https://www.peopledatalabs.com/) | [↗](https://www.peopledatalabs.com/) | High | Series B | data-sources, integration | Workforce and person/company data APIs; $45M Series B (Craft Ventures). Used for enrichment and job-posting data. | 2025 |
| [Truebase](https://profileapi.com/) | [↗](https://profileapi.com/) | Medium | TBD | data-sources | B2B profile and contact data via ProfileAPI. Niche enrichment provider for sales and marketing. | 2025 |
| [Veridion](https://veridion.com/) | [↗](https://veridion.com/) | High | TBD | data-sources, integration | AI-curated business data on 120M+ companies; Match & Enrich and Search APIs. Used for procurement, risk, and market intelligence. | 2025 |
| [Wappalyzer](https://www.wappalyzer.com/) | [↗](https://www.wappalyzer.com/) | Medium | TBD | data-sources | Technology detection (CMS, analytics, frameworks) on websites. Technographic enrichment for sales and research. | 2025 |
| [Zoominfo](https://www.zoominfo.com/) | [↗](https://www.zoominfo.com/) | High | Public | data-sources, integration | Leading B2B contact and intent data platform (NASDAQ: ZI). Enterprise org charts, intent signals, and sales intelligence. | 2025 |

### Data Marketplaces & Discovery

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AWS Data Exchange](https://aws.amazon.com/data-exchange/) | [↗](https://aws.amazon.com/data-exchange/) | High | Subsidiary | marketplace, data-sources | AWS’s data marketplace for discovering and subscribing to third-party data in the cloud. Part of Amazon Web Services. | 2025 |
| [Common Crawl](https://commoncrawl.org/) | [↗](https://commoncrawl.org/) | High | TBD | data-sources | Non-profit open web crawl repository (300B+ pages, 15 years). Hosted on S3; foundational for ML and research datasets. | 2025 |
| [Data.gov](https://data.gov/) | [↗](https://data.gov/) | Medium | TBD | data-sources, marketplace | US federal open data portal. Central discovery for government datasets and APIs. | 2025 |
| [Databricks Marketplace](https://www.databricks.com/product/marketplace) | [↗](https://www.databricks.com/product/marketplace) | High | Subsidiary | marketplace, data-sources | Data and asset marketplace on Databricks; share and consume datasets, models, and solutions across the lakehouse. | 2025 |
| [Dawex](https://www.dawex.com/en/) | [↗](https://www.dawex.com/en/) | Medium | TBD | marketplace, data-sources | Data exchange and marketplace platform for B2B data sharing and monetization; European presence. | 2025 |
| [European Data Portal](https://data.europa.eu/data/datasets?locale=en) | [↗](https://data.europa.eu/data/datasets?locale=en) | Medium | TBD | data-sources, marketplace | Official EU portal for European open data; datasets from institutions and member states, with discovery and standards. | 2025 |
| [Hugging Face Datasets](https://huggingface.co/datasets) | [↗](https://huggingface.co/datasets) | High | Series D | marketplace, data-sources, ml-ops | Hugging Face dataset hub and hosting; $4.5B valuation (Series D 2023). Core for ML datasets and model hosting. | 2025 |
| [Kaggle](https://www.kaggle.com/) | [↗](https://www.kaggle.com/) | High | Subsidiary | marketplace, data-sources, ml-ops | Google-owned platform for datasets, competitions, and notebooks. Key community for data science and public datasets. | 2025 |
| [Narrative](https://www.narrative.io/) | [↗](https://www.narrative.io/) | Medium | TBD | marketplace, data-sources | Data marketplace and delivery platform for buying and selling data. Focus on programmatic data transactions. | 2025 |
| [Nomad Data](https://www.nomad-data.com/) | [↗](https://www.nomad-data.com/) | Medium | TBD | marketplace, data-sources | Connects enterprises with data providers and custom data projects. Data sourcing and discovery marketplace. | 2025 |
| [Snowflake Marketplace](https://www.snowflake.com/data-marketplace/) | [↗](https://www.snowflake.com/data-marketplace/) | High | Subsidiary | marketplace, data-sources | Snowflake’s data marketplace; discover and use third-party data and applications in the Data Cloud. | 2025 |

### Financial & Alternative Data

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Bloomberg](https://www.bloomberg.com/) | [↗](https://www.bloomberg.com/) | High | TBD | data-sources, analytics, bi | Bloomberg L.P. provides terminal, data, and analytics for financial markets. Major source of financial and alternative data. | 2025 |
| [Factset](https://www.factset.com/) | [↗](https://www.factset.com/) | High | Public | data-sources, analytics, bi | Public company (NYSE: FDS). Financial data, analytics, and enterprise solutions for investment professionals. | 2025 |
| [Kaiko](https://www.kaiko.com/) | [↗](https://www.kaiko.com/) | Medium | TBD | data-sources, analytics | Cryptocurrency and digital asset market data. Used for crypto trading, research, and analytics. | 2025 |
| [Kpler](https://www.kpler.com/) | [↗](https://www.kpler.com/) | Medium | TBD | data-sources, analytics | Commodity and trade flow data (e.g. oil, gas, grains). Alternative data for commodities and supply chain. | 2025 |
| [Nasdaq Quandi](https://www.nasdaq.com/nasdaq-data-link) | [↗](https://www.nasdaq.com/nasdaq-data-link) | High | Subsidiary | data-sources, marketplace, integration | Nasdaq Data Link (formerly Quandl) provides financial and alternative datasets via API and marketplace. Key source for quant and enterprise data pipelines; integrated into many analytics platforms. | 2025 |
| [Pitchbook](https://pitchbook.com/) | [↗](https://pitchbook.com/) | High | Subsidiary | data-sources, analytics | VC, PE, and M&A data platform (Morningstar). Standard for deal flow, valuations, and firm-level intelligence; used for sourcing and due diligence in data-driven workflows. | 2025 |
| [S&P Global Capital IQ](https://www.spglobal.com/marketintelligence/en/solutions/sp-capital-iq-pro) | [↗](https://www.spglobal.com/marketintelligence/en/solutions/sp-capital-iq-pro) | High | Subsidiary | data-sources, analytics, integration | Enterprise financial and company data from S&P Global. Deep coverage for research, compliance, and modeling; often used as system of record in governance and reporting. | 2025 |
| [SEC EDGAR](https://www.sec.gov/edgar/search-and-access) | [↗](https://www.sec.gov/edgar/search-and-access) | High | TBD | data-sources, governance | Official SEC filing system; primary source for regulatory filings (10-K, 10-Q, etc.). Essential for compliance, financial data pipelines, and governance use cases. | 2025 |
| [Similarweb](https://www.similarweb.com/) | [↗](https://www.similarweb.com/) | Medium | Public | data-sources, product-analytics, analytics | Web traffic and digital intelligence data. Used for competitive and market analytics; relevance to governance hub is indirect (enrichment and market data). | 2025 |
| [Sparta Commodities](https://www.spartacommodities.com/) | [↗](https://www.spartacommodities.com/) | Low | Series B | data-sources | Commodity market data and analytics. Niche for energy/commodity verticals; limited overlap with core data governance and platform tooling. | 2025 |
| [Tegus by Alphasense](https://www.tegus.com/) | [↗](https://www.tegus.com/) | Medium | Subsidiary | data-sources, analytics | Expert call and transcript data (Alphasense). Used for research and diligence; data-source for downstream analytics rather than platform/infrastructure. | 2025 |
| [Thinknum](https://www.thinknum.com/) | [↗](https://www.thinknum.com/) | Medium | TBD | data-sources, analytics | Alternative data from web and app sources. Supports quant and strategy use cases; ingestion and integration relevance for data pipelines. | 2025 |
| [Vortexa](https://vortexa.com/) | [↗](https://vortexa.com/) | Low | Series C | data-sources | Maritime and energy flow analytics. Vertical-specific; tangential to general data governance and platform landscape. | 2025 |
| [Yipit Data](https://www.yipitdata.com/) | [↗](https://www.yipitdata.com/) | Medium | TBD | data-sources, analytics | Alternative data and research for investors. Data-source and integration use cases; moderate relevance to data stack tooling. | 2025 |

### Geospatial, Satellite & Location

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Atmo](https://www.atmo.ai/) | [↗](https://www.atmo.ai/) | Low | Seed | data-sources | Weather and climate data API. Early-stage; narrow use case for data landscape and governance. | 2025 |
| [Capella Space](https://www.capellaspace.com/) | [↗](https://www.capellaspace.com/) | Low | Public | data-sources | SAR satellite imagery and analytics. Geospatial vertical; limited direct relevance to data platform governance. | 2025 |
| [Carto](https://carto.com/) | [↗](https://carto.com/) | Medium | Series C | data-sources, analytics, integration | Location intelligence and spatial analytics platform. Connects to warehouses and BI; relevant for geo-enabled data pipelines and analytics. | 2025 |
| [Esri](https://www.esri.com/en-us/home) | [↗](https://www.esri.com/en-us/home) | Medium | TBD | data-sources, analytics, storage | Dominant GIS platform; geodatabases and spatial analytics. Enterprise data asset for location data; integration with data stacks common. | 2025 |
| [Google Maps Platform](https://mapsplatform.google.com/) | [↗](https://mapsplatform.google.com/) | High | Subsidiary | data-sources, integration | Maps, Places, and routing APIs from Google. Widely used for geocoding and location enrichment in data pipelines and applications. | 2025 |
| [Here](https://www.here.com/) | [↗](https://www.here.com/) | Medium | Subsidiary | data-sources, integration | Maps and location services (auto consortium). Used for fleet, logistics, and location-aware data; integration relevance. | 2025 |
| [ICEYE](https://www.iceye.com/) | [↗](https://www.iceye.com/) | Low | Series D | data-sources | SAR satellite data and analytics. Geospatial vertical; niche for governance hub context. | 2025 |
| [mapbox](https://www.mapbox.com/) | [↗](https://www.mapbox.com/) | High | Subsidiary | data-sources, integration | Maps, navigation, and location APIs (SoftBank-backed). Common in apps and data pipelines for geospatial enrichment and visualization. | 2025 |
| [Meteo Matics](https://www.meteomatics.com/) | [↗](https://www.meteomatics.com/) | Low | TBD | data-sources | Weather API and environmental data. Specialized source; low centrality to data governance and platform tooling. | 2025 |
| [OpenStreetMap](https://www.openstreetmap.org/#map=4/38.01/-95.84) | [↗](https://www.openstreetmap.org/#map=4/38.01/-95.84) | High | OSS | data-sources, integration | Community-driven global map and geodata. Foundational open data source for location pipelines and geo-enabled analytics. | 2025 |
| [Planet](https://www.planet.com/) | [↗](https://www.planet.com/) | Medium | Public | data-sources | Daily satellite imagery and earth analytics. Used in GIS and analytics pipelines; moderate relevance as geospatial data source. | 2025 |
| [SentinelHub](https://www.sentinel-hub.com/) | [↗](https://www.sentinel-hub.com/) | Medium | TBD | data-sources | Copernicus and EO imagery APIs (Sinergise). Standard for EU earth observation in data pipelines and research. | 2025 |
| [Tomorrow.io](https://www.tomorrow.io/) | [↗](https://www.tomorrow.io/) | Low | Series C | data-sources | Weather intelligence platform. Vertical data source; tangential to core data governance and platform focus. | 2025 |
| [Up42](https://up42.com/) | [↗](https://up42.com/) | Medium | Subsidiary | data-sources, marketplace | Geospatial data and processing marketplace (Airbus). Connects EO data to analytics; marketplace and integration relevance. | 2025 |
| [Vantor](https://vantor.com/) | [↗](https://vantor.com/) | Low | TBD | data-sources | Geospatial or location data provider. Limited visibility; tagged as data-sources with low relevance until clarified. | 2025 |

### Web Search & Crawl APIs

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Apify](https://apify.com/) | [↗](https://apify.com/) | High | Series B | data-sources, ingestion, unstructured-etl, integration | Web scraping and automation platform with actor marketplace. Directly supports ingestion and unstructured data pipelines; strong fit for data landscape. | 2025 |
| [Brave Search API](https://brave.com/search/api/) | [↗](https://brave.com/search/api/) | Medium | Subsidiary | data-sources, integration | Privacy-focused search API from Brave. Alternative to Google/Bing for search-backed data and agent use cases. | 2025 |
| [Crawl4AI](https://github.com/unclecode/crawl4ai) | [↗](https://github.com/unclecode/crawl4ai) | High | OSS | data-sources, ingestion, unstructured-etl | Open-source LLM-oriented web crawler. Used for ingestion and preprocessing of web content into RAG and data pipelines. | 2025 |
| [Exa](https://exa.ai/) | [↗](https://exa.ai/) | High | Series B | data-sources, ai-dev, agents | Neural search API for semantic retrieval from the web. Key for AI/agent and RAG pipelines; high relevance to modern data and AI stacks. | 2025 |
| [Firecrawl](https://github.com/mendableai/firecrawl) | [↗](https://github.com/mendableai/firecrawl) | High | OSS | data-sources, ingestion, unstructured-etl | Open-source crawler that converts pages to markdown/LLM-ready format. Widely used for ingestion and RAG pipelines; Mendable/contextual AI ecosystem. | 2025 |
| [GDELT](https://www.gdeltproject.org/) | [↗](https://www.gdeltproject.org/) | Medium | OSS | data-sources | Open project indexing global news and events. Free bulk data for research and analytics; ingestion and pipeline relevance. | 2025 |
| [Google Custom Search JSON API](https://developers.google.com/custom-search/v1/overview) | [↗](https://developers.google.com/custom-search/v1/overview) | Medium | Subsidiary | data-sources, integration | Programmatic web search from Google. Used for search-backed data retrieval and integration in apps and pipelines. | 2025 |
| [Linkup](https://www.linkup.so/) | [↗](https://www.linkup.so/) | Medium | Seed | data-sources | Job market and labor data. Used for talent and economic indicators; data-source for analytics and research pipelines. | 2025 |
| [Microsoft Bing Web Search](https://www.microsoft.com/en-us/bing/features/web-search/?form=MA13FV) | [↗](https://www.microsoft.com/en-us/bing/features/web-search/?form=MA13FV) | Medium | Subsidiary | data-sources, integration | Bing Web Search API for programmatic search. Alternative to Google for search-backed data and agent integrations. | 2025 |
| [Perplexity Web API](https://www.perplexity.ai/api-platform) | [↗](https://www.perplexity.ai/api-platform) | High | Series B | data-sources, ai-dev, agents, enterprise-ai | AI-powered search and answer API with citations. Directly relevant for RAG, agents, and enterprise AI data retrieval use cases. | 2025 |
| [Reddit API](https://www.reddit.com/dev/api/) | [↗](https://www.reddit.com/dev/api/) | Medium | Public | data-sources, integration | Official API for Reddit content and metadata; used for social data ingestion and research. Reddit is publicly traded. | 2025 |
| [Tavily](https://www.tavily.com/) | [↗](https://www.tavily.com/) | High | Series A | data-sources, ai-dev, agents | AI-optimized search API for agents and RAG pipelines; Series A (2025), widely adopted for retrieval-augmented workflows. | 2025 |
| [YouTube Data API](https://developers.google.com/youtube/v3) | [↗](https://developers.google.com/youtube/v3) | High | Subsidiary | data-sources, integration | Google-owned API for YouTube metadata, search, and channel data; common source for media and engagement analytics. | 2025 |
| [Zyte](https://www.zyte.com/) | [↗](https://www.zyte.com/) | High | TBD | data-sources, ingestion, unstructured-etl | Web scraping and data extraction API; profitable SaaS with venture debt, used for structured extraction at scale. | 2025 |

## Infrastructure — Integrate & Operate

### Cloud Observability

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AWS CloudWatch](https://aws.amazon.com/cloudwatch/) | [↗](https://aws.amazon.com/cloudwatch/) | High | Subsidiary | observability | AWS native metrics, logs, and alarms; default observability layer for data pipelines and workloads on AWS. | 2025 |
| [Azure Monitor](https://azure.microsoft.com/products/monitor) | [↗](https://azure.microsoft.com/products/monitor) | High | Subsidiary | observability | Azure-native monitoring for metrics, logs, and traces; central observability for data and analytics on Azure. | 2025 |
| [Chronosphere](https://chronosphere.io/) | [↗](https://chronosphere.io/) | High | Series C | observability | Cloud-native observability platform built on M3; focuses on scale and cost for metrics and traces. | 2025 |
| [Cisco AppDynamics](https://www.appdynamics.com/) | [↗](https://www.appdynamics.com/) | Medium | Subsidiary | observability | APM and business performance monitoring; Cisco-owned, enterprise application and transaction observability. | 2025 |
| [CloudZero](https://www.cloudzero.com/) | [↗](https://www.cloudzero.com/) | Medium | Series B | observability | Cloud cost intelligence and optimization; ties cost to units and products, adjacent to data pipeline cost observability. | 2025 |
| [Cribl](https://cribl.io/) | [↗](https://cribl.io/) | High | Series D | observability, streaming | Observability pipeline for routing, shaping, and reducing log and metric data; supports streaming and multiple backends. | 2025 |
| [Datadog](https://www.datadog.com/) | [↗](https://www.datadog.com/) | High | Public | observability, security-privacy | Full-stack observability; APM, logs, and security; market leader for infrastructure and application monitoring. | 2025 |
| [Elastic](https://www.elastic.co/) | [↗](https://www.elastic.co/) | High | Public | observability, storage | Elasticsearch and Kibana for search, logging, and APM; public company, used for log analytics and search-backed storage. | 2025 |
| [Finout](https://www.finout.io/) | [↗](https://www.finout.io/) | Medium | Series B | observability | FinOps and cloud cost management; allocates spend across teams and products, adjacent to data platform cost control. | 2025 |
| [Google Cloud Operations Suite](https://cloud.google.com/products/operations) | [↗](https://cloud.google.com/products/operations) | High | Subsidiary | observability | GCP native monitoring, logging, and tracing; default observability for data and analytics on Google Cloud. | 2025 |
| [Grafana Labs](https://grafana.com/) | [↗](https://grafana.com/) | High | Series D | observability, analytics | Observability and dashboards; OSS Grafana and Loki; widely used for metrics, logs, and visualization. | 2025 |
| [GrafanaLabs](https://grafana.com/) | [↗](https://grafana.com/) | High | Series D | observability, analytics | Duplicate of Grafana Labs; same company and product set. | 2025 |
| [honeycomb.io](https://www.honeycomb.io/) | [↗](https://www.honeycomb.io/) | High | Series C | observability | Event-centric observability and high-cardinality tracing; strong for debugging and request-level analysis. | 2025 |
| [Kubecost](https://www.apptio.com/products/kubecost/?src=kc-com) | [↗](https://www.apptio.com/products/kubecost/?src=kc-com) | Medium | Subsidiary | observability | Kubernetes cost visibility and optimization; part of Apptio (VMware/Broadcom), used for container and data workload cost. | 2025 |
| [New Relic](https://newrelic.com/) | [↗](https://newrelic.com/) | High | Public | observability, analytics | APM and full-stack observability; public company, supports metrics, logs, traces, and product analytics. | 2025 |
| [OpenTelemetry](https://opentelemetry.io/) | [↗](https://opentelemetry.io/) | High | OSS | observability | CNCF standard for traces, metrics, and logs; vendor-neutral instrumentation used by most observability platforms. | 2025 |
| [PagerDuty](https://www.pagerduty.com/) | [↗](https://www.pagerduty.com/) | Medium | Public | observability, security-privacy | Incident management and alerting; integrates with observability stacks for on-call and response automation. | 2025 |
| [Sentry](https://sentry.io/) | [↗](https://sentry.io/) | High | Series D | observability, quality | Error and performance monitoring for applications; supports data pipeline reliability and quality use cases. | 2025 |
| [Splunk](https://www.splunk.com/) | [↗](https://www.splunk.com/) | High | Subsidiary | observability, security-privacy | SIEM and machine data platform; Cisco-owned, used for logs, security, and operational analytics. | 2025 |

### Compute

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Amazon EKS / ECS](https://aws.amazon.com/eks/) | [↗](https://aws.amazon.com/eks/) | High | Subsidiary | compute | AWS managed Kubernetes (EKS) and container service (ECS); common compute for data and ML workloads. | 2025 |
| [AWS Lambda](https://aws.amazon.com/lambda/) | [↗](https://aws.amazon.com/lambda/) | High | Subsidiary | compute | Serverless functions on AWS; used for event-driven pipelines, streaming, and lightweight data processing. | 2025 |
| [Azure Functions](https://azure.microsoft.com/products/functions) | [↗](https://azure.microsoft.com/products/functions) | High | Subsidiary | compute | Serverless functions on Azure; supports event-driven and scheduled data and integration workloads. | 2025 |
| [Azure Kubernetes Service](https://azure.microsoft.com/products/kubernetes-service) | [↗](https://azure.microsoft.com/products/kubernetes-service) | High | Subsidiary | compute | Azure managed Kubernetes; standard compute for data pipelines, streaming, and ML on Azure. | 2025 |
| [Cloudflare Workers](https://workers.cloudflare.com/) | [↗](https://workers.cloudflare.com/) | Medium | Subsidiary | compute | Edge serverless compute from Cloudflare; used for APIs, lightweight transforms, and edge data handling. | 2025 |
| [Equinix](https://www.equinix.com/) | [↗](https://www.equinix.com/) | Medium | Public | compute, integration | Data center and interconnection; public company, enables colocation and network for data exchange and hybrid cloud. | 2025 |
| [Fastly](https://www.fastly.com/) | [↗](https://www.fastly.com/) | Medium | Public | compute | Edge CDN and compute; public company, used for edge logic and content delivery adjacent to data flows. | 2025 |
| [Google Cloud Functions](https://cloud.google.com/functions) | [↗](https://cloud.google.com/functions) | High | Subsidiary | compute | Serverless functions on GCP; supports event-driven and HTTP-triggered data and integration workloads. | 2025 |
| [Google Cloud Kubernetes Engine](https://cloud.google.com/kubernetes-engine) | [↗](https://cloud.google.com/kubernetes-engine) | High | Subsidiary | compute | GCP managed Kubernetes (GKE); common compute for data, ML, and streaming workloads on Google Cloud. | 2025 |
| [HPE](https://www.hpe.com/us/en/home.html) | [↗](https://www.hpe.com/us/en/home.html) | Medium | Public | compute | Enterprise servers, HPC, and hybrid cloud; public company, provides on-prem and cloud-adjacent compute for data. | 2025 |
| [Kubernetes](https://kubernetes.io/) | [↗](https://kubernetes.io/) | High | OSS | compute | CNCF orchestration for containers; de facto standard for running data, ML, and streaming workloads at scale. | 2025 |
| [Nvidia Bright Cluster](https://www.nvidia.com/en-us/data-center/bright-cluster-manager/) | [↗](https://www.nvidia.com/en-us/data-center/bright-cluster-manager/) | Medium | Subsidiary | compute | Nvidia cluster management for HPC and AI; used for GPU and multi-node compute in research and ML workloads. | 2025 |
| [Penguin Solutions](https://www.penguinsolutions.com/) | [↗](https://www.penguinsolutions.com/) | Low | TBD | compute | HPC and GPU appliance vendor; on-prem and cloud-adjacent compute for intensive workloads. | 2025 |
| [Rancher](https://www.rancher.com/) | [↗](https://www.rancher.com/) | Medium | Subsidiary | compute, orchestration | Kubernetes management platform (SUSE); used to run and orchestrate data and ML workloads. | 2025 |
| [Red Hat](https://www.redhat.com/en/products/high-performance-computing) | [↗](https://www.redhat.com/en/products/high-performance-computing) | Medium | Subsidiary | compute | Enterprise Linux and HPC offerings (IBM); foundational compute and container runtime for data stacks. | 2025 |
| [Ubuntu Canonical Kubernetes](https://ubuntu.com/kubernetes) | [↗](https://ubuntu.com/kubernetes) | Medium | TBD | compute, orchestration | Canonical’s Kubernetes distribution and tooling; common base for data/ML clusters. | 2025 |
| [Vercel Edge Functions](https://vercel.com/docs/functions) | [↗](https://vercel.com/docs/functions) | Low | TBD | compute | Serverless edge compute for web/apps; tangential to core data pipelines and analytics. | 2025 |
| [VMware Tanzu](https://www.vmware.com/products/app-platform/tanzu) | [↗](https://www.vmware.com/products/app-platform/tanzu) | Medium | Subsidiary | compute, orchestration | VMware’s Kubernetes and app platform; enterprise runtime for data and application workloads. | 2025 |

### Data Governance & Catalog

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Acryl Data](https://www.acryldata.io/) | [↗](https://www.acryldata.io/) | Medium | Series B | catalog, observability | Data catalog built on OpenMetadata with focus on reliability and observability of metadata. | 2025 |
| [Alation](https://www.alation.com/) | [↗](https://www.alation.com/) | High | Series D+ | catalog, governance | Behavioral catalog and stewardship; data intelligence and governance for enterprises. | 2025 |
| [Ataccama](https://www.ataccama.com/) | [↗](https://www.ataccama.com/) | Medium | Series D+ | governance, quality | Unified data governance and data quality platform; MDM and stewardship. | 2025 |
| [Atlan](https://atlan.com/) | [↗](https://atlan.com/) | High | Series C | catalog, governance | Modern data catalog with collaboration and embedded governance; popular with data teams. | 2025 |
| [AWS Glue Data Catalog](https://aws.amazon.com/glue/features/catalog/) | [↗](https://aws.amazon.com/glue/features/catalog/) | High | Subsidiary | catalog, governance | AWS-managed catalog for S3 and Glue; central metadata for lake and ETL in AWS. | 2025 |
| [BigID](https://bigid.com/) | [↗](https://bigid.com/) | High | Series D | governance, security-privacy | Data discovery and classification for privacy, security, and governance at scale. | 2025 |
| [Collibra](https://www.collibra.com/) | [↗](https://www.collibra.com/) | High | TBD | governance, catalog | Market leader in data governance; strong policy, workflow, and stewardship capabilities. | 2025 |
| [Databricks Unity Catalog](https://docs.databricks.com/data-governance/unity-catalog/) | [↗](https://docs.databricks.com/data-governance/unity-catalog/) | High | Series D+ | governance, catalog | Unified governance across Delta, Iceberg, Hudi; open-sourced; ABAC and lineage. | 2025 |
| [Google Cloud Dataplex](https://cloud.google.com/dataplex) | [↗](https://cloud.google.com/dataplex) | High | Subsidiary | governance, catalog | Google Cloud’s integrated data governance and catalog for lakes and BigQuery. | 2025 |
| [IBM Knowledge Catalog](https://www.ibm.com/products/knowledge-catalog) | [↗](https://www.ibm.com/products/knowledge-catalog) | Medium | Subsidiary | catalog, governance | Enterprise catalog and governance on IBM Cloud; integrates with Watson and Cloud Pak for Data. | 2025 |
| [Immuta](https://www.immuta.com/) | [↗](https://www.immuta.com/) | High | Series D+ | governance, security-privacy | Data access control and policy automation; privacy and security for analytics and AI. | 2025 |
| [Informatica](https://www.informatica.com/) | [↗](https://www.informatica.com/) | High | Public | governance, catalog, integration | Broad data management platform; catalog, governance, ETL, and integration. | 2025 |
| [Microsoft Purview](https://www.microsoft.com/en-us/security/business/data-governance/purview) | [↗](https://www.microsoft.com/en-us/security/business/data-governance/purview) | High | Subsidiary | governance, catalog, security-privacy | Unified data governance, catalog, and compliance across Microsoft and multi-cloud. | 2025 |
| [OpenMetadata](https://open-metadata.org/) | [↗](https://open-metadata.org/) | High | Series A | catalog, governance | Open-source catalog with APIs and connectors; foundation for Acryl and other catalogs. | 2025 |
| [Oracle Cloud Data Catalog](—) | [↗](—) | Medium | Subsidiary | catalog | Oracle’s managed data catalog for OCI data assets and lakehouse. | 2025 |
| [SAP Data Intelligence](https://www.sap.com/products/technology-platform/data-intelligence.html) | [↗](https://www.sap.com/products/technology-platform/data-intelligence.html) | Medium | Subsidiary | governance, catalog, orchestration | SAP’s data orchestration and governance layer for SAP and non-SAP data. | 2025 |
| [Snowflake Horizon](https://www.snowflake.com/horizon/) | [↗](https://www.snowflake.com/horizon/) | High | Public | governance, security-privacy, catalog | Snowflake’s governance, compliance, and security layer for the Data Cloud. | 2025 |
| [Solidatus](https://www.solidatus.com/) | [↗](https://www.solidatus.com/) | Medium | TBD | governance, catalog | Data lineage and governance platform; diagrammatic modeling and impact analysis. | 2025 |

### Data Integration

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Adobe Experience Platform](https://business.adobe.com/products/experience-platform/adobe-experience-platform.html) | [↗](https://business.adobe.com/products/experience-platform/adobe-experience-platform.html) | Medium | Subsidiary | integration, data-sources, product-analytics | CDP and experience data; ingestion and activation for marketing and product analytics. | 2025 |
| [AWS AppFlow](https://aws.amazon.com/appflow/) | [↗](https://aws.amazon.com/appflow/) | High | Subsidiary | ingestion, integration | Managed SaaS-to-S3/warehouse connectors; low-code ingestion and integration. | 2025 |
| [Azure Data Factory](https://azure.microsoft.com/en-us/products/data-factory/) | [↗](https://azure.microsoft.com/en-us/products/data-factory/) | High | Subsidiary | ingestion, transformation, orchestration | Microsoft’s cloud ETL/ELT and orchestration service; integrates with Purview and Synapse. | 2025 |
| [Azure Form Recognizer](https://azure.microsoft.com/en-us/products/ai-services/ai-document-intelligence) | [↗](https://azure.microsoft.com/en-us/products/ai-services/ai-document-intelligence) | Medium | Subsidiary | unstructured-etl, integration | Document intelligence (AI Document Intelligence); extract structured data from documents for pipelines. | 2025 |
| [Boomi](https://boomi.com/) | [↗](https://boomi.com/) | High | Subsidiary | integration, ingestion | Dell’s iPaaS; application and data integration, ingestion, and API management. | 2025 |
| [Cdata](https://www.cdata.com/) | [↗](https://www.cdata.com/) | Medium | TBD | integration, ingestion | Connectors and drivers for databases and apps; used for ingestion and integration patterns. | 2025 |
| [Celigo](https://www.celigo.com/) | [↗](https://www.celigo.com/) | Medium | Series C | integration | iPaaS for business users; app-to-app and data integration with prebuilt flows. | 2025 |
| [Census](https://www.getcensus.com/) | [↗](https://www.getcensus.com/) | High | Series B | transformation, integration | Reverse ETL and activation; syncs warehouse data to operational tools and product stacks. | 2025 |
| [Denodo](https://www.denodo.com/) | [↗](https://www.denodo.com/) | High | TBD | integration, catalog | Data virtualization and logical data fabric; unified access and catalog over disparate sources. | 2025 |
| [Google Cloud BigQuery Data Transfer](https://cloud.google.com/bigquery-transfer) | [↗](https://cloud.google.com/bigquery-transfer) | High | Subsidiary | ingestion | Managed batch ingestion into BigQuery from SaaS, cloud storage, and other sources. | 2025 |
| [Google Cloud Data Fusion](https://cloud.google.com/data-fusion) | [↗](https://cloud.google.com/data-fusion) | High | Subsidiary | ingestion, transformation, orchestration | Managed, visual ETL/ELT on CDAP; ingestion, transformation, and orchestration for BigQuery and GCS. | 2025 |
| [Hightouch](https://www.hightouch.com/) | [↗](https://www.hightouch.com/) | High | Series C | transformation, integration | Reverse ETL and sync from warehouse to CRMs; raised $80M Series C at $1.2B valuation (Feb 2025) for AI Decisioning. Category-defining in operational analytics and marketing activation. | 2025 |
| [Informatica IPaaS](https://www.informatica.com/ipaas.html) | [↗](https://www.informatica.com/ipaas.html) | High | Public | integration, transformation | Enterprise cloud data management (IDMC) and iPaaS; public (NYSE: INFA), ~$1.64B revenue FY2024. Core integration and data management for large enterprises. | 2025 |
| [Make](https://www.make.com/) | [↗](https://www.make.com/) | High | Subsidiary | integration, orchestration | Visual automation and integration platform (formerly Integromat); subsidiary of Celonis. Widely used for no-code workflows and app connectivity. | 2025 |
| [MuleSoft](https://www.mulesoft.com/) | [↗](https://www.mulesoft.com/) | High | Subsidiary | integration, ingestion | API-led integration platform; acquired by Salesforce (2018). Central to Salesforce Data Cloud and enterprise connectivity. | 2025 |
| [n8n](https://n8n.io/) | [↗](https://n8n.io/) | High | Series C | integration, orchestration | Open-source workflow automation; raised $180M Series C (Oct 2025), $2.5B valuation. Strong in AI agents and self-hosted orchestration. | 2025 |
| [Oracle Unity](—) | [↗](—) | Medium | Subsidiary | integration, governance, catalog | Oracle’s customer data platform (CDP) and 360° view; part of Oracle Cloud. Relevant for Oracle-centric enterprises. | 2025 |
| [Qlik Talend](https://www.qlik.com/) | [↗](https://www.qlik.com/) | High | TBD | integration, transformation | Qlik acquired Talend (2023); combined analytics and data integration. Private under Qlik; key player in integration and transformation. | 2025 |
| [Rudderstack](https://www.rudderstack.com/) | [↗](https://www.rudderstack.com/) | High | Series B | ingestion, integration, data-sources | Open-source Segment alternative; $56M Series B (2022). Event pipeline, CDP, and warehouse sync; strong developer adoption. | 2025 |
| [Salesforce - Data Cloud](https://www.salesforce.com/data/) | [↗](https://www.salesforce.com/data/) | High | Subsidiary | integration, governance, analytics, catalog | Salesforce Data Cloud (Data 360): unified CDP and activation across Sales, Service, Commerce, Marketing. Gartner Leader in CDPs; MuleSoft and AI governance. | 2025 |
| [Salesforce Data Cloud](https://www.salesforce.com/products/data-cloud/) | [↗](https://www.salesforce.com/products/data-cloud/) | High | Subsidiary | integration, governance, analytics, catalog | Same as Salesforce - Data Cloud; unified platform for 360° customer data, activation, and AI (e.g. Agentforce). Leader in enterprise CDP. | 2025 |
| [SnapLogic](https://www.snaplogic.com/) | [↗](https://www.snaplogic.com/) | Medium | Series D+ | integration, ingestion | Agentic integration platform; last major round $37.5M (2015) from Microsoft and Silver Lake. Established in iPaaS and data pipelines. | 2025 |
| [Tealium](https://tealium.com/) | [↗](https://tealium.com/) | High | TBD | integration, data-sources | CDP and tag management; $96M Series G (2021), ~$1.2B valuation. Vendor-neutral first-party data and real-time orchestration. | 2025 |
| [tray.ai](https://tray.io/) | [↗](https://tray.io/) | High | Series C | integration, orchestration | Tray.io: low-code automation and integration; $50M Series C (2019), $40M extension (2022). Enterprise workflow and general automation. | 2025 |
| [Treasure Data](https://www.treasuredata.com/) | [↗](https://www.treasuredata.com/) | Medium | Subsidiary | ingestion, integration | Arm subsidiary (acquired 2018); CDP with 200+ sources, ID resolution, and IoT. Strong in Composable CDP and vertical use cases. | 2025 |
| [Twilio Segment](https://segment.com/) | [↗](https://segment.com/) | High | Subsidiary | ingestion, integration, data-sources | Segment acquired by Twilio (2020); CDP and event collection with strong developer ecosystem. Core to customer data pipelines. | 2025 |
| [Workato](https://www.workato.com/) | [↗](https://www.workato.com/) | High | Series D | integration, orchestration | Enterprise automation and integration; Series D, significant growth. Competes with MuleSoft and Tray in enterprise iPaaS and workflows. | 2025 |

### Data Quality & Observability

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Acceldata](https://www.acceldata.io/) | [↗](https://www.acceldata.io/) | High | Series C | quality, observability | Data observability and reliability for data pipelines and Spark; Series C. Focus on scale and cost for data engineering. | 2025 |
| [Anomalo](https://www.anomalo.com/) | [↗](https://www.anomalo.com/) | High | Series B | quality, observability | Automated data quality and anomaly detection; Series B. ML-based checks and root-cause analysis for analytics and ML pipelines. | 2025 |
| [Atlan](https://atlan.com/) | [↗](https://atlan.com/) | High | Series C | catalog, governance, quality | Data catalog and governance; active in metadata, lineage, and collaboration. Key vendor in modern data governance and catalog. | 2025 |
| [AWS Glue Data Quality](https://aws.amazon.com/glue/features/data-quality/) | [↗](https://aws.amazon.com/glue/features/data-quality/) | High | TBD | quality, transformation | AWS-native data quality rules and profiling for Glue ETL. Relevant for teams standardizing on AWS data stack. | 2025 |
| [Bigeye](https://www.bigeye.com/) | [↗](https://www.bigeye.com/) | High | Series B | quality, observability | Data reliability and observability; Series B. Automated SLAs, anomaly detection, and pipeline monitoring for data teams. | 2025 |
| [Collibra](https://www.collibra.com/us/en) | [↗](https://www.collibra.com/us/en) | High | TBD | governance, catalog, quality | Data intelligence and governance platform; unicorn, private. Leader in governance, catalog, and policy for enterprise data. | 2025 |
| [Datafold](https://www.datafold.com/) | [↗](https://www.datafold.com/) | High | Series B | quality, observability | Data diff and impact analysis; deep dbt integration. Helps analytics engineers ship with confidence and catch regressions. | 2025 |
| [Elementary Data](https://www.elementary-data.com/) | [↗](https://www.elementary-data.com/) | Medium | Seed | quality, observability | dbt-native data quality and observability; open source, Seed stage. Lightweight option for dbt-based quality and monitoring. | 2025 |
| [Google Cloud Dataplex Data Quality](https://cloud.google.com/dataplex/docs/auto-data-quality-overview) | [↗](https://cloud.google.com/dataplex/docs/auto-data-quality-overview) | High | TBD | quality, governance | GCP auto data quality and governance within Dataplex. Relevant for organizations standardizing on Google Cloud data services. | 2025 |
| [Kensu](https://kensu.io/) | [↗](https://kensu.io/) | Medium | Series A | quality, observability | Data observability and lineage; Series A. Real-time lineage and quality for data and ML pipelines. | 2025 |
| [Lightup](https://lightup.ai/) | [↗](https://lightup.ai/) | Medium | Seed | quality, observability | Data reliability and observability; Seed stage. Targets data quality and pipeline health for modern stacks. | 2025 |
| [Masthead Data](—) | [↗](—) | Low | TBD | quality, observability | Data quality/observability vendor; limited public information. Included for landscape coverage. | 2025 |
| [Monte Carlo](https://www.montecarlodata.com/) | [↗](https://www.montecarlodata.com/) | High | Series D | quality, observability | Data observability category leader; $135M Series D (2022), $1.6B valuation. Lineage, incident management, and data downtime prevention. | 2025 |
| [Observe](https://www.observeinc.com/) | [↗](https://www.observeinc.com/) | Medium | Series B | observability, quality | Observability platform (metrics, logs, traces); Series B. Broader observability with data-quality use cases. | 2025 |
| [Pantomath](—) | [↗](—) | Low | TBD | quality, observability | Data quality/observability; limited public information. Included for landscape coverage. | 2025 |
| [Sifflet](https://www.siffletdata.com/) | [↗](https://www.siffletdata.com/) | High | Series B | quality, catalog | Data quality and catalog; Series B. Combines quality checks with metadata and catalog for data trust. | 2025 |
| [Soda](https://www.soda.io/) | [↗](https://www.soda.io/) | High | Series B | quality, observability | Open-source and commercial data quality; Series B. SodaCL and checks across warehouses and pipelines. | 2025 |
| [Telmai](https://www.telmai.com/) | [↗](https://www.telmai.com/) | Medium | Seed | quality, observability | Data quality and observability; Seed stage. Early-stage option for automated quality and monitoring. | 2025 |
| [Validio](https://validio.io/) | [↗](https://validio.io/) | Medium | Seed | quality, observability | Data validation and observability; Seed stage. Focus on validation and quality for data pipelines. | 2025 |

### ETL/ELT / Data Transformation

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Airbyte](https://airbyte.com/) | [↗](https://airbyte.com/) | High | Series B | ingestion, transformation | Open-source and cloud; 350+ connectors; fast-growing alternative to Fivetran. Widely adopted for self-managed and cloud ELT. | 2025 |
| [AWS Glue](https://aws.amazon.com/glue/) | [↗](https://aws.amazon.com/glue/) | High | Subsidiary | ingestion, transformation, catalog | AWS-native ETL and data catalog; serverless Spark and Glue Data Catalog. Default choice for AWS data lakes and Lake Formation. | 2025 |
| [Azure Data Factory](https://azure.microsoft.com/en-us/products/data-factory) | [↗](https://azure.microsoft.com/en-us/products/data-factory) | High | Subsidiary | ingestion, transformation | Microsoft Azure's managed ETL/ELT service; integrates with Synapse, Purview, and Azure data services. Core for Azure-centric estates. | 2025 |
| [Databricks Workflows](https://docs.databricks.com/workflows.html) | [↗](https://docs.databricks.com/workflows.html) | High | Series D+ | orchestration, transformation | Native lakehouse orchestration; tight with Delta and Unity Catalog. Central for Databricks-based data and AI pipelines. | 2025 |
| [dbt Labs](https://www.getdbt.com/) | [↗](https://www.getdbt.com/) | High | Series D+ | transformation, semantic-layer, orchestration | De facto standard for analytics engineering; semantic layer and MetricFlow. Merging with Fivetran (2025). | 2025 |
| [Estuary](https://www.estuary.dev/) | [↗](https://www.estuary.dev/) | Medium | Series B | ingestion, transformation, streaming | Real-time and batch in one platform; Flow for CDC and streaming. Growing option for unified batch and streaming pipelines. | 2025 |
| [Fivetran](https://www.fivetran.com/) | [↗](https://www.fivetran.com/) | High | Series D+ | ingestion, transformation | Managed ELT; 500+ connectors and low maintenance. Merging with dbt Labs (2025). Market leader in managed ingestion. | 2025 |
| [Google Cloud Data Fusion](https://cloud.google.com/data-fusion) | [↗](https://cloud.google.com/data-fusion) | Medium | Subsidiary | ingestion, transformation | GCP-managed ETL/ELT built on CDAP; supports batch and replication. Relevant for Google Cloud–centric data estates. | 2025 |
| [Hevo Data](https://hevodata.com/) | [↗](https://hevodata.com/) | Medium | Series B | ingestion, transformation | Managed pipeline platform with connectors and transformations. Strong in SMB and mid-market; real-time and batch. | 2025 |
| [IBM DataStage](https://www.ibm.com/products/datastage) | [↗](https://www.ibm.com/products/datastage) | Medium | Subsidiary | ingestion, transformation | Enterprise ETL on IBM Cloud Pak for Data; common in mainframe and hybrid IBM estates. Legacy but still widely deployed. | 2025 |
| [Informatica](https://www.informatica.com/) | [↗](https://www.informatica.com/) | High | Public | ingestion, transformation, governance, integration | Enterprise data management leader; IDMC covers integration, quality, and governance. Heavily used in regulated and large enterprises. | 2025 |
| [Matillion](https://www.matillion.com/) | [↗](https://www.matillion.com/) | High | TBD | ingestion, transformation | Cloud-native ETL for Snowflake, BigQuery, and Redshift; strong SMB and mid-market. Native to major cloud warehouses. | 2025 |
| [Meltano](https://meltano.com/) | [↗](https://meltano.com/) | Medium | Seed | transformation, ingestion, orchestration | Open-source ELT; dbt and Singer; dev-first and CLI. Good fit for eng-led teams and GitOps-style pipelines. | 2025 |
| [Oracle Data Integration](https://www.oracle.com/integration/) | [↗](https://www.oracle.com/integration/) | Medium | Subsidiary | ingestion, transformation | Oracle's integration and ETL stack; GoldenGate and ODI. Relevant where Oracle databases and apps dominate. | 2025 |
| [Prophecy](https://www.prophecy.io/) | [↗](https://www.prophecy.io/) | Medium | Series B | transformation, ingestion | Low-code data pipelines and Spark; Databricks-native option. Targets both citizen and technical users on the lakehouse. | 2025 |
| [SAP Data Intelligence](https://www.sap.com/products/technology-platform/data-intelligence.html) | [↗](https://www.sap.com/products/technology-platform/data-intelligence.html) | Medium | Subsidiary | ingestion, transformation, governance | SAP's data orchestration and ML platform; ties to S/4HANA and SAP data. Important in SAP-centric enterprises. | 2025 |
| [SnapLogic](https://www.snaplogic.com/) | [↗](https://www.snaplogic.com/) | Medium | TBD | ingestion, transformation, integration | Integration platform with ETL and API management. Used for application and data integration in mid-market and enterprise. | 2025 |
| [Talend](https://www.talend.com/) | [↗](https://www.talend.com/) | High | Subsidiary | ingestion, transformation, integration | Enterprise ETL veteran; strong SAP/ERP connectivity. Part of Qlik (private); still widely used for integration and quality. | 2025 |

### Orchestration

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Apache Airflow](https://airflow.apache.org/) | [↗](https://airflow.apache.org/) | High | OSS | orchestration | De facto open-source workflow orchestrator for data pipelines. Python-native DAGs; ecosystem of operators and integrations. | 2025 |
| [Apache Nifi](https://nifi.apache.org/) | [↗](https://nifi.apache.org/) | Medium | OSS | orchestration, ingestion | Flow-based data routing and ETL; strong for file and streaming ingestion. Common in on-prem and hybrid setups. | 2025 |
| [Argo](https://argoproj.github.io/) | [↗](https://argoproj.github.io/) | Medium | OSS | orchestration | Kubernetes-native workflows (Argo Workflows) and GitOps (Argo CD). Fits cloud-native and K8s-based data platforms. | 2025 |
| [Astronomer](https://www.astronomer.io/) | [↗](https://www.astronomer.io/) | High | Series D | orchestration, observability | Managed Airflow; strong enterprise and Astro platform. Leading commercial Airflow offering with observability and scale. | 2025 |
| [AWS Step Functions](https://aws.amazon.com/step-functions/) | [↗](https://aws.amazon.com/step-functions/) | High | Subsidiary | orchestration | AWS serverless workflow orchestration; integrates with Lambda, Glue, and other AWS services. Default for serverless data workflows on AWS. | 2025 |
| [Dagster](https://dagster.io/) | [↗](https://dagster.io/) | High | Series B | orchestration, transformation | Software-defined assets; strong dev experience and testing. Growing adoption as modern alternative to Airflow for asset-centric pipelines. | 2025 |
| [Databricks Workflows](https://docs.databricks.com/workflows.html) | [↗](https://docs.databricks.com/workflows.html) | High | Series D+ | orchestration | Native lakehouse orchestration with Delta and Unity Catalog. Core for jobs, DLT, and notebooks on Databricks. | 2025 |
| [dbt Labs Jobs](https://www.getdbt.com/product/dbt-cloud) | [↗](https://www.getdbt.com/product/dbt-cloud) | High | Series D+ | orchestration | Scheduling and run management for dbt in dbt Cloud. Key for analytics-engineering teams standardizing on dbt. | 2025 |
| [Flyte](https://flyte.org/) | [↗](https://flyte.org/) | Medium | OSS | orchestration, ml-ops | Open-source workflow engine for data and ML; type-safe and scalable. Adopted in ML platforms and data science workloads. | 2025 |
| [GitHub Actions](https://github.com/features/actions) | [↗](https://github.com/features/actions) | Medium | Subsidiary | orchestration | CI/CD and lightweight pipeline automation; can run dbt, ingestion, and data jobs. Relevant for dev-centric and GitOps workflows. | 2025 |
| [Google Cloud Composer](https://cloud.google.com/composer) | [↗](https://cloud.google.com/composer) | High | Subsidiary | orchestration | Managed Airflow on GCP; integrates with BigQuery, Dataflow, and GCP data services. Primary orchestration option for GCP data teams. | 2025 |
| [Google Cloud Workflows](https://cloud.google.com/workflows) | [↗](https://cloud.google.com/workflows) | Medium | Subsidiary | orchestration | Serverless workflow orchestration on GCP. Good for event-driven and lightweight pipelines; less data-native than Composer. | 2025 |
| [Jenkins](https://www.jenkins.io/) | [↗](https://www.jenkins.io/) | Low | OSS | orchestration | General-purpose CI/CD; sometimes used to trigger data jobs. Not data-native; Airflow/Dagster/Prefect preferred for data orchestration. | 2025 |
| [Kestra](https://kestra.io/) | [↗](https://kestra.io/) | Medium | Series A | orchestration | Declarative orchestration with YAML and plugin model. Emerging option for simple and event-driven data workflows. | 2025 |
| [Microsoft Azure Data Factory](https://azure.microsoft.com/products/data-factory) | [↗](https://azure.microsoft.com/products/data-factory) | High | Subsidiary | orchestration, ingestion | Same as Azure Data Factory; provides both ETL and pipeline orchestration. Central for Azure data estates. | 2025 |
| [Microsoft Azure Synapse Pipelines](https://azure.microsoft.com/products/synapse-analytics) | [↗](https://azure.microsoft.com/products/synapse-analytics) | High | Subsidiary | orchestration | Pipeline orchestration within Synapse Analytics; shares engine with Data Factory. Core for Synapse-based analytics and data engineering. | 2025 |
| [Prefect](https://www.prefect.io/) | [↗](https://www.prefect.io/) | High | Series B | orchestration, observability | Modern Python orchestration with dynamic workflows and strong observability. Popular alternative to Airflow for data and automation. | 2025 |
| [Temporal](https://temporal.io/) | [↗](https://temporal.io/) | High | Series D+ | orchestration | Durable workflow orchestration platform for long-running, distributed workflows; $5B valuation (2026), key for AI agents and used by OpenAI, Netflix, DoorDash. | 2025 |
| [Union.ai](https://union.ai/) | [↗](https://union.ai/) | High | Series B | orchestration | ML workflow orchestration with open-source Flyte; enables scalable data and ML pipelines across hybrid cloud. | 2025 |

### Privacy & Security

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Bedrock Security](https://bedrock.security/) | [↗](https://bedrock.security/) | High | Seed | security-privacy, governance | Data security platform for cloud and AI; $10M seed (Mar 2024), AI Reasoning Engine for discovery and protection of sensitive data. | 2025 |
| [BigID](https://bigid.com/) | [↗](https://bigid.com/) | High | Series D+ | security-privacy, governance | AI data security, compliance, and discovery; $60M growth round (Mar 2024), unicorn valuation, strong in unstructured data and privacy. | 2025 |
| [Collibra](https://www.collibra.com/) | [↗](https://www.collibra.com/) | High | Series D+ | governance, security-privacy | Data intelligence and governance platform; $5.25B valuation (Series G 2021), Data Intelligence Cloud with broad enterprise adoption. | 2025 |
| [Cyera](https://www.cyera.io/) | [↗](https://www.cyera.io/) | High | Series D+ | security-privacy, governance | Data security and posture; $300M Series D (Nov 2024) at $3B valuation, DLP and identity security, acquired Trail Security. | 2025 |
| [Duality Technologies](https://dualitytech.com/) | [↗](https://dualitytech.com/) | Medium | Series B | security-privacy, governance | Privacy-enhanced data collaboration using homomorphic encryption; $30M Series B (2021), enables analytics on encrypted data. | 2025 |
| [Enveil](https://www.enveil.com/) | [↗](https://www.enveil.com/) | Medium | TBD | security-privacy | Homomorphic encryption for enterprise data security; search and compute on encrypted data without decryption. | 2025 |
| [Immuta](https://www.immuta.com/) | [↗](https://www.immuta.com/) | High | Series D+ | security-privacy, governance | Data access control and policy automation for cloud and lakehouse; widely used for sensitive data and compliance. | 2025 |
| [Ketch](https://www.ketch.com/) | [↗](https://www.ketch.com/) | High | TBD | security-privacy, governance | Privacy and data governance platform for consent and compliance automation across first-party data. | 2025 |
| [OneTrust](https://www.onetrust.com/) | [↗](https://www.onetrust.com/) | High | Series C | security-privacy, governance | Market leader in data privacy and GRC software; $5.1B valuation (Series C), IDC #1 in data privacy market share. | 2025 |
| [Opaque Systems](https://opaque.co/) | [↗](https://opaque.co/) | Medium | TBD | security-privacy, compute | Confidential analytics and ML in confidential computing; secure collaborative analytics without exposing raw data. | 2025 |
| [Piiano](https://www.piiano.com/) | [↗](https://www.piiano.com/) | Medium | TBD | security-privacy | Developer-focused data security and privacy vault; secure storage and access control for PII in applications. | 2025 |
| [Privacera](https://www.privacera.com/) | [↗](https://www.privacera.com/) | High | Series B | security-privacy, governance | Cloud-first data governance and security; $50M Series B (2021), unified access control and discovery across clouds. | 2025 |
| [Securiti](https://securiti.ai/) | [↗](https://securiti.ai/) | High | Subsidiary | security-privacy, governance | Data security and privacy operations platform; acquired by Veeam for $1.7B (Oct 2025), automated privacy and governance. | 2025 |
| [SkyFlow](https://www.skyflow.com/) | [↗](https://www.skyflow.com/) | Medium | TBD | security-privacy | Data privacy vault and API for PII; tokenization and policy-based access for applications and analytics. | 2025 |
| [Teleskope](https://www.teleskope.ai/) | [↗](https://www.teleskope.ai/) | Medium | TBD | security-privacy, governance | Data security and compliance for cloud data stores; discovery, classification, and policy automation. | 2025 |
| [Transcend](https://transcend.io/) | [↗](https://transcend.io/) | High | Series B | security-privacy, governance | Privacy and compliance automation; $40M Series B (May 2024), data discovery, consent, and request fulfillment for enterprises. | 2025 |
| [TrustArc](https://trustarc.com/) | [↗](https://trustarc.com/) | High | TBD | security-privacy, governance | Privacy compliance and risk management; established vendor for assessments, consent, and vendor management. | 2025 |
| [Very Good Security](https://www.verygoodsecurity.com/) | [↗](https://www.verygoodsecurity.com/) | High | Series C | security-privacy | Data vault and tokenization platform; $60M Series C (2020), 3B+ tokens, reduces liability for sensitive data in apps. | 2025 |

### Unstructured & Vector ETL

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Adobe PDF Extract](https://developer.adobe.com/document-services/apis/pdf-extract/) | [↗](https://developer.adobe.com/document-services/apis/pdf-extract/) | Medium | Subsidiary | unstructured-etl | API for PDF structure and content extraction; part of Adobe Document Services for document intelligence pipelines. | 2025 |
| [AWS Textract](https://aws.amazon.com/textract/) | [↗](https://aws.amazon.com/textract/) | High | Subsidiary | unstructured-etl, ai-dev | Document text and table extraction; AWS-managed OCR and form parsing for pipelines and RAG. | 2025 |
| [Azure Form Recognizer](https://azure.microsoft.com/products/ai-services/ai-document-intelligence) | [↗](https://azure.microsoft.com/products/ai-services/ai-document-intelligence) | High | Subsidiary | unstructured-etl, ai-dev | Azure AI Document Intelligence for document parsing, layout, and tables; key for Microsoft-centric document pipelines. | 2025 |
| [Cleanlab](https://cleanlab.com/) | [↗](https://cleanlab.com/) | High | Series A | quality, ml-ops | Data-centric AI; label quality and confident learning for ML. $25M Series A (2023), used by Fortune 500 for data curation. | 2025 |
| [Gretel](https://gretel.ai/) | [↗](https://gretel.ai/) | High | Series B | unstructured-etl, security-privacy | Synthetic data and privacy APIs; $50M Series B (2021), generation and de-identification for safe data sharing and ML. | 2025 |
| [HyperScience Hypercell](—) | [↗](—) | Medium | Subsidiary | unstructured-etl | Document automation and IDP; Hypercell (Hyland) for enterprise document processing and classification. | 2025 |
| [Langchain Text Splitters](https://www.langchain.com/) | [↗](https://www.langchain.com/) | High | Series B | unstructured-etl, ai-dev | LLM application framework; text splitters and chains, $1.25B valuation (Series B 2025), LangSmith for agent engineering. | 2025 |
| [LlamaIndex LlamaParse](https://www.llamaindex.ai/) | [↗](https://www.llamaindex.ai/) | High | Series A | unstructured-etl, ai-dev | RAG and document parsing; $19M Series A (2025), LlamaParse and LlamaCloud for enterprise knowledge agents. | 2025 |
| [MostlyAI](https://mostly.ai/) | [↗](https://mostly.ai/) | High | Series B | unstructured-etl, security-privacy | Synthetic data generation for analytics and ML; privacy-preserving data sharing and testing. | 2025 |
| [Reducto](—) | [↗](—) | Medium | TBD | unstructured-etl | — | 2025 |
| [Superlinked](—) | [↗](—) | Medium | TBD | unstructured-etl, storage-vector | — | 2025 |
| [Tensorlake](—) | [↗](—) | Medium | TBD | unstructured-etl, storage | — | 2025 |
| [Towhee](—) | [↗](—) | Medium | OSS | unstructured-etl, ai-dev | Open-source ML pipeline and embedding framework for unstructured data and vector workflows. | 2025 |
| [Unstructured](—) | [↗](—) | High | TBD | unstructured-etl, transformation | Open-source document parsing and preprocessing for LLMs and RAG; widely used in AI pipelines. | 2025 |
| [Vectorize](—) | [↗](—) | Medium | TBD | unstructured-etl, storage-vector | — | 2025 |

## Infrastructure — Store & Stream

### Data Lakes / Lakehouses

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Apache Hudi](https://hudi.apache.org/) | [↗](https://hudi.apache.org/) | High | OSS | storage-lakehouse, storage | Open-source lakehouse table format for incremental upserts and deletes; widely used with Spark and aligned with modern data lake patterns. | 2025 |
| [Apache Iceberg](https://iceberg.apache.org/) | [↗](https://iceberg.apache.org/) | High | OSS | storage-lakehouse, storage | Vendor-neutral open-source table format for large analytic tables; strong ecosystem and adoption across clouds and query engines. | 2025 |
| [AWS Athena](https://aws.amazon.com/lake-formation/) | [↗](https://aws.amazon.com/lake-formation/) | High | Subsidiary | storage-lakehouse, analytics, compute | Serverless query service for S3 data lakes; pay-per-query SQL with federation and Lake Formation integration for governance. | 2025 |
| [AWS Lake Formation / EMR](https://aws.amazon.com/emr/) | [↗](https://aws.amazon.com/emr/) | High | Subsidiary | storage-lakehouse, compute, governance | Lake Formation for centralized access control and EMR for Spark/Hadoop; core AWS stack for building and governing data lakes. | 2025 |
| [Azure Synapse + ADLS](https://azure.microsoft.com/products/synapse-analytics) | [↗](https://azure.microsoft.com/products/synapse-analytics) | High | Subsidiary | storage-lakehouse, storage-warehouse, analytics | Unified analytics platform combining data warehouse and data lake on ADLS; integrated pipelines and governance. | 2025 |
| [Bauplan Labs](https://www.bauplanlabs.com/) | [↗](https://www.bauplanlabs.com/) | Medium | Series B | storage-lakehouse, quality, observability | Data quality and reliability platform for lakehouse and warehouse pipelines; focus on contracts and pipeline observability. | 2025 |
| [Cloudera](https://www.cloudera.com/) | [↗](https://www.cloudera.com/) | High | Public | storage-lakehouse, governance | Enterprise data platform (CDP) with strong governance and hybrid cloud; key player in regulated and on-prem lakehouse deployments. | 2025 |
| [Databricks Lakehouse (Delta Lake)](https://www.databricks.com/product/delta-lake) | [↗](https://www.databricks.com/product/delta-lake) | High | Series D+ | storage-lakehouse, governance | Unified batch and streaming; Delta Lake OSS; Unity Catalog. | 2025 |
| [Delta Lake](https://delta.io/) | [↗](https://delta.io/) | High | OSS | storage-lakehouse, storage | Open-source storage layer for lakehouses with ACID and time travel; originated at Databricks and widely adopted. | 2025 |
| [Dremio](https://www.dremio.com/) | [↗](https://www.dremio.com/) | High | Series D+ | storage-lakehouse, analytics | SQL query engine and data lakehouse platform with Apache Arrow; reflections for acceleration and semantic layer capabilities. | 2025 |
| [Google Cloud BigLake / Dataproc](https://cloud.google.com/biglake) | [↗](https://cloud.google.com/biglake) | High | Subsidiary | storage-lakehouse, compute | BigLake provides unified storage across BigQuery and object storage; Dataproc for Spark and Hadoop on GCP. | 2025 |
| [IBM Watsonx.Data](https://www.ibm.com/data-lake) | [↗](https://www.ibm.com/data-lake) | Medium | Subsidiary | storage-lakehouse, analytics, governance | IBM data lake and analytics for AI workloads; part of watsonx with governance and open formats. | 2025 |
| [Iceberg](https://github.com/apache/iceberg) | [↗](https://github.com/apache/iceberg) | High | OSS | storage-lakehouse, storage | Same as Apache Iceberg; open-source table format for scalable, schema-evolving analytic tables. | 2025 |
| [LakeFS](https://lakefs.io/) | [↗](https://lakefs.io/) | Medium | Series B | storage-lakehouse, governance | Git-like version control for data lakes; branching, merge, and rollback for reproducible pipelines and governance. | 2025 |
| [OneHouse](https://www.onehouse.io/) | [↗](https://www.onehouse.io/) | Medium | Series B | storage-lakehouse, streaming | Managed Apache Iceberg service with unified batch and streaming ingestion; simplifies lakehouse operations. | 2025 |
| [Snowflake Iceberg / Polaris / Unistore](https://www.snowflake.com/) | [↗](https://www.snowflake.com/) | High | Public | storage-lakehouse, storage-warehouse, catalog | Snowflake’s lakehouse (Iceberg), Polaris catalog, and Unistore for transactional and analytical workloads in one platform. | 2025 |
| [Starburst](https://www.starburst.io/) | [↗](https://www.starburst.io/) | High | Series D | storage-lakehouse, analytics, catalog | Enterprise Trino for querying across lakes and warehouses; Starburst Galaxy with built-in catalog and governance. | 2025 |

### Data Warehouses

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Amazon Redshift](https://aws.amazon.com/redshift/) | [↗](https://aws.amazon.com/redshift/) | High | Subsidiary | storage-warehouse, analytics | AWS cloud data warehouse with Redshift Spectrum for querying S3; widely used for analytics and BI. | 2025 |
| [AWS Amazon RedShift](https://aws.amazon.com/redshift/) | [↗](https://aws.amazon.com/redshift/) | High | Subsidiary | storage-warehouse, analytics | Same as Amazon Redshift; AWS’s managed cloud data warehouse with lake federation and ML integration. | 2025 |
| [Azure Synapse](https://azure.microsoft.com/products/synapse-analytics) | [↗](https://azure.microsoft.com/products/synapse-analytics) | High | Subsidiary | storage-warehouse, storage-lakehouse, analytics | Unified analytics service combining SQL data warehouse and lake analytics; integrated with Azure data services. | 2025 |
| [ClickHouse](https://clickhouse.com/) | [↗](https://clickhouse.com/) | High | Series B | storage-warehouse, analytics, streaming | Columnar OLAP database for real-time analytics; open source with strong adoption for event and log analytics. | 2025 |
| [Databricks SQL](https://www.databricks.com/product/databricks-sql) | [↗](https://www.databricks.com/product/databricks-sql) | High | Series D+ | storage-warehouse, analytics | SQL on lakehouse; Photon engine; Unity Catalog. | 2025 |
| [Firebolt](https://www.firebolt.io/) | [↗](https://www.firebolt.io/) | Medium | Series C | storage-warehouse, analytics | Cloud data warehouse focused on speed and efficiency for analytics; decoupled compute and storage. | 2025 |
| [Google Cloud BigQuery](https://cloud.google.com/bigquery) | [↗](https://cloud.google.com/bigquery) | High | Subsidiary | storage-warehouse, analytics | Serverless enterprise data warehouse on GCP; strong ML integration and multi-cloud via BigLake. | 2025 |
| [IBM Db2 Warehouse](https://www.ibm.com/products/db2-warehouse) | [↗](https://www.ibm.com/products/db2-warehouse) | Medium | Subsidiary | storage-warehouse, analytics | IBM cloud data warehouse with in-memory and columnar processing; fits existing IBM and hybrid estates. | 2025 |
| [Oracle ADW](https://www.oracle.com/autonomous-database/autonomous-data-warehouse/) | [↗](https://www.oracle.com/autonomous-database/autonomous-data-warehouse/) | High | Subsidiary | storage-warehouse, analytics | Autonomous Data Warehouse for automated tuning and scaling; strong in Oracle-centric enterprises. | 2025 |
| [Snowflake](https://www.snowflake.com/) | [↗](https://www.snowflake.com/) | High | Public | storage-warehouse, analytics, governance | AI Data Cloud; consumption-based; Arctic LLM; Horizon governance. | 2025 |
| [Teradata](https://www.teradata.com/) | [↗](https://www.teradata.com/) | Medium | Public | storage-warehouse, analytics | Legacy enterprise data warehouse vendor; VantageCloud for hybrid and multi-cloud analytics. | 2025 |
| [Vertica, An OpenText Company](https://www.vertica.com/overview/) | [↗](https://www.vertica.com/overview/) | Medium | Subsidiary | storage-warehouse, analytics | Columnar analytics database; now under OpenText, used for large-scale analytics and ML in enterprise. | 2025 |
| [Yellowbrick](https://yellowbrick.com/) | [↗](https://yellowbrick.com/) | Medium | Series C | storage-warehouse, analytics | Cloud data warehouse for analytics with emphasis on performance and cost; targets mid to large enterprises. | 2025 |

### Event Brokers & Messaging

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Ably](https://ably.com/) | [↗](https://ably.com/) | Medium | Series B | streaming, integration | Real-time data delivery and messaging platform; pub/sub, presence, and edge messaging for apps and data pipelines. | 2025 |
| [Aiven](https://aiven.io/) | [↗](https://aiven.io/) | Medium | Public | streaming, storage, integration | Managed open-source data infrastructure; Kafka, Flink, and other OSS services across clouds with operations handled. | 2025 |
| [Apache Kafka](https://kafka.apache.org/) | [↗](https://kafka.apache.org/) | High | OSS | streaming | De facto standard for event streaming and distributed log; foundational for real-time and event-driven data architectures. | 2025 |
| [AWS SNS / SQS](https://aws.amazon.com/sns/) | [↗](https://aws.amazon.com/sns/) | High | Subsidiary | streaming, integration | AWS messaging services for decoupled, event-driven architectures; SNS for pub/sub and SQS for queues. | 2025 |
| [Azure Event Hubs](https://azure.microsoft.com/en-us/products/event-hubs) | [↗](https://azure.microsoft.com/en-us/products/event-hubs) | High | Subsidiary | streaming, integration | Azure event ingestion and streaming at scale; Kafka-compatible API and integration with Azure data and analytics services. | 2025 |
| [Conduktor](https://www.conduktor.io/) | [↗](https://www.conduktor.io/) | High | Series B | streaming, ingestion, integration | Kafka control plane (Console) and data plane (Gateway); $30M Series B (Nov 2024). Enterprise Kafka management and guardrails; used by BMW, Lufthansa, Capital Group. | 2025 |
| [Confluent](https://www.confluent.io/) | [↗](https://www.confluent.io/) | High | Public | streaming, ingestion, integration | Kafka as a service; Flink; data streaming leader. Public company; core platform for event streaming and real-time data pipelines. | 2025 |
| [Google Pub / Sub](https://cloud.google.com/pubsub) | [↗](https://cloud.google.com/pubsub) | High | Subsidiary | streaming, ingestion, integration | Google Cloud managed messaging and event ingestion; at-least-once delivery, push/pull. Part of GCP; widely used for event-driven and streaming workloads. | 2025 |
| [HiveMQ](https://www.hivemq.com/) | [↗](https://www.hivemq.com/) | High | Series A | streaming, ingestion, integration | MQTT broker for IoT and real-time messaging; €40M Series A (2022). Enterprise MQTT 5.0; used by Fortune 500 for connected devices and event streaming. | 2025 |
| [Kafka](https://github.com/apache/kafka) | [↗](https://github.com/apache/kafka) | High | OSS | streaming, ingestion, storage | Apache open-source distributed event streaming platform; used by 80%+ of Fortune 100. De facto standard for high-throughput pipelines and streaming analytics. | 2025 |
| [Pulsar](https://github.com/apache/pulsar) | [↗](https://github.com/apache/pulsar) | High | OSS | streaming, ingestion, storage | Apache cloud-native messaging and streaming; multi-tenancy, geo-replication, Pulsar Functions. Top-tier Apache project; originated at Yahoo. | 2025 |
| [RabbitMQ](https://github.com/rabbitmq/rabbitmq-server) | [↗](https://github.com/rabbitmq/rabbitmq-server) | High | OSS | streaming, ingestion, integration | Open-source message broker (AMQP, MQTT); VMware Tanzu/Broadcom stewardship. Enterprise-grade messaging for microservices and distributed systems. | 2025 |
| [Redis Streams](https://redis.io/docs/latest/develop/data-types/streams/) | [↗](https://redis.io/docs/latest/develop/data-types/streams/) | Medium | OSS | streaming, ingestion, storage | Redis Streams data structure for messaging and event processing; append-only log with consumer groups. Part of Redis OSS; lightweight streaming option. | 2025 |
| [Redpanda](https://redpanda.com/) | [↗](https://redpanda.com/) | High | Series C | streaming, storage, ingestion | Kafka API–compatible streaming platform in C++; $100M Series C (2023). Cloud-native, lower cost and simpler ops than Kafka; BYOC and Iceberg integration. | 2025 |
| [StreamNative](https://streamnative.io/) | [↗](https://streamnative.io/) | High | Series A | streaming, ingestion, integration | Apache Pulsar cloud and platform; founded by Pulsar creators. $23.7M Series A (2021); StreamNative Cloud and Platform for managed Pulsar. | 2025 |

### GPU Databases

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [BlazingSQL](https://mad.firstmark.com/blazingsql.com) | [↗](https://mad.firstmark.com/blazingsql.com) | Low | TBD | storage, compute, analytics | GPU-accelerated SQL on RAPIDS; status unclear (legacy/absorbed). Historically targeted fast analytics on GPUs. | 2025 |
| [Brytlyt](https://brytlyt.io/) | [↗](https://brytlyt.io/) | Medium | TBD | storage, compute, analytics | GPU-accelerated analytics and database; real-time BI and spatial. Focus on speed and scale for analytics workloads. | 2025 |
| [Heavy.ai](https://www.heavy.ai/) | [↗](https://www.heavy.ai/) | High | Subsidiary | storage, compute, analytics | GPU-accelerated analytics (formerly OmniSci/MapD); acquired by NVIDIA (2025). HeavyDB and visualization for big data and geospatial. | 2025 |
| [HeteroDB](https://www.heterodb.com/) | [↗](https://www.heterodb.com/) | Medium | TBD | storage, compute, analytics | PG-Strom GPU acceleration for PostgreSQL; Japanese vendor. Enables GPU-accelerated analytics inside Postgres. | 2025 |
| [Kinetica](https://www.kinetica.com/) | [↗](https://www.kinetica.com/) | High | Series B | storage, compute, analytics | GPU-accelerated relational DB for real-time analytics; $50M+ Series A (2017). Used in intelligence and enterprise; GlaxoSmithKline, PG&E, USPS. | 2025 |
| [Oracle HeatWave](https://www.oracle.com/heatwave/) | [↗](https://www.oracle.com/heatwave/) | High | Subsidiary | storage, storage-warehouse, analytics | MySQL HeatWave: in-memory columnar accelerator for OLAP on MySQL; lakehouse and vector store. Oracle subsidiary; strong benchmarks vs Snowflake, Databricks, BigQuery. | 2025 |
| [SQream](https://sqream.com/) | [↗](https://sqream.com/) | Medium | TBD | storage, compute, analytics | GPU-based data warehouse and analytics; designed for very large datasets. Targets analytics speed and cost efficiency. | 2025 |

### Graph Databases

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AgensGraph](https://github.com/skaiworldwide-oss/agensgraph) | [↗](https://github.com/skaiworldwide-oss/agensgraph) | Low | OSS | storage, analytics | Graph layer on PostgreSQL (open source). Bitnine/skai OSS; graph extension for Postgres users. | 2025 |
| [Apache HugeGraph](https://github.com/apache/incubator-hugegraph) | [↗](https://github.com/apache/incubator-hugegraph) | Medium | OSS | storage, analytics | Apache graph database for knowledge graphs and link analysis. OSS; supports large-scale graph storage and Gremlin. | 2025 |
| [ArangoDB](https://www.arangodb.com/) | [↗](https://www.arangodb.com/) | High | TBD | storage, analytics, integration | Multi-model database (document, graph, key-value); single query language AQL. Native graph and flexible schema for polyglot workloads. | 2025 |
| [AWS Neptune](https://aws.amazon.com/neptune/) | [↗](https://aws.amazon.com/neptune/) | High | Subsidiary | storage, analytics | AWS managed graph database (Property Graph, Gremlin, SPARQL). Part of AWS; serverless option and broad AWS integration. | 2025 |
| [Azure CosmosDB (Gremlin API)](https://azure.microsoft.com/en-ca/products/cosmos-db/) | [↗](https://azure.microsoft.com/en-ca/products/cosmos-db/) | High | Subsidiary | storage, analytics | Cosmos DB with Gremlin API for graph workloads; globally distributed. Microsoft subsidiary; multi-model with graph support. | 2025 |
| [Dgraph](https://dgraph.io/) | [↗](https://dgraph.io/) | High | OSS | storage, analytics | Open-source distributed graph database with native GraphQL; horizontal scale, ACID. Apache 2.0; Dgraph Labs offers GraphQL Cloud. | 2025 |
| [FalkorDB](https://www.falkordb.com/) | [↗](https://www.falkordb.com/) | Medium | OSS | storage, analytics | Redis-compatible graph database; low-latency graph queries. OSS; good fit for Redis-centric stacks needing graph. | 2025 |
| [JanusGraph](https://github.com/JanusGraph/janusgraph) | [↗](https://github.com/JanusGraph/janusgraph) | Medium | OSS | storage, analytics | Open-source distributed graph DB; Gremlin, pluggable backends (Cassandra, HBase, etc.). Linux Foundation; scalable graph layer over existing stores. | 2025 |
| [Memgraph](https://memgraph.com/) | [↗](https://memgraph.com/) | High | TBD | storage, analytics | In-memory graph database; real-time analytics and streaming. Cypher-compatible; targets low-latency and operational graph use cases. | 2025 |
| [NebulaGraph](https://www.nebula-graph.io/) | [↗](https://www.nebula-graph.io/) | High | TBD | storage, analytics | Distributed graph database (open source and commercial); nGQL. Designed for large-scale graph storage and analytics. | 2025 |
| [neo4j](https://neo4j.com/) | [↗](https://neo4j.com/) | High | Series D+ | storage, analytics, governance | Leading native graph database; Cypher, Aura managed service. $325M Series F (2021); category leader for graph and knowledge graphs. | 2025 |
| [Oracle Graph](https://www.oracle.com/) | [↗](https://www.oracle.com/) | High | Subsidiary | storage, analytics | Graph capabilities in Oracle Database and Autonomous DB; PGQL and in-memory analyst. Part of Oracle; fits Oracle-centric enterprises. | 2025 |
| [OrientDB](https://github.com/orientechnologies/orientdb) | [↗](https://github.com/orientechnologies/orientdb) | Medium | OSS | storage, analytics | Multi-model OSS DB (document, graph, object); SQL and Gremlin. OrientDB Ltd; graph and document in one engine. | 2025 |
| [PuppyGraph](https://www.puppygraph.com/) | [↗](https://www.puppygraph.com/) | Medium | TBD | storage, analytics | Graph database and analytics platform. Focus on ease of use and graph analytics workloads. | 2025 |
| [Stardog](https://www.stardog.com/) | [↗](https://www.stardog.com/) | High | Series C | storage, analytics, governance, catalog | Enterprise knowledge graph platform; data unification and AI data assistants. Series C (2023); KG as a service and semantic layer. | 2025 |
| [TigerGraph](https://www.tigergraph.com/) | [↗](https://www.tigergraph.com/) | High | Series C | storage, analytics | Native distributed graph DB for advanced analytics and ML; $105M Series C (2021). Used by Amgen, Intuit, UnitedHealth; cloud and enterprise focus. | 2025 |
| [TypeDB](https://typedb.com/) | [↗](https://typedb.com/) | High | TBD | storage, analytics, governance | Strongly-typed knowledge graph and entity-relationship DB; TypeQL. Conceptual modeling and reasoning; from Vaticle. | 2025 |

### Multi-Model Databases & Abstractions

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [CedarDB](https://cedardb.com/) | [↗](https://cedardb.com/) | High | TBD | storage, analytics, integration | Single unified DB for transactions and analytics; PostgreSQL-compatible; from TUM Umbra research (2024). Replaces separate OLTP/OLAP stacks with one system. | 2025 |
| [Cloudflare D1](https://www.cloudflare.com/developer-platform/products/d1/) | [↗](https://www.cloudflare.com/developer-platform/products/d1/) | High | Subsidiary | storage, storage-warehouse | Serverless SQL database (SQLite) on Cloudflare's edge; part of Developer Platform with Workers. Public company (Cloudflare); GA 2024, jurisdictions and scale improvements in 2025. | 2025 |
| [dolthub](https://www.dolthub.com/) | [↗](https://www.dolthub.com/) | Medium | TBD | storage, catalog | Dolt is a version-controlled SQL database (Git for data); DoltHub is the collaboration platform. Enables fork, clone, branch, merge on databases; MySQL-compatible. | 2025 |
| [Fauna](https://fauna.com/home) | [↗](https://fauna.com/home) | Medium | Series A | storage, streaming | Distributed serverless document database with relational features, strong consistency, and TypeScript-like query language. Fauna service ending May 2025; raised $57M total. | 2025 |
| [FerretDB](https://github.com/FerretDB/FerretDB) | [↗](https://github.com/FerretDB/FerretDB) | Medium | OSS | storage | Open-source MongoDB API proxy backed by PostgreSQL or SQLite. Enables MongoDB compatibility without running MongoDB; community-driven. | 2025 |
| [Gel](https://www.geldata.com/) | [↗](https://www.geldata.com/) | Low | Series A | storage, storage-warehouse | Graph-relational data platform on Postgres; raised Series A ($15M, 2022). Gel Cloud shutting down Jan 2026; team joining Vercel; OSS remains. | 2025 |
| [HarperDB](https://www.harpersystems.dev/) | [↗](https://www.harpersystems.dev/) | Medium | OSS | storage | Unified backend platform combining database, caching, app hosting, and messaging; Node.js-based with REST/GraphQL and vector search. Also offered as Harper (harperdb.io). | 2025 |
| [Macrometa](https://www.macrometa.com/) | [↗](https://www.macrometa.com/) | Medium | Series A | storage, streaming | Edge data platform and global data network; serverless across 175+ PoPs. Raised $20M Series A (2021); targets real-time and edge use cases. | 2025 |
| [Prisma](https://www.prisma.io/) | [↗](https://www.prisma.io/) | High | Series B | transformation | Application data platform and ORM for Node.js/TypeScript; 150k+ developers. Raised $40M Series B (Altimeter); strong adoption for type-safe DB access and migrations. | 2025 |
| [SurrealDB](https://surrealdb.com/) | [↗](https://surrealdb.com/) | High | Series A | storage | Multi-model database (document, graph, relational) with SQL-like query language; AI-native positioning. Raised $20M then $23M Series A extension; 2.3M+ downloads, 31k GitHub stars. | 2025 |
| [TileDB](https://www.tiledb.com/) | [↗](https://www.tiledb.com/) | High | Series B | storage, storage-lakehouse | Multi-modal array database for genomics, geospatial, and ML; positions as modern database vs. complex data stack. $34M Series B (2023); strong in life sciences and pharma. | 2025 |
| [Xata](https://xata.io/) | [↗](https://xata.io/) | High | Series A | storage, storage-warehouse | Serverless database with spreadsheet-like UX, ACID, full-text search, and branching. $30M Series A (2022); targets serverless and low-code apps. | 2025 |

### NoSQL Databases

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Aerospike](https://aerospike.com/) | [↗](https://aerospike.com/) | High | Series D+ | storage | Real-time NoSQL database for mission-critical, low-latency workloads; strong in AI/ML pipelines. Raised $109M Series E (2024); customers include Adobe, PayPal, Barclays. | 2025 |
| [AWS DocumentDB](https://aws.amazon.com/documentdb/) | [↗](https://aws.amazon.com/documentdb/) | High | Subsidiary | storage | AWS managed document database compatible with MongoDB API; serverless option. Part of AWS managed database portfolio; reduces operational burden for document workloads. | 2025 |
| [AWS DynamoDB](https://aws.amazon.com/dynamodb/) | [↗](https://aws.amazon.com/dynamodb/) | High | Subsidiary | storage | Fully managed key-value and document database; serverless, multi-region. Core AWS building block for scalable, low-latency applications. | 2025 |
| [AWS Keyspaces](https://aws.amazon.com/keyspaces/) | [↗](https://aws.amazon.com/keyspaces/) | High | Subsidiary | storage | Serverless Apache Cassandra–compatible database on AWS. CQL API, multi-region, 99.999% availability; for low-latency and time-series workloads. | 2025 |
| [Azure CosmosDB](https://azure.microsoft.com/en-ca/products/cosmos-db/) | [↗](https://azure.microsoft.com/en-ca/products/cosmos-db/) | High | Subsidiary | storage | Globally distributed multi-model NoSQL database; single-digit ms latency, multiple APIs. Microsoft’s flagship managed database for scale-out apps. | 2025 |
| [Azure Table Storage](https://azure.microsoft.com/en-us/products/storage/tables) | [↗](https://azure.microsoft.com/en-us/products/storage/tables) | Medium | Subsidiary | storage | Azure key-value/table storage; consumption-based. Can migrate to Cosmos DB for Table for higher scale and global distribution. | 2025 |
| [Couchbase](https://www.couchbase.com/) | [↗](https://www.couchbase.com/) | High | Public | storage | NoSQL cloud database (key-value and document); public (Nasdaq BASE, 2021). Enterprise customers include Comcast, eBay; over $100M ARR at IPO. | 2025 |
| [Datastax (Cassandra)](https://www.datastax.com/) | [↗](https://www.datastax.com/) | High | Subsidiary | storage | Cassandra-based data platform (Astra DB, Langflow); acquired by IBM (May 2025) for watsonx. Had raised $300M+; strong in distributed NoSQL and AI tooling. | 2025 |
| [Fauna](https://fauna.com/home) | [↗](https://fauna.com/home) | Medium | Series A | storage, streaming | Distributed serverless document database with relational features; service ending May 2025. Raised $57M total. | 2025 |
| [Google Cloud Bigtable](https://cloud.google.com/bigtable) | [↗](https://cloud.google.com/bigtable) | High | Subsidiary | storage | Fully managed wide-column NoSQL database for high throughput and low latency; ML, IoT, analytics. Supports Cassandra and HBase APIs. | 2025 |
| [Google Cloud Firestore](https://cloud.google.com/products/firestore) | [↗](https://cloud.google.com/products/firestore) | High | Subsidiary | storage | Serverless document database on GCP; Native and Datastore modes. Part of Google Cloud databases with Database Center management. | 2025 |
| [HarperDB](https://www.harpersystems.dev/) | [↗](https://www.harpersystems.dev/) | Medium | OSS | storage | Unified backend (database, cache, app hosting, messaging); Node.js, REST/GraphQL, vector search. Also marketed as Harper. | 2025 |
| [MongoDB](https://www.mongodb.com/) | [↗](https://www.mongodb.com/) | High | Public | storage | Document database and Atlas platform; public (Nasdaq MDB). Dominant in document store and developer experience; strong analytics and search features. | 2025 |
| [Oracle NoSQL](https://www.oracle.com/) | [↗](https://www.oracle.com/) | Medium | Subsidiary | storage | Oracle’s key-value/document NoSQL database; flexible schema, scalability, and integration with Oracle ecosystem. | 2025 |
| [Progress MarkLogic](https://www.progress.com/marklogic) | [↗](https://www.progress.com/marklogic) | Medium | Subsidiary | storage | Multi-model NoSQL (XML, JSON, text, RDF, geospatial); enterprise security and search. Acquired by Progress (2023); strong for unstructured and evolving schemas. | 2025 |
| [Redis Enterprise](https://redis.io/docs/latest/operate/rs/) | [↗](https://redis.io/docs/latest/operate/rs/) | High | Series D+ | storage, streaming | Redis-based real-time data platform; enterprise clustering, multi-model (cache, document, vector). Raised $355M+; Series G 2021 at $2B valuation. | 2025 |
| [ScyllaDB](https://www.scylladb.com/) | [↗](https://www.scylladb.com/) | High | Series D+ | storage | High-performance Cassandra-compatible database (C++); drop-in replacement with lower latency. Raised $43M (2023); DynamoDB-compatible API option. | 2025 |
| [Upstash](https://upstash.com/) | [↗](https://upstash.com/) | High | Series A | storage, streaming | Serverless data platform (Redis, Kafka, QStash, Vector). $10M Series A (a16z, 2024); pay-per-request, strong developer adoption. | 2025 |

### Real-Time Analytics / HTAP

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Apache Doris](https://github.com/apache/doris) | [↗](https://github.com/apache/doris) | High | OSS | storage-warehouse, analytics | Apache MPP analytical database; sub-second queries, real-time analytics, reporting, and data lake acceleration. Open source, widely adopted. | 2025 |
| [Apache Druid](https://github.com/apache/druid) | [↗](https://github.com/apache/druid) | High | OSS | storage-warehouse, analytics | Apache real-time OLAP database; sub-second queries on streaming and batch, Kafka/Kinesis integration. Columnar, time-indexed, high concurrency. | 2025 |
| [Apache Pinot](https://github.com/apache/pinot) | [↗](https://github.com/apache/pinot) | High | OSS | storage-warehouse, analytics | Apache distributed OLAP store (LinkedIn-origin); low-latency at petabyte scale, batch and streaming ingestion. Rich indexing and SQL. | 2025 |
| [Clickhouse](https://clickhouse.com/) | [↗](https://clickhouse.com/) | High | Series D+ | storage-warehouse, analytics | OLAP database company (open-source core); $350M+ Series C (2025), $400M Series D. 2k+ customers, strong growth; used by Meta, Tesla, Anthropic. | 2025 |
| [e6data](https://www.e6data.com/) | [↗](https://www.e6data.com/) | Medium | Series A | analytics, compute | Compute engine for data intelligence platforms; aims to cut analysis cost ~50% and improve performance 5x, reduce vendor lock-in. $10M Series A (Accel, 2024). | 2025 |
| [Firebolt](https://www.firebolt.io/home-v2) | [↗](https://www.firebolt.io/home-v2) | High | TBD | storage-warehouse, analytics | Cloud data warehouse for analytics; positions for speed and elasticity. Used for analytical workloads on large data; stage not confirmed from search. | 2025 |
| [Imply](https://imply.io/) | [↗](https://imply.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [InfluxData](https://www.influxdata.com/) | [↗](https://www.influxdata.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [KX](https://kx.com/) | [↗](https://kx.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Materialize](https://materialize.com/) | [↗](https://materialize.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [MotherDuck](https://motherduck.com/) | [↗](https://motherduck.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [QuestDB](https://questdb.io/) | [↗](https://questdb.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Redis](https://redis.com/) | [↗](https://redis.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [RisingWave Labs](https://www.risingwave-labs.com/) | [↗](https://www.risingwave-labs.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [SingleStore](https://www.singlestore.com/) | [↗](https://www.singlestore.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [StarRocks](https://www.starrocks.io/) | [↗](https://www.starrocks.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Startree](https://startree.ai/) | [↗](https://startree.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Tinybird](https://www.tinybird.co/) | [↗](https://www.tinybird.co/) | TBD | TBD | (see taxonomy) | — | 2025 |

### Relational & Distributed SQL

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AWS Aurora](https://aws.amazon.com/rds/aurora/) | [↗](https://aws.amazon.com/rds/aurora/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [AWS RDS](https://aws.amazon.com/rds/) | [↗](https://aws.amazon.com/rds/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Azure SQL Database](https://azure.microsoft.com/en-us/products/azure-sql/database) | [↗](https://azure.microsoft.com/en-us/products/azure-sql/database) | TBD | TBD | (see taxonomy) | — | 2025 |
| [CockroachDB](https://www.cockroachlabs.com/) | [↗](https://www.cockroachlabs.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Dassault Systemes NuoDB](https://www.3ds.com/nuodb-distributed-sql-database) | [↗](https://www.3ds.com/nuodb-distributed-sql-database) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Google Cloud AlloyDB](https://cloud.google.com/alloydb) | [↗](https://cloud.google.com/alloydb) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Google Cloud Cloud SQL](https://cloud.google.com/sql) | [↗](https://cloud.google.com/sql) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Google Cloud Spanner](https://cloud.google.com/spanner) | [↗](https://cloud.google.com/spanner) | TBD | TBD | (see taxonomy) | — | 2025 |
| [IBM DB2](https://www.ibm.com/products/db2) | [↗](https://www.ibm.com/products/db2) | TBD | TBD | (see taxonomy) | — | 2025 |
| [MariaDB](https://mariadb.com/products/enterprise/xpand/) | [↗](https://mariadb.com/products/enterprise/xpand/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Microsoft SQL Server](https://www.microsoft.com/en-us/sql-server) | [↗](https://www.microsoft.com/en-us/sql-server) | TBD | TBD | (see taxonomy) | — | 2025 |
| [MySQL](https://github.com/mysql/mysql-server) | [↗](https://github.com/mysql/mysql-server) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Neon](https://neon.com/) | [↗](https://neon.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Nile](https://www.thenile.dev/) | [↗](https://www.thenile.dev/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Oracle](https://www.oracle.com/) | [↗](https://www.oracle.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [pgEdge](https://www.pgedge.com/) | [↗](https://www.pgedge.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [PlanetScale](https://planetscale.com/) | [↗](https://planetscale.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [PostgreSQL](https://github.com/postgres/postgres) | [↗](https://github.com/postgres/postgres) | TBD | TBD | (see taxonomy) | — | 2025 |
| [SAP ASE](https://www.sap.com/products/technology-platform/sybase-ase.html) | [↗](https://www.sap.com/products/technology-platform/sybase-ase.html) | TBD | TBD | (see taxonomy) | — | 2025 |
| [SAP HANA Cloud](https://www.sap.com/products/technology-platform/hana.html) | [↗](https://www.sap.com/products/technology-platform/hana.html) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Supabase](https://supabase.com/) | [↗](https://supabase.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [TigerBeetle](https://tigerbeetle.com/) | [↗](https://tigerbeetle.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [TigerData](https://www.tigerdata.com/) | [↗](https://www.tigerdata.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Volt Active Data](https://www.voltactivedata.com/) | [↗](https://www.voltactivedata.com/) | Medium | TBD | storage, compute | In-memory operational SQL database for high-throughput, low-latency use cases (telco, fintech). Formerly VoltDB; strong in real-time decisioning and event processing. | 2025 |
| [YugabyteDB](https://www.yugabyte.com/) | [↗](https://www.yugabyte.com/) | High | Series C | storage, storage-warehouse | Distributed SQL database with PostgreSQL compatibility; horizontal scaling and multi-region. Series C $188M (2022); key alternative to single-region RDS. | 2025 |

### Storage

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Amazon S3](https://aws.amazon.com/s3/) | [↗](https://aws.amazon.com/s3/) | High | Subsidiary | storage | Object storage standard for data lakes and analytics; S3-compatible APIs widely adopted. De facto cloud object store; integrates across AWS and many third-party tools. | 2025 |
| [Azure Storage](https://azure.microsoft.com/products/storage) | [↗](https://azure.microsoft.com/products/storage) | High | Subsidiary | storage | Object, block, and file storage on Azure; Data Lake Gen2 for analytics. Core storage for Azure Synapse, Databricks on Azure, and enterprise data lakes. | 2025 |
| [Backblaze](https://www.backblaze.com/b2/docs/s3_compatible_api.html) | [↗](https://www.backblaze.com/b2/docs/s3_compatible_api.html) | Medium | Public | storage | B2 cloud object storage with S3-compatible API; low-cost backup and archive. Public (BLZE); differentiator is pricing and simplicity for SMB/backup. | 2025 |
| [Cloudflare R2](https://www.cloudflare.com/products/r2/) | [↗](https://www.cloudflare.com/products/r2/) | High | Public | storage | S3-compatible object storage with zero egress fees; strong for edge and global apps. Public (Cloudflare); differentiator is egress pricing and Cloudflare network. | 2025 |
| [Google Cloud Storage](https://cloud.google.com/storage) | [↗](https://cloud.google.com/storage) | High | Subsidiary | storage | Object and multi-class storage for GCP; backbone for BigQuery, Dataproc, and data lakes. Unified with Google Cloud and strong for analytics workloads. | 2025 |
| [IBM Storage](https://www.ibm.com/storage) | [↗](https://www.ibm.com/storage) | Medium | Subsidiary | storage | Enterprise storage portfolio (block, file, object, tape); Cloud Object Storage and FlashSystem. Subsidiary of IBM; strong in hybrid and regulated industries. | 2025 |
| [MinIO](https://min.io/) | [↗](https://min.io/) | High | Series B | storage, storage-lakehouse | High-performance, S3-compatible object store for on-prem and cloud; often used as lakehouse storage layer. Series B; key in open data lake and Kubernetes-native deployments. | 2025 |
| [NetApp](https://www.netapp.com/) | [↗](https://www.netapp.com/) | Medium | Public | storage | Unified storage (file, block, object) and cloud data services (ONTAP, BlueXP). Public (NTAP); strong in hybrid and enterprise data management. | 2025 |
| [Oracle Object Storage](https://www.oracle.com/cloud/storage/object-storage/) | [↗](https://www.oracle.com/cloud/storage/object-storage/) | Medium | Subsidiary | storage | Object storage in Oracle Cloud; integrates with Oracle DB, Autonomous Data Warehouse, and analytics. Part of OCI; relevant for Oracle-centric estates. | 2025 |
| [Vast Data](https://vastdata.com/) | [↗](https://vastdata.com/) | High | Series D+ | storage, storage-lakehouse | Data platform unifying storage, database, and analytics; all-flash and scale-out. ~$9B valuation (2023); positioned for AI and large-scale data. | 2025 |
| [Wasabi](https://wasabi.com/) | [↗](https://wasabi.com/) | Medium | Series D+ | storage | Hot cloud object storage with predictable pricing and S3-compatible API. Series D $112M; differentiator is low cost and no egress fees for many use cases. | 2025 |

### Stream Processing & Streaming ETL

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Apache Beam](https://github.com/apache/beam) | [↗](https://github.com/apache/beam) | High | OSS | streaming, transformation | Portable unified model for batch and streaming pipelines; runs on Flink, Spark, Dataflow, etc. OSS; key for vendor-neutral stream and batch abstraction. | 2025 |
| [AWS Kinesis Data Analytics](https://aws.amazon.com/kinesis/) | [↗](https://aws.amazon.com/kinesis/) | High | Subsidiary | streaming, analytics | Managed streaming (Kinesis Data Streams, Firehose) and SQL/Flink-based analytics on AWS. Core streaming option for AWS-native data pipelines. | 2025 |
| [Azure Stream Analytics](https://azure.microsoft.com/en-us/products/stream-analytics) | [↗](https://azure.microsoft.com/en-us/products/stream-analytics) | High | Subsidiary | streaming, analytics | Managed real-time analytics and stream processing on Azure (Event Hubs, IoT Hub). SQL and scale-out; integrates with Power BI and Azure data services. | 2025 |
| [Chalk](https://chalk.ai/) | [↗](https://chalk.ai/) | High | Series A | ml-ops, ai-dev | Feature platform for real-time and batch feature computation; powers ML models in production. Series A $50M (2024); differentiator is online/offline consistency and low-latency features. | 2025 |
| [Confluent Kafka Connect / ksqlDB](https://docs.confluent.io/platform/current/connect/index.html) | [↗](https://docs.confluent.io/platform/current/connect/index.html) | High | Public | streaming, ingestion, transformation | Kafka Connect for source/sink integration and ksqlDB for stream SQL; managed Kafka ecosystem. Confluent is public; de facto standard for event streaming and CDC. | 2025 |
| [Debezium](https://github.com/debezium/debezium) | [↗](https://github.com/debezium/debezium) | High | OSS | streaming, ingestion | CDC platform for capturing DB change events and streaming to Kafka; supports PostgreSQL, MySQL, MongoDB, etc. OSS (Red Hat); key for log-based replication and real-time sync. | 2025 |
| [Decodable](https://www.decodable.co/) | [↗](https://www.decodable.co/) | High | Series B | streaming, transformation | Managed streaming data platform with SQL; real-time pipelines and connectors. Series B; serverless streaming with focus on developer experience and Flink under the hood. | 2025 |
| [DeltaStream](https://deltastream.io/) | [↗](https://deltastream.io/) | High | Series A | streaming | Managed streaming store and compute (Flink-based) with SQL; unified storage and processing. Series A; positioned for real-time analytics and event-driven apps. | 2025 |
| [Estuary](https://www.estuary.dev/) | [↗](https://www.estuary.dev/) | High | Series B | streaming, ingestion, transformation | Real-time data platform (Flow) for CDC and streaming ETL; batch and stream in one. Series B; differentiator is exactly-once and low-latency materialization to warehouses and lakes. | 2025 |
| [Flink](https://github.com/apache/flink) | [↗](https://github.com/apache/flink) | High | OSS | streaming, transformation | Apache Flink: distributed stream and batch processing engine; stateful computations and event time. OSS; industry standard for real-time stream processing and used by many managed offerings. | 2025 |
| [Google Cloud Dataflow](https://cloud.google.com/dataflow) | [↗](https://cloud.google.com/dataflow) | High | Subsidiary | streaming, transformation | Managed Beam runner for batch and streaming on GCP; autoscaling and serverless. Core option for Google-native data pipelines and BigQuery streaming. | 2025 |
| [Hazelcast](https://hazelcast.com/) | [↗](https://hazelcast.com/) | Medium | Series D+ | streaming, compute | In-memory data grid and stream processing (Hazelcast Jet/Viridian); real-time analytics and caching. Late-stage; used in financial and high-throughput workloads. | 2025 |
| [Quix](https://www.quix.io/) | [↗](https://www.quix.io/) | High | Series A | streaming, ai-dev | Stream processing platform for ML and real-time data; Python/SDK and Kafka-native. Series A; targets data scientists and ML teams building streaming pipelines. | 2025 |
| [Striim](https://www.striim.com/) | [↗](https://www.striim.com/) | High | Subsidiary | streaming, ingestion | Real-time data integration and CDC; streaming to cloud warehouses and lakes. Acquired by Oracle (GoldenGate); part of Oracle’s real-time data portfolio. | 2025 |
| [Upsolver](https://www.upsolver.com/) | [↗](https://www.upsolver.com/) | High | Series B | streaming, ingestion, storage-lakehouse | SQL-based streaming ingestion into data lakes (e.g. S3, Delta); incremental and batch. Series B; differentiator is simplicity for lakehouse ingestion from Kafka and DBs. | 2025 |

### Vector Databases

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Activeloop](https://www.activeloop.ai/) | [↗](https://www.activeloop.ai/) | High | Series B | storage-vector, ml-ops, ai-dev | Deep Lake: vector store and dataset format for ML/AI; integrates with PyTorch and training pipelines. Series B; differentiator is unified storage for embeddings and raw data for model training. | 2025 |
| [Chroma](https://www.trychroma.com/) | [↗](https://www.trychroma.com/) | High | Series A | storage-vector, ai-dev | Embedding store and vector DB for LLM apps; open-source and hosted. Series A; popular in RAG and developer-first AI stacks. | 2025 |
| [Databricks Vector Search](https://docs.databricks.com/generative-ai/vector-search.html) | [↗](https://docs.databricks.com/generative-ai/vector-search.html) | High | Series D+ | storage-vector, enterprise-ai | Native in lakehouse; Unity Catalog integration. | 2025 |
| [Elastic ES Vector](https://www.elastic.co/elasticsearch/vector-database) | [↗](https://www.elastic.co/elasticsearch/vector-database) | High | Public | storage-vector, analytics | Vector search in Elasticsearch; hybrid search combining vectors with keyword and filters. Elastic is public; strong for search and observability workloads needing vector capability. | 2025 |
| [LanceDB](https://lancedb.com/) | [↗](https://lancedb.com/) | High | OSS | storage-vector, ai-dev | Embedded and serverless vector DB built on Lance columnar format; OSS-first. Differentiator is no separate server for many use cases and tight integration with data lakes. | 2025 |
| [Marqo](https://www.marqo.ai/) | [↗](https://www.marqo.ai/) | Medium | Seed | storage-vector, ai-dev | Vector search and ML search platform; indexing and retrieval for RAG and semantic search. Early-stage; focuses on end-to-end indexing and multi-vector models. | 2025 |
| [MongoDB Atlas Vector](https://www.mongodb.com/products/platform/atlas-vector-search) | [↗](https://www.mongodb.com/products/platform/atlas-vector-search) | High | Public | storage-vector, storage-warehouse | Vector search in MongoDB Atlas; combines document store with vector index for RAG and search. MongoDB is public; strong for apps already on Atlas needing vector without a separate DB. | 2025 |
| [OpenSearch KNN](https://docs.opensearch.org/latest/query-dsl/specialized/k-nn/index/) | [↗](https://docs.opensearch.org/latest/query-dsl/specialized/k-nn/index/) | High | Subsidiary | storage-vector, ai-dev | AWS-managed k-NN and ANN vector search in OpenSearch; HNSW/IVF, hybrid search, disk-optimized mode. Recommended vector store for Amazon Bedrock and production RAG. | 2025 |
| [Pinecone](https://www.pinecone.io/) | [↗](https://www.pinecone.io/) | High | Series B | storage-vector, ai-dev | Managed vector DB; $100M Series B (2023) at $750M valuation. Strong brand and developer adoption; serverless option (2024) for lower cost. | 2025 |
| [PostgreSQL Pgvector](https://github.com/pgvector/pgvector) | [↗](https://github.com/pgvector/pgvector) | High | OSS | storage-vector, storage-warehouse | Open-source vector extension for PostgreSQL; embeds vector search in existing Postgres workloads. Widely used for RAG and hybrid SQL+vector. | 2025 |
| [Qdrant](https://qdrant.tech/) | [↗](https://qdrant.tech/) | High | Series A | storage-vector, ai-dev | Open-source vector DB (Rust); $28M Series A (Jan 2024). Strong adoption for RAG and GenAI; managed cloud and on-prem enterprise options. | 2025 |
| [Redis Vector](https://redis.io/solutions/vector-database/) | [↗](https://redis.io/solutions/vector-database/) | High | Series D+ | storage-vector, ai-dev | Redis Vector Search and RedisVL; in-memory vector indexes (FLAT, HNSW). Integrates with LangChain, LlamaIndex, Bedrock; positioned for low-latency GenAI. | 2025 |
| [Snowflake Cortex Vector](https://www.snowflake.com/) | [↗](https://www.snowflake.com/) | High | Public | storage-vector, enterprise-ai | Vector search and embeddings inside Snowflake; ties into Cortex AI for RAG and LLM apps. Single platform for warehouse and vector workloads. | 2025 |
| [Turbopuffer](https://turbopuffer.com/) | [↗](https://turbopuffer.com/) | Medium | TBD | storage-vector, ai-dev | Serverless vector and full-text search on object storage; hybrid vector+BM25. Used by Cursor, Notion, Linear; cost-focused, no public funding data. | 2025 |
| [Vald](https://vald.vdaas.org/) | [↗](https://vald.vdaas.org/) | Medium | OSS | storage-vector, ai-dev | Distributed ANN search engine (NGT); cloud-native, Kubernetes-friendly. Open-source (vdaas); async indexing and multi-language clients. | 2025 |
| [Vespa](https://vespa.ai/) | [↗](https://vespa.ai/) | High | OSS | storage-vector, ai-dev | Yahoo-origin open-source engine (2017); vector, text, and ML ranking at scale. Early vector adoption; powers RAG, recommendations, and search. | 2025 |
| [Weaviate](https://weaviate.io/) | [↗](https://weaviate.io/) | High | Series B | storage-vector, ai-dev | Vector DB with GraphQL and hybrid search; $50M Series B (2023). Open-source plus Weaviate Cloud; strong in RAG and GenAI tooling. | 2025 |
| [Zilliz](https://zilliz.com/) | [↗](https://zilliz.com/) | High | Series B | storage-vector, ai-dev | Milvus maintainer; $60M Series B extension (2022), $113M+ total. Zilliz Cloud managed service; Forrester Leader in vector DB (2024). | 2025 |

## ML & AI

### AI Developer Platforms & Agents

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Databricks Mosaic AI Gateway](https://docs.databricks.com/generative-ai/gateway.html) | [↗](https://docs.databricks.com/generative-ai/gateway.html) | High | Series D+ | enterprise-ai, ai-dev | Model routing and governance in lakehouse. Centralized API and policy for LLM calls across Databricks workloads. | 2025 |
| [Hugging Face](https://huggingface.co/) | [↗](https://huggingface.co/) | High | Series D | ai-dev, marketplace, ml-ops | Hub for models and datasets; Spaces and inference. $235M Series D (2023) at $4.5B; default platform for open and enterprise AI tooling. | 2025 |
| [LangChain](https://www.langchain.com/) | [↗](https://www.langchain.com/) | High | Series B | ai-dev, agents | Dominant framework for LLM apps and chains. $125M Series B (Oct 2025) at $1.25B; broad adoption for RAG and agent engineering. | 2025 |
| [LlamaIndex](https://www.llamaindex.ai/) | [↗](https://www.llamaindex.ai/) | High | Series A | ai-dev, unstructured-etl | RAG and data frameworks; LlamaParse, LlamaCloud. $19M Series A (Mar 2025); strong OSS adoption for knowledge agents and document pipelines. | 2025 |
| [Model Context Protocol](https://modelcontextprotocol.io/) | [↗](https://modelcontextprotocol.io/) | High | OSS | ai-dev, agents | Open standard (Anthropic, Nov 2024) for connecting AI apps to data and tools. SDKs and MCP servers; adopted by Claude, ChatGPT, Cursor, VS Code. | 2025 |

### Enterprise AI Platforms

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AWS Bedrock](https://aws.amazon.com/bedrock/) | [↗](https://aws.amazon.com/bedrock/) | High | Subsidiary | enterprise-ai, ai-dev | AWS managed service for foundation models and RAG; multiple model providers, agents, and Knowledge Bases. Core to AWS GenAI stack. | 2025 |
| [Databricks Mosaic AI](https://www.databricks.com/product/mosaic-ai) | [↗](https://www.databricks.com/product/mosaic-ai) | High | Series D+ | enterprise-ai, ml-ops | End-to-end GenAI on lakehouse; MosaicML, DBRX, gateway, RAG. Central to Databricks AI/ML and governance strategy. | 2025 |
| [Dataiku](https://www.dataiku.com/) | [↗](https://www.dataiku.com/) | High | Series D+ | enterprise-ai, ml-ops | Enterprise AI and analytics platform; $400M Series E (2021), $4.6B valuation. Data prep, AutoML, MLOps, and governance for large enterprises. | 2025 |
| [Google Cloud Vertex AI](https://cloud.google.com/vertex-ai) | [↗](https://cloud.google.com/vertex-ai) | High | Subsidiary | enterprise-ai, ml-ops | Unified ML and GenAI on GCP; training, deployment, agents, and RAG. Core to Google Cloud AI strategy. | 2025 |
| [Microsoft Azure AI Studio](https://azure.microsoft.com/products/ai-studio) | [↗](https://azure.microsoft.com/products/ai-studio) | High | Subsidiary | enterprise-ai, ai-dev | Azure hub for building GenAI apps; model catalog, prompt flow, RAG, and safety. Tied to Azure data and identity. | 2025 |
| [Palantir](https://www.palantir.com/) | [↗](https://www.palantir.com/) | High | Public | enterprise-ai, analytics, governance | Public company; AIP and Foundry for enterprise AI and data. Strong in government and defense; data governance and lineage. | 2025 |
| [Snowflake Cortex AI](https://www.snowflake.com/) | [↗](https://www.snowflake.com/) | High | Public | enterprise-ai, analytics | LLMs, embeddings, and RAG inside Snowflake. Unifies analytics and AI in the data cloud; competes with lakehouse AI offerings. | 2025 |

### MLOps & Data Science

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Amazon SageMaker](https://aws.amazon.com/sagemaker/) | [↗](https://aws.amazon.com/sagemaker/) | High | Subsidiary | ml-ops, enterprise-ai | AWS ML platform; build, train, deploy models and GenAI. Broad adoption; Bedrock integration for foundation models. | 2025 |
| [Azure Machine Learning](https://azure.microsoft.com/products/machine-learning) | [↗](https://azure.microsoft.com/products/machine-learning) | High | Subsidiary | ml-ops, enterprise-ai | Azure ML for training, deployment, and MLOps; integrates with Azure AI Studio and Synapse. Core to Microsoft data+AI stack. | 2025 |
| [Databricks Mosaic AI](https://www.databricks.com/product/mosaic-ai) | [↗](https://www.databricks.com/product/mosaic-ai) | High | Series D+ | enterprise-ai, ml-ops | End-to-end GenAI; MosaicML; DBRX; gateway. Primary AI/ML surface on Databricks lakehouse. | 2025 |
| [Databricks Notebooks](https://docs.databricks.com/notebooks/) | [↗](https://docs.databricks.com/notebooks/) | High | Series D+ | ml-ops, analytics | Collaborative notebooks with Delta and Unity Catalog. Core for data science and ML workflows on Databricks. | 2025 |
| [Google Cloud Vertex AI](https://cloud.google.com/vertex-ai) | [↗](https://cloud.google.com/vertex-ai) | High | Subsidiary | ml-ops, enterprise-ai | Unified ML and GenAI on GCP; training, deployment, MLOps, and model governance. | 2025 |
| [MLflow](https://mlflow.org/) | [↗](https://mlflow.org/) | High | OSS | ml-ops, ai-dev | Open-source ML lifecycle; experiments, models, registry, projects. De facto standard; native in Databricks and many platforms. | 2025 |
| [Snowflake Notebooks](https://www.snowflake.com/) | [↗](https://www.snowflake.com/) | High | Public | ml-ops, analytics | Notebooks and Python/SQL in Snowflake for analytics and ML. Part of Cortex and data cloud workflows. | 2025 |
| [Weights & Biases](https://wandb.ai/) | [↗](https://wandb.ai/) | High | Series C | ml-ops, ai-dev | Experiment tracking, visualization, and MLOps. $200M Series C (2024) at $1.25B; widely used for training and evaluation. | 2025 |

## Machine Learning & Artificial Intelligence — Build

### AI Developer Platforms

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Adaptive](https://www.adaptive-ml.com/) | [↗](https://www.adaptive-ml.com/) | Medium | TBD | ai-dev | AI developer platform; limited public information on funding or product. Positioned in MAD landscape under AI developer platforms. | 2025 |
| [Anyscale](https://www.anyscale.com/) | [↗](https://www.anyscale.com/) | High | Series C | ai-dev, compute, ml-ops | Managed Ray; $100M Series C (2024) at $1B. Scale AI training and serving; used by Amazon, Uber, Shopify; GPU-native and Ray Data GA. | 2025 |
| [Arcee AI](https://www.arcee.ai/#) | [↗](https://www.arcee.ai/#) | High | Series A | enterprise-ai, ai-dev | Enterprise AFM foundation models and platform; $24M Series A (2024), strategic round (2025). Compact, domain-optimized LLMs; open/partial open-source. | 2025 |
| [Contextual AI](https://contextual.ai/) | [↗](https://contextual.ai/) | High | Series A | enterprise-ai, ai-dev | Production CLMs and RAG 2.0 for enterprises; $80M Series A (Aug 2024). Qualcomm deployment; knowledge-intensive and on-prem/SaaS options. | 2025 |
| [Daytona](https://www.daytona.io/) | [↗](https://www.daytona.io/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Deepset](https://www.deepset.ai/) | [↗](https://www.deepset.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [E2B](https://e2b.dev/) | [↗](https://e2b.dev/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Hugging Face](https://huggingface.co/) | [↗](https://huggingface.co/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Langchain](https://www.langchain.com/) | [↗](https://www.langchain.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [LastMile AI](https://lastmileai.dev/) | [↗](https://lastmileai.dev/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Lightning AI](https://lightning.ai/) | [↗](https://lightning.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [LlamaIndex](https://www.llamaindex.ai/) | [↗](https://www.llamaindex.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Predibase](https://predibase.com/) | [↗](https://predibase.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Replicate](https://replicate.com/) | [↗](https://replicate.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Vercel AI SDK](https://ai-sdk.dev/docs/introduction) | [↗](https://ai-sdk.dev/docs/introduction) | TBD | TBD | (see taxonomy) | — | 2025 |

### Agent Infra / Tooling

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AgentOps](https://www.agentops.ai/) | [↗](https://www.agentops.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Anon](https://www.anon.com/) | [↗](https://www.anon.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Browser Use](https://browser-use.com/) | [↗](https://browser-use.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Browserbase](https://www.browserbase.com/) | [↗](https://www.browserbase.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Composio](https://composio.dev/) | [↗](https://composio.dev/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Crawl4AI](https://github.com/unclecode/crawl4ai) | [↗](https://github.com/unclecode/crawl4ai) | TBD | TBD | (see taxonomy) | — | 2025 |
| [DSPy](https://github.com/stanfordnlp/dspy) | [↗](https://github.com/stanfordnlp/dspy) | TBD | TBD | (see taxonomy) | — | 2025 |
| [FastMCP](https://github.com/jlowin/fastmcp) | [↗](https://github.com/jlowin/fastmcp) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Firecrawl](https://github.com/mendableai/firecrawl) | [↗](https://github.com/mendableai/firecrawl) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Fleet](https://fleetai.com/) | [↗](https://fleetai.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Kaizen](https://www.kaizenautomation.com/) | [↗](https://www.kaizenautomation.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Letta](https://www.letta.com/) | [↗](https://www.letta.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Mechanize](https://www.mechanize.work/) | [↗](https://www.mechanize.work/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Mem0](https://mem0.ai/) | [↗](https://mem0.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Model Context Protocol](https://docs.anthropic.com/en/docs/mcp) | [↗](https://docs.anthropic.com/en/docs/mcp) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Nango](https://github.com/NangoHQ/nango) | [↗](https://github.com/NangoHQ/nango) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Paragon](https://www.useparagon.com/) | [↗](https://www.useparagon.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | [↗](https://github.com/microsoft/semantic-kernel) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Tiny Fish](https://www.tinyfish.ai/) | [↗](https://www.tinyfish.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Toolhouse](https://toolhouse.ai/) | [↗](https://toolhouse.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Veris AI](https://veris.ai/) | [↗](https://veris.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Zep](https://www.getzep.com/) | [↗](https://www.getzep.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [Zeta Labs](https://www.zetalabs.ai/) | [↗](https://www.zetalabs.ai/) | TBD | TBD | (see taxonomy) | — | 2025 |

### Agent Platforms

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Agno](https://www.agno.com/) | [↗](https://www.agno.com/) | TBD | TBD | (see taxonomy) | — | 2025 |
| [BabyAGI](https://github.com/yoheinakajima/babyagi) | [↗](https://github.com/yoheinakajima/babyagi) | Medium | OSS | ai-dev, agents | Minimal autonomous task-driven agent loop (task creation, prioritization, execution) popular as a learning template. Open-source GitHub project; not a commercial product. | 2025 |
| [Crew AI](https://www.crewai.com/) | [↗](https://www.crewai.com/) | High | Series A | ai-dev, agents, enterprise-ai | Multi-agent framework for building collaborative AI crews with roles and goals. Raised $18M total ($12.5M Series A Oct 2024); used by Fortune 500 for agentic workflows. | 2025 |
| [Dataiku](https://www.dataiku.com/) | [↗](https://www.dataiku.com/) | High | Series D+ | ml-ops, analytics, governance, enterprise-ai | Enterprise AI and ML platform for data prep, model building, MLOps, and governance. Late-stage private company; strong in regulated industries and data science teams. | 2025 |
| [Dust](https://dust.tt/) | [↗](https://dust.tt/) | High | Series A | ai-dev, agents, enterprise-ai | Operating system for AI agents: deploy and orchestrate specialized agents connected to company knowledge and tools. Raised $21.5M (Series A 2024 led by Sequoia); Paris-based. | 2025 |
| [Ema](https://www.ema.co/) | [↗](https://www.ema.co/) | Medium | TBD | agents, enterprise-ai, integration | AI agent platform for business automation and customer-facing workflows. Product focus on autonomous execution; limited public funding data. | 2025 |
| [Emergence](https://www.emergence.ai/) | [↗](https://www.emergence.ai/) | Medium | TBD | ai-dev, agents | Agentic AI systems with planning, reasoning, long-term memory, and self-improvement. Frontier-style agent research; enterprise partnerships; funding not disclosed. | 2025 |
| [Flowise](https://github.com/FlowiseAI/Flowise) | [↗](https://github.com/FlowiseAI/Flowise) | High | Subsidiary | ai-dev, agents | Open-source low-code UI for building LLM flows and agents with drag-and-drop; LangChain-based. Acquired by Workday (Aug 2025); previously YC-backed. | 2025 |
| [Glean](https://www.glean.com/) | [↗](https://www.glean.com/) | High | Series D+ | agents, enterprise-ai, catalog | Enterprise search and work AI platform; connects to company data and apps for RAG and agent-style answers. Series E $260M (Sept 2024) at $4.6B valuation; strong enterprise adoption. | 2025 |
| [Google Cloud Vertex AI Agent Builder](https://cloud.google.com/products/agent-builder?hl=en) | [↗](https://cloud.google.com/products/agent-builder?hl=en) | High | Subsidiary | ai-dev, agents, enterprise-ai | Google Cloud service for building search and conversational agents on enterprise data with grounding and safety controls. Part of Vertex AI; integrates with BigQuery and Workspace. | 2025 |
| [Instalily](https://instalily.ai/) | [↗](https://instalily.ai/) | Medium | Series A | agents, enterprise-ai, integration | AI Teammates (InstaWorkers) for distribution-heavy industries; execute workflows in ERPs/CRMs. Raised $25M Series A (Insight Partners); focus on insurance, healthcare, industrial. | 2025 |
| [Langbase](https://langbase.com/) | [↗](https://langbase.com/) | Medium | TBD | ai-dev, agents | Platform for building and deploying LLM applications and agents with minimal code. Early-stage; funding not widely reported. | 2025 |
| [LangGraph](https://www.langchain.com/) | [↗](https://www.langchain.com/) | High | Series B | ai-dev, agents | LangChain’s framework for stateful, multi-step agent workflows and graphs. Part of LangChain ($1.25B valuation Oct 2025); widely used for production agents. | 2025 |
| [LlamaIndex](https://www.llamaindex.ai/) | [↗](https://www.llamaindex.ai/) | High | Series A | ai-dev, agents | Data framework for RAG and knowledge agents; ingestion, indexing, and querying over documents and APIs. $19M Series A (March 2025); strong open-source adoption. | 2025 |
| [Lyzr](https://www.lyzr.ai/) | [↗](https://www.lyzr.ai/) | High | Series A | ai-dev, agents, enterprise-ai | Enterprise agent infrastructure for building, deploying, and governing AI agents; supports on-prem and private cloud. $14.5M Series A+ (Accenture-led); focus on HR, sales, banking. | 2025 |
| [Microsoft Autogen](https://www.microsoft.com/en-us/research/project/autogen/) | [↗](https://www.microsoft.com/en-us/research/project/autogen/) | High | Subsidiary | ai-dev, agents | Microsoft Research framework for multi-agent conversations and human-in-the-loop workflows. Open-source; research-oriented; influences agent design patterns. | 2025 |
| [Microsoft Copilot Studio](https://www.microsoft.com/en-us/microsoft-365-copilot/microsoft-copilot-studio) | [↗](https://www.microsoft.com/en-us/microsoft-365-copilot/microsoft-copilot-studio) | High | Subsidiary | agents, enterprise-ai, integration | Low-code tool for building copilots and conversational agents in Microsoft 365 and Teams. Part of Microsoft; integrates with Power Platform and Graph. | 2025 |
| [Salesforce Agentforce](https://www.salesforce.com/agentforce/) | [↗](https://www.salesforce.com/agentforce/) | High | Subsidiary | agents, enterprise-ai | Salesforce’s AI agent layer for CRM: actions, knowledge grounding, and trust controls inside Sales, Service, and Data Cloud. Native to Salesforce ecosystem. | 2025 |
| [Servicenow](https://www.servicenow.com/) | [↗](https://www.servicenow.com/) | High | Public | agents, enterprise-ai, orchestration | Enterprise workflow and ITSM platform with Now Assist AI for agents, summarization, and automation. Public company; broad adoption in IT and HR. | 2025 |
| [Steamship](https://www.steamship.com/) | [↗](https://www.steamship.com/) | Medium | Seed | ai-dev, agents | Platform to build and deploy AI agents with Python SDK; serverless hosting, vector search, and integrations. Early-stage (Abstract, Formulate); also offers prebuilt “AI Employees.” | 2025 |
| [Writer](https://writer.com/) | [↗](https://writer.com/) | High | Series C | agents, enterprise-ai | Full-stack GenAI platform with Palmyra models, RAG, guardrails, and app builders for enterprise. $200M Series C (Nov 2024) at $1.9B valuation; strong in regulated verticals. | 2025 |

### Local / On-Device LLM Runtimes

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [GPT4ALL](https://github.com/nomic-ai/gpt4all) | [↗](https://github.com/nomic-ai/gpt4all) | High | OSS | ai-dev, compute | Open-source local LLM runtime and ecosystem by Nomic; run and fine-tune models on consumer hardware. Popular for privacy and offline use. | 2025 |
| [Jan](https://github.com/menloresearch/jan) | [↗](https://github.com/menloresearch/jan) | Medium | OSS | ai-dev, compute | Open-source local AI desktop app (Menlo Research); run models locally with a ChatGPT-like UI. Cross-platform; community-driven. | 2025 |
| [Llama.cpp](https://github.com/ggerganov/llama.cpp) | [↗](https://github.com/ggerganov/llama.cpp) | High | OSS | ai-dev, compute | C++ inference for LLaMA and compatible models; CPU and GPU, quantization, broad hardware support. De facto standard for local inference; no commercial entity. | 2025 |
| [llamafile](https://github.com/Mozilla-Ocho/llamafile) | [↗](https://github.com/Mozilla-Ocho/llamafile) | Medium | OSS | ai-dev, compute | Single-file distributable for running LLMs (Mozilla-Ocho); bundles llama.cpp and Cosmopolitan. Ease of distribution; no install for end users. | 2025 |
| [LMStudio](https://lmstudio.ai/) | [↗](https://lmstudio.ai/) | High | Series A | ai-dev, compute | Desktop app for discovering, running, and serving LLMs locally with a simple UI. $15.4M Series A1 (April 2025); strong developer adoption. | 2025 |
| [LocalAI](https://github.com/mudler/LocalAI) | [↗](https://github.com/mudler/LocalAI) | High | OSS | ai-dev, compute | Open-source local inference server; OpenAI-compatible API for LLMs and embeddings. Self-hosted alternative to cloud APIs; multiple backends. | 2025 |
| [LocalGPT](https://github.com/PromtEngineer/localGPT) | [↗](https://github.com/PromtEngineer/localGPT) | Medium | OSS | ai-dev, compute | Open-source local RAG and chat over documents; private document Q&A without cloud. Community project; built on local inference. | 2025 |
| [MLX](https://github.com/ml-explore/mlx) | [↗](https://github.com/ml-explore/mlx) | High | OSS | ai-dev, compute | Apple’s framework for ML on Apple Silicon; optimized for M-series. Used for local LLM inference and research; open-source from Apple ML Research. | 2025 |
| [Nexa AI](https://nexa.ai/) | [↗](https://nexa.ai/) | Medium | TBD | ai-dev, compute | On-device AI SDK and inference; run models on CPU/GPU/NPU. Hyperlink assistant and dev tools; funding stage not clearly reported. | 2025 |
| [Ollama](https://github.com/ollama/ollama) | [↗](https://github.com/ollama/ollama) | High | Seed | ai-dev, compute | Local LLM runtime with CLI and API; simple pull-and-run for models. Early-stage VC-backed (2024); very widely adopted for local dev and use. | 2025 |
| [Open WebUI](https://github.com/open-webui/open-webui) | [↗](https://github.com/open-webui/open-webui) | High | OSS | ai-dev, compute | Open-source web UI for local and remote LLMs; OpenAI-compatible, plugins, and multi-user. Community project; often paired with Ollama. | 2025 |
| [OpenLLM](https://github.com/bentoml/OpenLLM) | [↗](https://github.com/bentoml/OpenLLM) | High | OSS | ai-dev, compute, ml-ops | Open-source LLM serving and deployment by BentoML; production inference, quantization, and tooling. Fits into existing MLOps and Kubernetes stacks. | 2025 |

## Machine Learning & Artificial Intelligence — Modalities & Research

### AI R&D - Commercial

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [01.ai](https://01.ai/) | [↗](https://01.ai/) | High | Series D+ | ai-dev, enterprise-ai | Kai-Fu Lee’s company; Yi family of LLMs and enterprise AI. $300M+ Series D (2023–24), unicorn; known for cost-efficient training and global deployment. | 2025 |
| [AI21Labs](https://www.ai21.com/) | [↗](https://www.ai21.com/) | High | Series D+ | ai-dev, enterprise-ai | LLM provider (Jamba) and enterprise orchestration (Maestro); focus on reliability and lower hallucinations. $300M Series D (2025) from Google, Nvidia; ~$636M total raised. | 2025 |
| [Alibaba Cloud](https://www.alibabacloud.com/en/solutions/ai/data-intelligence?_p_lc=1) | [↗](https://www.alibabacloud.com/en/solutions/ai/data-intelligence?_p_lc=1) | High | Subsidiary | ai-dev, enterprise-ai, compute | Alibaba Cloud’s AI and data intelligence: models, PAI platform, and data services. Part of Alibaba Group; strong in APAC and enterprise cloud AI. | 2025 |
| [Anthropic](https://www.anthropic.com/) | [↗](https://www.anthropic.com/) | High | Series D+ | ai-dev, enterprise-ai, agents | Frontier LLM lab; Claude models and API; safety-focused; major enterprise and platform partner. $30B+ valuation (2026); core to agents and RAG stacks. | 2025 |
| [Apple Machine Learning Research](https://machinelearning.apple.com/) | [↗](https://machinelearning.apple.com/) | Medium | Subsidiary | ai-dev, ml-ops | Apple's ML research division; on-device and foundation models; publishes research and contributes to ecosystem. Not a standalone commercial product. | 2025 |
| [Cohere](https://cohere.com/) | [↗](https://cohere.com/) | High | Series D+ | ai-dev, enterprise-ai | Enterprise-focused LLMs and embeddings; RAG, search, and classification. Strong vertical and sovereign AI positioning; key API alternative to OpenAI. | 2025 |
| [DeepSeek](https://www.deepseek.com/) | [↗](https://www.deepseek.com/) | High | Series B | ai-dev, enterprise-ai | Leading Chinese foundation model lab; open and commercial models; strong on coding and reasoning. Widely used in global dev and enterprise pipelines. | 2025 |
| [G42](https://www.g42.ai/) | [↗](https://www.g42.ai/) | Medium | Subsidiary | enterprise-ai, ai-dev | UAE-based AI and cloud conglomerate; Jais models and sovereign cloud. Government and enterprise focus; regional strategic relevance. | 2025 |
| [Google DeepMind](https://www.deepmind.com/) | [↗](https://www.deepmind.com/) | High | Subsidiary | ai-dev, enterprise-ai | Google's frontier AI research and products; Gemini, AlphaFold, Veo. Core to Google Cloud and enterprise AI; major model and infra provider. | 2025 |
| [H Company](https://www.hcompany.ai/) | [↗](https://www.hcompany.ai/) | Low | Seed | ai-dev | Emerging AI lab with limited public traction; early-stage. Relevance for landscape is watch only. | 2025 |
| [Imbue](https://imbue.com/) | [↗](https://imbue.com/) | Medium | Series C | ai-dev, agents | Focus on AI agents and reasoning; substantial funding ($200M+). Agentic workflows and coding; enterprise and dev tools in development. | 2025 |
| [Krutrim](https://olakrutrim.com/) | [↗](https://olakrutrim.com/) | Medium | Series A | ai-dev, enterprise-ai | Ola-backed Indian LLM and AI company; multilingual and local language focus. Growing relevance in India and emerging markets. | 2025 |
| [Liquid](https://www.liquid.ai/) | [↗](https://www.liquid.ai/) | Low | Seed | ai-dev | Liquid neural networks and efficient AI research; early-stage. Niche research direction with limited commercial footprint so far. | 2025 |
| [Meta Research](https://research.facebook.com/) | [↗](https://research.facebook.com/) | High | Subsidiary | ai-dev, ml-ops | Meta's AI research; Llama, PyTorch, and open models. Critical for open-weight ecosystem and ML tooling; strong adoption in data/ML stacks. | 2025 |
| [Microsoft Research](https://www.microsoft.com/en-us/research/) | [↗](https://www.microsoft.com/en-us/research/) | High | Subsidiary | ai-dev, ml-ops | MSR AI; Phi, Copilot, and enterprise AI research. Core to Azure AI and enterprise deployments; tight with data and governance stack. | 2025 |
| [Mistral AI](https://mistral.ai/) | [↗](https://mistral.ai/) | High | Series C | ai-dev, enterprise-ai | European LLM leader; open and commercial models (Mixtral, etc.). Key alternative for sovereignty and cost; strong API and on-prem options. | 2025 |
| [Moonshot AI](https://www.moonshot.ai/) | [↗](https://www.moonshot.ai/) | Medium | Series B | ai-dev, enterprise-ai | Chinese LLM and long-context specialist; Kimi chatbot. Notable for long-context and search-integrated product; regional and global API relevance. | 2025 |
| [NDEA](https://ndea.com/) | [↗](https://ndea.com/) | Low | TBD | ai-dev | Limited public information; niche or regional AI R&D. Low relevance for core data/AI landscape until more traction is visible. | 2025 |
| [NVIDIA Research](https://www.nvidia.com/en-us/research/) | [↗](https://www.nvidia.com/en-us/research/) | High | Subsidiary | ai-dev, ml-ops, compute | GPU and AI research; NeMo, robotics, simulation. Central to training and inference infra; ecosystem lock-in for enterprise AI. | 2025 |
| [OpenAI](https://openai.com/) | [↗](https://openai.com/) | High | Public | ai-dev, enterprise-ai, agents | Market leader in GenAI; ChatGPT, GPT-4/5, API, and agents. Default choice for many enterprises; key partner and competitor for data/AI stacks. | 2025 |
| [Reflection](https://www.reflection.ai/) | [↗](https://www.reflection.ai/) | Low | Seed | ai-dev | AI safety and alignment research; early-stage. Watch for governance and safety tooling relevance. | 2025 |
| [Reka](https://reka.ai/) | [↗](https://reka.ai/) | High | Series B | ai-dev, enterprise-ai | Multimodal and fast models; European; enterprise API. Strong alternative for multimodal RAG and low-latency use cases. | 2025 |
| [Safe Superintelligence](https://ssi.inc/) | [↗](https://ssi.inc/) | Medium | Seed | ai-dev | Ilya Sutskever's lab focused on superintelligence and safety. Early; relevant for governance and safety narrative and future offerings. | 2025 |
| [Sakana AI](https://sakana.ai/) | [↗](https://sakana.ai/) | Medium | Series A | ai-dev, enterprise-ai | Nature-inspired and efficient AI; Tokyo-based. Emerging model provider with focus on smaller, efficient models and enterprise. | 2025 |
| [Tencent AI Lab](https://ailab.tencent.com/ailab/en/index/) | [↗](https://ailab.tencent.com/ailab/en/index/) | Medium | Subsidiary | ai-dev, ml-ops | Tencent's AI research; gaming, content, and enterprise models. Regional relevance and potential for APIs and partnerships. | 2025 |
| [Thinking Machines](https://thinkingmachines.ai/) | [↗](https://thinkingmachines.ai/) | Low | Series A | ai-dev, consulting | Philippines-based data science and AI; mix of consulting and product. Lower relevance for core platform landscape; regional services. | 2025 |
| [World Labs](https://www.worldlabs.ai/) | [↗](https://www.worldlabs.ai/) | Low | Seed | ai-dev | Synthetic media and gaming AI; early-stage. Niche for creative and gaming pipelines; watch for GenAI media tooling. | 2025 |
| [xAI](https://x.ai/) | [↗](https://x.ai/) | High | Series B | ai-dev, enterprise-ai | Grok and inference; integrated with X (Twitter). Large funding; enterprise and consumer; growing API and infra relevance. | 2025 |

### AI R&D - Nonprofit / Academic

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Allen Institute](https://allenai.org/) | [↗](https://allenai.org/) | Medium | TBD | ai-dev | Nonprofit AI research (AllenNLP, OLMo, etc.); open models and benchmarks. Influential for NLP and open science; no commercial product. | 2025 |
| [BAIR](https://bair.berkeley.edu/) | [↗](https://bair.berkeley.edu/) | Medium | TBD | ai-dev, ml-ops | Berkeley AI Research; academic lab with open research and impact on ML practice. No commercial stage; ecosystem and talent relevance. | 2025 |
| [BigScience](https://bigscience.huggingface.co/) | [↗](https://bigscience.huggingface.co/) | Medium | OSS | ai-dev, data-sources | Hugging Face–led collaborative project; BLOOM and large open datasets. Historical impact on open LLMs and data; now part of HF ecosystem. | 2025 |
| [CAIS](https://safe.ai/) | [↗](https://safe.ai/) | Low | TBD | ai-dev | Center for AI Safety; nonprofit focused on AI safety and policy. Relevant for governance and safety narrative; no product. | 2025 |
| [Eleuther AI](https://www.eleuther.ai/) | [↗](https://www.eleuther.ai/) | High | OSS | ai-dev | Nonprofit open-source LLM research; GPT-NeoX, Pythia, and evaluation tools. Key for open weights and reproducibility; used in many pipelines. | 2025 |
| [ELLIS](https://ellis.eu/) | [↗](https://ellis.eu/) | Low | TBD | ai-dev | European network of AI excellence; academic and institutional. Ecosystem and talent; no direct product relevance. | 2025 |
| [EPFL](https://www.epfl.ch/research/) | [↗](https://www.epfl.ch/research/) | Low | TBD | ai-dev, ml-ops | EPFL research; academic ML/AI. Publications and talent; low direct relevance for commercial landscape. | 2025 |
| [Epoch AI](https://epoch.ai/) | [↗](https://epoch.ai/) | Medium | TBD | ai-dev | Research org focused on AI trends and scaling; influential reports and forecasts. Useful for strategy and landscape context; no product. | 2025 |
| [FAR.AI](https://www.far.ai/) | [↗](https://www.far.ai/) | Low | TBD | ai-dev | AI safety and alignment research. Niche; watch for governance and evaluation tooling. | 2025 |
| [Kyutai](https://kyutai.org/) | [↗](https://kyutai.org/) | Medium | TBD | ai-dev | French nonprofit AI lab; open research and models (Moshi, etc.). European open-source and research relevance; no commercial product. | 2025 |
| [LAION](https://laion.ai/) | [↗](https://laion.ai/) | High | OSS | data-sources, ai-dev | Nonprofit providing large-scale open image-text datasets (e.g. LAION-5B) for training vision and multimodal models; widely used by research and industry. No venture funding; community and grant supported. | 2025 |
| [MILA](https://mila.quebec/en/) | [↗](https://mila.quebec/en/) | High | TBD | ai-dev, ml-ops | Quebec AI research institute; 1,300+ researchers, 700+ publications (2023–24); government and industry funded ($36M Quebec grant 2026). Major hub for deep learning and talent. | 2025 |
| [MIRI](https://intelligence.org/) | [↗](https://intelligence.org/) | Medium | TBD | ai-dev | Nonprofit AI safety institute (Berkeley); focuses on existential risk from superintelligence and governance. Funded by donations and philanthropy (e.g. Open Philanthropy); 2025 fundraiser ~$3.2M. | 2025 |
| [MIT Csail](https://www.csail.mit.edu/) | [↗](https://www.csail.mit.edu/) | High | TBD | ai-dev, ml-ops | MIT’s computer science and AI lab; foundational research in ML, NLP, robotics, and systems. Academic; grant and institutional funding, not a commercial stage. | 2025 |
| [ML Commons](https://mlcommons.org/) | [↗](https://mlcommons.org/) | High | OSS | ml-ops, ai-dev | Open consortium behind MLPerf and related benchmarks for training and inference; industry and academic members. Drives standard evaluation for ML systems. | 2025 |
| [OpenMined](https://openmined.org/) | [↗](https://openmined.org/) | Medium | OSS | ai-dev, security-privacy | Community and nonprofit for privacy-preserving ML; PySyft and partnerships (e.g. PyTorch, NSF NAIRR). Focus on federated learning, differential privacy, and secure computation. | 2025 |
| [Redwood Research](https://www.redwoodresearch.org/) | [↗](https://www.redwoodresearch.org/) | Medium | TBD | ai-dev | Nonprofit AI safety lab (Berkeley); applied alignment work on control and deceptive alignment. Funded by Open Philanthropy and others; advises labs and governments. | 2025 |
| [Stanford HAI](https://hai.stanford.edu/) | [↗](https://hai.stanford.edu/) | High | TBD | ai-dev, ml-ops | Stanford institute for human-centered AI; funds interdisciplinary research (e.g. Hoffman-Yee grants, $40M+ to date). Major academic hub for AI policy and research. | 2025 |
| [The Alan Turing Institute](https://www.turing.ac.uk/) | [↗](https://www.turing.ac.uk/) | High | TBD | ai-dev, ml-ops | UK national institute for data science and AI; joint venture of universities and government. Research, training, and policy; not venture-backed. | 2025 |
| [Vector Institute](https://vectorinstitute.ai/) | [↗](https://vectorinstitute.ai/) | High | TBD | ai-dev, ml-ops | Toronto nonprofit AI institute; Pan-Canadian AI Strategy and Ontario funding (~$27M 2023). Research and talent in ML/DL; industry partners include Google, Shopify. | 2025 |

### Computer Vision

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Amazon Rekognition](https://docs.aws.amazon.com/managedservices/latest/userguide/rekognition.html) | [↗](https://docs.aws.amazon.com/managedservices/latest/userguide/rekognition.html) | High | Subsidiary | ai-dev, enterprise-ai | AWS managed service for image and video analysis (faces, objects, labels, moderation). Part of AWS AI stack; pay-per-use, scales with other AWS services. | 2025 |
| [Apple Vision (CoreML)](https://developer.apple.com/machine-learning/core-ml/) | [↗](https://developer.apple.com/machine-learning/core-ml/) | High | Subsidiary | ai-dev, ml-ops | Apple’s on-device ML framework; Vision for image models and Vision framework integration. Optimized for iPhone/iPad/Mac; privacy-focused, no cloud inference required. | 2025 |
| [Chooch](https://www.chooch.com/) | [↗](https://www.chooch.com/) | Medium | TBD | ai-dev | Computer vision and video understanding platform for use cases like safety and retail. Stage and funding not confirmed. | 2025 |
| [Encord](https://encord.com/) | [↗](https://encord.com/) | High | TBD | ml-ops, quality, unstructured-etl | Platform for computer vision data labeling, active learning, and model evaluation. Used for training and improving CV models; venture-backed, stage TBD. | 2025 |
| [Google Vertex AI Vision](https://cloud.google.com/vertex-ai-vision?hl=en) | [↗](https://cloud.google.com/vertex-ai-vision?hl=en) | High | Subsidiary | ai-dev, enterprise-ai | Google Cloud vision APIs and pipelines (classification, detection, video). Integrated with Vertex AI and BigQuery for enterprise CV workloads. | 2025 |
| [Intel OpenVINO](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) | [↗](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) | High | Subsidiary | ai-dev, ml-ops, compute | Intel toolkit for optimizing and deploying vision and other models on Intel CPUs, GPUs, and NPUs. Open-source; strong for edge and inference efficiency. | 2025 |
| [Meta SAM 2](https://ai.meta.com/sam2/) | [↗](https://ai.meta.com/sam2/) | High | Subsidiary | ai-dev | Meta’s Segment Anything Model 2; open weights for image and video segmentation. Foundation model for zero-shot segmentation and downstream CV tasks. | 2025 |
| [Nvidia TAO Toolkit](https://developer.nvidia.com/tao-toolkit) | [↗](https://developer.nvidia.com/tao-toolkit) | High | Subsidiary | ai-dev, ml-ops | Nvidia’s train-adapt-optimize toolkit for custom vision and other models; transfer learning and export to TensorRT. Part of Nvidia AI Enterprise for edge and data center. | 2025 |
| [ONNX](https://github.com/onnx/onnx) | [↗](https://github.com/onnx/onnx) | High | OSS | ai-dev, ml-ops | Open standard and runtime for interchangeable ML models; broad framework support (PyTorch, TensorFlow, etc.). Enables portable deployment across runtimes and hardware. | 2025 |
| [OpenAI GPT-4o (Vision)](https://platform.openai.com/docs/guides/images-vision?api-mode=responses) | [↗](https://platform.openai.com/docs/guides/images-vision?api-mode=responses) | High | Series D+ | ai-dev, enterprise-ai | Multimodal model with vision and language; image understanding and generation via API. Leading capability for vision-language tasks in applications and agents. | 2025 |
| [OpenCV](https://github.com/opencv/opencv) | [↗](https://github.com/opencv/opencv) | High | OSS | ai-dev | Open-source computer vision library; classic CV, DNN module, and real-time pipelines. Industry standard for prototyping and production CV; C++, Python, broad adoption. | 2025 |
| [Rerun](https://www.rerun.io/) | [↗](https://www.rerun.io/) | Medium | TBD | ai-dev, observability | Open-source SDK for logging and visualizing multimodal data (images, 3D, point clouds); used in robotics and CV debugging. Venture-backed; stage TBD. | 2025 |
| [Roboflow](https://roboflow.com/) | [↗](https://roboflow.com/) | High | TBD | ml-ops, unstructured-etl, ai-dev | Platform for building and deploying computer vision models; data labeling, training, and deployment (edge and cloud). Popular with developers and teams; stage TBD. | 2025 |
| [YOLOv8](https://yolov8.com/) | [↗](https://yolov8.com/) | High | OSS | ai-dev | Ultralytics’ YOLOv8; open-source object detection and segmentation. Widely used for real-time detection; Python-first, easy training and export. | 2025 |

### Speech & Voice AI

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AssemblyAI](https://www.assemblyai.com/) | [↗](https://www.assemblyai.com/) | High | TBD | ai-dev, enterprise-ai | Speech-to-text and audio intelligence API; transcription, summarization, and content moderation. Developer-focused; used in media, contact center, and product analytics. | 2025 |
| [AWS Transcribe / Polly](https://aws.amazon.com/transcribe/) | [↗](https://aws.amazon.com/transcribe/) | High | Subsidiary | ai-dev, enterprise-ai | AWS speech-to-text (Transcribe) and text-to-speech (Polly); managed, scalable APIs. Integrated with rest of AWS for voice applications and analytics. | 2025 |
| [Cartesia](https://cartesia.ai/) | [↗](https://cartesia.ai/) | Medium | TBD | ai-dev | Voice synthesis API for low-latency, expressive TTS; used in conversational AI and content. Venture-backed; stage TBD. | 2025 |
| [DeepGram](https://deepgram.com/) | [↗](https://deepgram.com/) | High | TBD | ai-dev, enterprise-ai | Speech-to-text and understanding API; fast transcription and features like diarization and summarization. Strong adoption in contact center, media, and voice AI. | 2025 |
| [Eleven Labs](https://beta.elevenlabs.io/) | [↗](https://beta.elevenlabs.io/) | High | TBD | ai-dev | Voice synthesis platform; realistic TTS, cloning, and dubbing. Widely used for content and conversational AI; high-profile brand and usage. | 2025 |
| [Fixie Ultravox](https://fixie.ai/) | [↗](https://fixie.ai/) | Medium | TBD | ai-dev, agents | Fixie’s voice AI and agent platform; real-time voice interfaces. Part of Fixie’s agent stack; stage TBD. | 2025 |
| [Gladia](https://www.gladia.io/) | [↗](https://www.gladia.io/) | High | Series A | ai-dev | French speech-to-text API; real-time and batch, 100+ languages, built on optimized Whisper. $16M Series A (2024); 600+ companies; competes with AssemblyAI and Deepgram. | 2025 |
| [Google Cloud Speech AI (STT/TTS)](https://cloud.google.com/speech-to-text?hl=en) | [↗](https://cloud.google.com/speech-to-text?hl=en) | High | Subsidiary | ai-dev, enterprise-ai | Google Cloud speech-to-text and text-to-speech; multiple models and languages. Integrated with Vertex AI and other GCP services for enterprise voice apps. | 2025 |
| [Gradium](https://gradium.ai/) | [↗](https://gradium.ai/) | Medium | TBD | ai-dev | Voice or speech AI product; exact focus and funding not confirmed. Tagged ai-dev; stage and relevance TBD until verified. | 2025 |
| [Hume AI](https://hume.ai/) | [↗](https://hume.ai/) | Medium | TBD | ai-dev | Emotional expression and voice AI (e.g. EVI); measures and generates emotional tone. Applied in customer experience and conversational AI; venture-backed. | 2025 |
| [LiveKit](https://livekit.io/) | [↗](https://livekit.io/) | High | TBD | ai-dev, streaming, compute | Open-source real-time communication platform; WebRTC, server-side SDKs, and integrations for voice/video and AI. Used for live voice agents and multi-party apps. | 2025 |
| [Microsoft Azure AI Speech](https://azure.microsoft.com/en-us/products/ai-services/ai-speech) | [↗](https://azure.microsoft.com/en-us/products/ai-services/ai-speech) | High | Subsidiary | ai-dev, enterprise-ai | Enterprise speech APIs for STT, TTS, and speaker recognition; part of Azure AI Services and widely used in data pipelines and voice apps. | 2025 |
| [Nvidia Riva](https://www.nvidia.com/en-us/ai-data-science/products/riva/) | [↗](https://www.nvidia.com/en-us/ai-data-science/products/riva/) | High | Subsidiary | ai-dev, ml-ops | GPU-accelerated speech AI SDK and services for custom ASR and TTS; deploy on-prem or cloud for voice pipelines. | 2025 |
| [OpenAI Realtime API](https://platform.openai.com/docs/api-reference/realtime) | [↗](https://platform.openai.com/docs/api-reference/realtime) | High | TBD | ai-dev, agents | Low-latency voice conversation API for building voice agents and assistants; key infrastructure for real-time voice AI. | 2025 |
| [OpenAI Whisper](https://platform.openai.com/docs/models) | [↗](https://platform.openai.com/docs/models) | High | TBD | ai-dev, data-sources | Speech-to-text model and API widely used for transcription in data pipelines and content indexing. | 2025 |
| [Resemble.ai](https://www.resemble.ai/) | [↗](https://www.resemble.ai/) | Medium | TBD | ai-dev | Voice cloning and synthetic voice generation for content and applications; less central to data platform pipelines. | 2025 |
| [Retell AI](https://www.retellai.com/) | [↗](https://www.retellai.com/) | High | TBD | ai-dev, agents | Conversational voice AI platform for building phone and voice agents; infrastructure for voice-first applications. | 2025 |
| [Sesame](https://www.sesame.com/) | [↗](https://www.sesame.com/) | Medium | TBD | ai-dev | Interview and assessment platform with voice/communication focus; application-layer rather than core data infrastructure. | 2025 |
| [SpeechMatics](https://www.speechmatics.com/) | [↗](https://www.speechmatics.com/) | High | TBD | ai-dev, unstructured-etl | Speechmatics: speech-to-text and language data APIs for transcription and analytics in pipelines. | 2025 |
| [Vapi](https://vapi.ai/) | [↗](https://vapi.ai/) | High | TBD | ai-dev, agents | Platform for building and deploying voice AI agents for calls and assistants; developer-focused voice infrastructure. | 2025 |
| [Voicemod](https://www.voicemod.net/) | [↗](https://www.voicemod.net/) | Low | TBD | ai-dev | Real-time voice changer and effects for streaming and gaming; consumer entertainment rather than data or enterprise pipelines. | 2025 |
| [Wellsaid](https://wellsaidlabs.com/) | [↗](https://wellsaidlabs.com/) | Medium | TBD | ai-dev | Text-to-speech and voice cloning for enterprise and content; TTS output rather than data-ingestion infrastructure. | 2025 |

## Machine Learning & Artificial Intelligence — Operate & Supply

### Data Generation & Labelling

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Aindo](https://www.aindo.com/) | [↗](https://www.aindo.com/) | Medium | TBD | ml-ops, unstructured-etl | Synthetic data generation for ML training and privacy-safe analytics; supports data pipeline and model readiness. | 2025 |
| [Cleanlab](https://cleanlab.ai/) | [↗](https://cleanlab.ai/) | High | Series B | quality, ml-ops | Confident learning and label error detection for ML; data-centric AI tooling for training data quality. | 2025 |
| [Coactive](https://www.coactive.ai/) | [↗](https://www.coactive.ai/) | High | TBD | ml-ops, ai-dev | Computer vision data platform for labeling, search, and model training; supports visual data pipelines. | 2025 |
| [Gretel](https://gretel.ai/) | [↗](https://gretel.ai/) | High | Series B | unstructured-etl, security-privacy | Synthetic data and privacy APIs for generation and de-identification; used in data pipelines and ML workflows. | 2025 |
| [Hazy](https://hazy.com/) | [↗](https://hazy.com/) | Medium | TBD | ml-ops, security-privacy | Synthetic data for testing and analytics with privacy preservation; supports safe data sharing and dev/test. | 2025 |
| [Hive](https://thehive.ai/) | [↗](https://thehive.ai/) | High | TBD | ml-ops, ai-dev | Data labeling and model APIs for image, video, and text; training data and model-in-the-loop workflows. | 2025 |
| [HumanSignal](https://humansignal.com/) | [↗](https://humansignal.com/) | High | TBD | ml-ops, ai-dev | Label Studio open-source and commercial tools for data labeling; widely used in ML pipelines. | 2025 |
| [Kili](https://kili-technology.com/) | [↗](https://kili-technology.com/) | High | TBD | ml-ops, ai-dev | Training data platform for ML with labeling, QA, and automation; supports computer vision and NLP. | 2025 |
| [Labelbox](https://labelbox.com/) | [↗](https://labelbox.com/) | High | Series D+ | ml-ops, ai-dev | Leading training data platform for computer vision and NLP; model-assisted labeling and data management. | 2025 |
| [MostlyAI](https://mostly.ai/) | [↗](https://mostly.ai/) | High | Series B | ml-ops, security-privacy | Synthetic data generation for analytics and ML; privacy-safe data for modeling and testing. | 2025 |
| [Refuel](https://www.refuel.ai/) | [↗](https://www.refuel.ai/) | High | TBD | ai-dev, ml-ops | Data labeling and evaluation for LLMs; supports AI training data and evaluation pipelines. | 2025 |
| [Sama](https://www.sama.com/) | [↗](https://www.sama.com/) | High | TBD | ml-ops | Training data and annotation with impact sourcing; enterprise labeling for computer vision and content. | 2025 |
| [Scale](https://scale.com/) | [↗](https://scale.com/) | High | Series D+ | ml-ops, ai-dev | Major AI data and model evaluation provider; government, AV, and enterprise training data and RLHF. | 2025 |
| [super.ai](https://super.ai/) | [↗](https://super.ai/) | Medium | TBD | ml-ops | AI-powered data labeling and workflow automation; supports training data pipelines. | 2025 |
| [Surge AI](https://www.surgehq.ai/) | [↗](https://www.surgehq.ai/) | High | TBD | ml-ops, ai-dev | Specialized in LLM and AI training data; human-in-the-loop and evaluation for language models. | 2025 |
| [Synthesis AI](https://synthesis.ai/) | [↗](https://synthesis.ai/) | Medium | TBD | ml-ops, unstructured-etl | Synthetic human and face data for computer vision; supports training data generation for vision models. | 2025 |
| [Toloka](https://toloka.ai/) | [↗](https://toloka.ai/) | High | TBD | ml-ops | Crowdsourcing platform for data labeling; Yandex-backed and used in ML training pipelines. | 2025 |
| [Tonic AI](https://www.tonic.ai/) | [↗](https://www.tonic.ai/) | Medium | TBD | ml-ops, security-privacy | Synthetic and subset test data for dev/test; supports safe database copies and data masking. | 2025 |
| [V7](https://www.v7labs.com/) | [↗](https://www.v7labs.com/) | High | TBD | ml-ops, ai-dev | Automated labeling and dataset management for medical and industrial imaging; vision data pipelines. | 2025 |
| [Voxel51](https://voxel51.com/) | [↗](https://voxel51.com/) | High | TBD | ml-ops, ai-dev | FiftyOne toolkit for computer vision data curation, QA, and analysis; OSS and commercial. | 2025 |

### Data Science

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Amazon SageMaker Studio](https://aws.amazon.com/pm/sagemaker/) | [↗](https://aws.amazon.com/pm/sagemaker/) | High | Subsidiary | ai-dev, ml-ops, compute | Cloud IDE and MLOps for building, training, and deploying models on AWS; core data science and ML platform. | 2025 |
| [anaconda](https://www.anaconda.com/) | [↗](https://www.anaconda.com/) | High | TBD | ai-dev, data-sources | Python distribution and package ecosystem for data science; default environment for many ML and analytics workflows. | 2025 |
| [Azure Notebooks](https://visualstudio.microsoft.com/vs/features/notebooks-at-microsoft/) | [↗](https://visualstudio.microsoft.com/vs/features/notebooks-at-microsoft/) | Medium | Subsidiary | ai-dev | Jupyter-based notebooks in Azure; increasingly folded into VS Code and Azure ML experiences. | 2025 |
| [Databricks Notebooks](https://www.databricks.com/product/collaborative-notebooks) | [↗](https://www.databricks.com/product/collaborative-notebooks) | High | Series D+ | ai-dev, ml-ops | Collaborative notebooks on the lakehouse with Delta and Unity Catalog; central to Databricks data and ML workflows. | 2025 |
| [Deepnote](https://deepnote.com/) | [↗](https://deepnote.com/) | High | Series A | ai-dev, ml-ops, compute | Cloud-native collaborative data science notebooks (Jupyter-compatible) with real-time collab, SQL and Python, and data warehouse integrations. Raised $20M Series A (2022); acquired Hyperquery (2024) to strengthen analytics workflows. | 2025 |
| [Google Cloud Vertex AI Workbench](https://cloud.google.com/vertex-ai) | [↗](https://cloud.google.com/vertex-ai) | High | Subsidiary | ai-dev, ml-ops, compute | Managed Jupyter-based notebooks and environments on GCP for data science and ML; tight integration with Vertex AI for training and deployment. Part of Google Cloud's enterprise data and AI stack. | 2025 |
| [Google Colab](https://colab.research.google.com/) | [↗](https://colab.research.google.com/) | High | Subsidiary | ai-dev, compute | Free browser-based Jupyter-style notebooks with optional GPU/TPU; widely used for research and education. No install, sharing and GitHub integration; Colab Pro for more compute and features. | 2025 |
| [IBM SPSS Modeler](https://www.ibm.com/products/spss-modeler) | [↗](https://www.ibm.com/products/spss-modeler) | Medium | Subsidiary | analytics, ml-ops, transformation | Visual data mining and predictive analytics platform with drag-and-drop modeling and automation. Legacy enterprise install base; part of IBM's analytics portfolio alongside Watson. | 2025 |
| [IBM Watsonx.AI Studio](https://www.ibm.com/cloud/watson-studio) | [↗](https://www.ibm.com/cloud/watson-studio) | High | Subsidiary | ai-dev, ml-ops, enterprise-ai | IBM's studio for building, tuning, and deploying AI and ML models; supports watsonx foundation models and open-source. Part of watsonx platform with governance and data tools. | 2025 |
| [Jupyter](https://jupyter.org/) | [↗](https://jupyter.org/) | High | OSS | ai-dev, compute | Open-source project for interactive notebooks (Jupyter Notebook, JupyterLab); de facto standard for data science and teaching. Community and nonprofit-backed; runs from laptop to cloud. | 2025 |
| [Knime](https://www.knime.com/) | [↗](https://www.knime.com/) | High | Series B | transformation, analytics, ml-ops, ai-dev | Visual, node-based platform for data workflows, analytics, and AI; open-source KNIME Analytics Platform plus commercial Business Hub. Raised $30M Series B (2024); strong in life sciences and pharma. | 2025 |
| [Mathworks MATLAB](https://www.mathworks.com/) | [↗](https://www.mathworks.com/) | High | TBD | analytics, ai-dev, compute | Numerical computing and simulation environment; widely used in engineering, control systems, and research. Private company; MATLAB and Simulink are industry standards in many verticals. | 2025 |
| [noteable](https://noteable.io/) | [↗](https://noteable.io/) | High | TBD | ai-dev, compute, integration | Collaborative Jupyter-compatible notebook platform with real-time editing, scheduling, and connectivity to Snowflake, BigQuery, Databricks, and other warehouses. Managed cloud and self-hosting options. | 2025 |
| [Posit RStudio / Workbench](https://posit.co/) | [↗](https://posit.co/) | High | TBD | ai-dev, compute | IDE and workbench for R and Python data science (RStudio, Posit Workbench); open-source core with commercial support and enterprise features. Posit is a PBC; strong in reproducible research and publishing. | 2025 |
| [RapidMiner](https://rapidminer.com/) | [↗](https://rapidminer.com/) | Medium | Subsidiary | analytics, ml-ops, transformation | Visual analytics and ML platform for data prep, modeling, and deployment; low-code and automation. Acquired by Altair (2022), now part of Siemens; Gartner Leader in advanced analytics historically. | 2025 |
| [Sas](https://www.sas.com/en_us/home.html) | [↗](https://www.sas.com/en_us/home.html) | High | TBD | analytics, ml-ops, governance | Enterprise analytics and AI platform (SAS Viya, etc.) for statistics, ML, and decisioning; long-standing in regulated industries. Private company (SAS Institute); strong governance and model ops. | 2025 |
| [SaturnCloud](https://saturncloud.io/) | [↗](https://saturncloud.io/) | Medium | TBD | ai-dev, ml-ops, compute | Managed Dask and Python data science platform in the cloud; scalable compute and collaboration for teams. Focus on parallel computing and ML at scale; less brand visibility than major cloud notebooks. | 2025 |
| [Snowflake Notebooks](https://www.snowflake.com/en/product/features/notebooks/) | [↗](https://www.snowflake.com/en/product/features/notebooks/) | High | Subsidiary | ai-dev, compute, storage-warehouse | Native notebooks inside Snowflake for SQL, Python, and ML; data stays in Snowflake with no egress. Part of Snowflake's data cloud; simplifies analytics and ML workflows on the warehouse. | 2025 |
| [Visual Studio Code](https://code.visualstudio.com/) | [↗](https://code.visualstudio.com/) | High | Subsidiary | ai-dev, compute | General-purpose IDE with Jupyter extension and Python/R support; widely used for data science and scripting. Microsoft product; free, extensible, and standard in many developer and DS workflows. | 2025 |

### Enterprise AI Platforms

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Anthropic Claude Enterprise](https://www.anthropic.com/news/claude-for-enterprise) | [↗](https://www.anthropic.com/news/claude-for-enterprise) | High | TBD | enterprise-ai, ai-dev, agents | Enterprise offering for Claude LLM with security, compliance, and scale; API and product integrations. Anthropic is private with large funding; differentiator is safety and long-context models. | 2025 |
| [AWS Bedrock](https://aws.amazon.com/bedrock/) | [↗](https://aws.amazon.com/bedrock/) | High | Subsidiary | enterprise-ai, ai-dev, agents | Managed service for foundation models (Amazon and third-party) and building agents; RAG, guardrails, and AWS integration. Core to AWS's enterprise AI strategy; broad model choice and private deployment options. | 2025 |
| [C3 AI](https://c3.ai/) | [↗](https://c3.ai/) | High | Public | enterprise-ai, ai-dev, analytics | Enterprise AI applications and platform (C3 AI Suite) for supply chain, CRM, and industry use cases; low-code and no-code. Public company (NYSE: AI); turnkey apps and C3 AI Studio for custom builds. | 2025 |
| [Cohere North](https://cohere.com/north) | [↗](https://cohere.com/north) | High | Series D+ | enterprise-ai, ai-dev, agents | Enterprise LLM platform (Command R/R+) with RAG, multilingual support, and data privacy; cloud-agnostic. Raised $500M Series D (2024), ~$5.5B valuation; focused on enterprise and sovereign deployment. | 2025 |
| [Databricks Mosaic AI](https://www.databricks.com/product/artificial-intelligence) | [↗](https://www.databricks.com/product/artificial-intelligence) | High | Subsidiary | enterprise-ai, ai-dev, ml-ops | AI and ML on the Databricks lakehouse: foundation models, vector search, RAG, and MLOps. Unified with data and governance; key for enterprises already on Databricks. | 2025 |
| [Dataiku](https://www.dataiku.com/) | [↗](https://www.dataiku.com/) | High | Series D+ | enterprise-ai, ml-ops, ai-dev | Data and AI platform for prep, ML, and GenAI; collaborative projects and governance. Valued at $4.6B+ (Series E 2021); strong in 'Everyday AI' and governed self-service. | 2025 |
| [DataRobot](https://www.datarobot.com/) | [↗](https://www.datarobot.com/) | High | Series D+ | enterprise-ai, ml-ops, ai-dev | Automated ML and MLOps platform for building, deploying, and managing models; GenAI and time series. Large private company (~$1B+ raised); broad enterprise adoption and platform breadth. | 2025 |
| [Google Cloud Vertex AI](https://cloud.google.com/vertex-ai) | [↗](https://cloud.google.com/vertex-ai) | High | Subsidiary | enterprise-ai, ai-dev, ml-ops | Unified ML and GenAI on GCP: training, tuning, deployment, and foundation models (Gemini and others). Integrated with BigQuery and GCP data; enterprise controls and compliance. | 2025 |
| [H2O.ai](https://h2o.ai/) | [↗](https://h2o.ai/) | High | Series D+ | enterprise-ai, ml-ops, ai-dev | Open-source and commercial ML/AI platform (H2O, Driverless AI, LLM Studio) for automated ML and GenAI. ~$246M raised; strong in financial services and document AI. | 2025 |
| [IBM Watson](https://www.ibm.com/watson) | [↗](https://www.ibm.com/watson) | High | Subsidiary | enterprise-ai, ai-dev | IBM's AI portfolio: watsonx (models, studio, governance), Watson Assistant, and industry solutions. Long-standing enterprise AI brand; emphasis on trust and hybrid deployment. | 2025 |
| [Microsoft Azure AI Studio](https://azure.microsoft.com/en-us/blog/product/azure-ai-studio/) | [↗](https://azure.microsoft.com/en-us/blog/product/azure-ai-studio/) | High | Subsidiary | enterprise-ai, ai-dev, agents | Studio for building GenAI apps and agents on Azure; models (including OpenAI), RAG, and Copilot integration. Central to Microsoft's enterprise AI and data estate strategy. | 2025 |
| [Nvidia AI Enterprise](https://www.nvidia.com/en-us/data-center/products/ai-enterprise/) | [↗](https://www.nvidia.com/en-us/data-center/products/ai-enterprise/) | High | Subsidiary | enterprise-ai, ml-ops, compute | Software suite for enterprise AI: frameworks, MLOps, and support for training and inference on Nvidia GPUs. Enables governed, supported AI deployment on-prem and in cloud. | 2025 |
| [OpenAI ChatGPT Enterprise](https://openai.com/index/introducing-chatgpt-enterprise/) | [↗](https://openai.com/index/introducing-chatgpt-enterprise/) | High | TBD | enterprise-ai, ai-dev, agents | Enterprise ChatGPT with security, admin controls, and no training on customer data. OpenAI is private; dominant in GenAI adoption and API ecosystem. | 2025 |
| [Oracle OCI Generative AI](https://www.oracle.com/artificial-intelligence/generative-ai/generative-ai-service/) | [↗](https://www.oracle.com/artificial-intelligence/generative-ai/generative-ai-service/) | High | Subsidiary | enterprise-ai, ai-dev | Managed GenAI service on OCI with Cohere and Meta models; RAG and integration with Oracle DB and apps. Part of Oracle Cloud's AI strategy for existing Oracle customers. | 2025 |
| [Palantir Technologies](https://www.palantir.com/) | [↗](https://www.palantir.com/) | High | Public | enterprise-ai, ai-dev, analytics | Platforms (Foundry, AIP) for integrating data and deploying AI in government and enterprise. Public company; differentiator is large-scale, sensitive-data use cases and AIP for decisioning. | 2025 |
| [Salesforce AI Cloud](https://www.salesforce.com/artificial-intelligence/) | [↗](https://www.salesforce.com/artificial-intelligence/) | High | Subsidiary | enterprise-ai, ai-dev, agents | GenAI and CRM integration: Einstein Copilot, Data Cloud, and industry clouds. Ties AI to Salesforce data and workflows; strong in sales and marketing use cases. | 2025 |
| [SAP Joule / AI Core](https://www.sap.com/products/artificial-intelligence/ai-assistant.html) | [↗](https://www.sap.com/products/artificial-intelligence/ai-assistant.html) | High | Subsidiary | enterprise-ai, ai-dev | SAP's AI assistant (Joule) and AI Core for embedding AI across SAP apps and data. Integrated with S/4HANA and Business Technology Platform; ERP-centric enterprise AI. | 2025 |
| [Servicenow Now Assist Platform](https://www.servicenow.com/platform/now-assist.html) | [↗](https://www.servicenow.com/platform/now-assist.html) | High | Subsidiary | enterprise-ai, agents | GenAI and automation (Now Assist) for IT, HR, and customer workflows on the ServiceNow platform. Public company; AI embedded in ITSM and enterprise workflows. | 2025 |
| [Snowflake Cortex AI](https://www.snowflake.com/en/product/features/cortex/) | [↗](https://www.snowflake.com/en/product/features/cortex/) | High | Subsidiary | enterprise-ai, ai-dev, storage-warehouse | LLM and ML services (Cortex) inside Snowflake for SQL-based AI, document AI, and agents. Data stays in Snowflake; simplifies secure, governed AI on the data cloud. | 2025 |

### MLOps

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Amazon SageMaker](https://aws.amazon.com/sagemaker/) | [↗](https://aws.amazon.com/sagemaker/) | High | Subsidiary | ml-ops, ai-dev, compute | Managed ML platform on AWS for building, training, and deploying models; broad feature set and integrations. Core to AWS's ML strategy; scales from experimentation to production. | 2025 |
| [Azure Machine Learning](https://azure.microsoft.com/en-us/products/machine-learning/#product-overview) | [↗](https://azure.microsoft.com/en-us/products/machine-learning/#product-overview) | High | Subsidiary | ml-ops, ai-dev, compute | Microsoft's managed ML platform for training, deployment, and MLOps; integrates with Azure data services and open frameworks. Key part of Microsoft's enterprise AI stack. | 2025 |
| [BentoML](https://www.bentoml.com/) | [↗](https://www.bentoml.com/) | High | Series B | ml-ops | Open-source model serving framework; package models as standardized containers and deploy to any cloud or on-prem. Strong developer experience and multi-framework support. | 2025 |
| [ClearML](https://clear.ml/) | [↗](https://clear.ml/) | High | OSS | ml-ops, observability, orchestration | Open-source MLOps platform for experiment tracking, orchestration, and model deployment; commercial tier from Allegro. Unified pipeline and dataset versioning. | 2025 |
| [Databricks Mosaic AI](https://www.mosaicml.com/) | [↗](https://www.mosaicml.com/) | High | Subsidiary | ml-ops, ai-dev, compute | End-to-end ML training and inference platform; acquired by Databricks (2023) and integrated as Mosaic AI. Known for efficient training and open model recipes. | 2025 |
| [Domino](https://www.dominodatalab.com/) | [↗](https://www.dominodatalab.com/) | High | Series D+ | ml-ops, ai-dev, enterprise-ai | Enterprise ML platform for model development, deployment, and governance; strong in regulated and life sciences. Late-stage private company with large funding rounds. | 2025 |
| [Feast](https://feast.dev/) | [↗](https://feast.dev/) | High | OSS | ml-ops, data-sources | Open-source feature store for ML; offline and online feature storage and serving with a unified API. Widely adopted; Tecton and others contribute. | 2025 |
| [Featurebyte](https://featurebyte.com/) | [↗](https://featurebyte.com/) | High | Series B | ml-ops, data-sources, transformation | Feature store and feature engineering platform with declarative feature definitions and automatic backfills. Raised significant Series B; enterprise focus. | 2025 |
| [Flyte](https://github.com/flyteorg/flyte) | [↗](https://github.com/flyteorg/flyte) | High | OSS | ml-ops, orchestration | Open-source workflow orchestration for ML and data; type-safe, scalable, and cloud-native. Originated at Lyft; Linux Foundation project. | 2025 |
| [Google Cloud Vertex AI](https://cloud.google.com/vertex-ai) | [↗](https://cloud.google.com/vertex-ai) | High | Subsidiary | ml-ops, ai-dev, compute | GCP's managed ML platform for training, deployment, AutoML, and MLOps; integrates with BigQuery and Google's AI services. Full lifecycle and governance. | 2025 |
| [Hopsworks](https://www.hopsworks.ai/) | [↗](https://www.hopsworks.ai/) | High | Series B | ml-ops, storage-lakehouse, data-sources | Feature store and ML platform built on a data lakehouse; open-source and managed cloud. Differentiator: unified feature store and training data with Python-centric UX. | 2025 |
| [KServe](https://github.com/kserve/kserve) | [↗](https://github.com/kserve/kserve) | High | OSS | ml-ops | Standardized model serving on Kubernetes; supports multiple frameworks and autoscaling. Evolved from KFServing; part of the Kubeflow ecosystem. | 2025 |
| [KubeFlow](https://github.com/kubeflow/kubeflow) | [↗](https://github.com/kubeflow/kubeflow) | High | OSS | ml-ops, orchestration, compute | Kubernetes-native ML platform; pipelines, training operators, and serving (KServe). Widely used in hybrid and on-prem ML workloads. | 2025 |
| [Metaflow](https://github.com/Netflix/metaflow) | [↗](https://github.com/Netflix/metaflow) | High | OSS | ml-ops, orchestration | Framework for ML pipelines and workflows with a human-centric design; open-sourced by Netflix. Now maintained by Outerbounds with commercial support. | 2025 |
| [MLFlow](https://github.com/mlflow/mlflow) | [↗](https://github.com/mlflow/mlflow) | High | OSS | ml-ops | Open-source platform for ML lifecycle: tracking, projects, models, and registry. De facto standard for experiment tracking; stewarded by Databricks. | 2025 |
| [Ray Serve](https://docs.ray.io/en/latest/serve/index.html) | [↗](https://docs.ray.io/en/latest/serve/index.html) | High | OSS | ml-ops, compute | Scalable model serving on Ray; Python-native with autoscaling and batching. Part of the Ray ecosystem from Anyscale; supports many frameworks. | 2025 |
| [Seldon](https://www.seldon.io/) | [↗](https://www.seldon.io/) | High | Series B | ml-ops, observability | Enterprise ML deployment and monitoring on Kubernetes; explainability and drift detection. UK-based; strong in governance and production ML. | 2025 |
| [Tecton](https://www.tecton.ai/) | [↗](https://www.tecton.ai/) | High | Series C | ml-ops, data-sources, transformation | Enterprise feature platform with offline and online store, transformations, and real-time serving. Creators of Feast; raised large Series C; used by major tech companies. | 2025 |
| [Valohai](https://valohai.com/) | [↗](https://valohai.com/) | Medium | Series A | ml-ops, orchestration | ML training orchestration and experiment tracking; supports cloud and on-prem. Finnish company; focused on reproducibility and pipeline automation. | 2025 |
| [Weights & Biases](https://wandb.ai/site) | [↗](https://wandb.ai/site) | High | Series C | ml-ops, observability | Experiment tracking, model registry, and MLOps; widely adopted in research and industry. Strong visualization and collaboration; integrates with major frameworks. | 2025 |
| [ZenML](https://zenml.io/home) | [↗](https://zenml.io/home) | High | Seed | ml-ops, orchestration | Open-source MLOps framework for pipeline orchestration with integrations to feature stores, orchestrators, and deployers. Pipeline-as-code with stack abstraction. | 2025 |

## Machine Learning & Artificial Intelligence — Run & Deploy

### AI Hardware

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AMD MI300X / MI325X](https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html) | [↗](https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html) | High | Public | compute | AMD Instinct GPUs for AI training and inference; competitive alternative to NVIDIA in data centers. MI300X is widely deployed for LLM inference. | 2025 |
| [AMD MI350](https://www.amd.com/en/products/accelerators/instinct/mi350.html) | [↗](https://www.amd.com/en/products/accelerators/instinct/mi350.html) | High | Public | compute | Next-generation AMD Instinct accelerator for AI; successor roadmap to MI300 series for training and inference. | 2025 |
| [AWS Inferentia 2](https://aws.amazon.com/ai/machine-learning/inferentia/) | [↗](https://aws.amazon.com/ai/machine-learning/inferentia/) | High | Subsidiary | compute | AWS custom chip for high-throughput, cost-effective inference; used in SageMaker and EC2. Second-generation Inferentia; strong for LLM inference. | 2025 |
| [AWS Trainium 2](https://aws.amazon.com/ai/machine-learning/trainium/) | [↗](https://aws.amazon.com/ai/machine-learning/trainium/) | High | Subsidiary | compute | AWS custom chip for ML training; second-generation Trainium for high performance and efficiency. Used in SageMaker and EC2 Trn instances. | 2025 |
| [Cerebras WSE-3](https://www.cerebras.net/) | [↗](https://www.cerebras.net/) | High | Series D+ | compute | Wafer-scale engine for AI training; largest single chip. WSE-3 delivers very high memory bandwidth and compute; used in supercomputing and LLM training. | 2025 |
| [d-Matrix](https://www.d-matrix.ai/) | [↗](https://www.d-matrix.ai/) | High | Series C | compute | Inference-focused chips with in-memory compute for energy efficiency. Targeting data center inference for LLMs and large models. | 2025 |
| [Etched](https://www.etched.ai/) | [↗](https://www.etched.ai/) | Medium | Series A | compute | Startup building custom AI inference chips; focused on dedicated transformer inference. Early stage; raised notable funding for specialized silicon. | 2025 |
| [Google TPU V5e (Inference)](https://docs.cloud.google.com/tpu/docs/v5p) | [↗](https://docs.cloud.google.com/tpu/docs/v5p) | High | Subsidiary | compute | Google's TPU v5e for inference workloads on GCP; cost-efficient and scalable. Part of Google Cloud's AI infrastructure. | 2025 |
| [Google TPU V5p](https://docs.cloud.google.com/tpu/docs/v5p) | [↗](https://docs.cloud.google.com/tpu/docs/v5p) | High | Subsidiary | compute | Google's highest-performance TPU for training and inference; available on GCP. Used for large-scale model training and demanding inference. | 2025 |
| [Graphcore](https://www.graphcore.ai/) | [↗](https://www.graphcore.ai/) | Medium | Series D+ | compute | IPU (Intelligence Processing Unit) for AI training and inference; UK-based. Faced restructuring and layoffs; alternative architecture to GPUs. | 2025 |
| [Groq LPU](https://groq.com/) | [↗](https://groq.com/) | High | Series C | compute | Language Processing Unit for very fast LLM inference with deterministic latency. Differentiator: high tokens-per-second for inference; used in cloud and on-prem. | 2025 |
| [Intel Falcon Shores](https://mad.firstmark.com/) | [↗](https://mad.firstmark.com/) | High | Public | compute | Intel's next-generation AI accelerator (GPU + other); roadmap product for data center AI. Part of Intel's push into AI silicon. | 2025 |
| [Intel Gaudi 3](https://www.intel.com/content/www/us/en/products/details/processors/ai-accelerators/gaudi.html) | [↗](https://www.intel.com/content/www/us/en/products/details/processors/ai-accelerators/gaudi.html) | High | Public | compute | Intel's Gaudi 3 AI accelerator for training and inference; competitive alternative to NVIDIA. Available in OEM systems and cloud. | 2025 |
| [Meta MTIA V2](https://ai.meta.com/blog/next-generation-meta-training-inference-accelerator-AI-MTIA/) | [↗](https://ai.meta.com/blog/next-generation-meta-training-inference-accelerator-AI-MTIA/) | High | Subsidiary | compute | Meta's in-house inference accelerator for recommendation and ranking workloads. Second generation; not sold externally but material to Meta's AI infrastructure. | 2025 |
| [Microsoft Maia 100/200](https://azure.microsoft.com/en-us/blog/azure-maia-for-the-era-of-ai-from-silicon-to-software-to-systems/) | [↗](https://azure.microsoft.com/en-us/blog/azure-maia-for-the-era-of-ai-from-silicon-to-software-to-systems/) | High | Subsidiary | compute | Azure's first-party AI accelerators (Maia) for training and inference in Azure data centers. Part of Microsoft's vertical integration for AI infrastructure. | 2025 |
| [NVIDIA Blackwell (B100/B200)](https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/) | [↗](https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/) | High | Public | compute, ml-ops | NVIDIA’s latest data-center GPU architecture for training and inference; industry standard for large-scale AI. Dominant share in AI accelerators; B100/B200 power major clouds and sovereign AI. | 2025 |
| [NVIDIA Grace Blackwell Tie-Ins](https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/) | [↗](https://www.nvidia.com/en-us/data-center/technologies/blackwell-architecture/) | High | Public | compute, ml-ops | CPU–GPU coherent systems combining Grace CPUs with Blackwell GPUs for high-throughput AI and HPC. Key for integrated supercomputing and AI training clusters. | 2025 |
| [NVIDIA H200 (Hopper)](https://www.nvidia.com/en-us/data-center/technologies/hopper-architecture/) | [↗](https://www.nvidia.com/en-us/data-center/technologies/hopper-architecture/) | High | Public | compute, ml-ops | Current-generation data-center GPU with large memory and FP8; widely deployed for training and inference. Predecessor to Blackwell; still dominant in many clouds. | 2025 |
| [SambaNova SN40L](https://sambanova.ai/products/sn40l-rdu-ai-chip) | [↗](https://sambanova.ai/products/sn40l-rdu-ai-chip) | Medium | Series D+ | compute, ml-ops | SambaNova’s RDU-based AI accelerator and full-stack platform for training and inference; alternative to NVIDIA in enterprise and sovereign deployments. Backed by SoftBank and Intel; SN50 and systems shipping. | 2025 |
| [Tenstorrent](https://tenstorrent.com/) | [↗](https://tenstorrent.com/) | Medium | Series D+ | compute, ml-ops | AI chip and IP company (Jim Keller); raised $693M Series D (Dec 2024). Focus on scalable AI silicon and open-source software; design wins in automotive and data center. | 2025 |

### Edge AI

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AMD Ryzen AI](https://www.amd.com/en/products/processors/consumer/ryzen-ai.html) | [↗](https://www.amd.com/en/products/processors/consumer/ryzen-ai.html) | Medium | Subsidiary | compute, ai-dev | AMD’s NPU and Ryzen AI stack for PCs and laptops; enables on-device AI and Windows Copilot. Competing with Intel NPU and Qualcomm for the AI PC segment. | 2025 |
| [Apple Neural Engine](https://machinelearning.apple.com/research/neural-engine-transformers) | [↗](https://machinelearning.apple.com/research/neural-engine-transformers) | High | Subsidiary | compute, ai-dev | Apple’s on-device inference silicon and Core ML stack; powers iPhone, iPad, and Mac ML features. Strong ecosystem for privacy-preserving and low-latency edge AI. | 2025 |
| [Armada](https://www.armada.ai/) | [↗](https://www.armada.ai/) | Low | TBD | compute, observability | Edge platform (Atlas, Galleon, Bridge) for ruggedized edge compute and GPU management in remote environments. Targets oil & gas, defense, mining; partners include Azure and VAST. | 2025 |
| [Axelera AI](https://www.axelera.ai/) | [↗](https://www.axelera.ai/) | Medium | Series B | compute, ml-ops | Edge AI chip (Metis AIPU) for vision and inference; $68M Series B (Jun 2024). European fabless vendor targeting automotive, retail, and industrial; efficiency-focused edge inference. | 2025 |
| [Deeplite](https://www.deeplite.ai/) | [↗](https://www.deeplite.ai/) | Medium | Seed | ai-dev, ml-ops | TinyML optimization and compression (e.g. DeepliteRT) for edge deployment on low-power Arm; $6M seed. Used in cameras, drones, sensors; tinyML Foundation partner. | 2025 |
| [Edge Impulse](https://www.edgeimpulse.com/) | [↗](https://www.edgeimpulse.com/) | High | Subsidiary | ai-dev, ml-ops | Developer platform for building and deploying edge ML (sensors, audio, vision); acquired by Qualcomm (Mar 2025). De facto tooling for embedded and TinyML pipelines. | 2025 |
| [Google Coral (Edge TPU)](https://docs.cloud.google.com/tpu/docs/v5p) | [↗](https://docs.cloud.google.com/tpu/docs/v5p) | Medium | Subsidiary | compute, ml-ops | Google’s Edge TPU and Coral dev boards for on-device inference; docs now reference Cloud TPU v5p. Used in IoT and edge vision; ecosystem around TensorFlow Lite. | 2025 |
| [Hailo](https://hailo.ai/) | [↗](https://hailo.ai/) | High | Series C | compute, ml-ops | Edge AI processors (e.g. Hailo-10) for vision and generative AI at the edge; $120M Series C (Apr 2024), ~$1.2B valuation. Strong in smart city, retail, industrial; 300+ customers. | 2025 |
| [Intel NPU (Lunar Lake)](https://www.intel.com/content/www/us/en/support/articles/000099574/processors/intel-core-ultra-processors.html) | [↗](https://www.intel.com/content/www/us/en/support/articles/000099574/processors/intel-core-ultra-processors.html) | Medium | Subsidiary | compute, ai-dev | Intel’s NPU in Core Ultra (Lunar Lake) for AI PC workloads and Windows Copilot. Part of Intel’s AI PC push alongside AMD and Qualcomm. | 2025 |
| [Mythic](https://mythic.ai/) | [↗](https://mythic.ai/) | Medium | Series C | compute, ml-ops | Analog in-memory compute (APU) for low-power edge and data-center inference; $125M round (Dec 2025). Targets 100x energy efficiency vs GPUs; automotive and defense focus. | 2025 |
| [Nota AI](https://www.nota.ai/) | [↗](https://www.nota.ai/) | Medium | Series C | ai-dev, ml-ops | On-device AI optimization (NetsPresso) and model compression; $19.9M Series C (2024). Korean company with NVIDIA, ARM, Intel partnerships; targeting IPO. | 2025 |
| [NVIDIA Jetson Orin/Thor](https://www.nvidia.com/en-us/) | [↗](https://www.nvidia.com/en-us/) | High | Subsidiary | compute, ml-ops, ai-dev | NVIDIA’s embedded SoC platform (Orin, Thor) for robotics, autonomous systems, and edge AI. Dominant in robotics and autonomous vehicles; full CUDA and JetPack stack. | 2025 |
| [ONNX Runtime](https://github.com/onnx/onnx) | [↗](https://github.com/onnx/onnx) | High | OSS | ml-ops, ai-dev | Cross-platform inference runtime for ONNX models; Microsoft-led OSS. Default choice for deploying trained models across cloud and edge with broad hardware support. | 2025 |
| [OpenVINO](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) | [↗](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) | High | Subsidiary | ml-ops, ai-dev | Intel’s toolkit for optimizing and deploying models on Intel CPU, GPU, NPU, and VPU. Key for Intel edge and data-center inference; ONNX and Open Model Zoo support. | 2025 |
| [Qeexo](https://qeexo.com/) | [↗](https://qeexo.com/) | Medium | Subsidiary | ai-dev, ml-ops | AutoML and TinyML platform for sensors and edge devices; acquired by TDK (Jan 2023). Focus on touch, gesture, and sensor ML with low power and small footprint. | 2025 |
| [Qualcomm Snapdragon](https://www.qualcomm.com/snapdragon/overview) | [↗](https://www.qualcomm.com/snapdragon/overview) | High | Subsidiary | compute, ai-dev | Qualcomm’s mobile and IoT SoCs with NPU and AI stack; powers Android AI and AI PC (Snapdragon X). Leading mobile-edge AI; acquired Edge Impulse to strengthen dev tools. | 2025 |
| [Samsung Exynos](https://semiconductor.samsung.com/processor/) | [↗](https://semiconductor.samsung.com/processor/) | Medium | Subsidiary | compute, ai-dev | Samsung’s mobile and IoT processors with NPU for on-device AI. Used in Galaxy devices and IoT; part of Samsung’s edge and automotive roadmap. | 2025 |
| [SiMa.ai](https://sima.ai/) | [↗](https://sima.ai/) | High | Series D+ | compute, ml-ops | MLSoC (e.g. Modalix) for edge vision and generative AI; $70M (2024) and $85M (2025), total ~$355M. Targets robotics, automotive, industrial; unified software stack from vision to multimodal GenAI. | 2025 |
| [TensorFlow Lite](https://github.com/google-ai-edge/LiteRT) | [↗](https://github.com/google-ai-edge/LiteRT) | High | OSS | ml-ops, ai-dev | Google’s lightweight runtime and toolchain for on-device inference; evolved with LiteRT. Standard for mobile and embedded deployment; works with Coral and Android. | 2025 |

### GPU Cloud / Deployment Infra

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Anyscale](https://www.anyscale.com/) | [↗](https://www.anyscale.com/) | High | Series C | compute, ml-ops, ai-dev | Managed Ray platform for scaling AI and data workloads; $100M Series C (2021), ~$260M total. De facto for distributed training and serving beyond single-node; strong in LLM and RL. | 2025 |
| [AWS P5/P5e (H100/H200)](https://aws.amazon.com/ec2/instance-types/p5/) | [↗](https://aws.amazon.com/ec2/instance-types/p5/) | High | Subsidiary | compute, ml-ops | AWS EC2 instances with NVIDIA H100/H200 for training and inference; P5e for cost-optimized. Primary GPU cloud option for AWS-native customers and large-scale training. | 2025 |
| [Baseten](https://www.baseten.co/) | [↗](https://www.baseten.co/) | High | Series B | compute, ml-ops, ai-dev | Platform for deploying and running ML models in production with autoscaling and optimization; $40M Series B (Mar 2024). Used by Descript, Writer, Patreon; simplifies inference ops. | 2025 |
| [Beam](https://www.beam.cloud/) | [↗](https://www.beam.cloud/) | Medium | Seed | compute, ml-ops | Serverless GPU infrastructure for inference, training, and sandboxes; ~$3.6M seed (YC, Tiger). Fast boot and autoscaling; A10G, T4, A100 options for developers. | 2025 |
| [CoreWeave](https://www.coreweave.com/) | [↗](https://www.coreweave.com/) | High | Series C | compute, ml-ops | GPU cloud built on NVIDIA (H100, etc.) for AI training and inference; $23B valuation (Nov 2024), $7.5B debt (2024). Key alternative to hyperscalers; preferred by many AI labs and enterprises. | 2025 |
| [Crusoe](https://www.crusoe.ai/) | [↗](https://www.crusoe.ai/) | High | Series D+ | compute, ml-ops | Clean-energy-powered AI infrastructure and Crusoe Cloud for training and inference; $600M Series D (Dec 2024), $2.8B valuation. Differentiator is stranded energy and sustainability; GA Dec 2024. | 2025 |
| [DeepInfra](https://deepinfra.com/) | [↗](https://deepinfra.com/) | Medium | TBD | compute, ml-ops, ai-dev | API platform for open and proprietary LLM inference with pay-per-token pricing. Developer-focused alternative to direct cloud GPU provisioning; model zoo and simple integration. | 2025 |
| [DigitalOcean Paperspace](https://www.paperspace.com/) | [↗](https://www.paperspace.com/) | Medium | Subsidiary | compute, ml-ops | GPU VMs and ML workloads (Gradient) under DigitalOcean; acquired 2023. Targets developers and SMBs for training and inference with simpler UX than hyperscalers. | 2025 |
| [FluidStack](https://www.fluidstack.io/) | [↗](https://www.fluidstack.io/) | High | TBD | compute, ml-ops | AI cloud with large H100 clusters and bare-metal GPU; PE funding from Cacti (Oct 2024). Chosen by Anthropic for custom data centers; 10k+ H100s and EU supercomputer plans. | 2025 |
| [Google Cloud A3/A3 Mega](https://docs.cloud.google.com/compute/docs/gpus) | [↗](https://docs.cloud.google.com/compute/docs/gpus) | High | Subsidiary | compute, ml-ops | GCP VM families with NVIDIA H100 for training and inference; A3 Mega for large-scale workloads. Primary GPU option for GCP; integrated with Vertex AI and networking. | 2025 |
| [Lambda](https://lambdalabs.com/) | [↗](https://lambdalabs.com/) | High | Series C | compute, ml-ops | GPU cloud and on-prem offerings for AI training and inference; $320M Series C (Feb 2024), $1.5B+ valuation. 5,000+ customers; H100 and Quantum-2 InfiniBand; $500M GPU-backed facility (2024). | 2025 |
| [Microsoft Azure ND MI300X](https://learn.microsoft.com/en-us/azure/virtual-machines/sizes/gpu-accelerated/ndmi300xv5-series?tabs=sizebasic) | [↗](https://learn.microsoft.com/en-us/azure/virtual-machines/sizes/gpu-accelerated/ndmi300xv5-series?tabs=sizebasic) | High | Subsidiary | compute | Azure VM series powered by AMD MI300X GPUs for large-scale AI training and inference. Part of Microsoft’s cloud AI infrastructure; competes with NVIDIA-based instances. | 2025 |
| [Modal](https://modal.com/) | [↗](https://modal.com/) | High | Series B | compute, ml-ops, ai-dev | Serverless GPU and CPU platform for running ML workloads and batch jobs with minimal infra; Python-native, scale-to-zero. Strong for inference and training at startup and mid-market scale. | 2025 |
| [Nebius](https://nebius.com/) | [↗](https://nebius.com/) | Medium | Subsidiary | compute | Cloud and GPU platform spun out from Yandex; offers GPU instances and ML infra in EU. Differentiator: EU data residency and competitive pricing for training and inference. | 2025 |
| [NVIDIA DGX Cloud](https://www.nvidia.com/en-us/data-center/dgx-cloud/) | [↗](https://www.nvidia.com/en-us/data-center/dgx-cloud/) | High | Subsidiary | compute, enterprise-ai | NVIDIA’s managed AI training and inference cloud; DGX stacks with full software stack (AI Enterprise, NIM). Sold through partners (AWS, Azure, GCP, OCI) and direct; key for enterprise AI at scale. | 2025 |
| [Prime Intellect](https://www.primeintellect.ai/) | [↗](https://www.primeintellect.ai/) | Medium | Seed | compute | Decentralized GPU compute network for AI training and inference; aims to aggregate underutilized capacity. Early-stage; differentiator is decentralized ownership and pricing model. | 2025 |
| [Replicate](https://replicate.com/) | [↗](https://replicate.com/) | High | Series B | ml-ops, ai-dev, compute | API and platform to run open-source ML models (images, audio, video, LLMs) with one line of code; scale-to-zero billing. Strong developer adoption and large model catalog; Cog for packaging models. | 2025 |
| [RunPod](https://www.runpod.io/) | [↗](https://www.runpod.io/) | High | Series B | compute, ml-ops | GPU cloud and serverless inference for ML; pay-per-second, global GPU fleet, and RunPod Serverless for scale-to-zero. Popular with indie and mid-market teams for training and inference. | 2025 |
| [Scaleway](https://www.scaleway.com/en/) | [↗](https://www.scaleway.com/en/) | Medium | Subsidiary | compute | EU cloud provider (iliad group) offering GPU instances and general-purpose cloud; strong on data sovereignty and EU regions. Used for ML workloads and compliant deployments. | 2025 |
| [Vast.ai](https://vast.ai/) | [↗](https://vast.ai/) | Medium | TBD | compute, marketplace | Marketplace for renting GPU capacity from individuals and small providers; low-cost option for training and inference. Differentiator: often cheapest GPU hour; less SLA than enterprise clouds. | 2025 |
| [Voltage Park](https://www.voltagepark.com/) | [↗](https://www.voltagepark.com/) | Medium | TBD | compute | GPU cloud built on repurposed capacity (incl. ex-Tesla); aims to offer low-cost AI compute. Early commercial rollout; targets cost-sensitive training and inference workloads. | 2025 |

### Model Serving & Inference Runtimes

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [AWS Bedrock](https://aws.amazon.com/bedrock/) | [↗](https://aws.amazon.com/bedrock/) | High | Subsidiary | enterprise-ai, ai-dev | AWS managed service for foundation model access (Amazon and third-party) and custom model deployment. Central to AWS GenAI strategy; RAG, agents, and guardrails integrations. | 2025 |
| [Clarifai](https://www.clarifai.com/) | [↗](https://www.clarifai.com/) | Medium | Series D+ | ml-ops, ai-dev | Computer vision and ML platform for building, deploying, and managing models; strong in visual search and labeling. Long-standing player; enterprise and federal use cases. | 2025 |
| [DJL Serving](https://github.com/deepjavalibrary/djl-serving) | [↗](https://github.com/deepjavalibrary/djl-serving) | Medium | OSS | ml-ops | Open-source model serving from AWS Deep Java Library; supports multiple frameworks and auto-scaling. Java/JVM-native option for inference in enterprise environments. | 2025 |
| [Fireworks.ai](https://fireworks.ai/) | [↗](https://fireworks.ai/) | High | Series B | ml-ops, ai-dev | Inference API for open-source LLMs with low latency and high throughput; vLLM-based and model-optimized. Strong for production LLM apps and cost-efficient inference. | 2025 |
| [Google Cloud Vertex AI Predictions](https://cloud.google.com/vertex-ai) | [↗](https://cloud.google.com/vertex-ai) | High | Subsidiary | ml-ops, enterprise-ai | GCP’s managed service for deploying and serving custom and foundation models; supports batch and online prediction. Integrated with Vertex AI for training, tuning, and MLOps. | 2025 |
| [Groq](https://groq.com/) | [↗](https://groq.com/) | High | Series C | ml-ops, ai-dev | LPU-based inference for LLMs; very high tokens-per-second and low latency. Differentiator: speed-focused hardware and software stack; strong for real-time chat and API use cases. | 2025 |
| [Hugging Face TGI](https://github.com/huggingface/text-generation-inference) | [↗](https://github.com/huggingface/text-generation-inference) | High | OSS | ml-ops | Open-source inference server for LLMs (Tensor Parallelism, Flash Attention, continuous batching). Backbone of Hugging Face Inference Endpoints; widely used in industry and cloud offerings. | 2025 |
| [Microsoft Azure AI Inference](https://azure.microsoft.com/en-us/blog/product/azure-ai-studio/) | [↗](https://azure.microsoft.com/en-us/blog/product/azure-ai-studio/) | High | Subsidiary | ml-ops, enterprise-ai | Azure’s managed inference for foundation and custom models; integrated with Azure AI Studio and Copilot stack. Supports OpenAI and open models with enterprise SLAs and compliance. | 2025 |
| [NVIDIA FasterTransformer](https://github.com/NVIDIA/FasterTransformer) | [↗](https://github.com/NVIDIA/FasterTransformer) | High | OSS | ml-ops | NVIDIA’s inference library for Transformer models; optimized for Tensor Parallelism and low latency. Building block for Triton and NIM; key for GPU inference at scale. | 2025 |
| [NVIDIA NIM](https://developer.nvidia.com/nim) | [↗](https://developer.nvidia.com/nim) | High | Subsidiary | ml-ops, ai-dev, enterprise-ai | NVIDIA’s microservices for inference (LLMs, RAG, guardrails); run anywhere (cloud, on-prem, NGC). Part of AI Enterprise; simplifies deployment and optimization for enterprise AI. | 2025 |
| [ONNX Runtime](https://github.com/onnx/onnx) | [↗](https://github.com/onnx/onnx) | High | OSS | ml-ops | Cross-platform inference engine for ONNX models; supports many hardware backends and languages. De facto runtime for portable ML deployment; used by Microsoft and many cloud providers. | 2025 |
| [OpenVINO](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) | [↗](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html) | Medium | Subsidiary | ml-ops | Intel’s toolkit for optimizing and deploying models on CPU, GPU, and edge; ONNX and OpenVINO IR. Strong for edge and Intel-based data center inference. | 2025 |
| [SambaNova](https://sambanova.ai/) | [↗](https://sambanova.ai/) | High | Series D+ | enterprise-ai, ml-ops, compute | Full-stack AI from custom chips (SN40L) to models and APIs; training and inference for enterprises. Differentiator: integrated hardware-software stack and sovereign AI offerings. | 2025 |
| [SGLang](https://github.com/sgl-project/sglang) | [↗](https://github.com/sgl-project/sglang) | High | OSS | ml-ops | Open-source structured generation language and runtime for LLMs; frontend and backend for fast decoding and composition. Growing adoption for complex inference patterns and research. | 2025 |
| [TensorFlow](https://github.com/tensorflow/tensorflow) | [↗](https://github.com/tensorflow/tensorflow) | High | OSS | ml-ops, ai-dev | Open-source ML framework (Google); training and serving (TF Serving, TFLite). Mature ecosystem; still dominant in production ML and edge; Keras integrated. | 2025 |
| [TensorRT](https://github.com/NVIDIA/TensorRT) | [↗](https://github.com/NVIDIA/TensorRT) | High | OSS | ml-ops | NVIDIA’s inference optimizer and runtime for GPUs; quantization and kernel fusion. Key for low-latency, high-throughput deployment on NVIDIA hardware; used by Triton and many frameworks. | 2025 |
| [Together](https://together.ai/) | [↗](https://together.ai/) | High | Series C | ml-ops, ai-dev | Inference and training cloud for open-source models; fast inference API and fine-tuning. Strong open-model offering and pricing; used by many AI-native apps and enterprises. | 2025 |
| [TorchServe](https://github.com/pytorch/serve) | [↗](https://github.com/pytorch/serve) | High | OSS | ml-ops | PyTorch’s default model serving server; multi-model, batching, and metrics. Standard choice for PyTorch in production; supported by AWS and others. | 2025 |
| [Triton Inference Server](https://github.com/triton-inference-server/server) | [↗](https://github.com/triton-inference-server/server) | High | OSS | ml-ops | NVIDIA’s open-source inference server; multi-framework, dynamic batching, and multi-GPU. Industry standard for GPU inference; used in DGX, cloud, and on-prem. | 2025 |
| [vLLM](https://github.com/vllm-project/vllm) | [↗](https://github.com/vllm-project/vllm) | High | OSS | ml-ops | High-throughput LLM inference with PagedAttention and continuous batching; OSS standard for serving open LLMs. Backend for many APIs and cloud inference products. | 2025 |

## Machine Learning & Artificial Intelligence — Validate & Secure

### AI & Agent Governance

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Arthur](https://www.arthur.ai/) | [↗](https://www.arthur.ai/) | High | Series C | governance, ml-ops, quality | ML monitoring and model governance; performance, drift, bias, and explainability. Enterprise focus; differentiator for responsible AI and compliance in regulated industries. | 2025 |
| [Cranium](https://cranium.ai/) | [↗](https://cranium.ai/) | High | Series B | security-privacy, governance | AI/ML security platform; securing models and pipelines against adversarial and supply-chain risks. Differentiator: security-first governance for GenAI and agents. | 2025 |
| [Credo AI](https://www.credo.ai/) | [↗](https://www.credo.ai/) | High | Series B | governance | AI governance and risk platform; policy, risk assessment, and compliance for AI systems. Strong for financial services and regulated use cases; aligns with EU AI Act and similar frameworks. | 2025 |
| [Databricks Mosaic AI Gateway](https://www.databricks.com/product/artificial-intelligence/ai-gateway) | [↗](https://www.databricks.com/product/artificial-intelligence/ai-gateway) | High | Subsidiary | governance, enterprise-ai, ai-dev | Central gateway for model access, routing, and governance on Databricks; unified API to foundation and custom models with policy and audit. Core to Databricks AI and Unity Catalog integration. | 2025 |
| [Dataiku](https://www.dataiku.com/) | [↗](https://www.dataiku.com/) | High | Public | analytics, ml-ops, enterprise-ai, governance | Enterprise AI and analytics platform (Dataiku DSS); data prep, ML, MLOps, and GenAI with governance. Public (DKKY); strong in F500 and regulated sectors; differentiator is end-to-end governance and collaboration. | 2025 |
| [Google Cloud Vertex AI](https://cloud.google.com/vertex-ai) | [↗](https://cloud.google.com/vertex-ai) | High | Subsidiary | enterprise-ai, ml-ops, governance | Google Cloud's unified ML and GenAI platform; includes model governance, evaluation, and deployment. Strong for enterprises already on GCP; integrates with BigQuery and Data Catalog. | 2025 |
| [Holistic AI](https://www.holisticai.com/) | [↗](https://www.holisticai.com/) | High | TBD | governance, quality, observability | AI governance platform for continuous oversight across the AI lifecycle: identify (inventory, monitoring), protect (bias audits, red teaming), enforce (policies, compliance). Used by Unilever, Siemens, eBay; 1000+ AI use cases assessed. | 2025 |
| [IBM Watsonx.Governance](https://www.ibm.com/products/watsonx-governance) | [↗](https://www.ibm.com/products/watsonx-governance) | High | Subsidiary | governance, observability, enterprise-ai | Enterprise AI governance for GenAI and ML: model factsheets, policy management, agent monitoring, and compliance accelerators (EU AI Act, ISO 42001, NIST). Governs models on watsonx, Bedrock, Azure, OpenAI; IDC and Forrester leader. | 2025 |
| [Microsoft Entra Agent](https://learn.microsoft.com/en-us/entra/security-copilot/entra-agents) | [↗](https://learn.microsoft.com/en-us/entra/security-copilot/entra-agents) | Medium | Subsidiary | governance, security-privacy, agents | AI-powered identity agents for Microsoft Entra; work with Security Copilot to automate access reviews and identity operations. Access Review Agent (preview) assists reviewers in Teams; Tenant Compliance and Risk agents in development. | 2025 |
| [ModelOp](https://www.modelop.com/) | [↗](https://www.modelop.com/) | High | Series B | governance, ml-ops, observability | AI governance platform for ML, GenAI, and agentic AI at scale. Introduced AI Governance Score; used by Fidelity, FINRA, Bristol Myers Squibb. Raised $10M Series B (2024); Gartner Market Guide for AI Governance Platforms. | 2025 |
| [Monitaur](https://www.monitaur.ai/) | [↗](https://www.monitaur.ai/) | High | Series A | governance, quality | AI governance and model compliance platform for highly regulated industries (e.g. insurance). Defines, manages, and automates compliance across the model lifecycle. Raised $6M Series A (2024); 6x growth in 2023. | 2025 |
| [OneTrust](https://www.onetrust.com/) | [↗](https://www.onetrust.com/) | High | Series D+ | governance, security-privacy, catalog | Privacy, governance, and compliance platform; extends into AI governance and responsible AI. $1.1B+ raised, ~$4.5B valuation (2023); dominant in privacy management; expanding AI/GenAI governance offerings. | 2025 |
| [Salesforce Einstein Trust Layer](https://www.salesforce.com/artificial-intelligence/trusted-ai/) | [↗](https://www.salesforce.com/artificial-intelligence/trusted-ai/) | Medium | Subsidiary | enterprise-ai, governance, security-privacy | Trust and safety layer for Salesforce's Einstein AI: data masking, audit trails, and guardrails for GenAI in CRM. Tied to Salesforce Data Cloud and Einstein; relevant for existing Salesforce customers adopting GenAI. | 2025 |
| [Securiti](https://securiti.ai/) | [↗](https://securiti.ai/) | High | Series C | governance, security-privacy, catalog | Data Command Center for security, privacy, governance, and compliance across multicloud. AI-driven discovery, consent management, and automation; $75M Series C (2022), $50M Series B; 500+ employees, strong in financial services. | 2025 |
| [Snowflake](https://www.snowflake.com/en/) | [↗](https://www.snowflake.com/en/) | High | Public | storage-warehouse, governance, enterprise-ai | Data cloud with Cortex AI; governance via Horizon, Cortex Guard for LLM safety, and RBAC for Cortex. Public company; direct competitor to Databricks in data platform and AI governance. | 2025 |
| [Validmind](https://validmind.com/) | [↗](https://validmind.com/) | High | Seed | governance, quality, ml-ops | AI governance and model risk management for financial services: validation, testing, documentation, and regulatory compliance. $8.1M seed (2024), Point72-led; focused on banking and model risk. | 2025 |

### AI Observability & Evaluation

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Arize AI](https://arize.com/) | [↗](https://arize.com/) | High | Series C | observability, ml-ops, ai-dev | AI observability and LLM evaluation platform; Phoenix open source has 2M+ monthly downloads. $70M Series C (2025), largest AI observability round; customers include Uber, Spotify, Adobe, Duolingo. | 2025 |
| [Braintrust Data](https://www.braintrustdata.com/) | [↗](https://www.braintrustdata.com/) | High | Series B | observability, ai-dev, ml-ops | AI observability and evaluation platform with exhaustive tracing, automated evals (LLM-as-judge), prompt playground, and Brainstore for trace queries. $80M Series B (2026), Iconiq-led; customers include Notion, Replit, Stripe, Vercel. | 2025 |
| [Comet](https://www.comet.com/site/) | [↗](https://www.comet.com/site/) | High | Series B | ml-ops, observability | ML experiment tracking and MLOps platform for model development and monitoring. $50M Series B (2021); 150+ customers including Uber, Etsy, Zappos; strong in traditional ML lifecycle. | 2025 |
| [Confident AI](https://www.confident-ai.com/) | [↗](https://www.confident-ai.com/) | Medium | TBD | observability, ai-dev, quality | LLM evaluation platform (DeepEval); single- and multi-turn evals, datasets, and metrics. Run locally or on Confident AI cloud; supports team collaboration and project management. | 2025 |
| [Distributional](https://distributional.com/) | [↗](https://distributional.com/) | High | Seed | observability, ml-ops | Adaptive analytics for testing and monitoring LLMs in production; unsupervised ML for clustering, drift, and anomaly detection. $11M seed (2023), a16z-led; founded by SigOpt (Intel) alumni. | 2025 |
| [Evidently AI](https://www.evidentlyai.com/) | [↗](https://www.evidentlyai.com/) | High | Series A | observability, quality, ml-ops | Open-source ML monitoring and LLM evaluation; 100+ metrics, 7K+ GitHub stars. $15M Series A (2024); used by 1000+ companies for drift, testing, and RAG/agent evals. | 2025 |
| [Fiddler AI](https://www.fiddler.ai/) | [↗](https://www.fiddler.ai/) | High | Series C | observability, ml-ops, security-privacy | AI explainability and observability; control plane for AI agents. $30M Series C (2026), $100M total; CB Insights #1 in AI Agent Security & Risk; enterprise explainability and monitoring. | 2025 |
| [Galileo](https://www.rungalileo.io/) | [↗](https://www.rungalileo.io/) | High | TBD | observability, ai-dev, ml-ops | Evaluation intelligence platform for GenAI: hallucination detection, metrics, monitoring (Galileo Observe), and protection. Agent Leaderboard for agentic evals; Luna model for LLM-as-judge. | 2025 |
| [Gentrace](https://gentrace.ai/) | [↗](https://gentrace.ai/) | High | Series A | observability, ai-dev, quality | Testing and monitoring for GenAI apps; collaborative evaluation for engineers and non-engineers. $8M Series A (2024); Experiments product for collaborative LLM testing; total $14M raised. | 2025 |
| [Helicone](https://www.helicone.ai/) | [↗](https://www.helicone.ai/) | Medium | Seed | observability, ai-dev | Open-source observability for LLM apps: routing, debugging, and analytics. YC-backed ($500K seed); simple setup and transparent pricing for the LLM lifecycle. | 2025 |
| [HoneyHive](https://honeyhive.ai/) | [↗](https://honeyhive.ai/) | Medium | Seed | observability, ai-dev | AI observability, evaluation, and prompt management. $5.5M seed (Insight Partners, Zero Prime); closed-source; emphasis on evaluation and benchmarking. | 2025 |
| [Klu](https://klu.ai/) | [↗](https://klu.ai/) | Medium | TBD | observability, ai-dev | AI platform for building and optimizing LLM apps; prompt management and evaluation. Positioned for product and engineering teams iterating on GenAI features. | 2025 |
| [Kolena](https://www.kolena.com/) | [↗](https://www.kolena.com/) | High | Series A | observability, ml-ops, quality | ML testing platform for NLP, LLMs, computer vision, and structured data. $15M Series A (2023), $21M total; Lobby Capital-led; structured test authoring and analysis. | 2025 |
| [Langfuse](https://langfuse.com/) | [↗](https://langfuse.com/) | High | OSS | observability, ai-dev | Open-source LLM engineering platform: tracing (OpenTelemetry), prompt management, evals, datasets, and playground. 23K+ GitHub stars; managed cloud or self-hosted; 50+ framework integrations. | 2025 |
| [LangSmith](https://smith.langchain.com/) | [↗](https://smith.langchain.com/) | High | Subsidiary | observability, ai-dev | LangChain's observability platform for debugging and deploying agents and LLM apps. Framework-agnostic tracing, monitoring, and insights; managed, self-hosted, or BYOC; part of LangChain ecosystem. | 2025 |
| [LatticeFlow](https://latticeflow.ai/) | [↗](https://latticeflow.ai/) | High | Series A | governance, observability, quality | Platform linking AI governance and technical evaluations for EU AI Act and similar regimes. ~$3M from Swiss Innovation Agency (2024); partnership with KPMG Switzerland; ~$17.8M total funding. | 2025 |
| [Mercor](https://mercor.com/) | [↗](https://mercor.com/) | Low | TBD | observability | Listed in MAD under AI Observability & Evaluation; public positioning emphasizes technical recruiting. Limited public evidence of dedicated AI eval/observability product. | 2025 |
| [Patronus AI](https://www.patronus.ai/) | [↗](https://www.patronus.ai/) | High | Series A | observability, security-privacy, quality | Automated evaluation and security for detecting LLM mistakes at scale. $17M Series A (2024), $20M total; Notable Capital, Lightspeed, Datadog; focus on reliability and safety testing. | 2025 |
| [Ragas](https://github.com/explodinggradients/ragas) | [↗](https://github.com/explodinggradients/ragas) | High | OSS | observability, ai-dev, quality | Open-source framework for RAG and LLM evaluation; experiments, custom metrics, and integrations with LangChain and LlamaIndex. Systematic evaluation loops and LLM-driven metrics; widely used for RAG evals. | 2025 |
| [Trulens](https://github.com/truera/trulens) | [↗](https://github.com/truera/trulens) | High | OSS | observability, ai-dev, quality | Open-source instrumentation and evaluation for LLM apps; tracing and feedback functions for relevance, grounding, and context. From TruEra; supports reproducible evals and dashboards for RAG and agents. | 2025 |

### AI Safety & Security

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Apheris](https://www.apheris.com/) | [↗](https://www.apheris.com/) | Medium | Series A | security-privacy, ml-ops | Federated computing platform for training AI on decentralized data without moving it; life sciences focus. $20.8M Series A (2025); customers include Roche, J&J, AbbVie, Sanofi; addresses privacy and IP in pharma. | 2025 |
| [Calypso AI](https://calypsoai.com/) | [↗](https://calypsoai.com/) | High | Series A | security-privacy, observability | AI security for LLMs: test, validate, and monitor before deployment. CalypsoAI Moderator for real-time monitoring, data protection, and auditability. $23M Series A-1 (2023), $38.2M total; Paladin Capital. | 2025 |
| [Cloudflare AI Gateway Guardrails](https://developers.cloudflare.com/ai-gateway/features/guardrails/) | [↗](https://developers.cloudflare.com/ai-gateway/features/guardrails/) | Medium | Subsidiary | security-privacy, ai-dev | Guardrails in Cloudflare AI Gateway: filter and control prompts and responses for LLM traffic routed through the gateway. Part of Cloudflare's developer and security stack; useful for multi-provider inference. | 2025 |
| [Cranium](https://cranium.ai/) | [↗](https://cranium.ai/) | High | Series A | security-privacy, governance | Enterprise AI security and trust: visibility, security, and compliance across AI/ML systems; bridges data science, compliance, and security. $25M Series A (2023), $32M total; spun out of KPMG; Telstra Ventures-led. | 2025 |
| [Dynamo AI](https://www.dynamo.ai/) | [↗](https://www.dynamo.ai/) | High | Seed | ai-dev, security-privacy | AI red-teaming and security platform for validating and securing generative AI systems. Early-stage focus on enterprise AI safety. | 2025 |
| [Gray Swan](https://www.grayswan.ai/) | [↗](https://www.grayswan.ai/) | Medium | Seed | ai-dev, security-privacy | AI risk and resilience platform. Helps organizations assess and mitigate AI-related operational and security risks. | 2025 |
| [Guardrails AI](https://docs.guardrailsai.com/) | [↗](https://docs.guardrailsai.com/) | High | OSS | ai-dev, security-privacy | Open-source guardrails library for validating and constraining LLM outputs (PII, topics, structure). Widely used for safe LLM deployment. | 2025 |
| [Haize Labs](https://www.haizelabs.com/) | [↗](https://www.haizelabs.com/) | Medium | Seed | ai-dev, security-privacy | AI security and alignment research applied to enterprise safety. Focus on robust and reliable AI behavior. | 2025 |
| [HiddenLayer](https://hiddenlayer.com/) | [↗](https://hiddenlayer.com/) | High | Series B | ml-ops, security-privacy | ML model security: detection of model theft, adversarial attacks, and backdoors. Enterprise-focused; Gartner-recognized. | 2025 |
| [Kindo](https://kindo.ai/) | [↗](https://kindo.ai/) | High | Seed | ai-dev, security-privacy, enterprise-ai | AI security platform for safe adoption of GenAI: access control, prompt protection, and compliance. Targets regulated enterprises. | 2025 |
| [Lakera](https://lakera.com/) | [↗](https://lakera.com/) | High | Series A | ai-dev, security-privacy | Prompt injection and AI security; Guard and Gandalf for detecting and blocking malicious prompts. Strong developer adoption. | 2025 |
| [Mindgard](https://mindgard.ai/) | [↗](https://mindgard.ai/) | High | Seed | ml-ops, security-privacy | ML and AI security testing: adversarial robustness, model hardening, and continuous security for ML pipelines. | 2025 |
| [Nvidia NeMo Guardrails](https://developer.nvidia.com/nemo-guardrails) | [↗](https://developer.nvidia.com/nemo-guardrails) | High | Subsidiary | ai-dev, security-privacy | Nvidia’s framework for programmable guardrails on LLM outputs; topic, PII, and safety controls. Part of NeMo stack. | 2025 |
| [Prompt Security](https://www.prompt.security/) | [↗](https://www.prompt.security/) | High | Series A | ai-dev, security-privacy | Enterprise prompt security and GenAI protection: prompt injection detection, data leakage prevention, and policy enforcement. | 2025 |
| [Promptarmor](https://www.promptarmor.com/) | [↗](https://www.promptarmor.com/) | Medium | Seed | ai-dev, security-privacy | Prompt injection defense and AI input/output filtering for applications. Focus on real-time protection for LLM apps. | 2025 |
| [Promptfoo](https://www.promptfoo.dev/) | [↗](https://www.promptfoo.dev/) | High | OSS | ai-dev, observability | Open-source LLM testing and evaluation: regression tests, evals, and CI for prompts and models. Developer-focused. | 2025 |
| [Protect AI](https://protectai.com/) | [↗](https://protectai.com/) | High | Series B | ml-ops, security-privacy | ML security platform (NB Defense, ModelScan); supply chain and vulnerability scanning for ML models and notebooks. | 2025 |
| [Splx AI](https://splx.ai/) | [↗](https://splx.ai/) | Medium | TBD | ai-dev, security-privacy | AI safety and content moderation for generative AI. Helps ensure safe and compliant model outputs. | 2025 |
| [Troj.ai](https://www.troj.ai/) | [↗](https://www.troj.ai/) | High | Seed | ml-ops, security-privacy | ML model security: backdoor and trojan detection in trained models. Research-backed approach for supply chain and integrity. | 2025 |
| [Witness AI](https://witness.ai/) | [↗](https://witness.ai/) | Medium | TBD | ai-dev, security-privacy | AI assurance and monitoring for responsible deployment. Tracks behavior and risk of AI systems in production. | 2025 |

### Routing, Prompt Management & Experimentation

| Product | Link | Relevance | Stage | Tags | Notes | MAD |
|---------|------|-----------|-------|------|-------|-----|
| [Databricks Mosaic AI Gateway](https://www.databricks.com/product/artificial-intelligence/ai-gateway) | [↗](https://www.databricks.com/product/artificial-intelligence/ai-gateway) | High | Subsidiary | ai-dev, enterprise-ai | Unified gateway for LLM routing, rate limits, and key management on Databricks. Part of Mosaic AI platform. | 2025 |
| [Google Cloud Vertex AI Prompt Management](https://cloud.google.com/vertex-ai/generative-ai/docs/model-reference/prompt-classes) | [↗](https://cloud.google.com/vertex-ai/generative-ai/docs/model-reference/prompt-classes) | High | Subsidiary | ai-dev, enterprise-ai | Prompt versioning and management in Vertex AI; prompt classes and evaluation. Integrates with Gemini and Vertex models. | 2025 |
| [Keytalk.ai](https://www.keytalkai.com/) | [↗](https://www.keytalkai.com/) | Medium | TBD | ai-dev | Conversational AI and prompt management for customer-facing applications. Focus on key message and brand consistency. | 2025 |
| [LiteLLM](https://www.litellm.ai/) | [↗](https://www.litellm.ai/) | High | OSS | ai-dev | Open-source proxy and unified API for 100+ LLMs; drop-in OpenAI-compatible interface, routing, and cost tracking. | 2025 |
| [Martian](https://www.withmartian.com/) | [↗](https://www.withmartian.com/) | High | Series A | ai-dev, observability | Model router and observability: automatic model selection, cost and latency optimization, and debugging for LLM apps. | 2025 |
| [Microsoft Prompt Flow (Azure AI Studio)](https://learn.microsoft.com/en-us/azure/ai-foundry/concepts/prompt-flow) | [↗](https://learn.microsoft.com/en-us/azure/ai-foundry/concepts/prompt-flow) | High | Subsidiary | ai-dev, enterprise-ai | Prompt engineering, evaluation, and orchestration in Azure AI Studio. End-to-end flow design and deployment for GenAI apps. | 2025 |
| [OpenRouter](https://openrouter.ai/) | [↗](https://openrouter.ai/) | High | Seed | ai-dev | Single API for many open and closed LLMs; routing, fallbacks, and usage-based pricing. Popular among developers. | 2025 |
| [Parea](https://www.parea.ai/) | [↗](https://www.parea.ai/) | High | Series A | ai-dev, observability | LLM evaluation and observability: experiment tracking, evals, and production monitoring for prompt and model performance. | 2025 |
| [Portkey](https://portkey.ai/) | [↗](https://portkey.ai/) | High | Series A | ai-dev, observability | LLM gateway: routing, fallbacks, caching, and observability. Aims to improve reliability and cost for production LLM apps. | 2025 |
| [PromptHub](https://www.prompthub.us/) | [↗](https://www.prompthub.us/) | Medium | TBD | ai-dev | Prompt management and versioning for teams. Centralized prompt library and collaboration. | 2025 |
| [PromptLayer](https://www.promptlayer.com/) | [↗](https://www.promptlayer.com/) | High | Seed | ai-dev, observability | Prompt tracking and observability for OpenAI and other LLMs; versioning, analytics, and debugging in production. | 2025 |
| [Salesforce Prompt Studio / Trust Layer Hooks](https://www.salesforce.com/artificial-intelligence/prompt-builder/) | [↗](https://www.salesforce.com/artificial-intelligence/prompt-builder/) | High | Subsidiary | ai-dev, enterprise-ai | Prompt builder and Trust Layer integration in Salesforce; govern and tune prompts for Einstein and CRM GenAI. | 2025 |
| [TensorZero](https://www.tensorzero.com/) | [↗](https://www.tensorzero.com/) | High | Seed | ai-dev, observability | Evaluation and assurance for LLM applications; evals, guardrails, and compliance checks for production deployments. | 2025 |
| [Unify](https://unify.ai/) | [↗](https://unify.ai/) | High | Series A | ai-dev | Unified API and router across many LLM providers; one interface for inference, comparison, and switching. | 2025 |
| [Vellum](https://www.vellum.ai/?utm_source=direct&amp;utm_medium=none) | [↗](https://www.vellum.ai/?utm_source=direct&amp;utm_medium=none) | High | Series B | ai-dev, observability | Prompt engineering platform: design, version, evaluate, and deploy LLM workflows with observability and evaluation. | 2025 |


## Catalog maintenance

- **Relevance:** `High` / `Medium` / `Low` — how relevant to Databricks research
- **Stage:** Seed / Series A–D+ / Public / Subsidiary / OSS — from Crunchbase or press
- **Notes:** 1–2 sentence eval: traction, differentiator, "watch" / "partner" / "competitor"
- **Prior years:** add rows from 2023/2024 that dropped from 2025; set MAD to `2024` or `2023, 2024`
- **New categories:** MAD adds sections each year — follow the same table format
- **To refresh:** re-run `.cursor/scripts/parse_mad_card.py` + `.cursor/scripts/merge_mad_with_landscape.py`

---

*Landscape structure and company list derived from the [2025 MAD (ML, AI & Data) Landscape](https://mad.firstmark.com/) by Matt Turck / FirstMark. This document is a living catalog; extend with more rows and categories from current and prior MAD editions.*
