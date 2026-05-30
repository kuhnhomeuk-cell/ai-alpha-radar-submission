# Scoring Summary

Each trend card in `public/data.json` combines quantitative signals with
creator-focused enrichment.

## Ranking Signals

- `velocity_score` and `velocity_acceleration` estimate how quickly a topic is
  gaining attention.
- `novelty_score` estimates how new or under-discussed the topic is.
- `saturation` estimates whether the topic is already crowded.
- `hidden_gem_score` highlights topics that look early but promising.
- `convergence` and `sources_confirming` show whether multiple sources are
  pointing at the same pattern.
- `lifecycle_stage` labels the topic's maturity for faster scanning.

## Creator Fields

The latest snapshot is tuned for the Jack Roberts creator profile. Each trend
can include:

- `display_label` - human-readable card title
- `creator_fit` - why this trend fits the creator's audience and style
- `angles.video_title` - suggested YouTube-style title
- `angles.hook` - opening hook
- `angles.tutorial` - practical build angle
- `angles.contrarian` - counter-position or sharper take
- `angles.eli_creator` - creator-friendly explanation

## Frontend Contract

The dashboard expects these top-level fields:

- `snapshot_date`
- `generated_at`
- `meta.creator_profile`
- `trends`
- `briefing`
- `data_freshness_status`
- `youtube_outliers`

The app is resilient to optional fields, but the creator-profile fields above
are what make the latest dashboard polish visible.
