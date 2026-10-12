---
description: Build next week's plan for a product from brand.md and learnings.md.
argument-hint: <product-slug> [start date YYYY-MM-DD]
---

Plan one week for `products/$1/`. Use the start date in `$2` if given, otherwise the next Monday. Check Canadian statutory holidays and avoid posting on them.

1. Read `brand.md`, `claims.md`, `learnings.md`, the last two files in `plans/`, and `posts.csv` and `results.csv` if they have rows.
2. State the cycle's hypothesis in one sentence at the top. If `learnings.md` has a next variable to test, use it. Otherwise pick one and say why.
3. Allocate about 70% of the posts to what the last cycle's learnings say worked and about 30% to exactly one new variable. In the first cycle there is no prior data: say so, and make the one variable the whole test.
4. Choose a channel mix from `brand.md`. Do not add a channel without saying why.
5. List 6 to 8 posts: post_id (continue the numbering from `posts.csv`), date and time, platform, pillar, topic, hook type, angle, format, CTA, test variable.
6. Write `products/$1/plans/<start date>.md` with the hypothesis, the table, and a short list of what to measure.
7. Append the posts to `posts.csv` with status `drafted` blank until `/draft` runs. Build each `utm_link` by the rule in `CLAUDE.md`.

Work on a branch `cycle/<start date>` and open a PR.
