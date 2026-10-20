# Pizza Shop Enterprise — CPSC 201 MIS Lab

A static, browser-based pizza restaurant enterprise simulation with a left navigation sidebar and IndexedDB persistence.

## Deploy to GitHub Pages

1. Create a public GitHub repository, e.g. `pizza-shop-enterprise`.
2. Upload `index.html`, `styles.css`, and `app.js` to the **root** of the repository.
3. In **Settings → Pages**, choose **Deploy from a branch**.
4. Choose branch **main**, folder **/(root)**, and Save.
5. Open `https://YOUR-USERNAME.github.io/pizza-shop-enterprise/` after deployment.

## Included modules

Dashboard, Order Management, Kitchen Operations, Inventory & SCM, CRM & Service, Procurement, simulated EDI, Delivery, Executive Analytics, Decision Support, Data Explorer, and Simulation Controls.

## Suggested end-to-end test

Create an order → start preparation → finish preparation → approve quality → complete pickup or dispatch/deliver → inspect analytics. Create a purchase order → acknowledge → receive goods → verify inventory increases. Refresh to verify persistence. Export JSON, reset, and import backup.

## Data and security

Data is stored locally in IndexedDB on the student's device, not on GitHub. Each browser profile has independent data. Clearing site data can erase progress, so export JSON backups regularly. Do not enter real personal or payment data. There is no user authentication or central instructor reporting. EDI and payments are simulations.

## Scope

This is a first functional prototype, not a production POS or accounting system. It stores the full enterprise state in one IndexedDB object store. Advanced workflows, tax handling, refund accounting, real EDI validation, multi-device sync, and student assessment audit controls are not implemented.
