# Ev-Link

React and TypeScript web application built with Vite.

## Requirements

- Node.js 24 (see `.nvmrc`)
- npm 11

## Development

```sh
npm ci
npm run dev -- --host 0.0.0.0 --port 5173
```

Edit `src/App.tsx` to start building. Vite reloads the app when files change.

## Validation

```sh
npm run lint
npm run build
```

The build checks TypeScript and creates production files in `dist/`.
To serve that build locally, run `npm run preview -- --host 0.0.0.0 --port 4173`.
No automated test suite has been configured yet.

## Contributing

Create a branch with `git switch -c feature/your-change`, run validation,
and commit related changes with a descriptive message.
Keep credentials out of Git. Local `.env` files are ignored; commit only
placeholder configuration in `.env.example` when needed.

## Cloud environment

The cloud setup installs dependencies with `npm ci`. In restricted workspaces,
use `npm ci --cache /workspace/.npm-cache` to keep the npm cache writable.
Development server processes must be started again in each new task.
