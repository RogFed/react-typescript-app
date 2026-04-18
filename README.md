# react-typescript-app

A minimal React + TypeScript starter built with Rsbuild — fast builds, strict linting, and testing out of the box.

## Tech Stack

- **React** 19 — UI component library
- **TypeScript** 6 — static typing
- **Rsbuild** — build tool & dev server (powered by Rspack)
- **Biome** — formatter & linter
- **Rstest** — test runner
- **Bun** — package manager & script runner

## Setup

Install the dependencies:

```bash
bun install
```

## Get Started

Start the dev server — the app will be available at [http://localhost:3000](http://localhost:3000):

```bash
bun run dev
```

## Scripts

| Script | Command | Description |
|--------|---------|-------------|
| `dev` | `bun run dev` | Start the dev server |
| `build` | `bun run build` | Build the app for production |
| `preview` | `bun run preview` | Preview the production build locally |
| `test` | `bun run test` | Run tests |
| `test:watch` | `bun run test:watch` | Run tests in watch mode |
| `check` | `bun run check` | Lint and format code (run before committing) |
| `format` | `bun run format` | Format code only |

## Learn More

- [Rsbuild documentation](https://rsbuild.rs) — build config, plugins, and APIs
- [Rspack documentation](https://rspack.rs) — the bundler powering Rsbuild
- [Rstest documentation](https://rstest.rs) — test runner docs
- [Biome documentation](https://biomejs.dev) — formatter & linter config
