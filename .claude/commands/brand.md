---
description: One-time setup for a product. Writes brand.md and claims.md from a URL or brief.
argument-hint: <product-slug> <url or brief>
---

Set up `products/$1/`. The rest of `$ARGUMENTS` is a URL or a short brief.

1. If it is a URL, fetch it and read the pages that carry positioning, pricing and limits. Do not guess from the homepage alone.
2. Write `products/$1/brand.md` with these fields: product, core promise, primary audience, secondary audience, buyer pains, proof available (and what is not cleared for public use), primary and secondary CTAs, pricing that is safe to state, voice rules, 3 to 4 content pillars, channels for the first cycle, posting identity, measurement gaps.
3. Write `products/$1/claims.md` as a table: topic, safe to say, do not say, source. Only list what you can source. Put anything you cannot confirm under Do not say with the reason "not confirmed".
4. Create empty `posts.csv` and `results.csv` with the headers from `CLAUDE.md`, plus `learnings.md` with a Standing rule section and no cycles yet.
5. Say which fields you left as TBD and need an answer from the person.

Do not invent proof, customers or numbers.
