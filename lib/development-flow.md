# Development Workflow

## Checklist

- [ ] **Use yarn** when language is js (npm prohibited)

## Before Development

- Separate tasks with easily recognizable goals

## During Development

- **Beware of temporary code**: Remove debugging temporary code without fail
- Remove legacy code: Delete unused code immediately
- Keep structure clean
- Write comments for complex logic
- Follow [code style guide](./code-style.md)

## After Development

- [ ] **corepack yarn tsc** (TypeScript check)
- [ ] **corepack yarn lint** (ESLint check)
- [ ] Commit after smoke test confirmation
- [ ] List uncertainties
