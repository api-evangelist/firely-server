# Firely (firely-server)

Firely is an Amsterdam-based health IT company and one of the original co-developers of the HL7 FHIR (Fast Healthcare Interoperability Resources) specification. Co-founded by Ewout Kramer and Martijn Harthoorn (both long-time HL7 FHIR core team members), Firely builds the canonical FHIR toolchain used by payers, providers, health authorities, and digital health vendors worldwide. The Firely platform is anchored by Firely Server (formerly Vonk) — a certified production-grade FHIR server with native support for MongoDB and SQL Server, deployable on Windows, Linux, macOS, Docker, and Kubernetes across on-premise, Azure, AWS, and Google Cloud. Firely Server is G10, ONC, and ISiK certified and supports SMART on FHIR, Bulk Data, CDS Hooks, Subscriptions, Terminology Services, and FHIR Mapping. The product family also includes Simplifier.net (the global FHIR profile registry and package server hosting ~9,000 projects, 40,000+ profiles, and 1,600+ implementation guides), Forge (FHIR profile editor), Firely Terminal (command-line FHIR tool with FQL/FSH/FHIRPath support), the open-source Firely .NET SDK, the firely-cql-sdk for Clinical Quality Language, the Firely Validator API, FHIR Facade, Firely Server Ingest, and Firely Auth. Customers include UCSF, Humana, Roche, NHS, Opala, and the World Health Organization.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/firely-server/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

FHIR, HL7, Healthcare, Health IT, Interoperability, Clinical Data, FHIR Server, Vonk, Simplifier, Forge, Terminology, SMART on FHIR, Bulk Data, CDS Hooks, Implementation Guides, .NET SDK, CQL, Profile Registry

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Simplifier.net FHIR Package API

The Simplifier.net FHIR Package API serves every publicly published FHIR package — including packages from Simplifier.net, HL7 International, and other public feeds — and is the package backbone of the FHIR Registry at registry.fhir.org. Endpoints follow an NPM-compatible layout (`/{package-name}/-/{package-name}-{version}.tgz`) plus FHIR-specific catalog search by canonical URL, FHIR version, and package metadata. Public packages require no authentication; private feeds use JWT tokens from `api.simplifier.net/token`.

**Human URL:** [https://docs.fire.ly/projects/Simplifier/features/api.html](https://docs.fire.ly/projects/Simplifier/features/api.html)

**Base URL:** `https://packages.simplifier.net/`

#### Tags

FHIR, Packages, Registry, Implementation Guides, Profiles, NPM

#### Properties

- [Documentation](https://docs.fire.ly/projects/Simplifier/features/api.html)
- [SwaggerHub](https://app.swaggerhub.com/apis/firely/Simplifier.net_FHIR_Package_API/1.0.1)
- [OpenAPI](openapi/simplifier-package-api-openapi.yml)
- [Registry](https://registry.fhir.org/)

### Firely Server FHIR REST API

Every Firely Server (formerly Vonk) instance exposes the standard HL7 FHIR REST API contract — type-level and instance-level CRUD, search, history, batch/transaction, capability statement (`/metadata`), conditional operations, and conformance-driven validation — plus pluggable modules for Terminology Services, Bulk Data Access (`$export`), SMART on FHIR, CDS Hooks, Subscriptions/PubSub, FHIR Mapping Language, and custom search parameters. Firely Server supports FHIR R4, R4B, R5, and STU3 across MongoDB and SQL Server backends and is G10, ONC, and ISiK certified. The API contract is the HL7 FHIR specification itself; there is no public hosted multi-tenant base URL — customers self-host Firely Server on Windows, Linux, macOS, Docker, or Kubernetes.

**Human URL:** [https://docs.fire.ly/projects/Firely-Server/](https://docs.fire.ly/projects/Firely-Server/)

#### Tags

FHIR, REST, Healthcare, CRUD, Search, Terminology, Bulk Data, SMART on FHIR, CDS Hooks, Subscriptions

#### Properties

- [Documentation](https://docs.fire.ly/projects/Firely-Server/)
- [HL7 FHIR RESTful API](https://hl7.org/fhir/http.html)
- [HL7 FHIR Specification](https://hl7.org/fhir/)
- [Bulk Data Access IG](https://hl7.org/fhir/uv/bulkdata/)
- [SMART App Launch](https://hl7.org/fhir/smart-app-launch/)
- [Firely Server PubSub sample](https://github.com/FirelyTeam/firely-pubsub-sample)
- [Vonk Facade starter](https://github.com/FirelyTeam/Vonk.Facade.Starter)
- [Vonk $document plugin](https://github.com/FirelyTeam/Vonk.Plugin.DocumentOperation)
- [Vonk plugin template](https://github.com/FirelyTeam/Vonk.Plugin.ExampleOperation)

## Common Properties

- [Website](https://fire.ly)
- [Portal](https://docs.fire.ly)
- [Firely Server Documentation](https://docs.fire.ly/projects/Firely-Server/)
- [Firely .NET SDK Documentation](https://docs.fire.ly/projects/Firely-NET-SDK/)
- [Simplifier Documentation](https://docs.fire.ly/projects/Simplifier/)
- [Forge Documentation](https://docs.fire.ly/projects/Forge/)
- [Firely Terminal Documentation](https://docs.fire.ly/projects/Firely-Terminal/)
- [Firely Server (Vonk)](https://fire.ly/firely-server/)
- [Firely .NET SDK](https://fire.ly/products/firely-net-sdk/)
- [Simplifier.net](https://fire.ly/products/simplifier-net/)
- [Forge](https://fire.ly/forge/)
- [Firely Terminal](https://fire.ly/products/firely-terminal/)
- [Firely Auth](https://fire.ly/products/firely-auth/)
- [FHIR Facade](https://fire.ly/products/fhir-facade/)
- [Firely Server Ingest](https://fire.ly/products/firely-server-ingest/)
- [GitHub Organization](https://github.com/FirelyTeam)
- [Firely .NET SDK (C#)](https://github.com/FirelyTeam/firely-net-sdk)
- [Firely CQL SDK](https://github.com/FirelyTeam/firely-cql-sdk)
- [Spark FHIR Server](https://github.com/FirelyTeam/spark)
- [Firely Validator API](https://github.com/FirelyTeam/firely-validator-api)
- [Firely FHIR Packages library](https://github.com/FirelyTeam/Firely.Fhir.Packages)
- [Fhir.Metrics (UCUM)](https://github.com/FirelyTeam/Fhir.Metrics)
- [Firely Terminal GitHub Action](https://github.com/FirelyTeam/firely-terminal-pipeline)
- [Firely Helm Charts](https://github.com/FirelyTeam/Helm.Charts)
- [Vonk Helm Charts](https://github.com/FirelyTeam/Vonk.Helm.Charts)
- [Simplifier.net Registry](https://simplifier.net)
- [HL7 FHIR Specification](https://hl7.org/fhir/)
- [Firely Server Pricing (contact sales)](https://fire.ly/firely-server/)
- [Sign Up](https://simplifier.net/login)
- [Training](https://fire.ly/training/)
- [Consulting](https://fire.ly/services/)
- [Blog](https://fire.ly/blog/)
- [LinkedIn](https://www.linkedin.com/company/firely/)
- [Twitter](https://twitter.com/FirelyTeam)
- [YouTube](https://www.youtube.com/c/Firely)
- [Contact](https://fire.ly/contact/)
- [Customers](https://fire.ly/customers/)

## Features

- Firely Server (Vonk) — certified production FHIR server supporting FHIR R4, R4B, R5, and STU3
- G10, ONC Health IT, and ISiK (German interoperability) certifications
- MongoDB and SQL Server storage backends with flexible schemas
- Deployment on Windows, Linux, macOS, Docker, and Kubernetes via official Helm Charts
- Cloud-portable across Azure, AWS, Google Cloud, on-premise, and hybrid
- Native FHIR validation against profiles, extensions, and value sets
- SMART on FHIR authentication and authorization (latest version)
- Bulk Data Access (`$export`) for population-scale data exchange
- Terminology Service module (`$validate-code`, `$expand`, `$lookup`, `$translate`)
- FHIR Mapping Language engine and CDS Hooks support
- Subscriptions and PubSub for event-driven workflows
- Custom search parameters, conformance resources, and request/response interception
- Encryption at rest and in transit; event logging enabled by default
- Firely .NET SDK — official open-source C# FHIR library (de-facto reference SDK)
- Firely CQL SDK — Clinical Quality Language execution engine for .NET
- Firely Terminal — CLI for FHIR validation, FQL, FSH compilation, FHIRPath, package management
- Simplifier.net — global FHIR registry hosting 9,000+ projects and 40,000+ profiles
- Forge — desktop FHIR profile editor integrated with Simplifier
- Firely Validator API — standalone FHIR resource validation service
- FHIR Facade — adapter for exposing non-FHIR backends through a FHIR API
- Firely Server Ingest — high-volume FHIR data ingestion pipeline
- Firely Auth — SMART-on-FHIR-compatible authentication component
- Co-developers of HL7 FHIR (founders Ewout Kramer and Martijn Harthoorn on FHIR core team)
- Customers include UCSF, Humana, Roche, NHS, WHO, and Opala
- FHIR consulting, training, and implementation services

## Artifacts

| Artifact | File |
|----------|------|
| OpenAPI | [openapi/simplifier-package-api-openapi.yml](openapi/simplifier-package-api-openapi.yml) |

## Maintainers

- **FN:** Kin Lane
- **Email:** info@apievangelist.com
- **X:** [apievangelist](https://twitter.com/apievangelist)
- **URL:** [https://apievangelist.com](https://apievangelist.com)
