# Code Style

## Cognitive Load Minimization Rules

### File Size Limits

- **Single file: Maximum 350 lines**
- Recommended: 200 lines or less
- Split immediately if exceeding 350 lines
- Extract related logic into separate files

**Exceptions:**

- Simple data listings (constants, mock data)
- Type definition-only files
- Cases where splitting would harm readability (rare)

### Function Complexity Limits

- **Single function: Maximum 50 lines**
- Split into subfunctions if exceeding 50 lines
- Express intent clearly through function names
- Extract complex conditions into named variables

### Entity Count Limit Per File

- **Components/Functions/Types: Maximum 5**
- Split into separate files if exceeding 5
- Example: types.ts, utils.ts, hooks.ts, etc.

## Design Principles

### SOC (Separation of Concerns)

- Each component/module should have one clear responsibility
- Separate UI and business logic
- Data fetching/calculation should be done where it's used

### SSOT (Single Source of Truth)

- Identical data should be managed from a single source only
- Do not duplicate calculation logic

## Quality

- Prohibit eslint-disable and ts-ignore comments
- Consult with code reviewer beforehand if unavoidable
- Do not ignore warnings
- React: Avoid overusing useEffect
  - Specify dependency arrays accurately
  - Prevent unnecessary re-renders
- TypeScript: Prohibit any type and weak types
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
