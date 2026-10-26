# Firely (firely-server)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
