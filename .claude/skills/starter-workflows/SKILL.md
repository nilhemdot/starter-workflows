```markdown
# starter-workflows Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill provides guidance on the development patterns and conventions used in the `starter-workflows` TypeScript repository. It covers file organization, code style, import/export patterns, and testing approaches. This skill is ideal for developers looking to contribute to or maintain codebases with similar patterns.

## Coding Conventions

### File Naming
- Use **camelCase** for file names.
  - Example: `myWorkflow.ts`, `helperFunctions.ts`

### Import Style
- Use **relative imports** for internal modules.
  ```typescript
  import { myFunction } from './utils';
  ```

### Export Style
- Use **named exports** instead of default exports.
  ```typescript
  // utils.ts
  export function myFunction() { ... }
  
  // usage
  import { myFunction } from './utils';
  ```

### Commit Patterns
- Commits use **freeform messages** with no strict prefixing.
- Average commit message length: ~63 characters.

## Workflows

_No explicit workflows were detected in this repository._

## Testing Patterns

- **Testing Framework:** Unknown (not detected)
- **Test File Pattern:** Files with `.test.` in the filename.
  - Example: `myFunction.test.ts`
- **Test Example:**
  ```typescript
  // myFunction.test.ts
  import { myFunction } from './myFunction';

  test('should return true for valid input', () => {
    expect(myFunction('valid')).toBe(true);
  });
  ```

## Commands
| Command | Purpose |
|---------|---------|
| /test   | Run all test files matching *.test.* |
| /lint   | Run linter on the codebase (if configured) |
| /build  | Compile TypeScript sources (if applicable) |
```