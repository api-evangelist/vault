# HashiCorp Vault (vault)
HashiCorp Vault is an open source tool for securely storing and accessing secrets. A secret is anything you want to tightly control access to, such as API keys, passwords, certificates, and more. Vault provides a unified interface to any secret while providing tight access control via policies and recording a detailed audit log. It supports dynamic secrets, data encryption, PKI, SSH certificate issuance, and identity-based access through a comprehensive REST HTTP API.

**URL:** [https://developer.hashicorp.com/vault](https://developer.hashicorp.com/vault)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - DevOps, Encryption, Open Source, PKI, Secrets Management, Security

## Timestamps

- **Created:** 2024-01-01
- **Modified:** 2026-05-03

## APIs

### HashiCorp Vault KV Secrets Engine API
The KV v2 secrets engine provides key-value secret storage with versioning, metadata management, soft delete, and permanent destruction of secret versions. Essential for storing static secrets like API keys, passwords, and configuration values.

**Human URL:** [https://developer.hashicorp.com/vault/api-docs/secret/kv/kv-v2](https://developer.hashicorp.com/vault/api-docs/secret/kv/kv-v2)

#### Tags:

 - KV Secrets, Secrets Management, Versioning

#### Properties

- [Documentation](https://developer.hashicorp.com/vault/api-docs/secret/kv/kv-v2)
- [OpenAPI](openapi/vault-kv-openapi.yml)
- [JSONSchema - Secret Data Request Schema](json-schema/vault-kv-secret-data-request-schema.json)
- [JSONSchema - Secret Data Response Schema](json-schema/vault-kv-secret-data-response-schema.json)
- [JSONStructure - Secret Data Request Structure](json-structure/vault-kv-secret-data-request-structure.json)
- [Example - Secret Data Response](examples/vault-kv-secret-data-response-example.json)
- [JSON-LD](json-ld/vault-kv-context.jsonld)

### HashiCorp Vault System Backend API
The Vault system backend provides management operations for authentication methods, secrets engine mounts, ACL policies, token lifecycle, and lease management.

**Human URL:** [https://developer.hashicorp.com/vault/api-docs](https://developer.hashicorp.com/vault/api-docs)

#### Tags:

 - Auth Methods, Leases, Policies, Secrets Engines, System Administration

#### Properties

- [Documentation](https://developer.hashicorp.com/vault/api-docs)
- [OpenAPI](openapi/vault-sys-openapi.yml)
- [JSONSchema - Health Response Schema](json-schema/vault-sys-health-response-schema.json)
- [JSONStructure - Health Response Structure](json-structure/vault-sys-health-response-structure.json)
- [Example - Health Response](examples/vault-sys-health-response-example.json)
- [JSON-LD](json-ld/vault-sys-context.jsonld)

### Vault HTTP API
The complete Vault HTTP API with dynamic OpenAPI spec generation at /v1/sys/internal/specs/openapi.

**Human URL:** [https://developer.hashicorp.com/vault/api-docs](https://developer.hashicorp.com/vault/api-docs)

#### Tags:

 - Auth Methods, Dynamic Secrets, Secrets Management

#### Properties

- [Documentation](https://developer.hashicorp.com/vault/api-docs)
- [Authentication](https://developer.hashicorp.com/vault/docs/auth)
- [GettingStarted](https://developer.hashicorp.com/vault/tutorials/get-started)
- [ChangeLog](https://github.com/hashicorp/vault/blob/main/CHANGELOG.md)

## Common Properties

- [Portal](https://developer.hashicorp.com/vault)
- [Website](https://www.vaultproject.io)
- [Blog](https://www.hashicorp.com/blog/products/vault)
- [StatusPage](https://status.hashicorp.com)
- [TermsOfService](https://www.hashicorp.com/terms-of-service)
- [PrivacyPolicy](https://www.hashicorp.com/privacy)
- [GitHubOrganization](https://github.com/hashicorp)
- [GitHubRepository](https://github.com/hashicorp/vault)
- [Forum](https://discuss.hashicorp.com/c/vault)
- [StackOverflow](https://stackoverflow.com/questions/tagged/vault)
- [Training](https://developer.hashicorp.com/vault/tutorials)

## Features

| Name | Description |
|------|-------------|
| KV Secrets Engine | Versioned key-value secret storage with soft delete, undelete, and permanent destruction. |
| Dynamic Secrets | On-demand, time-limited credentials for databases, AWS, Azure, GCP, and other backends. |
| Data Encryption (Transit) | Encryption-as-a-Service for application data without storing plaintext in Vault. |
| PKI Certificate Authority | Built-in PKI secrets engine for issuing X.509 certificates with configurable TTLs. |
| SSH Certificate Issuance | Dynamic SSH certificates and OTPs for secure machine access management. |
| ACL Policies | Fine-grained HCL-based policies controlling access to any secret path with capabilities. |
| Auth Methods | Pluggable authentication supporting AppRole, LDAP, JWT/OIDC, Kubernetes, AWS, and more. |
| Lease Management | All dynamic secrets have TTL-bound leases that can be renewed or revoked on demand. |
| Audit Logging | Comprehensive audit trail of all API requests and responses for compliance. |
| MCP Server | Official HashiCorp Vault MCP server enabling AI-assisted secrets management workflows. |

## Use Cases

| Name | Description |
|------|-------------|
| Application Secret Injection | Inject database credentials, API keys, and config into applications at runtime via Vault Agent. |
| Kubernetes Secrets Management | Replace Kubernetes secrets with Vault-managed secrets using the Vault Secrets Operator. |
| Database Credential Rotation | Automatically rotate database credentials with dynamic secrets engine for zero-knowledge security. |
| PKI Automation | Automate certificate lifecycle management for internal services and mutual TLS. |
| CI/CD Secret Injection | Provide short-lived credentials to CI/CD pipelines via AppRole or GitHub Actions OIDC. |
| Secrets as Code | Manage Vault configuration as code using the Terraform Vault provider. |
| Compliance and Audit | Meet SOC 2, PCI-DSS, HIPAA, and FedRAMP requirements with immutable audit logs. |

## Integrations

| Name | Description |
|------|-------------|
| Terraform | Terraform Vault provider for managing Vault configuration and policies as code. |
| Kubernetes | Vault Secrets Operator and Vault Agent Injector for native Kubernetes integration. |
| GitHub Actions | OIDC-based authentication from GitHub Actions workflows without static credentials. |
| AWS | Dynamic AWS IAM credentials and EC2/IAM-based authentication methods. |
| Consul | Native HashiCorp Consul integration for service mesh secrets and ACL tokens. |
| PostgreSQL | Dynamic database credentials for PostgreSQL with configurable role TTLs. |
| Nomad | Native HashiCorp Nomad integration for workload identity and secrets. |
| Ansible | HashiCorp Vault lookup plugin for Ansible playbook secret retrieval. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [HashiCorp Vault KV Secrets Engine API](openapi/vault-kv-openapi.yml)
- [HashiCorp Vault System Backend API](openapi/vault-sys-openapi.yml)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [HashiCorp Vault KV Secrets Engine](capabilities/shared/kv-secrets.yaml) — 7 operations for secret CRUD, versioning, and metadata
- [HashiCorp Vault System Backend](capabilities/shared/sys-backend.yaml) — 12 operations for auth, mounts, policies, and leases

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Secrets Management](capabilities/secrets-management.yaml) | KV Secrets + System Backend | 12 | Platform Engineer |

## Rules

- [Vault Spectral Rules](rules/vault-spectral-rules.yml) — 28 rules across 9 categories enforcing HashiCorp Vault API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
