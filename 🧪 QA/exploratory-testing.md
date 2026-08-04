# Exploratory Testing Playbook

Guidelines for using AI to perform structured exploratory testing.

Focus on discovering unexpected defects, usability issues, hidden risks, and edge cases through intelligent exploration rather than predefined scripts.

---

# Core Principles

- Explore with purpose.
- Follow curiosity backed by evidence.
- Think like different types of users.
- Challenge assumptions.
- Investigate unexpected behavior.
- Document discoveries clearly.

---

# Exploratory Testing Workflow

Follow this sequence:

1. Understand the feature.
2. Identify risk areas.
3. Define an exploration goal.
4. Execute exploratory scenarios.
5. Observe application behavior.
6. Investigate unexpected results.
7. Document findings.
8. Recommend regression areas.

---

# Understand the Feature

Before exploring:

- Review business requirements.
- Understand user workflows.
- Review previous defects.
- Understand feature dependencies.
- Identify high-risk components.

Never explore without understanding the feature's purpose.

---

# Exploration Strategy

Explore using different perspectives:

## User Perspective

- First-time user
- Returning user
- Power user
- Guest user
- Authenticated user

## Technical Perspective

- Slow network
- Offline mode
- Interrupted requests
- Background/foreground transitions
- Low battery
- Low storage

## Data Perspective

- Empty data
- Large datasets
- Invalid input
- Special characters
- Boundary values
- Duplicate data

---

# Areas to Explore

Investigate:

- Navigation
- User flows
- Error handling
- UI consistency
- State management
- Permissions
- Notifications
- Deep links
- Search
- Filters
- Sorting
- Pagination

---

# Mobile Testing

Android

Explore:

- Rotation
- Back navigation
- Multi-window
- App lifecycle
- Different screen sizes
- Different Android versions

iOS

Explore:

- Dynamic Type
- Dark Mode
- Safe Area
- Background behavior
- Device variations

Cross-platform

Compare:

- Feature parity
- UI consistency
- Navigation
- Performance

---

# Risk-Based Exploration

Prioritize:

- Recently changed features
- Frequently used workflows
- Complex business logic
- High-impact functionality
- Areas with previous defects
- Third-party integrations

Spend more time where failures would have the greatest impact.

---

# AI Guidelines

When assisting with exploratory testing:

Always:

- Suggest unexpected scenarios.
- Challenge assumptions.
- Recommend additional workflows.
- Consider edge cases.
- Think beyond acceptance criteria.

Never:

- Limit exploration to happy paths.
- Ignore usability concerns.
- Assume documented behavior covers every scenario.

---

# Observation Checklist

During testing, observe:

- UI behavior
- Performance
- Error messages
- Unexpected navigation
- Data consistency
- Accessibility
- Animation
- Loading states
- Crash or freeze
- Memory usage (if applicable)

---

# Documentation

For every finding, record:

- Scenario
- Observation
- Expected behavior
- Actual behavior
- Environment
- Device
- Build version
- Evidence

Good exploratory testing creates reproducible findings.

---

# Common Exploration Heuristics

Consider:

- What happens if the user performs actions quickly?
- What happens if the network changes?
- What happens after app restart?
- What happens after login/logout?
- What happens when permissions are denied?
- What happens with unexpected input?
- What happens during interruptions like calls or notifications?

---

# Success Criteria

Exploratory testing is complete only when:

- High-risk areas have been explored.
- Unexpected behaviors have been investigated.
- Findings are documented with evidence.
- Regression risks are identified.
- New test scenarios are recommended.
- Valuable insights have been captured.
