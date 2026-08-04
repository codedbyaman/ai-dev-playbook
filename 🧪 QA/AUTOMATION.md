# Automation Testing Playbook

Guidelines for using AI to design, write, review, debug, and maintain automated tests.

Prioritize reliable, maintainable, and readable automation over simply increasing test coverage.

---

# Core Principles

- Automate stable behavior, not unstable UI.
- Prefer maintainability over clever implementations.
- Follow existing project architecture.
- Reuse existing utilities before creating new ones.
- Keep tests deterministic and independent.
- Avoid flaky automation.

---

# Before Writing Tests

Understand the feature before automating it.

Review:

- Functional requirements
- Acceptance criteria
- Existing automation
- Framework architecture
- Test utilities
- Mocking strategy
- Test data
- Known limitations

Never automate a feature you don't fully understand.

---

# Test Selection

Prioritize automating:

- Critical user journeys
- Frequently executed scenarios
- Stable functionality
- Regression-prone areas
- Business-critical workflows

Avoid automating:

- Frequently changing UI
- Experimental features
- One-time validation
- Unstable flows without proper synchronization

---

# Test Design

Every automated test should be:

- Independent
- Repeatable
- Easy to understand
- Easy to maintain
- Easy to debug

Prefer:

- One responsibility per test
- Clear assertions
- Small reusable helpers
- Existing page objects
- Existing utilities

Avoid:

- Large end-to-end tests
- Duplicate setup
- Nested logic
- Multiple unrelated assertions
- Shared state between tests

---

# Test Structure

A good test should clearly separate:

1. Setup
2. Action
3. Verification
4. Cleanup (if required)

Keep each section easy to identify.

---

# Locators

Prefer:

- Accessibility identifiers
- Resource IDs
- Stable test IDs
- Existing locator helpers

Avoid:

- XPath whenever possible
- Index-based locators
- Dynamic text
- Hardcoded coordinates

Stable locators create stable tests.

---

# Synchronization

Prefer:

- Explicit waits
- Existing wait utilities
- Expected conditions
- Framework synchronization

Avoid:

- Thread.sleep()
- Fixed delays
- Arbitrary waits

Tests should wait for application state, not elapsed time.

---

# Assertions

Assertions should verify behavior, not implementation.

Good assertions:

- Validate user-visible results
- Verify expected state
- Confirm business logic

Avoid excessive assertions in a single test.

---

# Test Data

Prefer:

- Reusable test data
- Independent datasets
- Deterministic inputs
- Mocked data when appropriate

Avoid dependencies between tests.

---

# Mobile Automation

Android

- Prefer Espresso synchronization.
- Use existing architecture.
- Reuse shared utilities.

iOS

- Prefer accessibility identifiers.
- Follow existing XCTest patterns.
- Keep tests platform consistent.

Cross-platform

- Reuse business logic.
- Minimize platform-specific duplication.
- Keep assertions consistent.

---

# API Automation

When validating APIs:

- Verify status codes.
- Validate response schema.
- Check required fields.
- Test negative scenarios.
- Verify error handling.
- Validate edge cases.

---

# Code Review Checklist

Before approving automation:

- Is the test readable?
- Is the locator stable?
- Can setup be reused?
- Are assertions meaningful?
- Is synchronization reliable?
- Is the test deterministic?
- Does it follow project conventions?

---

# Debugging Failed Tests

Investigate in this order:

1. Application issue
2. Environment issue
3. Test data
4. Synchronization
5. Locator changes
6. Timing issues
7. Framework issue

Avoid assuming the automation is at fault without evidence.

---

# Communication

When generating automation:

Explain:

- Why this approach was chosen.
- Which existing utilities were reused.
- Potential flakiness risks.
- Verification strategy.

Never claim a test was executed unless it was actually run.

---

# Success Criteria

Automation is complete only when:

- The correct behavior is validated.
- Tests are deterministic.
- Existing utilities are reused.
- Stable locators are used.
- Synchronization is reliable.
- Assertions verify meaningful behavior.
- Existing tests remain unaffected.
- The implementation is easy to maintain.
