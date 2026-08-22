# HashiCorp Vault (vault)

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

HashiCorp Vault is an open source tool for securely storing and accessing secrets. A secret is anything you want to tightly control access to, such as API keys, passwords, certificates, and more. Vault provides a unified interface to any secret while providing tight access control via policies and recording a detailed audit log. It supports dynamic secrets, data encryption, PKI, SSH certificate issuance, and identity-based access through a comprehensive REST HTTP API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/vault/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- DevOps
- Encryption
- Open Source
- PKI
- Secrets Management
- Security

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-05-19

## APIs

### HashiCorp Vault KV Secrets Engine API

The KV v2 secrets engine provides key-value secret storage with versioning, metadata management, soft delete, and permanent destruction of secret versions. Essential for storing static secrets like API keys, passwords, and configuration values with full version history and access control.

- **Human URL:** [https://developer.hashicorp.com/vault/api-docs/secret/kv/kv-v2](https://developer.hashicorp.com/vault/api-docs/secret/kv/kv-v2)
- **Base URL:** `https://vault.example.com/v1`

#### Tags

- KV Secrets
- Secrets Management
- Versioning

#### Properties

- [Documentation](https://developer.hashicorp.com/vault/api-docs/secret/kv/kv-v2)
- [OpenAPI](openapi/vault-kv-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vault-kv.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vault-kv.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/vault-kv-secret-data-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/vault-kv-secret-data-response-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/vault-kv-secret-data-request-structure.json)
- [Example](examples/vault-kv-secret-data-response-example.json)
- [JSON-LD](json-ld/vault-kv-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### HashiCorp Vault System Backend API

The Vault system backend provides management operations for authentication methods, secrets engine mounts, ACL policies, token lifecycle, and lease management. All sys/ endpoints control the core operational behavior of Vault.

- **Human URL:** [https://developer.hashicorp.com/vault/api-docs](https://developer.hashicorp.com/vault/api-docs)
- **Base URL:** `https://vault.example.com/v1`

#### Tags

- Auth Methods
- Leases
- Policies
- Secrets Engines
- System Administration

#### Properties

- [Documentation](https://developer.hashicorp.com/vault/api-docs)
- [OpenAPI](openapi/vault-sys-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/vault-sys.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vault-sys.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/vault-sys-health-response-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/vault-sys-health-response-structure.json)
- [Example](examples/vault-sys-health-response-example.json)
- [JSON-LD](json-ld/vault-sys-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Vault HTTP API

The complete Vault HTTP API gives full access to all Vault operations via REST. Includes authentication method APIs (AppRole, LDAP, JWT, Kubernetes, AWS, Azure), secrets engine APIs (Database, AWS, PKI, SSH, Transit), and the system backend. The OpenAPI spec is dynamically generated from a running Vault instance at /v1/sys/internal/specs/openapi.

- **Human URL:** [https://developer.hashicorp.com/vault/api-docs](https://developer.hashicorp.com/vault/api-docs)
- **Base URL:** `https://vault.example.com/v1`

#### Tags

- Auth Methods
- Dynamic Secrets
- Secrets Management

#### Properties

- [Documentation](https://developer.hashicorp.com/vault/api-docs)
- [Authentication](https://developer.hashicorp.com/vault/docs/auth)
- [Getting Started](https://developer.hashicorp.com/vault/tutorials/get-started)
- [Changelog](https://github.com/hashicorp/vault/blob/main/CHANGELOG.md)
- [Postman Collection](collections/vault-kv.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vault-kv.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/vault-sys.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/vault-sys.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Portal](https://developer.hashicorp.com/vault)
- [Website](https://www.vaultproject.io)
- [Blog](https://www.hashicorp.com/blog/products/vault)
- [Status Page](https://status.hashicorp.com)
- [Terms of Service](https://www.hashicorp.com/terms-of-service)
- [Privacy Policy](https://www.hashicorp.com/privacy)
- [GitHub Organization](https://github.com/hashicorp)
- [GitHub Repository](https://github.com/hashicorp/vault)
- [Forum](https://discuss.hashicorp.com/c/vault)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/vault)
- [Training](https://developer.hashicorp.com/vault/tutorials)
- [Spectral Rules](rules/vault-spectral-rules.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
