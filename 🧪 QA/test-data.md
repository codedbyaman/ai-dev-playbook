# Test Data Playbook

Guidelines for using AI to design, generate, manage, and maintain high-quality test data.

Focus on creating realistic, reusable, and secure test data that supports reliable manual and automated testing.

---

# Core Principles

- Design test data based on business requirements.
- Use realistic but non-production data.
- Keep test data reusable and maintainable.
- Protect sensitive information.
- Support positive, negative, and edge case testing.
- Ensure test data is deterministic whenever possible.

---

# Test Data Workflow

Follow this sequence:

1. Understand the feature.
2. Identify data requirements.
3. Define test scenarios.
4. Create representative datasets.
5. Validate data quality.
6. Execute testing.
7. Clean up test data if necessary.
8. Maintain reusable datasets.

---

# Understand Requirements

Review:

- Business requirements
- Acceptance criteria
- Validation rules
- Data dependencies
- API contracts
- Database relationships

Never create test data without understanding the feature.

---

# Data Categories

Create data for:

- Valid inputs
- Invalid inputs
- Empty values
- Null values
- Boundary values
- Large datasets
- Duplicate records
- Special characters
- International characters
- Date and time variations

---

# Positive Test Data

Include:

- Valid users
- Valid products
- Valid addresses
- Valid payment methods
- Valid search terms
- Valid account states

---

# Negative Test Data

Include:

- Invalid credentials
- Expired accounts
- Missing required fields
- Invalid formats
- Unauthorized users
- Duplicate values
- Unsupported characters

Applications should handle invalid data gracefully.

---

# Boundary Test Data

Validate:

- Minimum values
- Maximum values
- Empty strings
- Long strings
- Large numbers
- Zero values
- Negative values
- Maximum file sizes
- Minimum supported versions

---

# Environment Strategy

Maintain separate datasets for:

- Development
- QA
- Staging
- Performance
- UAT

Avoid sharing mutable test data across environments.

---

# Data Privacy

Never use:

- Real customer data
- Personal information
- Production credentials
- Sensitive business information

Prefer:

- Masked data
- Synthetic data
- Generated datasets
- Anonymized records

---

# Mobile Test Data

Prepare data for:

- Logged-in users
- Guest users
- New users
- Returning users
- Premium users
- Different locales
- Multiple currencies
- Different languages

---

# API Test Data

Include:

- Valid payloads
- Invalid payloads
- Missing fields
- Optional fields
- Large payloads
- Empty collections
- Nested objects
- Invalid data types

---

# Automation Considerations

Prefer:

- Reusable fixtures
- Factory methods
- Data builders
- Mock data
- Independent datasets
- Predictable values

Avoid hardcoded test data whenever possible.

---

# AI Guidelines

When generating test data:

Always:

- Explain why the data is needed.
- Cover positive and negative scenarios.
- Include edge cases.
- Recommend reusable datasets.
- Consider privacy and security.

Never:

- Generate production data.
- Ignore validation rules.
- Use personally identifiable information.
- Assume undocumented business rules.

---

# Test Data Documentation

Include:

- Dataset name
- Purpose
- Environment
- Dependencies
- Creation method
- Cleanup process
- Owner
- Last updated

---

# Success Criteria

Test data is complete only when:

- Business scenarios are supported.
- Positive and negative datasets exist.
- Edge cases are covered.
- Sensitive information is protected.
- Data is reusable and maintainable.
- Documentation is available.
