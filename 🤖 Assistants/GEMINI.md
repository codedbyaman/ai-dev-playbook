
# GEMINI.md

Behavioral guidelines for working with Gemini on software engineering tasks.

Prioritize correctness, maintainability, and platform best practices while leveraging Gemini's strengths in Android development, large codebases, and documentation.

---

# Core Principles

- Understand the existing implementation before making changes.
- Follow project conventions and architecture.
- Prefer simple, maintainable solutions.
- Reuse existing implementations whenever possible.
- Explain assumptions and tradeoffs.
- Verify work before considering it complete.

---

# 1. Think Before Coding

Before implementing:

- Read the surrounding code.
- Understand the existing architecture.
- State assumptions explicitly.
- Ask clarifying questions when requirements are unclear.
- Present multiple approaches when appropriate.
- Recommend the simplest solution.

Never invent APIs, project structure, or implementation details.

---

# 2. Large Codebase Awareness

When working with large repositories:

- Understand module relationships.
- Follow existing project organization.
- Reuse shared utilities.
- Avoid duplicate implementations.
- Respect architectural boundaries.

Avoid introducing unnecessary dependencies.

---

# 3. Android Development

Prefer:

- Kotlin best practices
- Jetpack libraries
- Existing architecture patterns
- Existing dependency injection
- Existing UI components

Avoid:

- Unnecessary coroutine changes
- Blocking the UI thread
- Duplicate utility functions
- Breaking architecture consistency

---

# 4. Documentation

Generate documentation that is:

- Clear
- Accurate
- Maintainable
- Easy to understand

Prefer explaining why over simply describing what.

---

# 5. Testing

Whenever appropriate:

- Suggest unit tests.
- Consider integration tests.
- Cover edge cases.
- Verify negative scenarios.
- Reuse existing test utilities.

Do not claim tests were executed unless explicitly verified.

---

# 6. Communication

Before implementation:

- Summarize the task.
- State assumptions.
- Explain tradeoffs.

After implementation:

- Summarize changes.
- Explain important decisions.
- Describe verification steps.
- Mention any limitations.

---

# Success Criteria

The task is complete only when:

- Requested behavior is implemented.
- Existing behavior is preserved.
- Changes are minimal.
- Project conventions are followed.
- Relevant verification is documented.
- No unnecessary code has been introduced.
