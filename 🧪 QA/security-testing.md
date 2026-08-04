# Security Testing Playbook

Guidelines for using AI to design, execute, and analyze security testing for applications and APIs.

Focus on identifying common security risks, validating secure behavior, and reducing vulnerabilities through practical QA techniques.

---

# Core Principles

- Security is a shared responsibility.
- Validate security requirements early and continuously.
- Test for common vulnerabilities.
- Protect sensitive user data.
- Follow the principle of least privilege.
- Verify security without disrupting application functionality.

---

# Security Testing Workflow

Follow this sequence:

1. Understand security requirements.
2. Identify sensitive assets.
3. Review authentication and authorization.
4. Validate input handling.
5. Test common attack scenarios.
6. Verify secure data handling.
7. Document findings.
8. Recommend remediation and regression testing.

---

# Authentication Testing

Verify:

- Valid login
- Invalid login
- Account lockout
- Password policies
- Multi-factor authentication (MFA)
- Session timeout
- Token expiration
- Logout behavior
- Remember Me functionality

---

# Authorization Testing

Validate:

- User roles
- Permission levels
- Resource ownership
- Privilege escalation
- Access to restricted resources
- Direct URL access
- API authorization
- Feature restrictions

Users should only access resources they are authorized to use.

---

# Input Validation

Test:

- SQL Injection
- Cross-Site Scripting (XSS)
- Command Injection
- HTML Injection
- Invalid characters
- Long inputs
- Empty values
- Null values
- Special characters

Applications should validate and sanitize user input.

---

# API Security

Verify:

- Authentication
- Authorization
- Rate limiting
- Input validation
- Sensitive data exposure
- Token handling
- Secure headers
- Error responses

Avoid exposing internal implementation details.

---

# Session Management

Validate:

- Secure session creation
- Session expiration
- Session invalidation after logout
- Session timeout
- Multiple active sessions
- Session fixation protection

---

# Data Protection

Verify:

- Sensitive data masking
- Encryption in transit
- Secure storage
- Secure logging
- No sensitive information in URLs
- No sensitive information in logs

Never expose passwords, tokens, or personal information.

---

# Mobile Security

Android

Validate:

- Secure storage
- Deep Link validation
- Root detection (if applicable)
- Certificate pinning (if applicable)
- Backup restrictions

iOS

Validate:

- Keychain usage
- Universal Link security
- Jailbreak detection (if applicable)
- Secure storage
- ATS configuration

---

# Error Handling

Verify:

- Generic error messages
- No stack traces exposed
- No internal server details
- Secure logging
- Consistent error responses

Errors should help users without exposing implementation details.

---

# AI Guidelines

When assisting with security testing:

Always:

- Recommend common security test scenarios.
- Verify authentication and authorization separately.
- Consider OWASP Top 10 risks.
- Suggest secure testing practices.
- Highlight potential data exposure.

Never:

- Suggest bypassing security controls.
- Recommend insecure workarounds.
- Ignore authorization validation.
- Assume a feature is secure without verification.

---

# Security Test Report

Include:

- Security scenario
- Environment
- Steps performed
- Expected behavior
- Actual behavior
- Risk level
- Evidence
- Recommendation

---

# Success Criteria

Security testing is complete only when:

- Authentication is verified.
- Authorization is validated.
- Common input validation scenarios are tested.
- Sensitive data is protected.
- Security findings are documented.
- Regression recommendations are provided.
