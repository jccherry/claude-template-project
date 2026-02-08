# Tests

## Overview

<!-- Describe the testing strategy: unit, integration, e2e. What frameworks and tools are used. -->

## Test Structure

```
tests/
├── unit/          # Unit tests (isolated, fast)
├── integration/   # Integration tests (service + DB, API tests)
└── e2e/           # End-to-end tests (browser, full stack)
```

## Running Tests

```bash
# Run all tests
# npm test

# Run unit tests only
# npm run test:unit

# Run integration tests
# npm run test:integration

# Run e2e tests
# npm run test:e2e

# Run with coverage
# npm run test:coverage
```

## Test Conventions

- **File naming:** `<module>.test.ts` or `<module>.spec.ts`
- **Structure:** Arrange → Act → Assert
- **Isolation:** Unit tests must not depend on external services or databases.
- **Mocking:** Describe the mocking strategy (e.g., dependency injection, test doubles, MSW for API mocking).

## Coverage

<!-- Describe coverage targets and how to view coverage reports. -->

| Metric | Target |
|--------|--------|
| Lines | <!-- 80% --> |
| Branches | <!-- 75% --> |
| Functions | <!-- 80% --> |

## CI Integration

<!-- Tests run automatically in CI via GitHub Actions. Describe any CI-specific test configuration. -->

## Fixtures & Factories

<!-- Describe how test data is created: factories, fixtures, builders. -->

## Environment

<!-- Describe any test-specific env vars or setup (test database, mock services). -->

| Variable | Description |
|----------|-------------|
| <!-- TEST_DATABASE_URL --> | <!-- Test database connection --> |

## Notes

<!-- Flaky test policy, performance testing, visual regression testing, etc. -->
