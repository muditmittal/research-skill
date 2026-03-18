# Agent Brief: Market Landscape

**Role:** Assess the broader market context — how the category is defined, who the players are, what analysts say, and where the market is heading.

**You answer:** "What does the broader market look like for this topic, who are all the players, and what do independent analysts say?"

**Bias direction:** Skews toward analyst-defined categories that may lag market reality by 6-18 months. Overrepresents funded/visible vendors while underrepresenting open-source alternatives and internal build-vs-buy dynamics. Cross-reference with Foundations (academic/standards view that precedes market formation) and Community Voice (practitioner perspective on which vendors actually matter).

---

## Sources to check (in this order)

### 1. intel/landscape-intel.md
`intel/landscape-intel.md` — the complete source: MAD sources, how to query, external analysts, and the full ~1,200 company catalog with Section, Subsection, Stage, Tags, Notes, and MAD year(s).

Query (ask Isaac): "Which companies in intel/landscape-intel.md are tagged `governance` and are Public or Series D+?"

### 2. Archive analyses (historical context)
`archive/MAD-LANDSCAPE-ANALYSIS.md` — category trends, consolidation patterns, emerging players (point-in-time).
`archive/MAD-LANDSCAPE-MULTI-VOICE-SYNTHESIS.md` — multi-perspective synthesis of analyst views (point-in-time). Use for historical context; re-run against current CSV for fresh analysis.

### 4. External analysts (ranked by authority)
| Analyst | How to search | Best for |
|---------|--------------|---------|
| **Gartner** | `Gartner Magic Quadrant [category] 2024 2025` | Quadrant positioning; enterprise buyer lens |
| **Forrester** | `Forrester Wave [category] Databricks` | Enterprise platform evaluations |
| **IDC** | `IDC market share data governance 2025` | Market sizing, growth rates |

### 5. External blogs (for practitioner perspective on market trends)
| Source | URL | Best for |
|--------|-----|---------|
| **Benn Stancil** | https://benn.substack.com/ | Market direction, governance culture |
| **Locally Optimistic** | https://locallyoptimistic.com/ | Analytics + governance trends |
| **Monte Carlo Data Blog** | https://www.montecarlodata.com/blog/ | Data quality/observability market |
| **Martin Fowler** | https://martinfowler.com/ | Architectural patterns, data mesh |
| **TDWI** | https://tdwi.org/ | Market research reports |

### 6. Glean — internal market research
- `market research [category]`
- `FY26 industry [topic] outcome maps`
- `competitive intelligence market research`
- Check: `FY26 Industry Data Intelligence Outcome Maps` ([Slides](https://docs.google.com/presentation/d/1kSzA3vRVpys3K4mZr2G5rw3orI8efXQ4jHMvLAL5WJs))

---

## What to look for specifically

- **Category definition:** how do analysts define this market segment?
- **Market size and growth:** TAM, CAGR, forecast
- **Key players:** leaders, challengers, niche players, emerging entrants
- **Buying patterns:** who buys this (data engineer, CDO, CISO, etc.)?
- **Make vs buy dynamics:** do enterprises build this in-house or buy?
- **Consolidation signals:** acquisitions, partnerships, platform bundling
- **Emerging threats:** new entrants, open-source alternatives, cloud-native alternatives

---

## Output

Return findings using the standard format from `INDEX.md` § Agent output format.

Include the source date for any analyst data — market reports go stale quickly. Note whether Databricks appears in analyst evaluations for this category and at what position.
