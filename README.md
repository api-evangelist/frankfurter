# Frankfurter (frankfurter)

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

Frankfurter is an open-source (MIT) currency exchange rates API that blends foreign-exchange reference rates published by 50+ central banks and monetary authorities. It hosts a free, no-key public endpoint at api.frankfurter.dev (current v2 and frozen v1) and ships as a Docker image for unlimited self-hosting. Historical data extends back to 1948 and covers 201 currencies; the API serves JSON, NDJSON, and CSV.

**APIs.json:** [https://frankfurter.dev](https://frankfurter.dev)

## Tags

- Currency Exchange
- Foreign Exchange
- FX
- Open Source
- MIT
- Self-Hosted
- Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Frankfurter API v2

Current Frankfurter API. Blended exchange rates across multiple institutional providers, one row per currency pair, with optional per-provider expansion, week/month downsampling, and NDJSON streaming.

- **Human URL:** [https://frankfurter.dev/docs](https://frankfurter.dev/docs)
- **Base URL:** `https://api.frankfurter.dev/v2`

#### Tags

- Currency Exchange
- Rates
- Currencies
- Providers

#### Properties

- [Documentation](https://frankfurter.dev/docs)
- [OpenAPI](openapi/frankfurter-v2-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/frankfurter-v2.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/frankfurter-v2.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://api.frankfurter.dev/v2/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [JSON Schema](json-schema/v2-rate-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/v2-currency-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/v2-currency-detail-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/v2-provider-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/v2-rate-structure.json)
- [JSON Structure](json-structure/v2-currency-structure.json)
- [JSON Structure](json-structure/v2-currency-detail-structure.json)
- [JSON Structure](json-structure/v2-provider-structure.json)
- [J S O N- L D](json-ld/frankfurter-v2-context.jsonld)
- [Example](examples/v2-rate-example.json)
- [Example](examples/v2-currency-example.json)
- [Example](examples/v2-currency-detail-example.json)
- [Example](examples/v2-provider-example.json)

### Frankfurter API v1

Frozen v1 Frankfurter API. ECB-style reference rates with single-base aggregate response shape (rates keyed by quote currency). Maintained for backward compatibility; new integrations should use v2.

- **Human URL:** [https://frankfurter.dev/docs](https://frankfurter.dev/docs)
- **Base URL:** `https://api.frankfurter.dev/v1`

#### Tags

- Currency Exchange
- Current Rates
- Historical Rates
- Metadata

#### Properties

- [Documentation](https://frankfurter.dev/docs)
- [OpenAPI](openapi/frankfurter-v1-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/frankfurter-v1.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/frankfurter-v1.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [OpenAPI](https://api.frankfurter.dev/v1/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [JSON Schema](json-schema/v1-rates-on-date-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/v1-rates-by-date-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/v1-rates-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/v1-currencies-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/v1-amount-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/v1-base-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/v1-base-in-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/v1-date-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/v1-rates-on-date-structure.json)
- [JSON Structure](json-structure/v1-rates-by-date-structure.json)
- [JSON Structure](json-structure/v1-rates-structure.json)
- [JSON Structure](json-structure/v1-currencies-structure.json)
- [JSON Structure](json-structure/v1-amount-structure.json)
- [JSON Structure](json-structure/v1-base-structure.json)
- [JSON Structure](json-structure/v1-base-in-structure.json)
- [JSON Structure](json-structure/v1-date-structure.json)
- [J S O N- L D](json-ld/frankfurter-v1-context.jsonld)
- [Example](examples/v1-rates-on-date-example.json)
- [Example](examples/v1-rates-by-date-example.json)
- [Example](examples/v1-currencies-example.json)

## Common Properties

- [Website](https://frankfurter.dev)
- [Documentation](https://frankfurter.dev/docs)
- [GitHub Organization](https://github.com/lineofflight)
- [GitHub Repository](https://github.com/lineofflight/frankfurter)
- [GitHub Repository](https://github.com/lineofflight/frankfurter-mcp)
- [License](https://github.com/lineofflight/frankfurter/blob/main/LICENSE)
- [Container Image](https://hub.docker.com/r/lineofflight/frankfurter)
- [Container Image](https://ghcr.io/lineofflight/frankfurter-mcp)
- [Tools](https://github.com/lineofflight/frankfurter-mcp)
- [Tools](https://mcp.frankfurter.dev/)
- [Tools](https://github.com/modelcontextprotocol/registry)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [Issues](https://github.com/lineofflight/frankfurter/issues)
- [Discussions](https://github.com/lineofflight/frankfurter/discussions)
- [Spectral Rules](rules/frankfurter-spectral-rules.yml)
- [Vocabulary](vocabulary/frankfurter-vocabulary.yml)
- [Plans](plans/frankfurter-plans-pricing.yml)
- [Rate Limits](rate-limits/frankfurter-rate-limits.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
