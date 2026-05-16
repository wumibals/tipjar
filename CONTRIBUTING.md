# Contributing to TipJar

Thank you for your interest in contributing to TipJar!

## Fork-and-branch workflow

1. Fork the repository on GitHub.
2. Clone your fork locally:
   ```bash
   git clone https://github.com/<your-username>/tipjar.git
   cd tipjar
   ```
3. Create a branch from `main` using the naming conventions below:
   ```bash
   git checkout -b feat/your-feature-name
   ```
4. Make your changes, commit, and push to your fork:
   ```bash
   git push -u origin feat/your-feature-name
   ```
5. Open a pull request against `bellabukss/tipjar:main`.

### Branch naming

| Type | Pattern | Example |
|---|---|---|
| Feature | `feat/<short-description>` | `feat/obs-overlay` |
| Bug fix | `fix/<short-description>` | `fix/memo-truncation` |
| Docs | `docs/<short-description>` | `docs/contributing` |
| Chore | `chore/<short-description>` | `chore/update-deps` |

## Commit message convention

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat(widget): add OBS browser-source overlay mode
fix(server): handle SEP-24 callback with missing memo field
docs(readme): expand development setup section
chore(deps): bump stellar-sdk to v10
```

Format: `type(scope): description`

Common types: `feat`, `fix`, `docs`, `chore`, `test`, `refactor`.

## Running tests locally

### Prerequisites

- Node.js 20+
- pnpm 9+ (`npm install -g pnpm`)

### Install dependencies

```bash
pnpm install
```

### Run all tests

```bash
pnpm test
```

### Run tests for a specific package

```bash
pnpm -F @tipjar/widget test
pnpm -F @tipjar/server test
```

### Lint and type-check

```bash
pnpm -r run lint
pnpm -r run typecheck
```

Both commands must pass before opening a PR — the CI pipeline runs them automatically on every pull request.