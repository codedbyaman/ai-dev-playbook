# Accessibility Testing Playbook

Guidelines for using AI to design, execute, and improve accessibility testing for web and mobile applications.

Focus on building inclusive experiences that are usable by everyone, including people using assistive technologies.

---

# Core Principles

- Accessibility is a product requirement, not an optional feature.
- Test using real assistive technologies whenever possible.
- Follow platform accessibility guidelines.
- Verify both functionality and usability.
- Prefer semantic information over visual assumptions.
- Consider accessibility throughout development, not only before release.

---

# Accessibility Testing Workflow

Follow this sequence:

1. Understand the feature.
2. Review accessibility requirements.
3. Validate semantic information.
4. Test with assistive technologies.
5. Verify interaction behavior.
6. Validate visual accessibility.
7. Document findings.
8. Recommend improvements.

---

# Semantic Validation

Verify:

- Accessibility labels
- Accessibility identifiers
- Accessibility hints
- Accessibility values
- Roles
- Traits
- States

Every interactive element should expose meaningful accessibility information.

---

# Screen Reader Testing

Android

Validate using TalkBack:

- Correct announcements
- Focus order
- Gesture navigation
- Accessible actions
- State changes

iOS

Validate using VoiceOver:

- Correct announcements
- Rotor navigation
- Focus movement
- Element grouping
- Custom actions

---

# Navigation

Verify:

- Logical focus order
- Keyboard navigation (where applicable)
- Screen reader navigation
- Modal dialogs
- Navigation between screens
- Back navigation

Navigation should be predictable and consistent.

---

# Visual Accessibility

Validate:

- Color contrast
- Text scaling
- Dynamic Type
- Zoom support
- Touch target size
- Dark Mode
- High contrast mode

Visual changes should not affect usability.

---

# Forms

Verify:

- Labels
- Placeholder text
- Required fields
- Error messages
- Validation feedback
- Focus after validation

Users should clearly understand what information is required.

---

# Dynamic Content

Validate:

- Loading indicators
- Success messages
- Error messages
- Live updates
- Progress indicators

Important updates should be announced to assistive technologies.

---

# Mobile Accessibility

Android

Verify:

- TalkBack
- Accessibility Scanner recommendations
- Large font support
- Gesture navigation

iOS

Verify:

- VoiceOver
- Dynamic Type
- Bold Text
- Reduce Motion
- Increase Contrast

---

# AI Guidelines

When assisting with accessibility testing:

Always:

- Recommend testing with assistive technologies.
- Suggest accessibility improvements.
- Verify semantic information.
- Consider users with different abilities.
- Include accessibility in regression recommendations.

Never:

- Assume visual correctness means accessibility.
- Ignore focus order.
- Skip screen reader validation.
- Recommend inaccessible alternatives.

---

# Accessibility Report

Include:

- Platform
- Screen
- Accessibility issue
- Expected behavior
- Actual behavior
- WCAG or platform guideline (if applicable)
- Severity
- Evidence
- Recommendation

---

# Success Criteria

Accessibility testing is complete only when:

- Interactive elements are accessible.
- Screen reader navigation is validated.
- Focus order is logical.
- Dynamic content is announced correctly.
- Visual accessibility requirements are met.
- Findings are documented with clear recommendations.
