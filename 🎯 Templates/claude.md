# CLAUDE.md Template

A reusable project-level `CLAUDE.md` for software engineering repositories.

Copy this file into the root of your project and customize it as needed.

---

# Project Guidelines

You are working in an existing software project.

Prioritize correctness, maintainability, and minimal changes over speed.

---

# Core Principles

- Understand existing code before making changes.
- Reuse existing implementations whenever possible.
- Keep changes focused on the requested task.
- Avoid unnecessary refactoring.
- Follow existing project conventions.
- Verify changes before considering the task complete.

---

# Before Coding

Always:

- Read surrounding files.
- Understand current architecture.
- State assumptions.
- Ask questions if requirements are unclear.
- Explain tradeoffs when multiple solutions exist.

Never invent APIs, project structure, or architecture.

---

# During Implementation

Prefer:

- Small commits
- Minimal diffs
- Existing utilities
- Existing naming conventions
- Existing testing patterns

Avoid:

- Premature optimization
- Duplicate implementations
- Unrelated refactoring
- Formatting-only changes
- Overengineering

---

# Testing

Whenever appropriate:

- Update existing tests.
- Add new tests only when valuable.
- Keep tests deterministic.
- Reuse existing test utilities.
- Verify edge cases.

---

# Communication

Before coding:

- Explain assumptions.
- Mention potential risks.

After coding:

- Summarize changes.
- Explain why they were made.
- Describe verification steps.
- Mention any limitations.

Never claim code has been tested unless it has actually been verified.

---

# Success Criteria

The task is complete only when:

- Requested behavior is implemented.
- Existing functionality is preserved.
- Changes remain minimal.
- Project conventions are followed.
- Relevant tests pass or verification steps are documented.
