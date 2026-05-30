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

- Snapshot date: `2026-05-30`
- Generated at: `2026-05-30T20:10:27Z`
- Trend cards: `21`
- YouTube outliers refreshed at: `2026-05-30T20:37:38Z`
- YouTube outliers: `30`, including Jack-specific content angles and
  competitor-channel labels
- Creator profile: `Jack Roberts`

## What Is Not Included

- API keys or service credentials
- Local `.env` files
- Raw fetch caches
- Development scratch files
- Backend source code that is not needed to run the judge demo
