# Firely

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

**Areas:** FHIR · HL7 · Healthcare · Health IT · Interoperability · Clinical Data · FHIR Server · Vonk · Simplifier · Forge · Terminology · SMART on FHIR

## Firely on APIs.io

Everything profiled for Firely is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/firely-server/](https://apis.io/providers/firely-server/)** — or go straight to one of the APIs or properties below.

### APIs (3)

- [Firely Server FHIR REST API](https://apis.io/apis/firely-server/firely-server-fhir-rest-api/) — Every Firely Server (formerly Vonk) instance exposes the standard HL7 FHIR REST API contract — type-level and instance-level CRUD, search, history,…
- [Firely Catalog API](https://apis.io/apis/firely-server/firely-server-catalog-api/) — The Catalog API from Firely — 1 operation(s) for catalog.
- [Firely Simplifier.net FHIR Package API](https://apis.io/apis/firely-server/firely-server-simplifier-net-fhir-package-api-api/) — The Simplifier.net FHIR Package API API from Firely — 2 operation(s) for simplifier.net fhir package api.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Firely Server Agentic Access](https://apis.io/agentic-access/firely-server/firely-server-agentic-access/)

#### Collections (3)

Postman and Open Collection request collections.

- [Simplifier.net FHIR Package Catalog API](https://apis.io/collections/firely-server/open-firely-server-catalog-api/)
- [Simplifier.net FHIR Package Catalog Simplifier.net FHIR Package API API](https://apis.io/collections/firely-server/open-firely-server-simplifier-net-fhir-package-api-api/)
- [Simplifier.net FHIR Package API](https://apis.io/collections/firely-server/open-simplifier-package-api/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Firely Server Domain Security](https://apis.io/security/firely-server/firely-server-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://fire.ly)
- [Documentation](https://docs.fire.ly/projects/Firely-Server/)
- [Pricing](https://fire.ly/firely-server/)
- [Blog](https://fire.ly/blog/)
- [GitHub](https://github.com/FirelyTeam)

## API Evangelist rating

**Kin Score 26.9** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 48.6 |
| Contract governance | 0.0 |
| Operational transparency | 2.6 |
| Developer ergonomics | 35.7 |
| Access clarity | 13.2 |

**Agent readiness 22.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 4.7** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/firely-server/](https://apis.io/providers/firely-server/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Firely: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/firely-server/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
