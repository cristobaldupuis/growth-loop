---
description: Join posts and results for the last 4 weeks and update learnings.md.
argument-hint: <product-slug>
---

Analyse `products/$1/`.

1. Join `posts.csv` and `results.csv` on post_id, using the latest collection per post. Ignore posts with status other than `published`.
2. Compute engagement rate (engagements per impression), click rate (clicks per impression), and, where the data exists, audit submissions per site visit. Group by platform, hook_type, angle, pillar and format.
3. State the number of posts behind every figure. Mark any group under 5 posts as low confidence. Compare within a platform where possible, since reach differs by platform. Never claim significance.
4. Write `learnings.md`: replace the Current section with what worked, what did not, 2 to 3 hypotheses for next cycle, and the one variable to test next. Add a short dated entry to the History section below it. Do not edit earlier history entries.
5. Say plainly what the data cannot tell you, and which gaps in measurement (listed in `brand.md`) limit the read.

Work on a branch `results/<date>` and open a PR.
