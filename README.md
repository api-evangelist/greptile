# Greptile (greptile)

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
