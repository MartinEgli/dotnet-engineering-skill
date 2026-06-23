---
name: dotnet-engineering
description: >
  .NET Engineering skill for C#, ASP.NET Core, Minimal APIs, Web APIs, Blazor,
  background services, EF Core, data access, dependency injection, testing,
  performance, observability, secure coding, Clean Architecture in .NET,
  modernization, NuGet, MSBuild, Azure SDK integration, Azure hosting handoff,
  and Mermaid, PlantUML, C4, sequence, component, and Clean Architecture
  diagrams for .NET systems.
---

# .NET Engineering

## Purpose

Design, review, and improve .NET systems so C# code, ASP.NET Core services,
data access, tests, performance, observability, modernization, and Azure
integration stay maintainable and production-ready.

## When to Use

Use when the user asks for:

- C# or .NET engineering review
- ASP.NET Core, Minimal API, Web API, worker service, Blazor, or hosted service
  design
- EF Core, repositories, migrations, transactions, or data access review
- dependency injection, options, configuration, logging, or middleware design
- .NET Clean Architecture, layering, ports/adapters, or modular monolith review
- testing strategy with unit, integration, contract, or architecture tests
- performance, memory, async, throughput, startup, or diagnostics guidance
- .NET modernization, package, SDK, target framework, or upgrade planning
- Azure SDK usage from .NET
- .NET diagrams using Mermaid, PlantUML, or C4-style notation

## Do Not Use When

Do not use for broad enterprise architecture, portfolio, capability, or roadmap
decisions. Use `enterprise-architecture`.

Do not use for cloud platform architecture, landing zones, or Azure governance.
Use `azure-architecture`.

Do not use for general software architecture that is not .NET-specific. Use
`software-architecture`.

Do not use for deep DDD modeling when the main output is context maps,
aggregates, event storming, or ubiquitous language. Use `domain-driven-design`.

Do not use for security approval, threat modeling, or control acceptance. Use
`enterprise-security-architecture`.

Do not use for final evidence acceptance or productive-use governance. Use
`mournival-architecture`.

## Mandatory Rules

- Start from runtime, target framework, application type, use case, constraints,
  and quality attributes.
- Preserve user-provided namespaces, project names, APIs, package names,
  configuration keys, commands, and error strings exactly.
- Separate domain/application logic from framework, persistence, transport, and
  hosting concerns.
- Keep findings, diagrams, code recommendations, package guidance, and handoffs
  traceable to supplied code, project files, tool results, sources, or clearly
  marked assumptions.
- Prefer idiomatic .NET patterns: dependency injection, async where appropriate,
  options pattern, structured logging, cancellation tokens, health checks, and
  explicit configuration.
- Mark assumptions, missing project facts, and unverified runtime behavior.
- Do not invent package versions, framework behavior, benchmark results, or
  production facts.
- Escalate broad architecture to `software-architecture`, Azure platform design
  to `azure-architecture`, security approval to
  `enterprise-security-architecture`, and final governance to
  `mournival-architecture`.

## Inputs Expected

- target framework and .NET SDK version
- application type
- project or solution structure
- relevant code, APIs, packages, config, logs, or errors
- data store and EF Core usage when relevant
- hosting target and runtime constraints
- quality attributes
- testing and CI context
- Azure services or SDKs when relevant

## Modes

### /dotnet assess

Review a .NET solution, service, or design for maintainability, correctness,
testability, performance, observability, and delivery risk. Read
`references/dotnet-engineering-method.md`.

### /dotnet api

Design or review ASP.NET Core, Minimal API, Web API, middleware, authentication
integration, validation, error handling, versioning, and OpenAPI concerns. Read
`references/aspnetcore.md`.

### /dotnet data

Review EF Core and data access: DbContext boundaries, migrations, transactions,
query performance, repositories, concurrency, and consistency. Read
`references/data-efcore.md`.

### /dotnet clean-architecture

Review .NET Clean Architecture, layers, dependency direction, use cases,
ports/adapters, modular monolith structure, and test boundaries. Read
`references/clean-architecture-dotnet.md`.

### /dotnet testing

Design or review unit, integration, contract, architecture, and end-to-end test
strategy for .NET. Read `references/testing.md`.

### /dotnet performance

Review performance, async, memory, allocation, startup, throughput, caching,
diagnostics, and observability concerns. Read `references/performance.md`.

### /dotnet upgrade

Plan modernization, target framework upgrade, package cleanup, NuGet/MSBuild
review, or migration from older .NET Framework/.NET versions. Read
`references/modernization.md`.

### /dotnet azure

Review .NET integration with Azure SDKs, managed identity, configuration,
Key Vault, App Service, Functions, Container Apps, messaging, storage, and
observability handoffs. Read `references/azure-integration.md`.

### /dotnet diagram

Create or review .NET software diagrams using Mermaid, PlantUML, C4-style,
sequence, component, Clean Architecture, or dependency notation. Read
`references/diagrams.md`.

## Evidence Handling

Use `references/evidence-traceability.md`.

- Evidence: supplied code, project file, package list, configuration, log,
  benchmark, test result, API contract, or explicit user fact.
- Inference: engineering conclusion derived from evidence.
- Assumption: useful but unverified project hypothesis.
- Gap: missing input that can change the engineering decision.

## Output Contracts

Use `assets/templates/dotnet-engineering-output.md` unless user asks for
another format.

## Quality Gates

- Runtime, project type, and target framework are explicit or marked as gaps.
- Recommendations are idiomatic for .NET and tied to quality attributes.
- Key engineering claims include source trace or are marked as assumptions.
- Domain/application logic is not coupled unnecessarily to infrastructure.
- Tests and observability are addressed when changing behavior.
- Azure platform concerns are handed to `azure-architecture`.
- Security approval concerns are handed to `enterprise-security-architecture`.
- Diagrams stay within .NET/software engineering scope.

## Boundaries

- Do not claim code is production-safe without tests and runtime evidence.
- Do not invent package versions or API availability when version matters.
- Do not replace accountable security, architecture, or production approval.
- Do not over-apply Clean Architecture when simple modular .NET design is
  enough.

## Output Style

- Practical, code-aware, and concise.
- Prefer concrete project/file/package guidance when evidence is available.
- Use tables for findings and options when comparison helps.
- Use Mermaid for quick diagrams and PlantUML/C4-style notation when persistent
  architecture-as-code is useful.
