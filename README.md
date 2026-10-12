# growth-loop

A weekly marketing loop that runs inside Claude Code on the web. It plans a week of content for a product, drafts it per platform, checks every draft against a list of claims the product can actually back up, and learns from the results you paste back.

It does not post anything. A person publishes.

## The weekly routine

1. `/plan <product>` builds next week's plan from `brand.md` and `learnings.md`.
2. `/draft <product>` writes every post, writes asset briefs, scores each draft, and checks it against `claims.md`.
3. You publish by hand and fill in each live post's URL in `posts.csv`.
4. A week later, paste the analytics export into the chat and run `/ingest <product>`.
5. `/analyze <product>` joins posts and results and updates `learnings.md`.

`/brand <product> <url or brief>` is the one-time setup for a new product.

## Layout

```
.claude/commands/        the five slash commands
products/<slug>/
  brand.md               audience, positioning, voice, pillars
  claims.md              what may and may not be said
  posts.csv              one row per post, tagged at draft time
  results.csv            one row per post per collection date
  learnings.md           current learnings plus dated history
  plans/YYYY-MM-DD.md    the weekly plan
  drafts/P01.md ...      copy, asset brief, critic note, claims check
```

## Products

- `rightoncall`: AI voice receptionist for Ontario home-service shops. First cycle starts 2026-10-13.

## Notes

- Everything here is meant to be driven from Claude Code web and github.com.
- A Google Sheet (RightOnCall Growth Loop) holds a copy of cycle 1 from before this repo existed. This repo is the source of truth. Do not edit the Sheet.
