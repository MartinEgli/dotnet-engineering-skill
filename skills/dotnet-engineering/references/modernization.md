# .NET Modernization Reference

Use for `/dotnet upgrade`.

## Review Areas

- Target framework and SDK version
- Legacy .NET Framework to modern .NET migration
- Package inventory and transitive risks
- MSBuild properties and project style
- Nullable reference types and language version
- ASP.NET to ASP.NET Core migration concerns
- EF6 to EF Core migration concerns
- Windows-specific dependencies
- Containerization and hosting target

## Rules

- Inventory before changing target framework.
- Identify breaking changes, unsupported packages, and hosting constraints.
- Prefer staged upgrades when runtime, dependencies, or deployment risk is high.
- Hand Azure hosting architecture to `azure-architecture`.

