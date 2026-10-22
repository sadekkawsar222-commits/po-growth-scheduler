# Po Growth Engine scheduler

Calls `https://po-growth-engine.vercel.app/api/cron` every 5 minutes so follow-ups, reminders and chasers run even when nobody has the workspace open. The engine only acts when **Automation on** is set in the app.

The endpoint is protected: the call uses the `CRON_SECRET` repository secret, which must match `CRON_SECRET` on the Vercel project.

GitHub may start scheduled runs a few minutes late during busy periods. Run it by hand from the Actions tab with **Run workflow**.

© PO AI. All rights reserved.
