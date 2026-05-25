# Vespa (vespa-ai)

Vespa is an open-source AI search engine, big-data serving engine, and vector database originally developed inside Yahoo and spun out as Vespa.ai AS. Vespa combines vector search, text search (BM25), structured filtering, and machine-learned ranking — including native tensor inference — into a single distributed serving engine that scales to billions of documents with sub-100ms latency. Vespa Cloud is the fully managed commercial offering operated by the Vespa.ai team across AWS and GCP.

**URL:** [https://vespa.ai](https://vespa.ai)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=opensource-api-evangelist&utm_content=repo)

## Tags

AI, Search, Vector Database, Big Data, Machine Learning, Semantic Search, Retrieval Augmented Generation, Open Source, Tensor, Recommendations

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Vespa Query API
Execute YQL queries with text, vector (HNSW nearest-neighbor), hybrid, and machine-learned ranking against a Vespa application.

- Documentation: [https://docs.vespa.ai/en/query-api.html](https://docs.vespa.ai/en/query-api.html)
- OpenAPI: [openapi/vespa-query-api-openapi.yml](openapi/vespa-query-api-openapi.yml)
- Naftiko Capability: [capabilities/vespa-query.yaml](capabilities/vespa-query.yaml)

### Vespa Document API
Synchronous Put / Get / Update / Remove / Visit operations against a Vespa content cluster.

- Documentation: [https://docs.vespa.ai/en/reference/document-v1-api-reference.html](https://docs.vespa.ai/en/reference/document-v1-api-reference.html)
- OpenAPI: [openapi/vespa-document-api-openapi.yml](openapi/vespa-document-api-openapi.yml)
- Naftiko Capability: [capabilities/vespa-documents.yaml](capabilities/vespa-documents.yaml)

### Vespa Deploy API
Application-package deployment, prepare/activate sessions, schema validation, zero-downtime updates.

- Documentation: [https://docs.vespa.ai/en/reference/deploy-rest-api-v2.html](https://docs.vespa.ai/en/reference/deploy-rest-api-v2.html)

### Vespa Tenant and Application API
Tenant and application management on a Vespa configuration server or Vespa Cloud control plane.

- Documentation: [https://docs.vespa.ai/en/reference/application-v2-tenant.html](https://docs.vespa.ai/en/reference/application-v2-tenant.html)

### Vespa Config API
Internal configuration distribution from the config-server to Vespa services.

- Documentation: [https://docs.vespa.ai/en/reference/config-rest-api-v2.html](https://docs.vespa.ai/en/reference/config-rest-api-v2.html)

### Vespa Cluster Controller API
Content-cluster runtime state and maintenance-mode orchestration.

- Documentation: [https://docs.vespa.ai/en/reference/cluster-v2.html](https://docs.vespa.ai/en/reference/cluster-v2.html)

### Vespa State API
Per-service health, version, and metrics for any Vespa node.

- Documentation: [https://docs.vespa.ai/en/reference/state-v1.html](https://docs.vespa.ai/en/reference/state-v1.html)
- Naftiko Capability: [capabilities/vespa-state.yaml](capabilities/vespa-state.yaml)

### Vespa Metrics API
JSON / Prometheus exposition endpoints (`/metrics/v1`, `/metrics/v2`, `/prometheus/v1`).

- Documentation: [https://docs.vespa.ai/en/operations/metrics.html](https://docs.vespa.ai/en/operations/metrics.html)

## Common Properties

- [Website](https://vespa.ai)
- [Documentation](https://docs.vespa.ai/)
- [Getting Started](https://docs.vespa.ai/en/getting-started.html)
- [Tutorials](https://docs.vespa.ai/en/learn/tutorials/)
- [GitHub Organization](https://github.com/vespa-engine)
- [GitHub Repository](https://github.com/vespa-engine/vespa)
- [License (Apache 2.0)](https://github.com/vespa-engine/vespa/blob/master/LICENSE)
- [Blog](https://blog.vespa.ai/)
- [Blog RSS](https://blog.vespa.ai/feed.xml)
- [Pricing](https://cloud.vespa.ai/pricing)
- [Vespa Cloud Console](https://console.vespa-cloud.com/)
- [Slack](https://slack.vespa.ai/)
- [Support / Issues](https://github.com/vespa-engine/vespa/issues)
- [Releases / Change Log](https://github.com/vespa-engine/vespa/releases)
- [Sample Apps](https://github.com/vespa-engine/sample-apps)
- [Docker Image](https://github.com/vespa-engine/docker-image)
- [Prometheus Exporter](https://github.com/vespa-engine/vespa_exporter)
- [setup-vespa-cli GitHub Action](https://github.com/vespa-engine/setup-vespa-cli-action)

## SDKs and Clients

- [Vespa CLI (Go)](https://github.com/vespa-engine/vespa/tree/master/client/go)
- [pyvespa (Python)](https://github.com/vespa-engine/pyvespa) — [docs](https://vespa-engine.github.io/pyvespa/)
- [vespa-feed-client (Java)](https://github.com/vespa-engine/vespa/tree/master/vespa-feed-client)
- [vespa-search (JavaScript)](https://github.com/vespa-engine/vespa-search)

## Use Cases

| Name | Description |
|------|-------------|
| Hybrid Search | Combine BM25, vector similarity, and structured filters in a single multi-phase ranked query. |
| Retrieval Augmented Generation | Serve grounded context to LLMs with sub-100ms hybrid retrieval over chunks and embeddings. |
| Recommendation and Personalization | ML-ranked recommendations with real-time feature updates and tensor inference. |
| Ad Targeting / RTB | Match candidate ads against user context within tight latency budgets. |
| E-Commerce Search and Browse | Faceted navigation + structured filters + learned ranking for large product catalogs. |
| Streaming Search | Scan a user's personal corpus on demand — ideal for mail, messaging, and document search. |

## Plans (Vespa Cloud)

| Plan | vCPU/hr | GiB Memory/hr | GiB Disk/hr | GPU GiB/hr | Notes |
|------|---------|---------------|-------------|------------|-------|
| Startup | $0.05 | $0.005 | $0.0002 | $0.03 | Shared, dev zones only, community support |
| Basic | $0.10 | $0.01 | $0.0004 | $0.07 | NBD support |
| Commercial | $0.145 | $0.0145 | $0.0005 | $0.10 | 24/7 1-hour SLA, backup + DR |
| Enterprise | $0.18 | $0.018 | $0.0007 | $0.125 | $20k/mo min, 15-min SLA, SSO, named rep |
| Self-Managed | per-contract | per-contract | per-contract | per-contract | Run open-source Vespa with commercial support |
| Open Source | free | free | free | free | Apache 2.0, community support |

Up to 50% volume discount; 15% committed-spend discount.

See [plans/vespa-ai-plans-pricing.yml](plans/vespa-ai-plans-pricing.yml).

## Artifacts

### OpenAPI
- [Vespa Query API OpenAPI](openapi/vespa-query-api-openapi.yml)
- [Vespa Document API OpenAPI](openapi/vespa-document-api-openapi.yml)

### JSON Schema
- [Vespa Document Schema](json-schema/vespa-ai-document-schema.json)
- [Vespa Query Schema](json-schema/vespa-ai-query-schema.json)

### JSON Structure
- [Vespa Document Structure](json-structure/vespa-ai-document-structure.json)

### JSON-LD
- [Vespa JSON-LD Context](json-ld/vespa-ai-context.jsonld)

### Examples
- [Vespa Query Example](examples/vespa-ai-query-example.json)
- [Vespa Document Put Example](examples/vespa-ai-document-put-example.json)

## Capabilities

Naftiko capabilities mapping Vespa business surfaces.

- [Vespa Query](capabilities/vespa-query.yaml) — YQL / hybrid / vector queries
- [Vespa Documents](capabilities/vespa-documents.yaml) — Put / Get / Update / Remove / Visit
- [Vespa State](capabilities/vespa-state.yaml) — Health, version, and per-service metrics

## Vocabulary

- [Vespa Vocabulary](vocabulary/vespa-ai-vocabulary.yml) — Domain taxonomy (concepts, services, tools, standards)

## Rules

- [Vespa Spectral Rules](rules/vespa-ai-rules.yml) — Spectral ruleset enforcing Vespa OpenAPI conventions

## Plans / Rate Limits / FinOps

- [Plans](plans/vespa-ai-plans-pricing.yml) — API Commons Plans 0.1
- [Rate Limits](rate-limits/vespa-ai-rate-limits.yml) — API Commons Rate Limits 0.1
- [FinOps](finops/vespa-ai-finops.yml) — FOCUS 1.3 aligned

## Maintainers

- Kin Lane — kin@apievangelist.com
