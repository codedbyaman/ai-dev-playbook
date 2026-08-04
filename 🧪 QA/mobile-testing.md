# Mobile Testing Playbook

Guidelines for using AI to design, execute, and analyze mobile application testing.

Focus on delivering a reliable, accessible, and consistent user experience across Android and iOS devices.

---

# Core Principles

- Understand the feature before testing.
- Validate user experience across platforms.
- Test on realistic devices and environments.
- Consider device fragmentation.
- Prioritize business-critical user journeys.
- Verify functionality, usability, accessibility, and performance.

---

# Mobile Testing Workflow

Follow this sequence:

1. Understand the feature.
2. Review requirements.
3. Identify supported platforms.
4. Prepare test devices.
5. Execute functional testing.
6. Validate platform-specific behavior.
7. Verify non-functional requirements.
8. Document findings.

---

# Functional Testing

Validate:

- User flows
- Navigation
- Forms
- Search
- Filters
- Sorting
- Authentication
- Payments
- Deep Links
- Notifications
- Offline behavior

Always verify business behavior before platform-specific details.

---

# Android Testing

Validate:

- Different Android versions
- Different screen sizes
- Different manufacturers
- Orientation changes
- Back navigation
- Multi-window mode
- Background and foreground transitions
- App permissions
- Battery optimization
- Push notifications

---

# iOS Testing

Validate:

- Different iPhone models
- Different iOS versions
- Safe Area layouts
- Dynamic Type
- Dark Mode
- Background and foreground transitions
- Face ID / Touch ID
- Push notifications
- Universal Links
- App lifecycle

---

# Cross-Platform Validation

Compare:

- Feature parity
- Navigation
- Business logic
- UI consistency
- Error handling
- Accessibility
- Performance

Platform differences should be intentional and documented.

---

# Network Testing

Validate under different conditions:

- Wi-Fi
- Mobile data
- Slow network
- High latency
- Packet loss
- Offline mode
- Network switching

Verify graceful recovery after connectivity returns.

---

# Accessibility Testing

Verify:

- VoiceOver
- TalkBack
- Accessibility labels
- Accessibility hints
- Focus order
- Dynamic Type
- Color contrast
- Touch target size
- Screen reader announcements

Accessibility should be treated as a core quality requirement.

---

# Performance Testing

Observe:

- App launch time
- Screen loading
- Scrolling performance
- Memory usage
- CPU usage
- Battery consumption
- Network efficiency
- Animation smoothness

Identify regressions rather than isolated measurements.

---

# Device Compatibility

Consider:

- Screen sizes
- OS versions
- Hardware capabilities
- Tablets
- Foldable devices
- Different locales
- Different time zones

Prioritize devices based on usage analytics.

---

# API Validation

Verify:

- Correct requests
- Correct responses
- Error handling
- Retry behavior
- Timeout handling
- Data synchronization

Use API validation to support mobile testing.

---

# Mobile Automation

Prefer:

- Appium
- Espresso
- XCUITest

Automation should:

- Reuse existing utilities
- Prefer accessibility identifiers
- Avoid hardcoded waits
- Follow existing framework architecture

---

# Debugging

Collect:

- Screenshots
- Screen recordings
- Logcat
- Xcode Console logs
- Crash reports
- API logs
- Charles Proxy traces
- Proxyman captures

Use evidence to support conclusions.

---

# AI Guidelines

When assisting with mobile testing:

Always:

- Consider Android and iOS separately.
- Suggest device coverage.
- Recommend accessibility validation.
- Include network scenarios.
- Think about lifecycle events.
- Recommend regression scope.

Never:

- Assume platform parity.
- Ignore OS-specific behavior.
- Recommend testing on a single device only.
- Skip accessibility or network testing.

---

# Mobile Test Report

Include:

- Platform
- Device
- OS Version
- App Version
- Build Number
- Environment
- Test Results
- Defects
- Evidence
- Recommendations

---

# Success Criteria

Mobile testing is complete only when:

- Business requirements are validated.
- Android and iOS behavior is verified.
- Device compatibility is considered.
- Accessibility is validated.
- Network scenarios are tested.
- Performance observations are recorded.
- Findings are documented with evidence.
