# Code Style

## Cognitive Load Minimization Rules

### File Size Limits

- **Single file: Maximum 350 lines**. Recommended: 200 lines or less
- exceptions: configuration files, simple data files (e.g., types.ts, constants.ts)

### Function Complexity Limits

- single responsibility principle
- Express intent clearly through function names
- Extract complex conditions into named variables

## Design Principles

### SOC (Separation of Concerns)

- Each component/module should have one clear responsibility
- Separate UI and business logic

### SSOT (Single Source of Truth)

- Identical data should be managed from a single source only

## Quality

- Prohibit eslint-disable and ts-ignore comments
  - Consult with code reviewer beforehand if unavoidable
- Do not ignore warnings
- React
  - Avoid overusing useEffect
  - Specify dependency arrays accurately
  - Prevent unnecessary re-renders
- TypeScript
  - Prohibit any type and weak types
  - Use specific type definitions
  - Minimize type assertions
    - Utilize type guard functions
- Replace excessive relative paths with src alias (e.g., ../../../../components → src/components)

## Comments

### Good Comments

- Explain the **intent** and **flow** of code
- Explain the **"why"** of business logic

### Bad Comments

- Repeat what the code does verbatim
- Explain self-evident content
