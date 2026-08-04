# CURSOR.md

Behavioral guidelines for working with Cursor on software engineering tasks.

Prioritize focused edits, maintainable code, and seamless integration with the existing codebase.

---

# Core Principles

- Understand the surrounding code before making changes.
- Keep edits as small and reviewable as possible.
- Follow existing project conventions.
- Reuse existing implementations before creating new ones.
- Verify changes before considering the task complete.

---

# 1. Work Incrementally

When modifying code:

- Make one logical change at a time.
- Avoid unrelated modifications.
- Keep diffs small and easy to review.
- Preserve existing formatting and style.
- Respect project architecture.

Never rewrite large sections of working code without a clear reason.

---

# 2. Context Awareness

Before implementing:

- Read nearby files and related code.
- Understand dependencies.
- Follow existing naming conventions.
- Reuse utilities, helpers, and shared components.
- Match the project's coding patterns.

Never invent project structure or APIs.

---

# 3. Code Generation

Generate code that is:

- Clean
- Readable
- Maintainable
- Consistent with the existing project

Avoid:

- Overengineering
- Duplicate implementations
- Unnecessary abstractions
- Premature optimization
- Large-scale refactoring

---

# 4. Refactoring

Only refactor when requested or when necessary to support the requested change.

When refactoring:

- Preserve existing behavior.
- Make incremental improvements.
- Keep commits easy to review.
- Avoid mixing refactoring with feature work.

---

# 5. Testing

Whenever appropriate:

- Update existing tests.
- Add tests only when they provide value.
- Reuse existing test helpers.
- Keep tests deterministic.
- Verify edge cases.

Do not claim tests were executed unless explicitly verified.

---

# 6. Mobile Development

Android

- Follow existing Kotlin architecture.
- Prefer existing utilities.
- Avoid unnecessary coroutine changes.
- Keep UI logic simple.

iOS

- Follow existing Swift and SwiftUI conventions.
- Respect lifecycle behavior.
- Reuse shared components.

UI Automation

- Prefer accessibility identifiers.
- Avoid brittle selectors.
- Use existing synchronization utilities.
- Avoid arbitrary waits.

---

# 7. Communication

Before coding:

- Explain assumptions.
- Mention potential risks.
- Clarify ambiguous requirements.

After coding:

- Summarize changes.
- Explain why they were necessary.
- Describe verification steps.
- Mention any limitations.

---

# Success Criteria

The task is complete only when:

- Requested behavior is implemented.
- Existing behavior is preserved.
- Changes remain minimal.
- Code follows project conventions.
- Relevant verification steps are documented.
- No unnecessary code or files were introduced.
