# AGENTS.md

You are an expert in React, TypeScript, JavaScript, Rsbuild, Biome, and web application development. You write maintainable, performant, and accessible code.

## Tech Stack

| Tool | Version | Role |
|------|---------|------|
| React | 19.2.4 | UI component library |
| TypeScript | 6.0.2 | Static typing |
| Rsbuild | 1.7.5 | Build tool & dev server (powered by Rspack) |
| Biome | 2.4.10 | Formatter & linter |
| Rstest | 0.8.4 | Test runner |
| Bun | latest | Package manager & script runner |

## Project Structure

```
├── public/          # Static assets (served as-is)
├── src/             # Application source code
│   ├── index.tsx    # Entry point
│   ├── App.tsx      # Root component
│   └── App.css      # Root component styles
├── tests/           # Test files (.test.tsx)
├── biome.json       # Biome formatter & linter config
├── rsbuild.config.ts  # Rsbuild build config
├── rstest.config.ts   # Rstest config
└── tsconfig.json    # TypeScript config
```

## Commands

- `bun run dev` - Start the dev server
- `bun run build` - Build the app for production
- `bun run preview` - Preview the production build locally

## Docs

- Rsbuild: https://rsbuild.rs/llms.txt
- Rspack: https://rspack.rs/llms.txt
- Rstest: https://rstest.rs/llms.txt

## Tools

### Rstest

- Run `bun run test` to run tests
- Run `bun run test:watch` to run tests in watch mode
- Test files live in `tests/` with a `.test.tsx` suffix
- Import test utilities from `@rstest/core`
- Use `@testing-library/react` for component rendering and queries
- `happy-dom` is configured as the test environment

### Biome

- Run `bun run check` to lint and format your code (run before committing)
- Run `bun run format` to format your code only
- Key style rules enforced via `biome.json`:
  - **Indentation**: spaces
  - **Quotes**: single quotes for JS/TS
  - **Arrow functions**: parentheses only when required
  - **Imports**: automatically organized/sorted
  - **Linter**: Biome recommended rules enabled

## Dependency Management

- Always use exact versions (no `^` or `~`) for both `dependencies` and `devDependencies`.
- Update all dependencies once a month.
