# GroundedGraph frontend

Next.js (App Router) client for GroundedGraph. It renders graphs with Cytoscape.js, keeps graph and
session state in Zustand stores, and talks to the FastAPI backend through `src/lib/api.ts`.

```bash
cp .env.example .env.local    # set NEXT_PUBLIC_API_BASE_URL to the backend URL
npm install
npm run dev                   # http://localhost:3000
```

| path | contents |
|---|---|
| `src/app/` | pages: landing, dashboard, sign-in, sign-up |
| `src/components/` | `GraphDisplay`, `TextInput`, `AskBox`, `EdgeDetail`, `SideBar`, `Navbar`, auth forms |
| `src/lib/` | `api.ts` (backend client), `types.ts` |
| `src/store/` | `graphStore.ts`, `authStore.ts` |

See the [root README](../README.md) for the full stack, configuration and API reference.
