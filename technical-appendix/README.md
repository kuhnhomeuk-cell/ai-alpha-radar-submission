# Technical Appendix

This repository is the slim judge-facing product demo. It includes the landing
page, dashboard, and one generated data snapshot.

The backend pipeline runs separately and publishes its output as
`public/data.json`. That keeps this submission easy to deploy while still
showing the final product exactly as judges will use it.

## Included Notes

- `data-flow.md` - how the backend turns raw signals into the static dashboard
  snapshot
- `scoring-summary.md` - how trend ranking and creator-fit fields are produced

## Latest Snapshot

- Snapshot date: `2026-05-31`
- Generated at: `2026-05-31T08:51:47Z`
- Trend cards: `24`
- YouTube outliers refreshed at: `2026-05-30T20:58:06Z`
- YouTube outliers: `30` total ideas, including `22` adjacent ideas and `8`
  general ideas
- Competitor watchlist: `15` channels, with `0` exact hits in this snapshot
- Creator profile: `Jack Roberts`

## What Is Not Included

- API keys or service credentials
- Local `.env` files
- Raw fetch caches
- Development scratch files
- Backend source code that is not needed to run the judge demo
