# Pizza Shop Enterprise — CPSC 201

Static GitHub Pages application. Autumn palette retained from the approved prototype. 5 business functions, 15 roles, 40 business processes, role-filtered sidebar, Enterprise View, IndexedDB storage, embedded Data Flow / Database / Data Quality / Analytics tabs, JSON export/import and reset.

## Publish to the SAME GitHub Pages URL

1. Open the GitHub repository that currently hosts the Pizza Shop simulation. **Do not create a new repository** if you want to keep the same URL.
2. Download and extract the ZIP on your computer. Upload the **contents of the extracted folder** (`index.html`, `styles.css`, `app.js`, `README.md`) to the repository's published folder. Usually this is the repository root of the `main` branch; some repositories use `/docs` or a `gh-pages` branch.
3. On GitHub, select **Add file → Upload files**, drag the files, choose **Commit changes**. When GitHub asks whether to replace existing files, use the repository editing workflow (or Git locally) to overwrite the existing versions; ensure the old `index.html` is replaced. If old files conflict, delete them in the same update as appropriate.
4. Verify **Settings → Pages → Build and deployment** still points to the same branch and folder. Do not change the repository name, custom domain or Pages source.
5. Wait for the Pages deployment to complete under **Actions** or **Settings → Pages**, then open the existing URL and hard-refresh (Ctrl+Shift+R).

**Important:** Browser IndexedDB data is origin-scoped. Keeping the same Pages URL preserves the origin, but the new app uses a new database (`cpsc201_pizza_enterprise_v2`) and **does not automatically migrate data from the old version**. Back up the old version before replacing it. Data on different devices/browsers is not synchronized.

## Notes and limitations

- All 40 processes have interactive forms and save operational records or documented managerial/executive decisions; they are educational simulations, not production ERP functions.
- Ingredient consumption happens when a submitted order is prepared, not when it is placed. Payment must match order total and cannot be duplicated. Purchase receiving updates inventory; supplier EDI messages and acknowledgments are **local educational simulations**, not real supplier connectivity.
- Reports and scenarios use simple calculations; no external AI or trained ML model is provided. Cash-based profitability figures are simplified and not full accrual accounting.
- Only one pizza type per order is supported in this release. Delivery records can be marked completed; pickup orders remain Ready. Partial receipt tracking is limited: a partially received purchase cannot be received again through the same purchase order in this release.
- Records persist in browser-local IndexedDB. Export JSON before clearing browser storage, using private browsing, or resetting the simulation.
- Role filtering is a learning interface, **not a security boundary**. Enterprise View lets learners inspect all processes.
- Browser tests are recommended before class distribution. The application does not have automated end-to-end test coverage or server-side concurrency control.
