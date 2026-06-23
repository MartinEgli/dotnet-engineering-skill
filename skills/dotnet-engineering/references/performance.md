# .NET Performance Reference

Use for `/dotnet performance`.

## Review Areas

- Async and thread pool usage
- Cancellation tokens and timeouts
- Allocation hot paths and memory pressure
- LINQ and EF Core query shape
- Serialization and payload size
- Caching and invalidation
- Startup and dependency graph
- Logging volume and expensive log construction
- Benchmark and profiling evidence

## Rules

- Do not claim performance gains without measurement path or evidence.
- Prefer clarity unless the path is proven hot.
- Use benchmark, profiler, trace, log, or production telemetry evidence when
  available.
- Separate performance bottlenecks from architecture preferences.

