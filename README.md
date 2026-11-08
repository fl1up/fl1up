# FL1UP — Reseller Workspace

A responsive, English-language React/Vite MVP for resellers. Includes inventory management, sales tracking, deal profitability calculator, dashboard and storefront preview.

## Run locally

Requires Node.js 20+.

```bash
npm install
npm run dev
```

Open the URL shown in your terminal (usually http://localhost:5173).

## Build

```bash
npm run build
npm run preview
```

## Publish to GitHub

Create an empty GitHub repository named `fl1up`, then from this folder:

```bash
git init
git add .
git commit -m "Initial FL1UP MVP"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/fl1up.git
git push -u origin main
```

## Deploy

Import the GitHub repository into Vercel. Select Vite (if prompted), build command `npm run build`, output directory `dist`.

## MVP limitations — important

- Data is stored in **localStorage on the current browser only**. Clearing browser data deletes it. No cross-device sync or accounts.
- Sample products are fictional and can be deleted.
- Storefront is a **preview**, not a shareable public website yet.
- Sales are recorded by changing product status to **Sold**; there is no separate order/payment system.
- Profit calculations use entered cost, fees and shipping, and exclude tax, refunds and unrecorded expenses.
- Photos use external URLs; there is no upload/storage backend.
- No marketplace API integrations, payment processing, or multi-tenant isolation yet.
- This is a working front-end prototype, **not production-ready SaaS**. Add authentication, per-user authorization, database, validation and security controls before accepting real customer data.

## Suggested next steps

1. Add Supabase authentication and tables scoped by user ID, with Row Level Security.
2. Add a public storefront route and hosted product images.
3. Add sales records, returns, taxes and CSV import.
4. Test with 5–10 resellers, then add Stripe subscriptions.
5. Verify marketplace API terms before implementing automated discovery.
