# Firely (firely-server)

Firely is an Amsterdam-based health IT company and one of the original co-developers of the HL7 FHIR (Fast Healthcare Interoperability Resources) specification. Co-founded by Ewout Kramer and Martijn Harthoorn (both long-time HL7 FHIR core team members), Firely builds the canonical FHIR toolchain used by payers, providers, health authorities, and digital health vendors worldwide. The Firely platform is anchored by Firely Server (formerly Vonk) — a certified production-grade FHIR server with native support for MongoDB and SQL Server, deployable on Windows, Linux, macOS, Docker, and Kubernetes across on-premise, Azure, AWS, and Google Cloud. Firely Server is G10, ONC, and ISiK certified and supports SMART on FHIR, Bulk Data, CDS Hooks, Subscriptions, Terminology Services, and FHIR Mapping. The product family also includes Simplifier.net (the global FHIR profile registry and package server hosting ~9,000 projects, 40,000+ profiles, and 1,600+ implementation guides), Forge (FHIR profile editor), Firely Terminal (command-line FHIR tool with FQL/FSH/FHIRPath support), the open-source Firely .NET SDK (the de-facto reference C# FHIR library), the firely-cql-sdk for Clinical Quality Language, the Firely Validator API, FHIR Facade, Firely Server Ingest, and Firely Auth. Customers include UCSF, Humana, Roche, NHS, Opala, and the World Health Organization. Firely does not operate a hosted multi-tenant FHIR-as-a-service offering with a public REST endpoint; customers run Firely Server in their own environments. The public developer surface is therefore the Firely software products (Firely Server, .NET SDK, Terminal), the Simplifier.net package and registry APIs, and the open HL7 FHIR REST API contract that every Firely Server instance implements.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/firely-server/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/firely-server/refs/heads/main/apis.yml)

## Scope

- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- FHIR
- HL7
- Healthcare
- Health IT
- Interoperability
- Clinical Data
- FHIR Server
- Vonk
- Simplifier
- Forge
- Terminology
- SMART on FHIR
- Bulk Data
- CDS Hooks
- Implementation Guides
- .NET SDK
- CQL
- Profile Registry

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Simplifier.net FHIR Package API

The Simplifier.net FHIR Package API serves every publicly published FHIR package — including packages from Simplifier.net, HL7 International, and other public feeds — and is the package backbone of the FHIR Registry at registry.fhir.org. Endpoints follow an NPM-compatible layout (`/{package-name}/-/{package-name}-{version}.tgz`) plus FHIR-specific catalog search by canonical URL, FHIR version, and package metadata. Public packages require no authentication; private feeds use JWT tokens from api.simplifier.net/token.

- **Human URL:** [https://docs.fire.ly/projects/Simplifier/features/api.html](https://docs.fire.ly/projects/Simplifier/features/api.html)
- **Base URL:** `https://packages.simplifier.net/`

#### Tags

- FHIR
- Packages
- Registry
- Implementation Guides
- Profiles
- NPM

#### Properties

- [Documentation](https://docs.fire.ly/projects/Simplifier/features/api.html)
- [Documentation](https://app.swaggerhub.com/apis/firely/Simplifier.net_FHIR_Package_API/1.0.1)
- [OpenAPI](openapi/simplifier-package-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/simplifier-package-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/simplifier-package-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Registry](https://registry.fhir.org/)

### Firely Server FHIR REST API

Every Firely Server (formerly Vonk) instance exposes the standard HL7 FHIR REST API contract — type-level and instance-level CRUD, search, history, batch/transaction, capability statement (/metadata), conditional operations, and conformance-driven validation — plus pluggable modules for Terminology Services, Bulk Data Access ($export), SMART on FHIR, CDS Hooks, Subscriptions/PubSub, FHIR Mapping Language, and custom search parameters. Firely Server supports FHIR R4, R4B, R5, and STU3 across MongoDB and SQL Server backends and is G10, ONC, and ISiK certified. The API contract is the HL7 FHIR specification itself; there is no public hosted multi-tenant base URL — customers self-host Firely Server on Windows, Linux, macOS, Docker, or Kubernetes.

- **Human URL:** [https://docs.fire.ly/projects/Firely-Server/](https://docs.fire.ly/projects/Firely-Server/)

#### Tags

- FHIR
- REST
- Healthcare
- CRUD
- Search
- Terminology
- Bulk Data
- SMART on FHIR
- CDS Hooks
- Subscriptions

#### Properties

- [Documentation](https://docs.fire.ly/projects/Firely-Server/)
- [Standards](https://hl7.org/fhir/http.html)
- [Standards](https://hl7.org/fhir/)
- [Documentation](https://hl7.org/fhir/uv/bulkdata/)
- [Documentation](https://hl7.org/fhir/smart-app-launch/)
- [Sample](https://github.com/FirelyTeam/firely-pubsub-sample)
- [Sample](https://github.com/FirelyTeam/Vonk.Facade.Starter)
- [Plugin](https://github.com/FirelyTeam/Vonk.Plugin.DocumentOperation)
- [Plugin](https://github.com/FirelyTeam/Vonk.Plugin.ExampleOperation)
- [Postman Collection](collections/simplifier-package-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/simplifier-package-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://fire.ly)
- [Portal](https://docs.fire.ly)
- [Documentation](https://docs.fire.ly/projects/Firely-Server/)
- [Documentation](https://docs.fire.ly/projects/Firely-NET-SDK/)
- [Documentation](https://docs.fire.ly/projects/Simplifier/)
- [Documentation](https://docs.fire.ly/projects/Forge/)
- [Documentation](https://docs.fire.ly/projects/Firely-Terminal/)
- [Product](https://fire.ly/firely-server/)
- [Product](https://fire.ly/products/firely-net-sdk/)
- [Product](https://fire.ly/products/simplifier-net/)
- [Product](https://fire.ly/forge/)
- [Product](https://fire.ly/products/firely-terminal/)
- [Product](https://fire.ly/products/firely-auth/)
- [Product](https://fire.ly/products/fhir-facade/)
- [Product](https://fire.ly/products/firely-server-ingest/)
- [GitHub Organization](https://github.com/FirelyTeam)
- [SDK](https://github.com/FirelyTeam/firely-net-sdk)
- [SDK](https://github.com/FirelyTeam/firely-cql-sdk)
- [Tool](https://github.com/FirelyTeam/spark)
- [Tool](https://github.com/FirelyTeam/firely-validator-api)
- [Tool](https://github.com/FirelyTeam/Firely.Fhir.Packages)
- [Tool](https://github.com/FirelyTeam/Fhir.Metrics)
- [Tool](https://github.com/FirelyTeam/firely-terminal-pipeline)
- [Helm Chart](https://github.com/FirelyTeam/Helm.Charts)
- [Helm Chart](https://github.com/FirelyTeam/Vonk.Helm.Charts)
- [Code Examples](https://github.com/FirelyTeam/firely-pubsub-sample)
- [Code Examples](https://github.com/FirelyTeam/fhirstarters)
- [Code Examples](https://github.com/FirelyTeam/Vonk.Facade.Starter)
- [Code Examples](https://github.com/FirelyTeam/Vonk.Facade.Relational)
- [Code Examples](https://github.com/FirelyTeam/Firely.Fhir.ValidationDemo)
- [Code Examples](https://github.com/FirelyTeam/ACME-FSH-IG-Example)
- [Code Examples](https://github.com/FirelyTeam/ACME-FSH-Example)
- [Plugin](https://github.com/FirelyTeam/Vonk.Plugin.DocumentOperation)
- [Plugin](https://github.com/FirelyTeam/Vonk.Plugin.ExampleOperation)
- [SDK](https://github.com/FirelyTeam/RonFHIR)
- [Tool](https://github.com/FirelyTeam/Wind.Tunnel)
- [Tool](https://github.com/FirelyTeam/firely-browser-extension)
- [Tool](https://github.com/FirelyTeam/fhir-codegen)
- [Tool](https://github.com/FirelyTeam/Hl7.Fhir.Validation.Legacy)
- [Template](https://github.com/FirelyTeam/fhir-specification-template-repository)
- [Documentation](https://github.com/FirelyTeam/firely-docs)
- [Skills](https://github.com/FirelyTeam/skills)
- [Registry](https://simplifier.net)
- [Standards](https://hl7.org/fhir/)
- [Pricing](https://fire.ly/firely-server/)
- [Sign Up](https://simplifier.net/login)
- [Training](https://fire.ly/training/)
- [Consulting](https://fire.ly/services/)
- [Blog](https://fire.ly/blog/)
- [LinkedIn](https://www.linkedin.com/company/firely/)
- [Twitter](https://twitter.com/FirelyTeam)
- [YouTube](https://www.youtube.com/c/Firely)
- [Contact](https://fire.ly/contact/)
- [Customers](https://fire.ly/customers/)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
