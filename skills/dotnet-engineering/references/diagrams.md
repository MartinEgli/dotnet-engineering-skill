# .NET Engineering Diagrams

Use for `/dotnet diagram`.

## Scope

Create diagrams for .NET software engineering:

- C4 context/container/component diagrams for .NET systems
- ASP.NET Core request pipeline and middleware flows
- Clean Architecture layers and project references
- EF Core DbContext, aggregate, migration, and transaction boundaries
- sequence diagrams for API, messaging, and background job flows
- dependency and package boundary diagrams
- Azure SDK integration flows from .NET code

## Notation

- Mermaid `flowchart` for architecture, dependency, and pipeline diagrams.
- Mermaid `sequenceDiagram` for request, message, and background processing
  flows.
- Mermaid `classDiagram` only for stable domain or DTO relationships.
- PlantUML or C4-style notation when the user wants persistent
  architecture-as-code.

## Rules

- Use exact project, namespace, class, endpoint, and package names when supplied.
- Mark unknown code paths as assumptions or gaps.
- Hand enterprise/platform diagrams to `azure-architecture` or
  `enterprise-architecture`.
- Hand threat/control diagrams to `enterprise-security-architecture`.

