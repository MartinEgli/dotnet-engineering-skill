# ASP.NET Core Reference

Use for `/dotnet api`.

## Review Areas

- Minimal API, controller, endpoint, middleware, or hosted service structure
- Request validation, binding, filters, and problem details
- Authentication and authorization integration
- Versioning and OpenAPI description
- Dependency injection lifetime correctness
- Options pattern and configuration binding
- Logging, correlation, health checks, and readiness endpoints
- Error handling and exception boundaries
- Streaming, async, cancellation, and timeouts

## Rules

- Keep domain logic out of controllers and endpoint mapping.
- Prefer explicit validation and consistent error contracts.
- Use scoped dependencies carefully; avoid capturing scoped services in
  singletons.
- Hand security approval and threat modeling to
  `enterprise-security-architecture`.

