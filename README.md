# Depot Simulator

Static simulator suite for depot planning and costing.

## Entry Point

- Main app: `index.html`
- Hub page: `depot_suite.html`

## Included Simulators

- `depot_fitout_v2.html`
- `rail_store_En_Cost_Vref.html`
- `track_vehicles_washing_opex_v2.html`

## Local Run

Open `index.html` or `depot_suite.html` in a browser.

For best browser behavior with iframe messaging and storage, use a local static server when possible.

Example:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

## Deployment

This project is compatible with static hosting on GitHub and Vercel.

### Vercel

- Framework preset: `Other`
- Build command: none
- Output directory: `.`

### Important Note About Saved Projects

Project persistence currently uses browser-side `IndexedDB`.

That means:

- saved projects stay local to the browser/device
- data is not shared automatically between users or machines
- redeploying on Vercel does not erase the deployed files, but user project data remains browser-local

If cross-device/shared project storage is needed later, add a backend or a hosted database.

## Repository Layout

```text
.
├─ index.html
├─ depot_suite.html
├─ depot_fitout_v2.html
├─ rail_store_En_Cost_Vref.html
├─ track_vehicles_washing_opex_v2.html
├─ Archives/
└─ documentation/
```
