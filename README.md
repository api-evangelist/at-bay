# At-Bay (at-bay)

At-Bay is an InsurSec company that pairs cyber insurance with proactive security monitoring. Underwrites Surplus Cyber, Surplus Tech E&O, and Surplus Miscellaneous Professional Liability (MPL) coverage and bundles them with the At-Bay Stance platform — advisory, fraud defense, incident response — and 24/7 Managed Detection and Response (MDR) across endpoint, email (MXDR), and multi-vector surfaces. Distribution is through independent brokerages and partner platforms, integrated via a production REST Partner API (v2).

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/at-bay/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Insurance, Cyber Insurance, InsurSec, Tech E&O, MPL, Managed Detection And Response, MDR, Security Monitoring, Brokers, Quoting, Binding, Policy Lifecycle, Webhooks

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Products

| Code | Product | Notes |
|---|---|---|
| CYB | Surplus Cyber | First-party + third-party cyber coverage. |
| TEO | Surplus Tech E&O | Tech errors and omissions for technology companies. |
| MPL | Surplus MPL | Miscellaneous professional liability. |
| Stance | Security platform | Advisory, fraud defense, incident response. |
| MDR | Managed Detection and Response | 24/7 endpoint, email (MXDR), and multi-vector monitoring. |

## APIs

### At-Bay Partner API

End-to-end Partner REST API (v2) for the At-Bay quote-to-bind-to-renew workflow. Authentication is HTTP Bearer with a JWT (~150–200 chars). Quote creation is asynchronous: `POST /quotes` returns a `quote_identifier` and `company_id`, then poll `GET /quotes/{quote_identifier}` every ~10 seconds (p90 completion under 40 seconds). Production submissions are subject to Broker-of-Record (BOR) clearance — duplicate domains/addresses within 60 days are blocked; the demo host bypasses BOR.

**Human URL:** [https://developers.at-bay.com/docs/getting-started](https://developers.at-bay.com/docs/getting-started)

**Reference:** [https://developers.at-bay.com/reference](https://developers.at-bay.com/reference)

**Base URLs:**
- Production: `https://api.at-bay.com/v2`
- Demo: `https://api-demo.at-bay.com/v2`

- [OpenAPI](openapi/at-bay-partner-api-openapi.yml)
- [JSON Schema — Quote](json-schema/at-bay-quote-schema.json)
- [JSON Schema — Policy](json-schema/at-bay-policy-schema.json)
- [JSON Structure — Quote](json-structure/at-bay-quote-structure.json)
- [JSON-LD Context](json-ld/at-bay-context.jsonld)
- [Naftiko Capability — Quotes](capabilities/quotes.yaml)
- [Naftiko Capability — Binding](capabilities/binding.yaml)
- [Naftiko Capability — Documents](capabilities/documents.yaml)
- [Naftiko Capability — Webhooks](capabilities/webhooks.yaml)
- [Naftiko Capability — Policies](capabilities/policies.yaml)
- [Spectral Rules](rules/at-bay-rules.yml)
- [Example — Create Quote](examples/at-bay-create-quote-example.json)
- [Example — Get Quote](examples/at-bay-get-quote-example.json)
- [Example — Register Webhook](examples/at-bay-register-webhook-example.json)

## Plans, Rate Limits, FinOps

- [Plans & Pricing](plans/at-bay-plans-pricing.yml)
- [Rate Limits](rate-limits/at-bay-rate-limits.yml)
- [FinOps](finops/at-bay-finops.yml)
- [Vocabulary](vocabulary/at-bay-vocabulary.yml)

## Common Links

- [Website](https://www.at-bay.com)
- [Developer Portal](https://developers.at-bay.com)
- [LLMs Index](https://developers.at-bay.com/llms.txt)
- [Partnerships](https://www.at-bay.com/about/partnerships/)
- [Brokers](https://www.at-bay.com/brokers/)
- [Broker Platform](https://www.at-bay.com/brokers/platform/)
- [Stance Security Platform](https://www.at-bay.com/stance/)
- [MDR](https://www.at-bay.com/stance/mdr/)
- [Incident Response](https://www.at-bay.com/stance/incident-response/)
- [GitHub](https://github.com/at-bay)
- [LinkedIn](https://www.linkedin.com/company/at-bay-insurance)

## Maintainers

- Kin Lane — kin@apievangelist.com
