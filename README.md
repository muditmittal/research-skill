# Research Skill for Databricks

A multi-agent research system for Databricks product teams. Ask a question, get a synthesized Google Doc — 10 agents search in parallel, conflicts resolved via trust hierarchy, design implications included.

> **[Open the visual explainer](index.html)** in a browser for the full overview.

## Quick start

```bash
# 1. Copy the skill files
cp -r skill/ ~/.cursor/docs/research/

# 2. Customize for your product area (ships with Data Governance defaults)
cat skill/CUSTOMIZE.md

# 3. Verify MCP connections: Google Docs, Glean, Databricks, Slack, Jira, Confluence

# 4. Run research
/research <your question>
```

## How it works

```
/research Should we build an Ontology feature?
    ↓
Phase 1 — Dispatch:   Match question to one of 20 patterns → select agents
Phase 2 — Collect:    Agents search in parallel, return structured findings with citations
Phase 3 — Synthesize: Coverage check → themes → conflict resolution → design implications
Phase 4 — Publish:    Google Doc with inline citations, tables, code blocks, appendix
```

Output is **findings-first** — executive summary, themes, conflicts, gaps, design implications. Research methodology and raw agent outputs go in the appendix.

## The 10 agents

| Agent | Searches | Bias |
|-------|----------|------|
| Official Docs | Databricks docs, release notes, blog | Shipped features only |
| Community Voice | Forums, Reddit, Ideas Portal | Vocal power users |
| Internal Intel | PRDs, UXR, customer notes, ES tickets, CUJs | Past internal thinking |
| Competitive | Battlecards, competitor features, win/loss | Databricks-favorable framing |
| Quantitative | Logfood SQL queries, SimpleBricks/CUJ scores | Instrumented features only |
| Market Landscape | Analyst views, MAD landscape (~1,200 companies) | Analyst views lag 6–18 months |
| Roadmap & Planning | Pre-reads, Aha!, Jira, leadership priorities | Formally planned work only |
| Foundations | Academic papers, W3C/ISO standards | Theoretical |
| Sales & GTM | BrickBites, SFDC win/loss, PMM messaging | Deal-winning narratives |
| Product Design | NNGroup, design systems, competitor UX | UX elegance over feasibility |

The **Quantitative agent** executes actual SQL queries against Logfood — not just hypothetical queries. The **Product Design agent** runs twice: once as a researcher, then again to synthesize all findings into design implications.

## Key behaviors

- **Inline citations** — every factual claim has a `[N]` reference linking to the source
- **Trust hierarchy** — 9 levels, from Logfood data (rank 1) to external blogs (rank 9)
- **Coverage confidence** — flags under-researched topics before synthesis
- **Follow-up research** — updates the existing doc in place (URL never changes)
- **No empty sections** — omits sections with no content rather than showing empty tables
- **Design implications** — consolidated section at the end connecting findings to UX decisions

## Prerequisites

| MCP | Required for |
|-----|--------------|
| Google Docs | Output publishing (without it, output stays in terminal) |
| Glean | Internal Intel, Roadmap, Sales & GTM agents |
| Databricks | Quantitative agent (Logfood SQL) |
| Confluence | Internal Intel, Roadmap agents |
| Slack | Supplemental signal (optional) |
| Jira | Roadmap & Planning agent |

Missing access = the agent notes a gap. The run won't break.

## Customization

Ships with Data Governance defaults. Swap three files for other product areas:

- `intel/governance-intel.md` — topic-specific doc links
- `intel/db-data.md` — Logfood schemas and workspace URLs
- `agents/agent-competitive.md` — competitor table

Full walkthrough: `skill/CUSTOMIZE.md`

## Browse the skill

Open `index.html` in any browser — no server or dependencies needed.

## Example outputs

`skill/output/` ships with two real research syntheses so you can see what to expect:
- `ontology-research-synthesis.md` — full 10-agent research on Ontology
- `tags-research-synthesis.md` — deep dive across 8 subtopics for Tags

After install, your own research outputs are saved to `~/.cursor/docs/research/output/`.

## Contributing

Found a missing source or agent gap? Message Mudit on Slack or file a PR.
