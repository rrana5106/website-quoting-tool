# Scope — project cost estimator

A single-file, client-side quoting tool for web design and development studios. Set the shape of a project — type, page count, design tier, features, timeline, revisions, maintenance — and the ledger panel totals it live, as a range rather than a fake-precise number.

**Live demo:** [website-quoting-tool.vercel.app](https://website-quoting-tool.vercel.app/)

## Features

- Live-updating itemised quote as you adjust inputs
- Estimated delivery time in weeks
- Quote number and date, auto-generated
- Copy the summary to clipboard, or print straight to PDF
- Figures in GBP (£)
- No build step, no dependencies, no backend — one HTML file

## Running locally

Just open `index.html` in a browser. There's nothing to install or build.

## Customising

All pricing lives in plain JS objects near the top of the `<script>` block in `index.html`:

- `PROJECT_TYPES` — base price, base timeline, and included page count per project type
- `TIERS` — design-tier cost multipliers
- `FEATURES` — flat-fee add-ons
- `TIMELINES` — rush-delivery multipliers
- `REVISIONS` / `MAINTENANCE` — revision-round and maintenance-plan pricing

Edit the numbers to match your own studio's rates, then redeploy.

## Deploying

This is a static file, so it deploys anywhere that serves static HTML — Vercel, Netlify, GitHub Pages, or a plain web server. No build command or environment variables are required.

## License

MIT — use, adapt, and resell estimates freely.
