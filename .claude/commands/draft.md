---
description: Draft every post in the current plan, write asset briefs, run the critic pass and the claims check.
argument-hint: <product-slug>
---

Draft the posts for `products/$1/` that are in `posts.csv` without a file in `drafts/`.

1. For rightoncall, attach `cristobaldupuis/voice-agent` with `add_repo` (read), read `docs/CLAIMS.md`, and update `claims.md` if it differs. Do this first.
2. Read `brand.md`, `claims.md` and `learnings.md`.
3. For each post write `drafts/<post_id>.md` with: a front matter block (post_id, platform, date_planned, status), the Copy (with `[LINK]` where the UTM link goes), the Asset brief, the Critic note and the Claims check.
4. Write for the platform. LinkedIn: short paragraphs, no hashtags. Facebook: conversational, one idea. Instagram: caption plus slide or beat-by-beat script. Reddit: value first, disclose who you are in the first lines, no link.
5. Critic pass: score each draft 1 to 10 on hook strength, clarity, brand fit and platform fit. Rewrite anything under 8, up to 3 rounds. Record the final score and the one thing a human should check before posting.
6. Claims check: list each capability the copy mentions and the line in `claims.md` that clears it. Any claim that cannot be cleared gets cut.
7. Run the humanizer pass on the final copy: no em dashes, no not-X-but-Y, no forced triads, no invented statistics.
8. Set `status` to `drafted` in `posts.csv`.

Do not generate images, audio or video here. The Asset brief is the handoff to Canva or ElevenLabs.
