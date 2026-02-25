# Project Guidelines

## Package Manager

Use `pnpm` as the package manager for this project. All npm-related commands should use `pnpm` instead of `npm` or `yarn`.

## Git Operations

Before performing any git or GitHub (`gh`) operations, **read the `atomic-git` skill** first to follow proper atomic commit conventions and best practices.

## Naming Conventions

- **Components**: PascalCase (e.g., `BlogCard.astro`, `Header.tsx`)
- **Variables**: camelCase (e.g., `const postList = []`)
- **Files**: kebab-case (e.g., `blog-post.md`, `main-layout.astro`)

## Code Style

- **No code comments** unless complex logic requires explanation
- Keep code self-documenting through clear variable and function names

## Scripts to Avoid

Do **NOT** run the following scripts:
- `pnpm dev` or any dev-prefixed scripts — assume development server is already running
- `pnpm build` — CI/CD only, do not run locally
