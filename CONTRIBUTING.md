# Contributing to TipJar

Thank you for your interest in contributing!

## Fork-and-Branch Workflow

1. Fork the repository and clone your fork:
   ```bash
   git clone https://github.com/YOUR_USERNAME/tipjar.git
   cd tipjar
   git remote add upstream https://github.com/bellabukss/tipjar.git
   ```
2. Create a feature branch:
   ```bash
   git checkout -b feat/your-feature
   ```
3. Make changes, commit, and push to your fork, then open a pull request against `main`.

## Commit Message Convention

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <short summary>
```

Common types: `feat`, `fix`, `docs`, `chore`, `refactor`, `test`.

Examples:
- `feat(server): add webhook endpoint`
- `fix(demo): correct balance rounding`
- `docs: update contributing guide`

## Running Tests Locally

```bash
# Install dependencies
pnpm install

# Typecheck all packages
pnpm typecheck

# Lint all packages
pnpm lint

# Run all tests
pnpm test
```
