# HashiCorp Vault (vault)

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
