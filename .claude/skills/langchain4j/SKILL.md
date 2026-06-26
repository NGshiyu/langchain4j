```markdown
# langchain4j Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill provides a comprehensive guide to the development patterns used in the `langchain4j` Java codebase. It covers coding conventions, commit patterns, and testing approaches, equipping contributors with the knowledge to write consistent, maintainable code. While no specific workflows were detected, this guide includes suggested commands and best practices for common development tasks.

## Coding Conventions

### File Naming
- **Convention:** PascalCase  
  Example:  
  ```java
  public class MyServiceClass { ... }
  ```

### Import Style
- **Convention:** Relative imports  
  Example:  
  ```java
  import mypackage.subpackage.MyClass;
  ```

### Export Style
- **Convention:** Named exports (Java public classes and interfaces)  
  Example:  
  ```java
  public class DataProcessor { ... }
  public interface Chainable { ... }
  ```

### Commit Patterns
- **Types:** Mixed (bug fixes, documentation, etc.)
- **Prefixes:**  
  - `fix:` for bug fixes  
  - `docs:` for documentation updates  
- **Average commit message length:** 49 characters  
  Example:  
  ```
  fix: handle null pointer in ChainExecutor
  docs: update README with usage examples
  ```

## Workflows

*No explicit workflows were detected in the repository. Below are suggested workflows for common development tasks.*

### Fixing a Bug
**Trigger:** When you identify and resolve a bug in the codebase  
**Command:** `/fix-bug`

1. Create a new branch for your fix.
2. Make necessary code changes following coding conventions.
3. Write or update tests to cover the fix.
4. Commit with a message prefixed by `fix:`.
5. Open a pull request for review.

### Updating Documentation
**Trigger:** When you improve or add documentation  
**Command:** `/update-docs`

1. Edit or add documentation files.
2. Commit with a message prefixed by `docs:`.
3. Open a pull request for review.

## Testing Patterns

- **Framework:** Unknown (no explicit testing framework detected)
- **Test File Pattern:** `*.test.ts` (suggests some TypeScript tests, possibly for integration or examples)
- **Best Practice:**  
  - Place test files alongside the code they test, using the `.test.ts` suffix.
  - Ensure tests cover both expected and edge case behaviors.
  - Example test file name:  
    ```
    DataProcessor.test.ts
    ```

## Commands

| Command       | Purpose                                  |
|---------------|------------------------------------------|
| /fix-bug      | Standard workflow for fixing a bug       |
| /update-docs  | Standard workflow for updating docs      |
```