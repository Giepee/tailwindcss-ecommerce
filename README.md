# Tailwind E-commerce Template

CODEX
## Run in Chrome

1. Open a terminal in this project folder.
2. Run `npm start`.
3. Open the URL printed in the terminal (by default, `http://localhost:3000`) in Chrome.
4. Stop the server with `Ctrl+C` when you are done.

The project includes its generated stylesheet at `dist/output.css`, so the storefront can start without rebuilding CSS first. To regenerate the stylesheet after changing Tailwind classes, run `npm run build:css`. To rebuild it automatically while editing, run `npm run dev` in a second terminal.

The Alpine.js scripts load from unpkg, so an internet connection is needed for interactive features. The static pages and generated CSS are served locally.

COPILOT
## Python backend

Run `python Backend/index.py` from the project folder to start the Python server at `http://127.0.0.1:8000`. It serves the storefront pages and exposes a JSON API under `/api`; data is stored in `Backend/store.sqlite3`.

The API includes product listing/details, account registration and login, bearer-token authentication, a persistent cart, and order creation/history. Use the returned token in an `Authorization: Bearer <token>` header for account, cart, and order endpoints. This demo backend records orders but does not process payments. The existing Alpine.js interactions still use browser storage until the frontend is wired to call these API endpoints.
