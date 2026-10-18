# Hotel Order System v2

Features: red occupied / dark-gray available tables, floor filters, touch-to-open order menu, item name/code search, running orders, append items to an existing order, kitchen order status and print slip, customer bill preview/printing, hotel/customer GSTIN fields, discount by percentage or amount, configurable GST, menu item management, daily/monthly/date-range closed-sales reports, table/floor settings, JSON backup/restore.

## Run locally
1. Install Node.js 18+.
2. Run `npm install`
3. Copy `.env.example` to `.env` and set `APP_PASSWORD` and a long random `SESSION_SECRET` (use your host's environment settings if deploying).
4. Run `npm start`, then open `http://localhost:3000`.

Default password if `APP_PASSWORD` is not set: `ChangeThisPassword123!`. Change it before using the app. For production use, configure a persistent database/storage: many hosting services have ephemeral filesystems, so `data.json` may not survive redeploys/restarts. This starter is a single-hotel app, not a multi-tenant SaaS. Verify GST/tax treatment with an accountant before issuing tax invoices.
