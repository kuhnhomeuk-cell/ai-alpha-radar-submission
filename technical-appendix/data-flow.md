# Backend Data Flow

AI Alpha Radar uses a scheduled backend pipeline to convert public AI-market
signals into a static JSON snapshot for the dashboard.

## Flow

1. Fetch public signals from multiple sources such as AI news, developer
   communities, research feeds, GitHub activity, and video outliers.
2. Normalize each source into comparable documents with source names, URLs,
   timestamps, engagement signals, and extracted topic text.
3. Cluster related documents into trend candidates.
4. Score each trend for velocity, novelty, saturation, convergence, hidden-gem
   potential, and creator fit.
5. Enrich each trend into dashboard-ready copy: summary, why-now explanation,
   risks, top questions, creator angle, and video title.
6. Write the final snapshot to `public/data.json`.
7. The frontend reads that static JSON file directly, so the deployed demo does
   not need backend credentials at runtime.

## Runtime Shape

The deployed app is intentionally static:

- `public/index.html` renders the landing page.
- `public/dashboard.html` renders the dashboard.
- `public/data.json` contains all dashboard data.
- `public/tokens.css` contains shared visual tokens.

This means judges can open the app without a database connection, queue worker,
or private API key.
