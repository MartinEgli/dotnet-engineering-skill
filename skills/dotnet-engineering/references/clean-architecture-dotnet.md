# Clean Architecture In .NET

Use for `/dotnet clean-architecture`.

## Review Areas

- Domain model and invariants
- Application use cases, commands, queries, handlers, and ports
- Infrastructure adapters: persistence, messaging, files, clock, email, external
  APIs
- API/UI boundary and transport concerns
- Dependency direction and project references
- Test boundaries for domain, application, and adapters

## Rules

- Dependencies point inward toward domain/application rules.
- Infrastructure implements ports defined inward.
- Avoid excessive ceremony for simple CRUD.
- Keep framework attributes and persistence concerns out of domain objects
  unless the project deliberately accepts that trade-off.

