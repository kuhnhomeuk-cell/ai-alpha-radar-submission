# AI Alpha Radar

AI Alpha Radar is an early-warning dashboard for AI operators and creators who
want to spot useful AI trends before they become obvious. Instead of showing
generic news, it turns public signal sources into creator-ready opportunities:
what is moving, why it matters, how crowded it is, and what angle a creator can
turn into a video, tutorial, or product idea.

## Live Demo

- Landing page: <https://ai-alpha-radar-submission.vercel.app/>
- Dashboard: <https://ai-alpha-radar-submission.vercel.app/dashboard>

## What The Dashboard Is For

The product is built around one question: "What should a creator or operator
pay attention to before the market gets crowded?"

The dashboard helps with that by:

- Ranking AI topics by momentum, opportunity, lifecycle stage, and source
  confidence.
- Separating early first-mover signals from broader demand centers and YouTube
  breakout ideas.
- Showing creator-focused hooks, contrarian takes, tutorial angles, and dated
  predictions for accountability.
- Surfacing Jack Roberts-specific competitor and adjacent-channel signals so
  the recommendations are grounded in a real creator niche.

## Dashboard Sections

- `Radar` - the main opportunity map and ranked signal list.
- `First-Mover Signals` - early, less-crowded topics with creator upside.
- `Demand Centers` - unanswered audience questions and problem clusters.
- `Story Log` - predictions the system has filed and is tracking over time.
- `Briefings` - copy-ready hooks, contrarian angles, and tutorial ideas.
- `Outliers` - YouTube videos outperforming their channel baseline, with All
  Ideas and Adjacent Ideas tabs plus a competitor watchlist.

## Latest Snapshot

The deployed dashboard is powered by a generated static snapshot at
`public/data.json`.

- Snapshot date: `2026-05-31`
- Generated at: `2026-05-31T08:51:47Z`
- Creator profile: `Jack Roberts`
- Trend cards: `24`
- Demand centers: `6`
- YouTube outliers: `30`
- Competitor watchlist: `15` channels
- YouTube outliers refreshed at: `2026-05-30T20:58:06Z`

The live backend pipeline is intentionally not included in this judge-facing
repo so the submission stays small and does not expose operational secrets.
The included static snapshot lets judges use the final product exactly as it is
deployed.

## What Is Included

- `public/index.html` - landing page
- `public/dashboard.html` - dashboard app
- `public/data.json` - generated dashboard snapshot
- `public/tokens.css` - shared design tokens
- `public/bg-pingpong.mp4` - landing-page background video
- `public/cloud-light.mp3` - landing-page ambient audio
- `public/og-image.png` - social preview image
- `technical-appendix/` - backend architecture and scoring notes
- `vercel.json` - static Vercel deployment config

## Technical Appendix

The backend notes live in `technical-appendix/`:

- `data-flow.md` explains how raw public signals become the static dashboard
  snapshot.
- `scoring-summary.md` explains how ranking, lifecycle, opportunity, and
  creator-fit fields are produced.

## Deploy

Import this repo into Vercel. The output directory is `public`.
