# Product Design Intelligence — Source Guide

Industry-leading sources for product design research, UX patterns, and design decision-making. Used by `agent-product-design.md` and available to any researcher who needs the design lens.

---

## Tier 1: Canonical UX Research & Guidelines

These are the gold standard for evidence-based design decisions. Cite these when justifying design choices.

### Nielsen Norman Group (NNGroup)
**URL:** https://www.nngroup.com/
**What:** The most cited UX research organization. Publishes research-backed articles on every major interaction pattern, with usability study data. Founded by Jakob Nielsen and Don Norman.
**When to use:** Any time you need research-backed guidance on a specific UX pattern (tables, search, navigation, forms, dashboards, error handling, onboarding, etc.)
**Key topic areas for Databricks:**
- [Enterprise UX](https://www.nngroup.com/topic/enterprise-applications/) — complex workflows, data-heavy interfaces
- [Information Architecture](https://www.nngroup.com/topic/information-architecture/) — navigation, categorization, labeling
- [Dashboard Design](https://www.nngroup.com/topic/dashboards/) — data visualization in products
- [Search UX](https://www.nngroup.com/topic/search/) — catalog search, faceted search, filters
- [Tables & Data](https://www.nngroup.com/topic/tables/) — data table patterns, sorting, filtering
- [Permission & Access Control](https://www.nngroup.com/articles/permission-requests/) — relevant for governance UX
- [Progressive Disclosure](https://www.nngroup.com/articles/progressive-disclosure/) — essential for enterprise complexity
- [Error Messages](https://www.nngroup.com/articles/error-message-guidelines/) — critical for data pipeline and governance errors

### Baymard Institute
**URL:** https://baymard.com/
**What:** Enterprise UX benchmarks and large-scale usability research. More quantitative than NNGroup.
**When to use:** When you need benchmark data on UX patterns (e.g., "what % of enterprise users expect X behavior")

### Laws of UX
**URL:** https://lawsofux.com/
**What:** Concise reference for foundational UX principles (Fitts's Law, Hick's Law, Jakob's Law, Miller's Law, etc.) with links to supporting research.
**When to use:** Quick principle check when making interaction decisions.

---

## Tier 2: Design Systems (Pattern Libraries)

These codify how major tech companies design enterprise products. Use for component-level and interaction-level patterns.

| Design System | URL | Best for |
|--------------|-----|---------|
| **Carbon (IBM)** | https://carbondesignsystem.com/ | Enterprise data product patterns — IBM faces the same "complex data for enterprise users" challenge as Databricks. Excellent data table, form, and notification patterns. |
| **Material Design 3 (Google)** | https://m3.material.io/ | Component fundamentals, motion design, accessibility, data visualization guidelines |
| **Primer (GitHub)** | https://primer.style/ | Developer-facing product patterns — relevant for Databricks' developer persona |
| **Ant Design** | https://ant.design/ | Data-heavy enterprise UI; best-in-class table component, form patterns, dashboard templates |
| **Atlassian Design** | https://atlassian.design/ | Enterprise collaboration patterns — relevant for multi-user governance workflows |
| **Polaris (Shopify)** | https://polaris.shopify.com/ | Merchant-facing enterprise patterns; excellent empty state and onboarding patterns |
| **Lightning (Salesforce)** | https://www.lightningdesignsystem.com/ | Enterprise CRM patterns — permission models, role-based views, complex data entry |
| **Fluent (Microsoft)** | https://fluent2.microsoft.design/ | Microsoft's enterprise design language — relevant when comparing to Fabric/Purview UX |
| **Spectrum (Adobe)** | https://spectrum.adobe.com/ | Creative-tool UX patterns — relevant for data exploration and visual interfaces |
| **Paste (Twilio)** | https://paste.twilio.design/ | Developer-focused enterprise patterns; good accessibility documentation |

---

## Tier 3: Data Product UX — Competitors & Peers

Study these for domain-specific UX patterns in data governance, catalogs, and analytics.

### Data Catalogs & Governance
| Product | What to study | Where to find UX examples |
|---------|--------------|--------------------------|
| **Atlan** | Modern metadata UX, AI-assisted governance, search-first IA | atlan.com, YouTube demos, G2 screenshots |
| **Alation** | Enterprise catalog search, data stewardship workflows | alation.com, YouTube demos |
| **Collibra** | Governance workflow design, business glossary UX, stewardship | collibra.com, YouTube demos |
| **Secoda** | AI-native catalog, automated documentation UX | secoda.co, YouTube demos |
| **DataHub (LinkedIn OSS)** | Open-source catalog UX, lineage visualization | datahubproject.io, GitHub, demo videos |
| **OpenMetadata** | Open-source metadata platform UX | open-metadata.org, GitHub |

### Analytics & BI
| Product | What to study | Where to find UX examples |
|---------|--------------|--------------------------|
| **Snowflake (Horizon)** | Governance tab UX, data sharing, access policies | Snowflake docs, YouTube, Snowflake Summit sessions |
| **dbt Cloud** | Lineage visualization, documentation UX, explorer | cloud.getdbt.com, dbt docs |
| **Looker** | Semantic layer UX, explore interface, governance | cloud.google.com/looker |
| **Tableau** | Catalog integration, data management, prep flows | tableau.com |
| **Power BI / Fabric** | Unified analytics + governance UX | Microsoft docs, Ignite sessions |

### Observability & Quality
| Product | What to study | Where to find UX examples |
|---------|--------------|--------------------------|
| **Monte Carlo** | Data incident UX, lineage + observability integration, alert design | montecarlodata.com, YouTube |
| **Great Expectations** | Data quality expectation authoring UX | greatexpectations.io, docs |
| **Soda** | Data quality check UX, SodaCL authoring | soda.io |
| **Bigeye** | Automated monitoring UX, anomaly detection visualization | bigeye.com |

---

## Tier 4: Design Thinking & Product Strategy

For product-level design decisions (not just UI patterns).

| Source | URL | Best for |
|--------|-----|---------|
| **Luke Wroblewski** | lukew.com | Pioneer in mobile-first design, form design, and input patterns. Recently prolific on AI-native interaction models and data-driven product design. His "Ideation + Implementation" series explores how AI changes product design workflows. Essential reading for any AI-assisted or data-heavy UX work. |
| **Julie Zhuo** | juliezhuo.com | Design leadership, design quality, decision-making in product teams |
| **Lenny's Newsletter** | lennysnewsletter.com | Product strategy, growth, user research methods |
| **Dive Club** | dive.club | Modern design leadership content — interviews and essays from top design leaders at tech companies. Fresh perspectives on how design orgs operate, make decisions, and scale. |
| **Soleio Cuervo** | x.com/soleio | Early Facebook/Dropbox designer; shares sharp takes on product design craft and design leadership. Follow for real-time design thinking from one of the field's most influential practitioners. |
| **Intercom Blog** | intercom.com/blog | Jobs-to-be-done, product-led growth, SaaS product design |
| **Spotify Design** | spotify.design | Design culture, design ops, prototyping methodologies |
| **Reforge** | reforge.com | Product strategy frameworks, growth models, retention loops |
| **IDEO** | ideo.com | Design thinking methodology, human-centered design |
| **InVision Blog** | invisionapp.com/inside-design | Product design process, remote design collaboration |
| **UX Collective** | uxdesign.cc | Curated essays on UX design practice |
| **A List Apart** | alistapart.com | Information architecture, content strategy, web standards |
| **Smashing Magazine** | smashingmagazine.com | Front-end patterns, accessibility, responsive design |

---

## Tier 5: Information Visualization & Data UX

For data-heavy interfaces — dashboards, lineage graphs, metric displays, table design.

| Source | URL | Best for |
|--------|-----|---------|
| **Edward Tufte** | edwardtufte.com | Canonical data visualization principles — data-ink ratio, small multiples, sparklines |
| **Tamara Munzner** | *Visualization Analysis and Design* (book) | Systematic framework for choosing visualization types based on data and task |
| **Observable** | observablehq.com | Interactive data visualization examples and techniques |
| **D3.js Gallery** | d3-graph-gallery.com | Comprehensive catalog of visualization types with code |
| **From Data to Viz** | data-to-viz.com | Decision tree for choosing the right chart type |
| **Storytelling with Data** | storytellingwithdata.com | Data communication, dashboard storytelling |
| **Information is Beautiful** | informationisbeautiful.net | Creative visualization inspiration |
| **Flowing Data** | flowingdata.com | Statistical visualization, data exploration patterns |

---

## Tier 6: Accessibility & Inclusive Design

Non-negotiable for enterprise products. Every design implication should be checked against these.

| Source | URL | Best for |
|--------|-----|---------|
| **WCAG 2.2** | w3.org/WAI/WCAG22/ | Web accessibility standard — the legal and ethical baseline |
| **Microsoft Inclusive Design** | inclusive.microsoft.design | Inclusive design methodology and toolkit |
| **Deque aXe** | deque.com/axe/ | Accessibility testing and patterns |
| **A11y Project** | a11yproject.com | Practical accessibility checklist and resources |
| **WebAIM** | webaim.org | Color contrast, screen reader testing, ARIA patterns |

---

## Tier 7: Academic HCI Research

For novel interaction concepts or when existing patterns don't fit.

| Source | Best for |
|--------|---------|
| **ACM CHI Proceedings** | Human-computer interaction research — `[concept] user interface` |
| **ACM CSCW** | Computer-supported cooperative work — relevant for multi-user governance |
| **IEEE VIS** | Information visualization — lineage, graph, dashboard design |
| **ACM UIST** | User interface technology — novel interaction techniques |
| **DIS (Designing Interactive Systems)** | Design research methodology |

---

## How to use this file

1. **For a specific UX pattern question** (e.g., "how should we design tag inheritance?") → Start with NNGroup, then check design systems (Carbon, Material), then competitor approaches.

2. **For a new feature concept** (e.g., "design an ontology browser") → Start with competitor UX examples, then NNGroup for underlying patterns, then academic HCI if the concept is novel.

3. **For a design review** → Reference design system patterns for consistency, NNGroup for usability principles, and competitor UX for differentiation opportunities.

4. **For the Product Design Implications synthesis section** → Pull from all tiers as relevant: principles (NNGroup), patterns (design systems), precedents (competitors), and open questions (academic HCI).
