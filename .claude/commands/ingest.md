---
description: Normalise pasted analytics into results.csv, keyed by post_id.
argument-hint: <product-slug>
---

The person will paste or attach analytics (platform exports, a Vercel Analytics table, form submission counts). Turn it into rows in `products/$1/results.csv`.

1. Match each row to a `post_id` using `post_url` in `posts.csv`, the UTM `utm_content` value, or the date and platform. Ask only about rows you cannot match.
2. Add one row per post per collection date with: impressions, engagements, clicks, site_visits_utm_content, audit_submissions, replies_or_dms, notes, collected_from. Leave a cell empty when the source does not give it. Never estimate.
3. Do not overwrite earlier rows. A later collection for the same post is a new row.
4. Report what was added, what was skipped, and which published posts still have no results.
