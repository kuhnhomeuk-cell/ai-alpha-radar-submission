# AI Alpha Radar

Judge-facing static submission for the AI Alpha Radar landing page and dashboard.

## What is included

- `public/index.html` - landing page
- `public/dashboard.html` - dashboard app
- `public/data.json` - dashboard snapshot data
- `public/tokens.css` - shared design tokens
- `public/bg-pingpong.mp4` - landing-page background video
- `technical-appendix/` - backend architecture notes for judges
- `vercel.json` - static Vercel deployment config

## Snapshot

The dashboard is powered by a generated static snapshot at `public/data.json`.
The latest included snapshot was generated on `2026-05-30T20:10:27Z` for the
Jack Roberts creator profile.
The YouTube outliers feed in that snapshot was refreshed on
`2026-05-30T20:58:06Z` and includes Jack-specific content angles, an All Ideas
view, an Adjacent Ideas view, and Jack's 15-channel Competitor Watchlist.

The live backend pipeline is intentionally not included in this judge-facing
repo so the submission stays small and does not expose operational secrets.
See `technical-appendix/` for the backend data flow and scoring summary.

## Deploy

Import this repo into Vercel. The output directory is `public`.
