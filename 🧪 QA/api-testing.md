# API Testing Playbook

Guidelines for using AI to design, execute, and analyze API testing.

Focus on validating API functionality, reliability, security, and data integrity rather than only checking response codes.

---

# Core Principles

- Understand the API before testing.
- Validate business behavior, not just HTTP responses.
- Test both positive and negative scenarios.
- Verify data integrity.
- Consider security, performance, and compatibility.
- Use reusable and maintainable test strategies.

---

# API Testing Workflow

Follow this sequence:

1. Understand the API.
2. Review the API contract.
3. Validate request parameters.
4. Execute positive scenarios.
5. Execute negative scenarios.
6. Verify responses.
7. Validate backend data if applicable.
8. Document findings.

---

# Understand the API

Review:

- Business requirements
- API documentation
- OpenAPI / Swagger specification
- Authentication method
- Request parameters
- Response schema
- Error responses
- Dependencies

Never test an API without understanding its purpose.

---

# Request Validation

Verify:

- HTTP method
- Endpoint
- Headers
- Authentication
- Authorization
- Query parameters
- Path parameters
- Request body
- Required fields
- Optional fields

---

# Response Validation

Validate:

- HTTP status code
- Response body
- Schema
- Required fields
- Data types
- Field values
- Pagination
- Sorting
- Filtering

Never rely only on status codes.

---

# Functional Testing

Verify:

- Business rules
- CRUD operations
- Data consistency
- Search
- Filtering
- Sorting
- Pagination
- Relationships
- State transitions

---

# Negative Testing

Test:

- Missing parameters
- Invalid parameters
- Invalid data types
- Empty values
- Null values
- Duplicate requests
- Invalid authentication
- Expired tokens
- Unauthorized access
- Invalid HTTP methods

The API should fail gracefully with meaningful error responses.

---

# Authentication & Authorization

Validate:

- Valid credentials
- Invalid credentials
- Expired tokens
- Missing tokens
- Token refresh
- User roles
- Permission levels
- Resource ownership

---

# Error Handling

Verify:

- Error codes
- Error messages
- Validation errors
- Server errors
- Rate limiting
- Timeout behavior
- Retry behavior

Errors should be consistent and informative.

---

# Data Validation

Verify:

- Data persistence
- Data updates
- Data deletion
- Duplicate prevention
- Data integrity
- Database consistency
- Cross-service consistency

---

# Performance Testing

Observe:

- Response time
- Throughput
- Latency
- Timeout behavior
- Concurrent requests
- Large payload handling

Highlight unusual performance degradation.

---

# Security Testing

Consider:

- SQL Injection
- XSS
- Broken authentication
- Sensitive data exposure
- Input validation
- Rate limiting
- Authorization bypass
- Mass assignment
- Security headers

Security testing should follow organizational policies.

---

# Compatibility Testing

Validate:

- API versioning
- Backward compatibility
- Forward compatibility
- Deprecated endpoints
- Client compatibility

Avoid breaking existing consumers.

---

# AI Guidelines

When assisting with API testing:

Always:

- Review API documentation.
- Suggest positive and negative scenarios.
- Validate business logic.
- Consider edge cases.
- Recommend automation opportunities.

Never:

- Assume undocumented behavior.
- Ignore error responses.
- Skip authorization testing.
- Validate only happy paths.

---

# Automation Considerations

Prefer:

- Existing API test frameworks
- Reusable request builders
- Shared test data
- Schema validation
- Data-driven testing

Avoid duplicate API tests.

---

# API Test Report

Include:

- Endpoint
- Environment
- Request
- Response
- Status Code
- Result
- Defects Found
- Logs
- Recommendations

---

# Success Criteria

API testing is complete only when:

- Business behavior is validated.
- Positive and negative scenarios pass.
- Responses match the API contract.
- Authentication and authorization are verified.
- Data integrity is confirmed.
- Performance concerns are identified.
- Findings are documented clearly.
