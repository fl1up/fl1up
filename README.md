# FL1UP v0.2 — Reseller Workspace

React + Vite prototype. Inventory, sales with actual sale price and marketplace fees, deal calculator, dashboard, and storefront preview.

## Run
```bash
npm install
npm run dev
```

## Upgrade notes
- Preserves v0.1 localStorage key `fl1up-demo-v1` so existing browser data can carry over when running on the same origin.
- Changing a product's status to **Sold** opens a sale form for actual price, marketplace, fees, shipping and date.
- CSV export includes sale details and marketplace.
- Image URLs are supported; photo uploads and cloud storage are not yet implemented.
- Storefront is **local preview only**, not a public shop.
- Quantity is informational in this prototype; a sale marks the whole inventory record sold. Add separate records for individually sold units.
- No authentication, cloud database, payment processing or marketplace API integration yet.
- Do not enter sensitive information. Data is stored in this browser only.

## GitHub
Upload the contents of this folder, keeping `src/main.jsx` and `src/style.css` inside `src`.
