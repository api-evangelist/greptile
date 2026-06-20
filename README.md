# Greptile (greptile)

Greptile builds an AI layer that understands entire codebases. Its public REST API indexes Git repositories into a graph plus embeddings, then answers natural-language questions and searches over that code. Greptile also ships an AI code-review product delivered as a GitHub App that reviews pull requests for bugs and anti-patterns.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/greptile/refs/heads/main/apis.yml)

## Tags

- AI
- Codebase Understanding
- Code Review
- Code Search
- Developer Tools

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Greptile Query API

Submit a natural-language question against one or more indexed repositories and receive a synthesized answer plus the relevant source files, functions, and classes. Supports session continuity, an optional higher-accuracy genius mode, and streaming responses.

- **Human URL:** [https://docs.greptile.com/api-reference/query](https://docs.greptile.com/api-reference/query)
- **Base URL:** `https://api.greptile.com/v2`

#### Tags

- Query
- Natural Language
- Codebase Q&A

#### Properties

- [Documentation](https://docs.greptile.com/quickstart)
- [API Reference](https://docs.greptile.com/api-reference/query)
- [OpenAPI](openapi/greptile-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/greptile.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/greptile.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Review](review.yml)

### Greptile Repositories (Indexing) API

Submit a Git repository for indexing and check indexing progress. POST /repositories queues a repo (remote, repository, branch) for processing into a graph and embeddings; GET /repositories/{repositoryId} returns processing status, file counts, and the indexed commit SHA.

- **Human URL:** [https://docs.greptile.com/api-reference/repositories](https://docs.greptile.com/api-reference/repositories)
- **Base URL:** `https://api.greptile.com/v2`

#### Tags

- Repositories
- Indexing
- Embeddings

#### Properties

- [Documentation](https://docs.greptile.com/quickstart)
- [API Reference](https://docs.greptile.com/api-reference/repositories)
- [OpenAPI](openapi/greptile-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/greptile.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/greptile.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Greptile Search API

Search one or more indexed repositories in natural language and receive just the ranked list of relevant files, functions, and classes - without the synthesized answer returned by the Query API.

- **Human URL:** [https://docs.greptile.com/api-reference/search](https://docs.greptile.com/api-reference/search)
- **Base URL:** `https://api.greptile.com/v2`

#### Tags

- Search
- Code Search
- Retrieval

#### Properties

- [Documentation](https://docs.greptile.com/quickstart)
- [API Reference](https://docs.greptile.com/api-reference/search)
- [OpenAPI](openapi/greptile-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/greptile.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/greptile.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Greptile Code Review (GitHub App)

AI code-review product delivered as a GitHub App (also GitLab / Bitbucket). Installed on repositories, it reviews pull requests against full-codebase context, flagging bugs and anti-patterns. Billed per seat with included reviews per seat, distinct from the metered REST API.

- **Human URL:** [https://www.greptile.com/](https://www.greptile.com/)
- **Base URL:** `https://github.com/apps/greptile`

#### Tags

- Code Review
- GitHub App
- Pull Requests

#### Properties

- [Documentation](https://docs.greptile.com/)
- [Plans](https://www.greptile.com/pricing)

## Common Properties

- [GitHub Organization](https://github.com/greptileai)
- [LinkedIn](https://www.linkedin.com/company/greptile)
- [Website](https://www.greptile.com)
- [Documentation](https://docs.greptile.com)
- [Plans](plans/greptile-plans-pricing.yml)
- [Rate Limits](rate-limits/greptile-rate-limits.yml)
- [Fin Ops](finops/greptile-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
