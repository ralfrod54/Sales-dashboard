# Sales Command Center (v1)

A personal B2B SaaS sales KPI dashboard: revenue, pipeline health,
win rate, funnel, goals, and a "needs attention" list.

**Status:** v1 prototype. Runs on generated demo data only. No backend,
no real CRM connection.

## Run it
Open `sales-dashboard.html` in a browser. No build step.

## How it's organized
Everything is in `sales-dashboard.html`:
- `CFG`: pipeline-health thresholds, stage probabilities, goals
- `MockDataProvider`: demo data. Replace with a HubSpot or Google
  Sheets provider that returns the same shapes
- `K`: KPI calculation functions (win rate = Won / (Won + Lost))
- `classify()`: pipeline health rules (heuristics, not facts)

## Roadmap
- [ ] Company/account view
- [ ] Settings screen
- [ ] Pipeline, win rate, and proposal trend charts
- [ ] More table filters (owner, value, probability, close date)
- [ ] CSV import / real data provider
- [ ] Tests for KPI functions

## Data
Nothing is stored except your theme preference (in your browser).
