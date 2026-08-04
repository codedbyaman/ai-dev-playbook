# COPILOT.md

Behavioral guidelines for working with GitHub Copilot on software engineering tasks.

Prioritize context-aware code generation, maintainability, and consistency with the existing codebase.

---

# Core Principles

- Use surrounding code as the primary source of context.
- Follow existing project conventions.
- Generate small, focused code suggestions.
- Reuse existing implementations before creating new ones.
- Prefer readability over cleverness.
- Avoid unnecessary complexity.

---

# 1. Context First

Before generating code:

- Analyze nearby files and existing implementations.
- Follow established naming conventions.
- Match the project's architecture and coding style.
- Reuse existing utilities and helper functions.
- Respect module boundaries.

Never invent APIs or project structure.

---

# 2. Code Completion

Generate code that is:

- Small and focused
- Easy to understand
- Consistent with surrounding code
- Easy to review
- Production-ready

Avoid:

- Large rewrites
- Overengineering
- Duplicate logic
- Unnecessary abstractions
- Premature optimization

---

# 3. Existing Code

When modifying code:

- Extend existing implementations whenever possible.
- Preserve current behavior.
- Match formatting and style.
- Avoid unrelated refactoring.
- Remove only code made obsolete by your own changes.

---

# 4. Documentation

Generate documentation that is:

- Concise
- Accurate
- Helpful
- Consistent with existing documentation

Avoid redundant comments that simply repeat the code.

---

# 5. Testing

Whenever appropriate:

- Update existing tests.
- Generate meaningful unit tests.
- Cover common edge cases.
- Reuse existing test utilities.
- Follow existing testing patterns.

Do not claim tests have been executed unless explicitly verified.

---

# 6. Mobile Development

Android

- Follow existing Kotlin conventions.
- Respect project architecture.
- Reuse existing utilities.
- Avoid unnecessary coroutine changes.

iOS

- Follow existing Swift and SwiftUI patterns.
- Respect UIKit and SwiftUI architecture.
- Avoid unnecessary lifecycle changes.

UI Automation

- Prefer accessibility identifiers.
- Avoid brittle selectors.
- Use existing synchronization utilities.
- Avoid arbitrary waits.

---

# 7. Communication

When explanations are requested:

- Explain generated code clearly.
- Mention assumptions.
- Highlight important implementation details.
- Suggest verification steps.
- Identify potential limitations.

---

# Success Criteria

The task is complete only when:

- Generated code integrates cleanly with the existing project.
- Existing behavior is preserved.
- Changes remain minimal.
- Project conventions are followed.
- Relevant verification steps are documented.
- No unnecessary code has been introduced.
