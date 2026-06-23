# .NET Engineering Method

Use for `/dotnet assess`.

## Review Lenses

- Project type, target framework, SDK, and hosting model
- Solution and project boundaries
- Domain/application/infrastructure/API separation
- Dependency injection, options, configuration, logging, and health checks
- Async, cancellation, error handling, validation, and resilience
- Data access, transactions, consistency, migrations, and query behavior
- Testing strategy and CI feedback
- Observability: structured logs, metrics, traces, correlation, and diagnostics
- Security-sensitive code paths and security review triggers
- Deployment and Azure integration handoffs

## Output Expectations

- Identify high-risk findings first.
- Tie recommendations to concrete code, project files, or design surfaces when
  available.
- Mark version-sensitive advice when the target framework is unknown.
- Hand broad software architecture questions to `software-architecture`.

