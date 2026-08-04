# ParadeDB (paradedb)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
