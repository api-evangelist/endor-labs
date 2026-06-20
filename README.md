# Endor Labs (endor-labs)

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
