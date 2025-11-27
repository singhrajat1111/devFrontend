# Celestial Pulse — Converted to JavaScript (Vite)

This project was converted from a TypeScript/TSX codebase to plain JavaScript (.js/.jsx) on a best-effort basis.

What I changed:
- Converted `.ts` -> `.js` and `.tsx` -> `.jsx` files (removed TypeScript types and interfaces where possible).
- Removed TypeScript config files (`tsconfig.json`, `*.d.ts`) when found.
- Updated `package.json` to use Vite (`vite` in devDependencies) and added scripts: `dev`, `build`, `preview`.
- Created a basic `index.html` if none existed, pointing to `src/main.jsx` or the detected entry point.
- Did not add PropTypes by default.

How to run:
1. `npm install`
2. `npm run dev`
(If you prefer yarn: `yarn` then `yarn dev`)

Notes & remaining issues:
- Files that may still contain TypeScript-like patterns (interfaces, type annotations, casts) were detected — you should review these manually and fix any runtime issues. A list is below.

Files with possible leftover TypeScript markers:
- src/App.jsx
- src/components/pages/BookingPage.jsx
- src/components/ui/carousel.jsx
- src/components/ui/chart.jsx
- src/components/ui/form.jsx
- src/components/ui/utils.js