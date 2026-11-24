# PROJECT G — Executive Command Center Dashboard

A single-page executive dashboard for PROJECT G (Chiang Khan Sovereign Green Energy & ESG Data Center Hub, Master SOW Resolution Rev 6.0). It shows:

- Key schedule windows and a live countdown to project start
- KPI scorecards (PSF grant, combined financial backing, clean baseload capacity, G-Hall compute)
- Financial ring-fencing, the 4-phase tranche schedule and the collateral breakdown (Chart.js)
- An explorer for the 30 hydro-vortex basins, with filters, search and grid/table views
- The 13-year energy and Clause 16.3 cash-flow waterfall, as a chart and a table
- GCP workloads, governance clauses and an SHA-256 seal ledger you can click to copy
- Loading a codex JSON file (upload or drag-and-drop) with a SHA-256 digest computed in the browser, plus JSON and CSV export

## Technologies

Plain static HTML with Tailwind CSS (CDN), Chart.js (CDN), Google Fonts and the browser's Web Crypto API. There is no build step and no backend. Hosted on Netlify.

## Run locally

Open `public/index.html` in a browser, or run `netlify dev` from the project root.
