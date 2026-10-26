# Daily Mind Tracker — Numeric Mental State Edition

Separate new app. Mental State uses ratings 1–5 only; Sato/Rajo/Tamo are not part of this version.

## Files
- `public/index.html` — app interface
- `worker.js` — Cloudflare Worker API
- `schema.sql` — fresh D1 schema
- `wrangler.jsonc.example` — configuration example

## Setup
1. Create a NEW D1 database, e.g. `daily-mind-tracker-seniors-db`. Do not use the old app database.
2. Run `schema.sql` once in the new database's D1 Console.
3. Replace the placeholders in `wrangler.jsonc.example` with the new database name and ID, then save as `wrangler.jsonc`.
4. Deploy with D1 binding `DB` and static assets binding `ASSETS` pointing to `public/`.
5. Open the app and create a new account. Old accounts and check-ins are not carried over.
6. Test registration, login, check-in saves, charts, goals, and password change before sharing.

Passwords must be at least 12 characters.
