# .NET Azure Integration Reference

Use for `/dotnet azure`.

## Review Areas

- Azure SDK client registration and lifetime
- Managed identity and `DefaultAzureCredential` usage
- Key Vault configuration and secretless design
- App Configuration and options binding
- Application Insights, OpenTelemetry, logging, metrics, and traces
- Azure Storage, Service Bus, Event Hubs, Cosmos DB, SQL, Functions, App
  Service, Container Apps, and AKS handoffs
- Retry, timeout, idempotency, and poison-message behavior
- Local development configuration without production secrets

## Handoffs

- Use `azure-architecture` for landing zone, hosting, networking, governance,
  and platform design.
- Use `azure-prepare`, `azure-deploy`, and `azure-validate` for deployment
  preparation, execution, and preflight checks.
- Use `azure-diagnostics` for live Azure troubleshooting.
- Use `enterprise-security-architecture` for security approval and risk
  acceptance.

