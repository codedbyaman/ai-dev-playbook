# Root Cause Analysis (RCA) Playbook

Guidelines for using AI to identify, analyze, and document the underlying cause of software defects.

Focus on understanding *why* a problem occurred rather than simply fixing its symptoms.

---

# Core Principles

- Investigate facts before forming conclusions.
- Differentiate symptoms from root causes.
- Support findings with evidence.
- Consider people, process, and technology.
- Recommend preventive actions, not just fixes.
- Avoid assumptions without verification.

---

# RCA Workflow

Follow this sequence:

1. Understand the reported issue.
2. Collect all available evidence.
3. Reproduce the issue.
4. Identify contributing factors.
5. Determine the root cause.
6. Recommend corrective actions.
7. Recommend preventive actions.
8. Identify regression areas.

---

# Understand the Problem

Review:

- Bug description
- Expected behavior
- Actual behavior
- Environment
- Build version
- Device / Browser
- User impact
- Severity

Clearly distinguish between:

- Symptom
- Failure
- Root Cause

---

# Evidence Collection

Gather:

- Application logs
- Crash logs
- Stack traces
- API requests and responses
- Network traffic
- Analytics
- Screenshots
- Screen recordings

Use evidence to validate every conclusion.

---

# Root Cause Categories

Consider whether the issue was caused by:

## Product

- Incorrect requirements
- Missing requirements
- Ambiguous requirements

## Development

- Logic error
- Incorrect implementation
- Null handling
- State management
- Concurrency
- Memory issues

## Backend

- API failure
- Data inconsistency
- Configuration issue
- Database problem

## Testing

- Missing test case
- Weak regression coverage
- Incomplete automation
- Insufficient edge case validation

## Process

- Communication gap
- Missing review
- Incomplete acceptance criteria
- Deployment issue

---

# Ask "Why?" Repeatedly

Use the Five Whys technique.

Example:

Issue

↓

Why did it happen?

↓

Why did that happen?

↓

Why was that possible?

↓

Why wasn't it detected?

↓

What process should prevent it?

---

# Corrective Actions

Recommend:

- Code changes
- Test improvements
- Better validation
- Documentation updates
- Monitoring improvements

Keep recommendations practical.

---

# Preventive Actions

Suggest improvements such as:

- New automated tests
- Better code reviews
- Stronger acceptance criteria
- Improved logging
- Better monitoring
- Static analysis
- CI/CD validation

The goal is preventing similar defects.

---

# Regression Scope

Recommend validating:

- Related features
- Similar workflows
- Platform-specific scenarios
- Edge cases
- Existing automation
- API compatibility

---

# AI Guidelines

When performing RCA:

Always:

- Explain your reasoning.
- Reference supporting evidence.
- Identify assumptions.
- Separate confirmed findings from hypotheses.

Never:

- Guess the cause.
- Blame individuals.
- Recommend major changes without evidence.

---

# RCA Report Template

Include:

- Problem Summary
- Root Cause
- Supporting Evidence
- Impact
- Corrective Action
- Preventive Action
- Regression Scope
- Lessons Learned

---

# Success Criteria

A Root Cause Analysis is complete only when:

- The true underlying cause is identified or narrowed down.
- Evidence supports the findings.
- Corrective actions are defined.
- Preventive actions are recommended.
- Regression risks are identified.
- Lessons learned are documented.
