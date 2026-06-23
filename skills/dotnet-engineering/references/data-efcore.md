# EF Core And Data Access Reference

Use for `/dotnet data`.

## Review Areas

- DbContext boundary and lifetime
- Aggregate or module ownership of data
- Migration strategy and deployment safety
- Query shape, tracking behavior, includes, projections, and pagination
- Transactions, concurrency tokens, idempotency, and consistency boundaries
- Repository usage and when direct DbContext use is clearer
- Connection resiliency and retry behavior
- Secrets, connection configuration, and managed identity when on Azure

## Rules

- Do not treat database tables as the domain model by default.
- Avoid hidden N+1 queries, unbounded result sets, and accidental tracking.
- Keep migrations reviewable and deployment-aware.
- Hand deep aggregate and bounded-context modeling to `domain-driven-design`.

