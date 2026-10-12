# CLAUDE.md: growth-loop

Weekly marketing loop for one or more products. Read `README.md` for the routine and layout. This file has the rules that are easy to get wrong.

## Rules

1. **Never invent metrics, quotes, customers or results.** If data is missing, say so in the output. A hypothetical in copy (for example 5 calls x $350) must be framed as a hypothetical or an estimate.
2. **Claims come from `products/<slug>/claims.md`.** A capability may be mentioned only if it appears under Safe to say. Anything under Do not say is a hard stop, however well it would work as a hook. If the claim is not listed at all, treat it as not cleared and ask.
3. **For rightoncall, the ground truth is `cristobaldupuis/voice-agent`, file `docs/CLAIMS.md`.** At the start of every `/draft`, attach that repo with `add_repo` (read access), read the file, and update `claims.md` if the two differ before drafting anything. The marketing site (`cristobaldupuis/rightoncall`) must agree with it; where the site claims more, the site is wrong, not the doc.
4. **Humans publish.** Nothing in this repo posts, sends or schedules to a platform.
5. **One test variable per cycle.** About 70% of a week repeats what `learnings.md` says worked, about 30% tests exactly one new variable, named in `posts.csv` under `test_variable`.
6. **Every post gets an ID and a UTM link at draft time.** Format: `?utm_source=<platform>&utm_medium=social&utm_campaign=c<cycle>w<week>&utm_content=<post_id>`. Reddit posts carry no link.
7. **Small samples.** Flag any group with fewer than 5 posts as low confidence. Never claim statistical significance.
8. **Copy follows `brand.md`.** For rightoncall: plain, specific, limits stated as plainly as features, no em dashes, no AI buzzwords, no not-X-but-Y contrasts, scripted sample calls always labelled as scripted.
9. **Web only.** Every instruction to the person must work in Claude Code web, claude.ai or github.com. Never tell them to run a local command.

## Data files

- `posts.csv` columns: post_id, date_planned, platform, pillar, topic, hook_type, angle, format, cta, test_variable, utm_link, status, post_url.
- `results.csv` columns: post_id, date_collected, impressions, engagements, clicks, site_visits_utm_content, audit_submissions, replies_or_dms, notes, collected_from.
- Quote any field containing a comma. Keep post_ids stable across cycles by continuing the numbering (P09 and on).
- `status` is one of: drafted, approved, published, skipped.

## Git

- One concern per commit. A weekly plan and its drafts go on a branch named `cycle/YYYY-MM-DD` and are merged by PR so the plan can be reviewed before the week starts.
- Results and learnings updates go straight to a branch `results/YYYY-MM-DD`, also by PR.
