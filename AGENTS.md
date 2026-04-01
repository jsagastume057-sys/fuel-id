# AGENTS.md

## Cursor Cloud specific instructions

This repository contains a Next.js website for **FuelID Lunch Delivery** — a farm-fresh school lunch delivery pilot program landing page.

### Project layout
- All website code lives in `test-cursor-fuelid-website-development-076d/`
- Stack: Next.js 16 (App Router), TypeScript, Tailwind CSS v4, localStorage (no backend/auth)

### Common commands
Run from `test-cursor-fuelid-website-development-076d/`:
- `npm run dev` — start dev server on port 3000
- `npm run build` — production build
- `npm run lint` — ESLint
- No automated test suite exists yet

### Non-obvious notes
- The project uses `package-lock.json` (npm), not pnpm or yarn.
- External images (Unsplash, momables.com) are allowed via `next.config.ts` `remotePatterns`.
- The app is purely client-side — no database, no API routes, no authentication. State is stored in `localStorage`.
- The `components/AppShell.tsx` "Baseline" planner app is imported but not currently rendered from the main `app/page.tsx` landing page; `page.tsx` renders the FuelID landing page directly.
