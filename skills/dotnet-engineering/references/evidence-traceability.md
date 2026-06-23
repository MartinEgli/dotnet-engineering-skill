# Evidence And Traceability

Use this reference whenever .NET engineering findings, diagrams, package
guidance, performance claims, or recommendations depend on supplied inputs.

## Input Register

Track meaningful inputs by source type:

- User fact: stated directly by the user.
- Artifact: C# file, `.csproj`, `.sln`, package list, configuration, log, test,
  benchmark, API contract, migration, diagram, or project tree.
- Tool result: `dotnet build`, `dotnet test`, analyzer output, benchmark,
  profiler, package audit, code search, or generated report.
- External source: cited Microsoft Learn page, package documentation, framework
  reference, or public source.
- Assumption: useful but unverified project premise.

## Traceability Rules

- Preserve project names, namespaces, class names, APIs, package names, config
  keys, commands, paths, and error strings exactly.
- Tie each finding to code, project metadata, tool output, source, or
  assumption.
- Do not claim runtime behavior, package availability, or performance
  improvement without evidence or a measurement path.
- Mark missing target framework, SDK version, hosting model, and workload
  details as gaps.
- Keep Azure platform decisions separate from .NET implementation evidence.

## Evidence Receipt

For substantial outputs, include a compact receipt:

| Finding Or Recommendation | Source/Input | Type | Confidence | Gap Or Follow-up |
| --- | --- | --- | --- | --- |

Use `not supplied` when the input is missing. Use `assumption` when proceeding
with a working premise.

## Verification Pattern

Follow the small-loop pattern:

1. Locate relevant code, project files, packages, config, tests, and logs.
2. Make the smallest scoped .NET recommendation.
3. Verify the output against evidence, assumptions, tests, runtime constraints,
   and skill boundaries.

Avoid drive-by refactors or new abstractions unless they directly solve the
observed .NET engineering problem.
