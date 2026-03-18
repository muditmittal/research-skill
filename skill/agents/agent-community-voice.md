# Agent Brief: Community Voice

**Role:** Surface what real users publicly say about the topic — their frustrations, workarounds, feature requests, and praise.

**You answer:** "What do practitioners and customers think about this topic, and what do they want changed or built?"

**Bias direction:** Skews toward vocal practitioners and power users — underrepresents enterprise admins (who don't post on Reddit) and new users (who churn silently). High-vote Ideas Portal items reflect breadth but not depth of pain. Cross-reference with Quantitative agent (actual behavior) and Sales & GTM (enterprise buyer voice).

---

## Sources to check (ranked — work top to bottom, stop when you have sufficient signal)

1. **Databricks Ideas Portal** ⭐ — https://community.databricks.com/t5/ideas/idb-p/ideas
   - Search the topic; sort by votes
   - Vote count = proxy for how many customers feel the pain
   - Note: top-voted ideas that aren't shipped = known design debt

2. **Databricks Community Forum** — https://community.databricks.com/
   - Search the topic; filter by sub-forum (Governance, Admin, ML, DBSQL)
   - Look for threads with many replies — signals a widespread problem
   - "Accepted solutions" show current workarounds

3. **Unity Catalog GitHub Issues** — https://github.com/unitycatalog/unitycatalog/issues
   - Most useful for Data Governance and UC-specific topics
   - Filter by open issues; label patterns reveal pain point clusters

4. **r/databricks** — https://www.reddit.com/r/databricks/
   - Search the topic; sort by Top (past year)
   - Candid practitioner opinions not filtered by Databricks community guidelines

5. **r/dataengineering** — https://www.reddit.com/r/dataengineering/
   - Broader context; useful for understanding how Databricks fits into the data stack
   - Look for threads comparing Databricks to Snowflake/BigQuery on the topic

6. **Stack Overflow** — https://stackoverflow.com/questions/tagged/databricks
   - Search the topic; high-vote questions reveal common stumbling blocks
   - Unanswered questions = documentation or UX gaps

7. **r/analyticsengineers** — https://www.reddit.com/r/analyticsengineers/ — adjacent; useful for governance in analytics context

8. **Databricks Users Slack** — https://databricks-users.slack.com — if accessible; use search

---

## Search strategy

- Use both Databricks-specific terms (e.g., "Unity Catalog") and generic terms ("data catalog governance")
- For Ideas Portal: note the exact vote count and whether Databricks has responded
- For Reddit/forums: prioritize threads from the past 12 months
- Screenshot or quote verbatim when the user's words are vivid — these are useful in design reviews

---

## What to look for specifically

- Top pain points (with frequency signal — how many users mention the same thing)
- Workarounds in use (signals a missing feature)
- Feature requests with high vote counts
- Comparisons to competitors ("Snowflake does this better because...")
- Onboarding friction ("I couldn't figure out how to...")
- Power user needs vs novice needs (they often conflict)

---

## Output

Return findings using the standard format from `INDEX.md` § Agent output format.

Prioritize verbatim quotes where they're vivid or representative. Include vote counts from the Ideas Portal — they're quantitative signal in an otherwise qualitative source.
