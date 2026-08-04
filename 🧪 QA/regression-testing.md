# Regression Testing Playbook

Guidelines for using AI to plan, prioritize, execute, and analyze regression testing.

Focus on validating existing functionality affected by recent changes while optimizing testing effort through risk-based prioritization.

---

# Core Principles

- Protect existing functionality.
- Prioritize business-critical workflows.
- Use risk-based regression.
- Reuse existing test assets.
- Avoid redundant testing.
- Balance coverage with execution time.

---

# Regression Testing Workflow

Follow this sequence:

1. Understand the change.
2. Perform impact analysis.
3. Identify affected features.
4. Select regression scenarios.
5. Prioritize execution.
6. Execute regression tests.
7. Investigate failures.
8. Document results.

---

# Understand the Change

Before planning regression:

Review:

- Feature requirements
- Code changes
- Pull Request
- Release notes
- Related defects
- Architecture changes
- API changes
- Database changes

Never begin regression without understanding what changed.

---

# Impact Analysis

Determine whether the change affects:

- Business logic
- UI
- APIs
- Database
- Authentication
- Navigation
- Search
- Performance
- Accessibility
- Integrations

Expand regression scope based on actual impact.

---

# Regression Scope

Always include:

- Happy path
- Core business flows
- Recently modified features
- Related functionality
- High-risk areas
- Previously failed scenarios

Consider excluding:

- Deprecated features
- Unrelated modules
- Experimental functionality

Only if supported by impact analysis.

---

# Prioritization

Execute in this order:

## Critical

- Login
- Checkout
- Payments
- Search
- Authentication
- User account
- Core workflows

## High

- Frequently used features
- Recently modified components
- API integrations

## Medium

- Supporting features
- Reports
- Settings

## Low

- Cosmetic changes
- Rarely used functionality

Risk should determine priority.

---

# Mobile Regression

Android

Validate:

- Different Android versions
- Screen sizes
- Orientation
- Background/foreground
- Notifications

iOS

Validate:

- Device models
- iOS versions
- Dynamic Type
- Dark Mode
- Safe Area

Cross-platform

Verify:

- Feature parity
- Navigation
- UI consistency
- Business behavior

---

# Automation Strategy

Prefer:

- Existing automated regression suites
- Stable UI tests
- API automation
- Smoke suites
- Integration tests

Avoid creating duplicate automation unless necessary.

---

# AI Guidelines

When planning regression:

Always:

- Perform impact analysis.
- Recommend regression scope.
- Prioritize based on risk.
- Explain why scenarios were selected.
- Suggest automation opportunities.

Never:

- Recommend testing everything.
- Ignore related features.
- Skip regression because a fix appears small.

---

# Failure Analysis

If regression fails:

Investigate:

1. Product defect
2. Regression defect
3. Test data
4. Environment
5. Automation issue
6. Configuration issue

Document findings before proceeding.

---

# Regression Report

Include:

- Build version
- Features covered
- Scenarios executed
- Passed
- Failed
- Blocked
- Defects found
- Risks
- Recommendations

---

# Success Criteria

Regression testing is complete only when:

- Impacted functionality has been validated.
- Business-critical workflows pass.
- Regression scope is risk-based.
- Failures are investigated.
- Results are documented.
- Release risks are clearly communicated.
