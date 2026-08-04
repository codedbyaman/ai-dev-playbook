# Bug Investigation Playbook

Guidelines for using AI to investigate, analyze, and document software defects.

Prioritize identifying the root cause over suggesting immediate fixes.

---

# Core Principles

- Understand the reported issue before investigating.
- Reproduce the issue whenever possible.
- Collect evidence before drawing conclusions.
- Validate assumptions with logs, screenshots, or traces.
- Focus on identifying the actual root cause.
- Avoid guessing.

---

# Investigation Workflow

Follow this sequence:

1. Understand the reported issue.
2. Reproduce the problem.
3. Gather evidence.
4. Analyze application behavior.
5. Identify possible causes.
6. Narrow down the root cause.
7. Suggest a fix.
8. Recommend regression testing.

---

# Understand the Issue

Review:

- Bug summary
- Expected behavior
- Actual behavior
- Steps to reproduce
- Environment
- Build version
- Device information
- Severity
- Priority

Do not skip understanding the problem before investigating.

---

# Reproduce the Issue

Attempt to reproduce using:

- Same environment
- Same application version
- Same user flow
- Same test data
- Same device or browser

If the issue cannot be reproduced:

- Identify missing information.
- Request additional evidence.
- Document the findings.

---

# Evidence Collection

Collect as much evidence as possible:

- Screenshots
- Screen recordings
- Logs
- Stack traces
- API responses
- Network traffic
- Console output
- Crash reports

Never rely on assumptions without supporting evidence.

---

# Root Cause Analysis

Investigate potential causes in the following order:

- Incorrect business logic
- UI implementation
- API failure
- Backend issue
- Data inconsistency
- Configuration issue
- Network problem
- Environment issue
- Automation issue

Avoid blaming a specific layer without verification.

---

# Mobile Applications

Android

Review:

- Logcat
- Crash logs
- ANRs
- Device configuration

iOS

Review:

- Xcode logs
- Crash reports
- Console logs
- Device configuration

Cross-platform

Compare behavior across:

- Android
- iOS
- Different OS versions
- Different devices

---

# API Investigation

Verify:

- Request payload
- Response payload
- Status codes
- Headers
- Authentication
- Timeouts
- Error messages

Compare successful and failed responses.

---

# Questions AI Should Ask

When information is missing:

- Can the issue be reproduced consistently?
- Which build was tested?
- Which environment was used?
- Is the issue platform specific?
- Does it affect all users?
- Has this worked previously?
- Are there recent related changes?

---

# Suggesting Fixes

Before proposing a fix:

- Explain the likely root cause.
- Identify impacted components.
- Consider side effects.
- Recommend the smallest possible change.

Avoid suggesting speculative fixes.

---

# Regression Recommendations

After identifying the issue, recommend validating:

- Related features
- Similar workflows
- Edge cases
- Existing automation
- Platform-specific scenarios

---

# Communication

When documenting findings:

Include:

- Root cause
- Supporting evidence
- Impact
- Suggested fix
- Regression scope

Clearly separate confirmed findings from assumptions.

---

# Success Criteria

A bug investigation is complete only when:

- The issue is understood.
- Evidence has been collected.
- The root cause has been identified or narrowed down.
- Supporting data is documented.
- Regression risks are identified.
- Recommendations are actionable.
