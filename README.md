# ClearVIN (clearvin)

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
