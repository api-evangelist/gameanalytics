# GameAnalytics (gameanalytics)

GameAnalytics is a free analytics platform purpose-built for games, used to track player behavior, retention and cohorts, progression funnels, in-game economy and resource flows, and monetization and ads analytics. Data is collected through the HMAC-signed Collection (Collector) REST API or platform SDKs, queried through the Metrics API, streamed to a customer's own cloud via PipelineIQ Data Export, and administered through the Organization API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/gameanalytics/refs/heads/main/apis.yml)

## Tags

- Analytics
- Games
- Gaming
- Player Behavior
- Retention
- Monetization
- Ad Analytics
- Telemetry

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### GameAnalytics Collection API

HMAC-SHA256 authenticated REST ingestion API for submitting game events. Clients POST an init request to /v2/{game_key}/init for a server timestamp and enabled flag, then batch and POST event objects (user/session, business, resource, progression, design, error, ad) to /v2/{game_key}/events, signing the gzipped JSON body with the game's secret key.

- **Human URL:** [https://docs.gameanalytics.com/event-tracking-and-integrations/sdks-and-collection-api/api/setup/](https://docs.gameanalytics.com/event-tracking-and-integrations/sdks-and-collection-api/api/setup/)
- **Base URL:** `https://api.gameanalytics.com/v2`

#### Tags

- Collection
- Collector
- Event Ingestion
- Telemetry
- HMAC

#### Properties

- [Documentation](https://docs.gameanalytics.com/event-tracking-and-integrations/sdks-and-collection-api/api/setup/)
- [API Reference](https://docs.gameanalytics.com/event-tracking-and-integrations/sdks-and-collection-api/api/collector)
- [OpenAPI](openapi/gameanalytics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gameanalytics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gameanalytics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GameAnalytics Metrics API

X-API-Key authenticated reporting API that returns aggregated gameplay metrics - DAU/MAU, retention (retention_retro), ARPU/ARPPU/ARPDAU, session length, revenue and ad revenue - as JSON, queried by POSTing an interval, granularity, and a group/split/timeseries query object per metric.

- **Human URL:** [https://docs.gameanalytics.com/products-and-features/pipeline-iq/metrics-api/how-to-use-the-metrics-api/](https://docs.gameanalytics.com/products-and-features/pipeline-iq/metrics-api/how-to-use-the-metrics-api/)
- **Base URL:** `https://metrics.gameanalytics.com/metrics/v1`

#### Tags

- Metrics
- Reporting
- Retention
- DAU
- MAU
- ARPU

#### Properties

- [Documentation](https://docs.gameanalytics.com/products-and-features/pipeline-iq/metrics-api/how-to-use-the-metrics-api/)
- [API Reference](https://docs.gameanalytics.com/products-and-features/pipeline-iq/metrics-api/query-examples/)
- [OpenAPI](openapi/gameanalytics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gameanalytics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gameanalytics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GameAnalytics Organization API

API-key authenticated administration API for programmatically managing games, studios, users, and user access permissions (ACLs) across a GameAnalytics organization, including inviting users and uploading game icons.

- **Human URL:** [https://docs.gameanalytics.com/products-and-features/pipeline-iq/organization-api/api-specification/](https://docs.gameanalytics.com/products-and-features/pipeline-iq/organization-api/api-specification/)
- **Base URL:** `https://organization.gameanalytics.com/api/v1`

#### Tags

- Organization
- Administration
- Games
- Studios
- Users
- Permissions

#### Properties

- [Documentation](https://docs.gameanalytics.com/products-and-features/pipeline-iq/organization-api/overview-and-use-cases)
- [API Reference](https://docs.gameanalytics.com/products-and-features/pipeline-iq/organization-api/api-specification/)
- [OpenAPI](openapi/gameanalytics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/gameanalytics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/gameanalytics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### GameAnalytics Data Export (PipelineIQ)

PipelineIQ raw data export streams every gameplay event as JSON objects (a metadata wrapper plus an event data object) in real time, with historical backfill, into a customer's own cloud environment - AWS S3, Google BigQuery, Google Cloud Storage - for use in Tableau, Looker, or Power BI. It is a data pipeline rather than a request/response REST API.

- **Human URL:** [https://www.gameanalytics.com/pipelineiq/data-export](https://www.gameanalytics.com/pipelineiq/data-export)
- **Base URL:** `https://docs.gameanalytics.com/products-and-features/pipeline-iq/data-export/json-schemas/`

#### Tags

- Data Export
- PipelineIQ
- Raw Events
- Streaming
- Data Warehouse

#### Properties

- [Documentation](https://www.gameanalytics.com/pipelineiq/data-export)
- [API Reference](https://docs.gameanalytics.com/products-and-features/pipeline-iq/data-export/json-schemas/)

## Common Properties

- [GitHub Organization](https://github.com/GameAnalytics)
- [LinkedIn](https://www.linkedin.com/company/gameanalytics)
- [Website](https://gameanalytics.com/)
- [Documentation](https://docs.gameanalytics.com/)
- [Plans](plans/gameanalytics-plans-pricing.yml)
- [Rate Limits](rate-limits/gameanalytics-rate-limits.yml)
- [Fin Ops](finops/gameanalytics-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
