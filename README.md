# Endor Labs (endor-labs)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Endor Labs is a software supply chain security and application security platform built around reachability-based Software Composition Analysis (SCA), SBOM/VEX, secrets and SAST scanning, CI/CD discovery, and AI security. Its public REST API at https://api.endorlabs.com/v1 is a uniform resource API over namespaces, exposing projects, packages, findings, policies, scan results, and more, driven by the endorctl CLI.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/endor-labs/refs/heads/main/apis.yml)

## Tags

- Security
- Software Supply Chain
- SCA
- Reachability
- AppSec
- AI Security

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Endor Labs Projects API

List, get, and create Project resources - the logical root of all scanned source code, repositories, and package manager references - under a namespace via /v1/namespaces/{namespace}/projects.

- **Human URL:** [https://docs.endorlabs.com/rest-api/](https://docs.endorlabs.com/rest-api/)
- **Base URL:** `https://api.endorlabs.com/v1`

#### Tags

- Projects
- Repositories
- Inventory

#### Properties

- [Documentation](https://docs.endorlabs.com/rest-api/using-the-rest-api/getting-started/)
- [API Reference](https://docs.endorlabs.com/api/)
- [OpenAPI](openapi/endor-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/endor-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/endor-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Endor Labs Dependencies & Packages API

Query PackageVersion and DependencyMetadata resources - ecosystem, package name, version, and importer/dependency relationships - powering reachability-based Software Composition Analysis.

- **Human URL:** [https://docs.endorlabs.com/rest-api/using-the-rest-api/data-model/resource-kinds/](https://docs.endorlabs.com/rest-api/using-the-rest-api/data-model/resource-kinds/)
- **Base URL:** `https://api.endorlabs.com/v1`

#### Tags

- Packages
- Dependencies
- SCA

#### Properties

- [Documentation](https://docs.endorlabs.com/rest-api/using-the-rest-api/data-model/resource-kinds/)
- [API Reference](https://docs.endorlabs.com/api/)
- [OpenAPI](openapi/endor-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/endor-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/endor-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Endor Labs Findings API

List and get Finding resources - detected problems requiring remediation including reachable vulnerabilities, license risks, malware, secrets, and SAST results - filtered and field-masked under a namespace.

- **Human URL:** [https://docs.endorlabs.com/rest-api/using-the-rest-api/use-cases/](https://docs.endorlabs.com/rest-api/using-the-rest-api/use-cases/)
- **Base URL:** `https://api.endorlabs.com/v1`

#### Tags

- Findings
- Vulnerabilities
- Reachability

#### Properties

- [Documentation](https://docs.endorlabs.com/rest-api/using-the-rest-api/use-cases/)
- [API Reference](https://docs.endorlabs.com/api/)
- [OpenAPI](openapi/endor-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/endor-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/endor-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Endor Labs Policies API

Create, list, get, update, and delete Policy resources that define rules, queries, and target resource kinds for governing findings, releases, and remediation across namespaces.

- **Human URL:** [https://docs.endorlabs.com/rest-api/](https://docs.endorlabs.com/rest-api/)
- **Base URL:** `https://api.endorlabs.com/v1`

#### Tags

- Policies
- Governance
- Guardrails

#### Properties

- [Documentation](https://docs.endorlabs.com/rest-api/)
- [API Reference](https://docs.endorlabs.com/api/)
- [OpenAPI](openapi/endor-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/endor-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/endor-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Endor Labs Scan Results API

Retrieve ScanResult and Metric resources capturing scan execution configuration, findings produced, triggered policies, and diagnostics for a project under a namespace.

- **Human URL:** [https://docs.endorlabs.com/rest-api/using-the-rest-api/data-model/resource-kinds/](https://docs.endorlabs.com/rest-api/using-the-rest-api/data-model/resource-kinds/)
- **Base URL:** `https://api.endorlabs.com/v1`

#### Tags

- Scan Results
- Metrics
- Diagnostics

#### Properties

- [Documentation](https://docs.endorlabs.com/rest-api/using-the-rest-api/data-model/resource-kinds/)
- [API Reference](https://docs.endorlabs.com/api/)
- [OpenAPI](openapi/endor-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/endor-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/endor-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Endor Labs Auth & Namespaces API

Exchange an API key and secret for a bearer access token via POST /v1/auth/api-key, and list the namespaces (tenants and child namespaces) a token is authorized to access.

- **Human URL:** [https://docs.endorlabs.com/rest-api/authentication/](https://docs.endorlabs.com/rest-api/authentication/)
- **Base URL:** `https://api.endorlabs.com/v1`

#### Tags

- Authentication
- Namespaces
- Tenancy

#### Properties

- [Documentation](https://docs.endorlabs.com/rest-api/authentication/)
- [API Reference](https://docs.endorlabs.com/api/)
- [OpenAPI](openapi/endor-labs-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/endor-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/endor-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/endorlabs)
- [LinkedIn](https://www.linkedin.com/company/endor-labs)
- [Website](https://www.endorlabs.com)
- [Documentation](https://docs.endorlabs.com/rest-api/)
- [Plans](plans/endor-labs-plans-pricing.yml)
- [Rate Limits](rate-limits/endor-labs-rate-limits.yml)
- [Fin Ops](finops/endor-labs-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
