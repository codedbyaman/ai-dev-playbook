# CLAUDE.md

Behavioral guidelines for working in this repository.

Prioritize correctness, minimal changes, and consistency with the existing codebase over speed or creativity.

---

# Core Principles

- Prefer correctness over speed.
- Understand the existing implementation before writing code.
- Ask questions instead of making assumptions.
- Keep changes as small as possible.
- Reuse existing code before introducing new code.
- Verify work before declaring it complete.

---

# 1. Think Before Coding

Before making changes:

- Read the surrounding code and understand existing patterns.
- State any assumptions explicitly.
- If requirements are ambiguous, ask clarifying questions.
- If multiple approaches are possible, explain the tradeoffs instead of silently choosing one.
- If a simpler implementation exists, recommend it.

Never invent APIs, utilities, project structure, or architecture.

---

# 2. Simplicity First

Write the minimum code necessary.

Do not:

- Add features that weren't requested.
- Introduce abstractions for one-time use.
- Add configurability unless requested.
- Optimize prematurely.
- Handle impossible scenarios.
- Rewrite working code without reason.

If the solution feels over-engineered, simplify it.

---

# 3. Respect Existing Code

Before creating anything new:

- Search for an existing implementation.
- Reuse existing helpers and utilities.
- Follow existing architecture.
- Match existing naming conventions.
- Match formatting already used in the file.

Do not:

- Refactor unrelated code.
- Rename unrelated variables.
- Reorganize files.
- Reformat large sections.
- Introduce new architectural patterns without justification.

Only remove code made obsolete by your own changes.

If you notice unrelated issues, mention them instead of fixing them.

Every changed line should directly support the requested task.

---

# 4. Goal-Driven Execution

For non-trivial tasks:

1. Explain the plan.
2. Define success criteria.
3. Implement the smallest possible change.
4. Verify the result.
5. Summarize what changed.

When fixing bugs:

1. Explain the root cause.
2. Reproduce the issue if possible.
3. Fix only the actual cause.
4. Verify the fix.
5. Check for regressions.

---

# 5. Testing

Whenever appropriate:

- Update existing tests instead of creating duplicates.
- Write new tests only when they add value.
- Keep tests deterministic.
- Avoid unnecessary mocks.
- Reuse existing test helpers.
- Follow existing testing patterns.

Never break existing tests unnecessarily.

---

# 6. Mobile Development

Respect platform conventions.

Android

- Prefer existing Kotlin utilities.
- Use existing architecture.
- Avoid unnecessary coroutine changes.
- Avoid Thread.sleep when synchronization utilities exist.

iOS

- Follow existing Swift style.
- Respect existing UIKit/SwiftUI architecture.
- Avoid changing lifecycle behavior unless necessary.

UI Automation

- Prefer accessibility identifiers.
- Prefer stable selectors.
- Avoid brittle XPath-like approaches.
- Avoid arbitrary waits.
- Use existing wait utilities.

---

# 7. Communication

Before coding:

- Explain assumptions.
- Mention risks if applicable.

After coding:

- Summarize changes.
- Explain why they were necessary.
- Mention any limitations.
- Explain how the solution was verified.

Do not claim code was tested if it was not.

---

# 8. Success Criteria

The task is complete only when:

- Requested behavior is implemented.
- Existing behavior is preserved.
- Changes are minimal.
- Relevant tests pass or verification steps are documented.
- No unnecessary files were modified.
- No unnecessary code was introduced.
- No unused imports or dead code remain because of the change.
