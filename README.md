# ClearVIN (clearvin)

ClearVIN is a vehicle-history and VIN data provider and an approved NMVTIS data provider. Its REST API decodes North American (U.S. and Canada) VINs into 100+ specification data points and returns full vehicle history reports - title, junk / salvage / total-loss records, odometer events, and market valuation - sourced directly from government and industry data, covering model years 1981 to present.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/clearvin/refs/heads/main/apis.yml)

## Tags

- VIN
- Vehicle History
- Automotive
- NMVTIS
- Vehicle Data

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### VIN Decode API

Breaks a North American VIN into 100+ data points - year, make, model, trim, engine, technical VIN specs, standard features, and recall data - via ClearVIN's proprietary decoder over the shared report endpoint.

- **Human URL:** [https://www.clearvin.com/en/api-subscribers/vin-decode-api/](https://www.clearvin.com/en/api-subscribers/vin-decode-api/)
- **Base URL:** `https://www.clearvin.com/rest/vendor`

#### Tags

- VIN
- Decode
- Vehicle Specifications

#### Properties

- [Documentation](https://www.clearvin.com/en/api-subscribers/vin-decode-api/)
- [OpenAPI](openapi/clearvin-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/clearvin.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/clearvin.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vehicle History Report API

Full vehicle history report from the NMVTIS government database and industry sources - DMV title records, brand codes, junk / salvage / total-loss events, insurance claims, odometer / mileage history, and market valuation - returned by VIN from the report endpoint as JSON or HTML.

- **Human URL:** [https://www.clearvin.com/en/api-subscribers/nmvtis-history-api/](https://www.clearvin.com/en/api-subscribers/nmvtis-history-api/)
- **Base URL:** `https://www.clearvin.com/rest/vendor`

#### Tags

- Vehicle History
- NMVTIS
- Title

#### Properties

- [Documentation](https://www.clearvin.com/en/api-subscribers/nmvtis-history-api/)
- [OpenAPI](openapi/clearvin-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/clearvin.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/clearvin.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Report Preview API

Retrieves a report by VIN with the format query parameter to obtain an HTML rendering or summary view of available data before pulling the full report. Exact preview parameters are not separately documented and require reconciliation.

- **Human URL:** [https://www.clearvin.com/en/api-subscribers/](https://www.clearvin.com/en/api-subscribers/)
- **Base URL:** `https://www.clearvin.com/rest/vendor`

#### Tags

- Preview
- Sample
- Report

#### Properties

- [Documentation](https://www.clearvin.com/en/api-subscribers/)
- [OpenAPI](openapi/clearvin-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/clearvin.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/clearvin.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Account Authentication API

Exchanges account email and password for a JWT bearer token (valid 120 minutes) used to authorize report requests. Requests must originate from a registered IP address. Account credit balance is managed through the ClearVIN account and is not exposed via a separately documented public endpoint.

- **Human URL:** [https://www.clearvin.com/en/api-subscribers/](https://www.clearvin.com/en/api-subscribers/)
- **Base URL:** `https://www.clearvin.com/rest/vendor`

#### Tags

- Authentication
- Account
- Token

#### Properties

- [Documentation](https://www.clearvin.com/en/api-subscribers/)
- [OpenAPI](openapi/clearvin-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/clearvin.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/clearvin.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/clearvin)
- [Website](https://www.clearvin.com/)
- [Documentation](https://www.clearvin.com/en/api-subscribers/)
- [Plans](plans/clearvin-plans-pricing.yml)
- [Rate Limits](rate-limits/clearvin-rate-limits.yml)
- [Fin Ops](finops/clearvin-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
