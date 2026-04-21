# TS-Dash

Privacy-first, local-first time-series dashboard for CSV-based personal data (weight, calories, steps, etc.).

## What It Does

- Imports CSV data with a guided mapping wizard.
- Visualizes one primary metric with fast zoom/pan and time presets.
- Shows milestone snapshots, insights feed, and visible-range table.
- Supports deterministic analysis (date probe, comparisons, thresholds, recurrence).
- Stores data locally in your browser (IndexedDB).

## How To Use

1. Open the app.
2. Click `+ Import CSV`.
3. Map timestamp + value columns (and optional metric/unit columns).
4. Click `Confirm & Import`.
5. Use graph presets (`1W` ... `ALL`) and hover to inspect values.
6. Use:
   - `Milestone Markers` for quick historical checkpoints.
   - `Insights Feed` for summarized visible-range findings.
   - `Tabular Fallback` for exact raw rows.
7. Expand `Guided Analysis` (collapsed by default) if you want deeper controls.

## Static Hosting (GitHub Pages, dist-only)

If you are uploading only the final `dist` contents:

1. Run build locally:
   - `npm run build`
2. Upload **all files inside `dist/`** to your GitHub Pages publish target.
3. Ensure Pages serves `index.html` at the site root.
4. If you deploy to a subpath (for example `/repo-name/`), set Vite `base` for that path before building.

## Local Dev

- Install: `npm install`
- Run dev server: `npm run dev`
- Build: `npm run build`
- Unit tests: `npm test -- --run`
- E2E tests: `npm run test:e2e`

## Notes

- Browser extension console errors can appear in DevTools and may not be from this app.
- All analytics shown are deterministic, not LLM-generated.
