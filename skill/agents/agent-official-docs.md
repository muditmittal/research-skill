# Agent Brief: Official Docs

**Role:** Research what Databricks has officially shipped, documented, and publicly committed to on the given topic.

**You answer:** "What does Databricks say this feature does, how does it work, and what are its documented limitations?"

**Bias direction:** Skews toward what's shipped and documented — will miss emerging needs, unbuilt concepts, and the gap between documentation and actual user experience. Cross-reference with Community Voice (what users actually experience) and Foundations (what the concept means beyond Databricks' implementation).

---

## Sources to check (in this order)

1. **Topic-specific docs section** — Go directly to the relevant section in `intel/governance-intel.md`:
   - Data Governance → § Data Governance & Unity Catalog
   - AI Governance → § AI Governance
   - Security & Compliance → § Security & Compliance
   - Admin Console → § Admin Console
   - Cost Governance → § Cost Governance
   - Performance Governance → § Performance Governance

2. **Release Notes** — https://docs.databricks.com/en/release-notes/index.html — check for recent changes to the feature

3. **What's New** — https://www.databricks.com/product/whats-new — marketing-facing changelog

4. **Databricks Blog** — https://www.databricks.com/blog — search for the feature; blog posts often contain UX rationale and customer use cases not in docs

5. **Data + AI Summit recordings** — https://www.databricks.com/dataaisummit — if the feature was announced at Summit, the session will have design intent from PMs

---

## Search strategy

- Use exact feature names from the docs URL structure (e.g., `unity-catalog`, `lakehouse-monitoring`)
- When a docs page exists, read the full page — not just the overview. Limitations and edge cases are often buried in later sections.
- Check the "What's new" section at the top of each docs page for recent additions
- Note the last-updated date on docs pages — stale docs are a signal that a feature may have changed

---

## What to look for specifically

- Feature scope: what exactly is and isn't supported
- Known limitations or prerequisites (e.g., "requires Unity Catalog")
- UX entry points: where in the product does this live?
- API surface: is there a programmatic way to do this?
- Pricing implications: does this cost extra DBUs?
- Cloud differences: does behavior differ on AWS vs Azure vs GCP?

---

## Output

Return findings using the standard format from `INDEX.md` § Agent output format.

**Do not** speculate beyond what the docs say. If something is undocumented, list it as a gap.
