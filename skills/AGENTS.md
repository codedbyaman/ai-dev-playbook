# AGENTS.md

Instructions for AI coding assistants working in this repository. Follow these guidelines unless explicitly instructed otherwise.

Prioritize correctness, maintainability, and minimal, well-scoped changes over speed.

---

# Core Principles

- Understand existing code before making changes.
- Follow existing project conventions.
- Search for existing implementations before creating new ones.
- Reuse existing code whenever possible.
- Keep changes focused on the requested task.
- Prefer simple solutions over complex ones.
- Verify changes before considering the task complete.

---

# Before Coding

Always:

- Read the surrounding code and understand existing patterns.
- Understand the current architecture before making changes.
- State assumptions explicitly.
- Ask clarifying questions when requirements are ambiguous.
- Explain tradeoffs when multiple approaches are reasonable.
- Recommend the simplest solution that satisfies the requirements.

Never:

- Invent APIs.
- Invent project structure.
- Invent architecture.
- Assume behavior without evidence from the codebase.

---

# During Implementation

Prefer:

- Small, focused changes.
- Minimal diffs.
- Existing utilities and helpers.
- Existing naming conventions.
- Existing testing patterns.
- Remove code made obsolete by your changes.
- Consistency with nearby code.

Avoid:

- Premature optimization.
- Duplicate implementations.
- Unnecessary abstractions.
- Unrelated refactoring.
- Formatting-only changes.
- Overengineering.
- Modifying unrelated files.

Every code change should directly support the requested task.

---

# Testing

Whenever appropriate:

- Update existing tests instead of creating duplicates.
- Add new tests only when they provide value.
- Reuse existing test utilities.
- Keep tests deterministic.
- Verify edge cases.
- Avoid introducing flaky tests.
- Do not disable or weaken existing tests to make changes pass.

Never claim code was tested unless it was actually verified.

---

# Communication

Before coding:

- Explain assumptions.
- Mention potential risks.
- Highlight any unclear requirements.

After coding:

- Summarize what changed.
- Explain why the changes were necessary.
- Describe how the solution was verified, or explain why verification was not possible.
- Clearly state what was not verified.
- Mention any limitations or follow-up work.

---

# Success Criteria

The task is complete only when:

- The requested behavior is implemented.
- Existing functionality is preserved.
- Changes remain minimal and focused.
- Documentation or comments are updated when required by the change.
- Project conventions are followed.
- Relevant tests pass or verification steps are documented.
- No unnecessary code was introduced.
- No unused imports or dead code remain because of the change.
