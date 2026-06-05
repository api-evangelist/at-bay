# At-Bay (at-bay)

At-Bay is an InsurSec company that combines cyber insurance with proactive security monitoring for businesses. Headquartered in New York with offices in San Francisco and Tel Aviv, At-Bay underwrites Surplus Cyber, Surplus Tech E&O, and Surplus Miscellaneous Professional Liability (MPL) coverage and bundles them with the At-Bay Stance security platform (advisory, fraud defense, incident response) and 24/7 Managed Detection and Response (MDR) across endpoint, email (MXDR), and multi-vector surfaces. At-Bay distributes through a network of independent brokers and partners and exposes a production-grade REST Partner API (v2) that lets brokerage platforms, digital distributors, and agency management systems quote, customize, bind, renew, retrieve documents, and receive webhook callbacks for the full policy lifecycle. Demo environment at api-demo.at-bay.com lets partners integrate without going through Broker of Record clearance.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/at-bay/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/at-bay/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Insurance
- Cyber Insurance
- InsurSec
- Insurtech
- Tech E&O
- Professional Liability
- MPL
- Managed Detection And Response
- MDR
- Security Monitoring
- Email Security
- Endpoint Security
- Incident Response
- Brokers
- Quoting
- Binding
- Policy Lifecycle
- Webhooks

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### At-Bay Partner API

End-to-end Partner REST API (v2) for the At-Bay quote-to-bind-to-renew workflow. Supports three insurance products selected via the `insurance_product` field on the policy object: CYB (Surplus Cyber), TEO (Surplus Tech E&O), and MPL (Surplus MPL). Core operations: POST /quotes to submit a new quote, GET /quotes/{quote_identifier} polled every 10 seconds until status leaves `quote_pending` (typical p90 under 40 seconds), bind/referral/update operations, document upload and download, auto-renewal pause, plus webhook registration and verification for asynchronous status callbacks. JWT bearer authentication; production at api.at-bay.com/v2 and demo at api-demo.at-bay.com/v2. Production submissions are subject to Broker-of-Record (BOR) clearance — duplicate domains/addresses within 60 days are blocked; the demo environment bypasses BOR.

- **Human URL:** [https://developers.at-bay.com/docs/getting-started](https://developers.at-bay.com/docs/getting-started)
- **Base URL:** `https://api.at-bay.com/v2`

#### Tags

- Insurance
- Cyber Insurance
- Quoting
- Binding
- Policy Lifecycle

#### Properties

- [Documentation](https://developers.at-bay.com/docs/getting-started)
- [Reference](https://developers.at-bay.com/reference)
- [L L Ms](https://developers.at-bay.com/llms.txt)
- [OpenAPI](openapi/at-bay-partner-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/at-bay-partner-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/at-bay-partner-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/at-bay-quote-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/at-bay-policy-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/at-bay-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Common Properties

- [Website](https://www.at-bay.com)
- [Developer Portal](https://developers.at-bay.com)
- [Documentation](https://developers.at-bay.com/docs/getting-started)
- [Reference](https://developers.at-bay.com/reference)
- [L L Ms](https://developers.at-bay.com/llms.txt)
- [Partnerships](https://www.at-bay.com/about/partnerships/)
- [Brokers](https://www.at-bay.com/brokers/)
- [Broker Platform](https://www.at-bay.com/brokers/platform/)
- [Insurance](https://www.at-bay.com/insurance/)
- [Cyber Insurance](https://www.at-bay.com/insurance/cyber/)
- [Tech E O](https://www.at-bay.com/insurance/tech-eo/)
- [M P L](https://www.at-bay.com/insurance/mpl/)
- [Stance](https://www.at-bay.com/stance/)
- [M D R](https://www.at-bay.com/stance/mdr/)
- [Incident Response](https://www.at-bay.com/stance/incident-response/)
- [Newsroom](https://www.at-bay.com/news/)
- [About](https://www.at-bay.com/about/)
- [Careers](https://www.at-bay.com/careers/)
- [Contact](https://www.at-bay.com/contact/)
- [Login](https://platform.at-bay.com/)
- [Git Hub](https://github.com/at-bay)
- [LinkedIn](https://www.linkedin.com/company/at-bay-insurance)
- [Twitter](https://twitter.com/AtBayInsurance)
- [Plans](plans/at-bay-plans-pricing.yml)
- [Rate Limits](rate-limits/at-bay-rate-limits.yml)
- [Fin Ops](finops/at-bay-finops.yml)
- [Vocabulary](vocabulary/at-bay-vocabulary.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
