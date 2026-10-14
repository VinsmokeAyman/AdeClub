# Frontend NERA

React frontend connected to the Express API. See `../TUTORIAL.md` for full installation and operation instructions.

```powershell
npm ci
npm run dev
```

Start the API separately from `../Express/backend`. Vite proxies `/api` to `http://127.0.0.1:3000`.

- `/` : public planning and club access.
- `/admin` : protected admin workflows, with ADE-only club password management and database viewer.
- `src/api.js` : JSON API client and CSRF handling.
- `src/usePortal.js` : session/reservation refresh.
- `src/Catalog.jsx` and `src/useCatalog.js` : catalog loaded from the database.
- `src/data.js` : date helpers only; no credentials or demo reservations.
- `src/reservations.js` : display helpers only; authorization lives on the server.

`npm run build`, `npm run lint`, and `npm test` verify the frontend. Workflow and authorization integration tests live in the backend.
"# AdeClub" 
