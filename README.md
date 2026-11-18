# Noa Ellsworth

Personal portfolio/site for Noa Ellsworth: a product engineer and site builder showcasing work across software, brand/showreel experiences, and learning resources.

## Tech stack

- [Vite](https://vite.dev/)
- [React](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/)
- [Tailwind CSS](https://tailwindcss.com/) (via `@tailwindcss/vite`)

## Getting started

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS recommended)
- npm

### Install

```bash
npm install
```

### Environment variables

Copy `.env.example` to `.env` and provide values as needed:

```bash
cp .env.example .env
```

| Variable | Description |
| --- | --- |
| `GEMINI_API_KEY` | API key for Gemini-powered features/integrations (if used by your deployment). |
| `APP_URL` | Public/base URL of the app (e.g. for callbacks or self-referential links). |

> In AI Studio deployments, these values may be injected automatically at runtime.

## Available scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the Vite dev server on `http://localhost:3000` (configured with `--host=0.0.0.0`). |
| `npm run build` | Create a production build. |
| `npm run preview` | Preview the production build locally. |
| `npm run lint` | Run TypeScript type-checking (`tsc --noEmit`). |
| `npm run clean` | Remove `dist/` and `server.js` artifacts. |

## Project structure

```text
.
├─ index.html        # Main page and interactive experience
├─ src/
│  ├─ App.tsx        # React app entry component
│  ├─ main.tsx       # Client bootstrap
│  └─ index.css      # Global styles (Tailwind import)
├─ vite.config.ts    # Vite configuration
├─ tsconfig.json     # TypeScript configuration
└─ .env.example      # Example environment variables
```

## Notes

- The dev server runs on port **3000** by default (`npm run dev`).
- A VS Code debug configuration is available in `.vscode/launch.json` for launching Chrome/Edge against `http://localhost:3000`.
