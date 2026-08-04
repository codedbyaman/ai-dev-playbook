# Manual Testing Playbook

Guidelines for using AI to plan, execute, and document effective manual testing.

Focus on validating real user behavior, business requirements, and product quality rather than simply executing predefined steps.

---

# Core Principles

- Understand the feature before testing.
- Validate business requirements.
- Test from the user's perspective.
- Think beyond the happy path.
- Record clear and reproducible observations.
- Report evidence, not assumptions.

---

# Manual Testing Workflow

Follow this sequence:

1. Understand the feature.
2. Review requirements and acceptance criteria.
3. Prepare the test environment.
4. Execute planned test scenarios.
5. Explore related functionality.
6. Record observations.
7. Report defects with evidence.
8. Identify regression areas.

---

# Understand the Feature

Before testing:

- Review business requirements.
- Read acceptance criteria.
- Understand the user journey.
- Review related features.
- Identify feature dependencies.

Never begin testing without understanding what the feature is intended to do.

---

# Test Planning

Plan testing for:

- Happy path
- Negative scenarios
- Edge cases
- Empty states
- Error handling
- Permission scenarios
- Network interruptions
- Device or browser variations

Prioritize scenarios based on business impact and user risk.

---

# Test Execution

During execution:

- Follow the intended user flow.
- Verify each expected result.
- Observe unexpected behavior.
- Compare actual behavior against requirements.
- Capture screenshots or videos when necessary.

Do not assume expected behavior if it is undocumented.

---

# Validation Areas

Verify:

- Functionality
- UI and layout
- Navigation
- Data validation
- Error messages
- Performance
- Accessibility
- Localization
- Device compatibility
- Security considerations

---

# Mobile Testing

Android

- Different screen sizes
- OS versions
- Orientation changes
- Background and foreground behavior
- App lifecycle

iOS

- Different devices
- iOS versions
- Dynamic Type
- Dark Mode
- Safe Area layouts

Cross-platform

- Feature parity
- UI consistency
- Performance consistency

---

# Observations

Document:

- What was tested
- Expected result
- Actual result
- Environment
- Build version
- Device information
- Supporting evidence

Keep observations factual and objective.

---

# Defect Reporting

Include:

- Summary
- Steps to reproduce
- Expected result
- Actual result
- Severity
- Priority
- Screenshots or recordings
- Logs when available

A defect report should allow another person to reproduce the issue without additional explanation.

---

# AI Guidelines

When assisting with manual testing:

Always:

- Suggest additional edge cases.
- Consider related workflows.
- Recommend regression areas.
- Ask clarifying questions when requirements are unclear.
- Organize findings clearly.

Never:

- Assume undocumented functionality.
- Mark a feature as working without validation.
- Skip negative testing.
- Ignore usability concerns.

---

# Review Checklist

Before completing testing:

- Were all acceptance criteria verified?
- Were positive and negative scenarios tested?
- Were edge cases considered?
- Were defects documented with evidence?
- Were regression areas identified?
- Were environment details recorded?

---

# Success Criteria

Manual testing is complete only when:

- All planned scenarios are executed.
- Requirements are validated.
- Defects are documented clearly.
- Supporting evidence is captured.
- Regression risks are identified.
- Test results are reproducible.
