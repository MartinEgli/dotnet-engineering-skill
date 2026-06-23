# .NET Testing Reference

Use for `/dotnet testing`.

## Test Types

- Unit tests for pure domain and application logic
- Integration tests for EF Core, HTTP endpoints, messaging, and external
  adapters
- Contract tests for APIs and events
- Architecture tests for dependency direction and layering
- End-to-end tests only for critical flows where lower-level tests are
  insufficient

## Review Areas

- Test project structure and naming
- Fixture lifecycle and isolation
- Test data strategy
- Deterministic time, IDs, and external dependencies
- CI runtime and flakiness
- Coverage of failure paths and edge cases

## Rules

- Prefer fast tests near the logic.
- Use integration tests for infrastructure behavior that mocks cannot validate.
- Do not claim behavior is safe without a test or runtime evidence path.

