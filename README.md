# Frankfurter (frankfurter)

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
