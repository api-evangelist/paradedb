# ParadeDB (paradedb)

ParadeDB is an open-source Postgres extension stack (pg_search for BM25 full-text search and pg_analytics for columnar OLAP) that turns PostgreSQL into a real-time search and analytics engine, positioned as an Elasticsearch alternative. Its interface is SQL over the PostgreSQL wire protocol - custom operators (@@@) and paradedb.* functions - not a REST API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/paradedb/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/paradedb/refs/heads/main/apis.yml)

## Tags

- Search
- Full-Text Search
- Analytics
- PostgreSQL
- Database
- Elasticsearch Alternative

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### ParadeDB pg_search (Full-Text Search)

BM25 full-text search inside Postgres via the pg_search extension, built on Tantivy. Consumed as SQL over the PostgreSQL wire protocol - BM25 indexes are created with CREATE INDEX ... USING bm25, queried with the @@@ operator, and scored or highlighted with paradedb.score() and paradedb.snippet(). No REST API.

- **Human URL:** [https://docs.paradedb.com/documentation/full-text/overview](https://docs.paradedb.com/documentation/full-text/overview)
- **Base URL:** `postgresql://`

#### Tags

- Full-Text Search
- BM25
- Search
- SQL

#### Properties

- [Documentation](https://docs.paradedb.com/documentation/full-text/overview)
- [API Reference](https://docs.paradedb.com/documentation/getting-started/quickstart)
- [GitHub](https://github.com/paradedb/paradedb)
- [OpenAPI](openapi/paradedb-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paradedb.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paradedb.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ParadeDB Analytics (pg_analytics)

Columnar storage, fast aggregates, and OLAP-style analytics over Postgres data, powered by Apache DataFusion and Postgres parallel workers. Accessed entirely through standard SQL aggregate queries over the PostgreSQL wire protocol - there is no REST interface.

- **Human URL:** [https://docs.paradedb.com/documentation/aggregates/overview](https://docs.paradedb.com/documentation/aggregates/overview)
- **Base URL:** `postgresql://`

#### Tags

- Analytics
- OLAP
- Columnar
- SQL

#### Properties

- [Documentation](https://docs.paradedb.com/documentation/aggregates/overview)
- [GitHub](https://github.com/paradedb/paradedb)
- [OpenAPI](openapi/paradedb-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paradedb.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paradedb.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ParadeDB Postgres SQL Interface

The primary integration surface for ParadeDB - the PostgreSQL wire protocol itself. Any standard Postgres client, driver, or ORM (psql, libpq, Drizzle, Django, SQLAlchemy, Rails, EF Core) connects over the wire protocol and invokes ParadeDB features as SQL functions, operators, and index access methods. ParadeDB exposes no HTTP/REST or WebSocket API.

- **Human URL:** [https://docs.paradedb.com/welcome/introduction](https://docs.paradedb.com/welcome/introduction)
- **Base URL:** `postgresql://`

#### Tags

- PostgreSQL
- SQL
- Wire Protocol
- Interface

#### Properties

- [Documentation](https://docs.paradedb.com/welcome/introduction)
- [GitHub](https://github.com/paradedb/paradedb)
- [OpenAPI](openapi/paradedb-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/paradedb.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/paradedb.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/paradedb)
- [LinkedIn](https://www.linkedin.com/company/paradedb)
- [Website](https://www.paradedb.com)
- [Documentation](https://docs.paradedb.com)
- [Plans](plans/paradedb-plans-pricing.yml)
- [Rate Limits](rate-limits/paradedb-rate-limits.yml)
- [Fin Ops](finops/paradedb-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
