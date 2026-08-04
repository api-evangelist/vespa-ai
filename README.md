# Vespa (vespa-ai)

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

Vespa is an open-source AI search engine, big-data serving engine, and vector database originally developed inside Yahoo and spun out as Vespa.ai AS. Vespa combines vector search, text search (BM25), structured filtering, and machine-learned ranking — including native tensor inference — into a single distributed serving engine that scales to billions of documents with sub-100ms latency. Vespa Cloud is the fully managed commercial offering operated by the Vespa.ai team across AWS and GCP, with Startup, Basic, Commercial, and Enterprise plans plus a Self-Managed option for customers running the open-source engine on their own infrastructure. Vespa is widely used at Spotify, Perplexity, Yahoo, Farfetch, and Elicit for search, recommendation, personalization, and Retrieval-Augmented Generation (RAG).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/vespa-ai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/vespa-ai/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- AI
- Search
- Vector Database
- Big Data
- Machine Learning
- Semantic Search
- Retrieval Augmented Generation
- Open Source
- Tensor
- Recommendations

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Vespa Query API

The Vespa Query (Search) API executes structured and vector queries against a Vespa application using YQL (Vespa Query Language). It supports text search with BM25, approximate-nearest-neighbor vector search over HNSW indexes, hybrid search, machine-learned ranking with multi-phase rank profiles, grouping/aggregation, pagination, result presentation, and tracing. Queries can be issued as GET requests with query-string parameters or POST requests with a JSON body for complex expressions.

- **Human URL:** [https://docs.vespa.ai/en/query-api.html](https://docs.vespa.ai/en/query-api.html)

#### Tags

- AI
- Search
- Query
- YQL
- Vector Search
- Ranking
- Hybrid Search

#### Properties

- [OpenAPI](openapi/vespa-query-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vespa-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vespa-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://docs.vespa.ai/en/query-api.html)
- [Documentation](https://docs.vespa.ai/en/reference/api/query.html)
- [Getting Started](https://docs.vespa.ai/en/getting-started.html)

### Vespa Document API

The Vespa Document API (/document/v1) provides synchronous REST access to document operations against a Vespa content cluster. It supports Put, Get, Update (partial update with assign/add/remove operators), Remove, and Visit (streaming visit, copy, delete-where, update-where) over JSON or JSON Lines, with conditional writes, multi-tenant namespaces, field-set projection, time-window selection, and pagination via continuation tokens.

- **Human URL:** [https://docs.vespa.ai/en/reference/document-v1-api-reference.html](https://docs.vespa.ai/en/reference/document-v1-api-reference.html)

#### Tags

- Documents
- CRUD
- Indexing
- Data
- Streaming

#### Properties

- [OpenAPI](openapi/vespa-document-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Documentation](https://docs.vespa.ai/en/reference/document-v1-api-reference.html)
- [Documentation](https://docs.vespa.ai/en/writing/document-v1-api-guide.html)
- [Documentation](https://docs.vespa.ai/en/reads-and-writes.html)

### Vespa Deploy API

The Vespa Deploy API (/application/v2) manages application packages on a Vespa configuration server. It supports preparing, activating, and tearing down application packages, session-based deployments, schema validation, and zero-downtime updates of services, schemas, and rank profiles.

- **Human URL:** [https://docs.vespa.ai/en/reference/deploy-rest-api-v2.html](https://docs.vespa.ai/en/reference/deploy-rest-api-v2.html)

#### Tags

- Deployment
- Configuration
- Application
- DevOps

#### Properties

- [Documentation](https://docs.vespa.ai/en/reference/deploy-rest-api-v2.html)
- [Documentation](https://docs.vespa.ai/en/application-packages.html)
- [Postman Collection](collections/vespa-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vespa-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vespa Tenant and Application API

The Vespa Tenant API (/application/v2/tenant) manages tenants and applications hosted on a Vespa configuration server or Vespa Cloud control plane. It exposes operations for creating tenants, listing applications, and binding application sessions to a tenant.

- **Human URL:** [https://docs.vespa.ai/en/reference/application-v2-tenant.html](https://docs.vespa.ai/en/reference/application-v2-tenant.html)

#### Tags

- Tenants
- Applications
- Multi-Tenancy
- Administration

#### Properties

- [Documentation](https://docs.vespa.ai/en/reference/application-v2-tenant.html)
- [Postman Collection](collections/vespa-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vespa-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vespa Config API

The Vespa Config API (/config/v2) lets services in a Vespa application retrieve their configuration from a Vespa configuration server using the config-server / config-proxy protocol. It is primarily used by Vespa services and tooling rather than end users, but is documented as a stable HTTP API.

- **Human URL:** [https://docs.vespa.ai/en/reference/config-rest-api-v2.html](https://docs.vespa.ai/en/reference/config-rest-api-v2.html)

#### Tags

- Configuration
- Internal

#### Properties

- [Documentation](https://docs.vespa.ai/en/reference/config-rest-api-v2.html)
- [Postman Collection](collections/vespa-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vespa-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vespa Cluster Controller API

The Vespa Cluster Controller API (/cluster/v2) exposes runtime state and management endpoints for a Vespa content cluster — including node state queries, maintenance-mode transitions, and storage cluster orchestration.

- **Human URL:** [https://docs.vespa.ai/en/reference/cluster-v2.html](https://docs.vespa.ai/en/reference/cluster-v2.html)

#### Tags

- Cluster
- Operations
- Content
- State

#### Properties

- [Documentation](https://docs.vespa.ai/en/reference/cluster-v2.html)
- [Postman Collection](collections/vespa-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vespa-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vespa State API

The Vespa State API (/state/v1) exposes per-service health, version, and metrics endpoints for any Vespa node — used by orchestration tooling, monitoring agents, and load balancers to check liveness, readiness, and runtime metrics.

- **Human URL:** [https://docs.vespa.ai/en/reference/state-v1.html](https://docs.vespa.ai/en/reference/state-v1.html)

#### Tags

- Health
- Monitoring
- Metrics
- Observability

#### Properties

- [Documentation](https://docs.vespa.ai/en/reference/state-v1.html)
- [Postman Collection](collections/vespa-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vespa-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Vespa Metrics API

Vespa exposes a family of metrics endpoints (/metrics/v1, /metrics/v2, /prometheus/v1) that publish Vespa engine and application metrics in JSON or Prometheus exposition format for scraping by Prometheus, Grafana, or other observability stacks.

- **Human URL:** [https://docs.vespa.ai/en/operations/metrics.html](https://docs.vespa.ai/en/operations/metrics.html)

#### Tags

- Metrics
- Prometheus
- Observability
- Monitoring

#### Properties

- [Documentation](https://docs.vespa.ai/en/operations/metrics.html)
- [Documentation](https://docs.vespa.ai/en/reference/metrics-v1.html)
- [Documentation](https://docs.vespa.ai/en/reference/metrics-v2.html)
- [Documentation](https://docs.vespa.ai/en/reference/prometheus-v1.html)
- [Postman Collection](collections/vespa-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vespa-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://vespa.ai)
- [Documentation](https://docs.vespa.ai/)
- [Getting Started](https://docs.vespa.ai/en/getting-started.html)
- [Tutorials](https://docs.vespa.ai/en/learn/tutorials/)
- [GitHub Organization](https://github.com/vespa-engine)
- [GitHub Repository](https://github.com/vespa-engine/vespa)
- [License](https://github.com/vespa-engine/vespa/blob/master/LICENSE)
- [Blog](https://blog.vespa.ai/)
- [Blog R S S](https://blog.vespa.ai/feed.xml)
- [Pricing](https://cloud.vespa.ai/pricing)
- [Console](https://console.vespa-cloud.com/)
- [Slack](https://slack.vespa.ai/)
- [Support](https://github.com/vespa-engine/vespa/issues)
- [Changelog](https://github.com/vespa-engine/vespa/releases)
- [SDK](https://github.com/vespa-engine/vespa/tree/master/client/go)
- [SDK](https://github.com/vespa-engine/pyvespa)
- [SDK](https://vespa-engine.github.io/pyvespa/)
- [SDK](https://github.com/vespa-engine/vespa/tree/master/vespa-feed-client)
- [SDK](https://github.com/vespa-engine/vespa-search)
- [Sample Apps](https://github.com/vespa-engine/sample-apps)
- [Prometheus Exporter](https://github.com/vespa-engine/vespa_exporter)
- [Docker Image](https://github.com/vespa-engine/docker-image)
- [Git Hub Action](https://github.com/vespa-engine/setup-vespa-cli-action)
- [Spectral Rules](rules/vespa-ai-rules.yml)
- [Vocabulary](vocabulary/vespa-ai-vocabulary.yml)
- [J S O N L D Context](json-ld/vespa-ai-context.jsonld)
- [Plans](plans/vespa-ai-plans-pricing.yml)
- [Rate Limits](rate-limits/vespa-ai-rate-limits.yml)
- [Fin Ops](finops/vespa-ai-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
