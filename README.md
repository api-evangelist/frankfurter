# Frankfurter (frankfurter)

Frankfurter is an open-source (MIT) currency exchange rates API that blends foreign-exchange reference rates published by 50+ central banks and monetary authorities. It hosts a free, no-key public endpoint at api.frankfurter.dev (current v2 and frozen v1) and ships as a Docker image for unlimited self-hosting. Historical data extends back to 1948 and covers 201 currencies; the API serves JSON, NDJSON, and CSV.

**URL:** [https://frankfurter.dev](https://frankfurter.dev)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Currency Exchange, Foreign Exchange, FX, Open Source, MIT, Self-Hosted, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Frankfurter API v2
Current Frankfurter API. Blended exchange rates across multiple institutional providers, one row per currency pair, with optional per-provider expansion, week/month downsampling, and NDJSON streaming.

**Human URL:** [https://frankfurter.dev/docs](https://frankfurter.dev/docs)

**Base URL:** `https://api.frankfurter.dev/v2`

#### Tags:

 - Currency Exchange, Rates, Currencies, Providers

#### Properties

- [Documentation](https://frankfurter.dev/docs)
- [OpenAPI](openapi/frankfurter-v2-openapi.yml)
- [Upstream OpenAPI](https://api.frankfurter.dev/v2/openapi.json)
- [NaftikoCapability](capabilities/v2-rates.yaml)
- [NaftikoCapability](capabilities/v2-currencies.yaml)
- [NaftikoCapability](capabilities/v2-providers.yaml)
- [JSONSchema](json-schema/v2-rate-schema.json)
- [JSONSchema](json-schema/v2-currency-schema.json)
- [JSONSchema](json-schema/v2-currency-detail-schema.json)
- [JSONSchema](json-schema/v2-provider-schema.json)
- [JSONStructure](json-structure/v2-rate-structure.json)
- [JSONStructure](json-structure/v2-currency-structure.json)
- [JSONStructure](json-structure/v2-currency-detail-structure.json)
- [JSONStructure](json-structure/v2-provider-structure.json)
- [JSON-LD](json-ld/frankfurter-v2-context.jsonld)
- [Example](examples/v2-rate-example.json)
- [Example](examples/v2-currency-example.json)
- [Example](examples/v2-currency-detail-example.json)
- [Example](examples/v2-provider-example.json)

### Frankfurter API v1
Frozen v1 Frankfurter API. ECB-style reference rates with single-base aggregate response shape (rates keyed by quote currency). Maintained for backward compatibility; new integrations should use v2.

**Human URL:** [https://frankfurter.dev/docs](https://frankfurter.dev/docs)

**Base URL:** `https://api.frankfurter.dev/v1`

#### Tags:

 - Currency Exchange, Current Rates, Historical Rates, Metadata

#### Properties

- [Documentation](https://frankfurter.dev/docs)
- [OpenAPI](openapi/frankfurter-v1-openapi.yml)
- [Upstream OpenAPI](https://api.frankfurter.dev/v1/openapi.json)
- [NaftikoCapability](capabilities/v1-current-rates.yaml)
- [NaftikoCapability](capabilities/v1-historical-rates.yaml)
- [NaftikoCapability](capabilities/v1-metadata.yaml)
- [JSONSchema](json-schema/v1-rates-on-date-schema.json)
- [JSONSchema](json-schema/v1-rates-by-date-schema.json)
- [JSONSchema](json-schema/v1-rates-schema.json)
- [JSONSchema](json-schema/v1-currencies-schema.json)
- [JSONSchema](json-schema/v1-amount-schema.json)
- [JSONSchema](json-schema/v1-base-schema.json)
- [JSONSchema](json-schema/v1-base-in-schema.json)
- [JSONSchema](json-schema/v1-date-schema.json)
- [JSONStructure](json-structure/v1-rates-on-date-structure.json)
- [JSONStructure](json-structure/v1-rates-by-date-structure.json)
- [JSONStructure](json-structure/v1-rates-structure.json)
- [JSONStructure](json-structure/v1-currencies-structure.json)
- [JSONStructure](json-structure/v1-amount-structure.json)
- [JSONStructure](json-structure/v1-base-structure.json)
- [JSONStructure](json-structure/v1-base-in-structure.json)
- [JSONStructure](json-structure/v1-date-structure.json)
- [JSON-LD](json-ld/frankfurter-v1-context.jsonld)
- [Example](examples/v1-rates-on-date-example.json)
- [Example](examples/v1-rates-by-date-example.json)
- [Example](examples/v1-currencies-example.json)

## Common Properties

- [Website](https://frankfurter.dev)
- [Documentation](https://frankfurter.dev/docs)
- [GitHubOrganization](https://github.com/lineofflight)
- [Frankfurter (canonical)](https://github.com/lineofflight/frankfurter)
- [Frankfurter MCP Server](https://github.com/lineofflight/frankfurter-mcp)
- [MIT License](https://github.com/lineofflight/frankfurter/blob/main/LICENSE)
- [Docker (Frankfurter)](https://hub.docker.com/r/lineofflight/frankfurter)
- [Docker (Frankfurter MCP)](https://ghcr.io/lineofflight/frankfurter-mcp)
- [MCP Server](https://github.com/lineofflight/frankfurter-mcp)
- [Hosted MCP Endpoint](https://mcp.frankfurter.dev/)
- [MCP Registry Listing](https://github.com/modelcontextprotocol/registry)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [Issues](https://github.com/lineofflight/frankfurter/issues)
- [Discussions](https://github.com/lineofflight/frankfurter/discussions)
- [SpectralRules](rules/frankfurter-spectral-rules.yml)
- [Vocabulary](vocabulary/frankfurter-vocabulary.yml)
- [Plans](plans/frankfurter-plans-pricing.yml)
- [RateLimits](rate-limits/frankfurter-rate-limits.yml)

## Features

| Name | Description |
|------|-------------|
| Blended Reference Rates | Combines daily FX rates from 50+ central banks and monetary authorities into a consensus-filtered, outlier-rejecting blend. |
| Multi-Format Output | JSON, NDJSON (streamed), and CSV from the same endpoint. |
| Historical Time Series | Daily rates back to 1948 with optional week/month downsampling. |
| 201 Currencies | Active and legacy currency coverage with ISO 4217 metadata. |
| Per-Provider Expansion | `expand=providers` exposes each provider's individual quote so callers can audit the blend, with `excluded: true` flags on outliers and peg overrides. |
| No Authentication | No keys, no accounts, no monthly or daily caps. |
| Self-Hostable | Single Docker image with optional SQLite volume mount. |
| Free Upstream Provider Keys | Optional, no-cost provider keys for Bank Al-Maghrib, Banco de México, Banco Central de Chile, Bank of Thailand, US Federal Reserve, and the Turkish Central Bank widen self-hosted coverage. |
| Open CORS | GET and OPTIONS allowed from any origin — direct browser use. |
| Open Source (MIT) | Full source on GitHub; community contributions and fork-friendly. |

## Use Cases

| Name | Description |
|------|-------------|
| Treasury and Payments Pricing | Embed blended FX rates into invoicing, payouts, and conversion. |
| E-commerce Storefront Localization | Convert displayed prices into the visitor's currency on page load. |
| Reporting and Analytics | Backfill historical FX into BI dashboards and finance reports. |
| Reference Data Maintenance | Sync ISO 4217 currency tables and provider metadata into ERPs. |
| AI Assistant Tooling | Equip Claude and other MCP-capable agents with the official Frankfurter MCP server (get_rates, convert, list_currencies, list_providers). |
| Private FX Service | Self-host inside a VPC for compliance-sensitive workloads. |
| Academic and Research | Long historical series for FX econometric studies. |

## Integrations

| Name | Description |
|------|-------------|
| European Central Bank | Primary upstream provider (ECB reference rates). |
| US Federal Reserve | Optional upstream provider via free FED API key. |
| Bank of Canada | Upstream provider (BOC) included in the blend. |
| Banco Central do Brasil | Upstream provider (BCB). |
| Turkish Central Bank | Optional upstream provider via free TCMB key. |
| Bank of Thailand | Optional upstream provider via free BOT key. |
| Banco Central de Chile | Optional upstream provider via free BCCh key. |
| Banco de México | Optional upstream provider via free Banxico key. |
| Bank Al-Maghrib (Morocco) | Optional upstream provider via free BAM key. |
| Model Context Protocol | Official MCP server (lineofflight/frankfurter-mcp) registered at the MCP registry. |
| Docker Hub / GHCR | Container distribution for self-hosting. |
| GitHub Discussions | Community 'Show and Tell' for libraries and tools built on Frankfurter. |

## Solutions

| Name | Description |
|------|-------------|
| Public Hosted (Free) | api.frankfurter.dev — no key, soft fair-use limits, ideal for prototypes and low-volume production. |
| Self-Hosted FOSS | Run lineofflight/frankfurter via Docker; no application-level rate limit. |
| MCP Tooling | Drop the Frankfurter MCP server into any Claude / agent stack for natural-language FX access. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [frankfurter-v1-openapi.yml](openapi/frankfurter-v1-openapi.yml)
- [frankfurter-v2-openapi.yml](openapi/frankfurter-v2-openapi.yml)

### JSON Schema

- [v1-amount-schema.json](json-schema/v1-amount-schema.json)
- [v1-base-in-schema.json](json-schema/v1-base-in-schema.json)
- [v1-base-schema.json](json-schema/v1-base-schema.json)
- [v1-currencies-schema.json](json-schema/v1-currencies-schema.json)
- [v1-date-schema.json](json-schema/v1-date-schema.json)
- [v1-rates-by-date-schema.json](json-schema/v1-rates-by-date-schema.json)
- [v1-rates-on-date-schema.json](json-schema/v1-rates-on-date-schema.json)
- [v1-rates-schema.json](json-schema/v1-rates-schema.json)
- [v2-currency-detail-schema.json](json-schema/v2-currency-detail-schema.json)
- [v2-currency-schema.json](json-schema/v2-currency-schema.json)
- [v2-provider-schema.json](json-schema/v2-provider-schema.json)
- [v2-rate-schema.json](json-schema/v2-rate-schema.json)

### JSON Structure

- [v1-amount-structure.json](json-structure/v1-amount-structure.json)
- [v1-base-in-structure.json](json-structure/v1-base-in-structure.json)
- [v1-base-structure.json](json-structure/v1-base-structure.json)
- [v1-currencies-structure.json](json-structure/v1-currencies-structure.json)
- [v1-date-structure.json](json-structure/v1-date-structure.json)
- [v1-rates-by-date-structure.json](json-structure/v1-rates-by-date-structure.json)
- [v1-rates-on-date-structure.json](json-structure/v1-rates-on-date-structure.json)
- [v1-rates-structure.json](json-structure/v1-rates-structure.json)
- [v2-currency-detail-structure.json](json-structure/v2-currency-detail-structure.json)
- [v2-currency-structure.json](json-structure/v2-currency-structure.json)
- [v2-provider-structure.json](json-structure/v2-provider-structure.json)
- [v2-rate-structure.json](json-structure/v2-rate-structure.json)

### JSON-LD

- [frankfurter-v1-context.jsonld](json-ld/frankfurter-v1-context.jsonld)
- [frankfurter-v2-context.jsonld](json-ld/frankfurter-v2-context.jsonld)

### Examples

- [v1-amount-example.json](examples/v1-amount-example.json)
- [v1-base-example.json](examples/v1-base-example.json)
- [v1-base-in-example.json](examples/v1-base-in-example.json)
- [v1-currencies-example.json](examples/v1-currencies-example.json)
- [v1-date-example.json](examples/v1-date-example.json)
- [v1-rates-by-date-example.json](examples/v1-rates-by-date-example.json)
- [v1-rates-example.json](examples/v1-rates-example.json)
- [v1-rates-on-date-example.json](examples/v1-rates-on-date-example.json)
- [v2-currency-detail-example.json](examples/v2-currency-detail-example.json)
- [v2-currency-example.json](examples/v2-currency-example.json)
- [v2-provider-example.json](examples/v2-provider-example.json)
- [v2-rate-example.json](examples/v2-rate-example.json)

## Capabilities

Self-contained Naftiko capabilities — one file per business surface (OpenAPI tag), each inlining its consumes, REST exposer, and MCP exposer.

| Capability | API | Tools | File |
|---|---|---|---|
| Frankfurter API — current-rates | v1 | 1 | [v1-current-rates.yaml](capabilities/v1-current-rates.yaml) |
| Frankfurter API — historical-rates | v1 | 3 | [v1-historical-rates.yaml](capabilities/v1-historical-rates.yaml) |
| Frankfurter API — metadata | v1 | 1 | [v1-metadata.yaml](capabilities/v1-metadata.yaml) |
| Frankfurter API — Currencies | v2 | 2 | [v2-currencies.yaml](capabilities/v2-currencies.yaml) |
| Frankfurter API — Providers | v2 | 1 | [v2-providers.yaml](capabilities/v2-providers.yaml) |
| Frankfurter API — Rates | v2 | 2 | [v2-rates.yaml](capabilities/v2-rates.yaml) |

## Rules

- [frankfurter-spectral-rules.yml](rules/frankfurter-spectral-rules.yml) — 37 Spectral rules enforcing Frankfurter API conventions

## Vocabulary

- [frankfurter-vocabulary.yml](vocabulary/frankfurter-vocabulary.yml) — 3 resources, 5 actions, 6 workflows, 4 personas

## Plans

- [frankfurter-plans-pricing.yml](plans/frankfurter-plans-pricing.yml) — 2 plan(s) (Public Hosted (Free), Self-Hosted (FOSS))

## Rate Limits

- [frankfurter-rate-limits.yml](rate-limits/frankfurter-rate-limits.yml) — 2 limits, 5 policies

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
