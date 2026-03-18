# Governance Intel — Databricks Product Docs

Topic-specific documentation links for Databricks product areas. Governance-focused first; extend with new sections as needed.

> For universal external sources (community, blogs, analysts) see `intel/external-intel.md`. For internal sources (Glean, Confluence, Slack, Logfood) see `intel/internal-intel.md`.

---

## Data Governance & Unity Catalog

| Source | URL | Notes |
|--------|-----|-------|
| Data Governance overview | https://docs.databricks.com/en/data-governance/index.html | Top-level entry point |
| Unity Catalog overview | https://docs.databricks.com/en/data-governance/unity-catalog/index.html | Metastore, catalogs, schemas, tables, volumes |
| UC best practices | https://docs.databricks.com/en/data-governance/unity-catalog/best-practices.html | Setup and org guidance |
| Privileges & access control | https://docs.databricks.com/en/data-governance/unity-catalog/manage-privileges/index.html | GRANT/REVOKE, privilege model |
| Data lineage | https://docs.databricks.com/en/data-governance/unity-catalog/data-lineage.html | Column-level lineage, lineage graph |
| Tags | https://docs.databricks.com/en/data-governance/unity-catalog/tags.html | Tagging catalogs, schemas, tables, columns |
| Data classification | https://docs.databricks.com/en/data-governance/unity-catalog/data-classification.html | Automated classification, sensitive data detection |
| Row & column filters | https://docs.databricks.com/en/data-governance/unity-catalog/row-and-column-filters.html | Dynamic data masking, row-level security |
| Delta Sharing | https://docs.databricks.com/en/delta-sharing/index.html | Open protocol for secure data sharing |
| Lakehouse Federation | https://docs.databricks.com/en/query-federation/index.html | Govern external databases under UC |
| Metastore administration | https://docs.databricks.com/en/data-governance/unity-catalog/create-metastore.html | Setup, workspace assignment |
| Unity Catalog OSS (GitHub) | https://github.com/unitycatalog/unitycatalog | OSS repo; Issues tab = real user pain points |
| Delta Lake docs | https://docs.delta.io/ | Open table format underlying UC tables |

---

## AI Governance

| Source | URL | Notes |
|--------|-----|-------|
| AI governance overview | https://docs.databricks.com/en/machine-learning/model-governance/index.html | Model registry, lineage, access control for ML |
| MLflow Model Registry | https://docs.databricks.com/en/mlflow/model-registry.html | Stage transitions, approval workflows |
| Inference tables | https://docs.databricks.com/en/machine-learning/model-serving/inference-tables.html | Log model I/O for auditing and drift monitoring |
| Foundation Model APIs | https://docs.databricks.com/en/machine-learning/foundation-models/index.html | Managed LLM access; pay-per-token |
| Model Serving | https://docs.databricks.com/en/machine-learning/model-serving/index.html | Serving infra, monitoring |
| Feature Store | https://docs.databricks.com/en/machine-learning/feature-store/index.html | Governed feature sharing across teams |
| AI/BI Genie | https://docs.databricks.com/en/genie/index.html | NL analytics; governance of spaces and access |
| MLflow docs (OSS) | https://mlflow.org/docs/latest/index.html | Open source ML lifecycle tracking and registry |

---

## Security & Compliance

| Source | URL | Notes |
|--------|-----|-------|
| Security overview | https://docs.databricks.com/en/security/index.html | Top-level security hub |
| Trust & compliance | https://www.databricks.com/trust | SOC 2, ISO 27001, HIPAA, FedRAMP, GDPR certs + DPA |
| ABAC | https://docs.databricks.com/en/data-governance/unity-catalog/attribute-based-access-control.html | Tag-based row/column access policies |
| UC permissions model | https://docs.databricks.com/en/data-governance/unity-catalog/manage-privileges/privilege-model.html | Full RBAC model reference |
| Audit log (system table) | https://docs.databricks.com/en/admin/system-tables/audit.html | `system.access.audit` — all user actions |
| Authentication & SSO | https://docs.databricks.com/en/admin/users-groups/single-sign-on/index.html | SAML, SCIM, OAuth, OIDC |
| Network security | https://docs.databricks.com/en/security/network/index.html | Private Link, IP access lists, firewall |
| Encryption | https://docs.databricks.com/en/security/keys/index.html | CMK, BYOK, encryption at rest |
| Secret management | https://docs.databricks.com/en/security/secrets/index.html | Secrets API, Vault integration |

---

## Admin Console

| Source | URL | Notes |
|--------|-----|-------|
| Account console overview | https://docs.databricks.com/en/admin/index.html | Account-level vs workspace-level admin |
| Workspace administration | https://docs.databricks.com/en/administration-guide/index.html | Full workspace admin guide |
| System tables overview | https://docs.databricks.com/en/admin/system-tables/index.html | All `system.*` tables — billing, compute, access, lineage |
| User & group management | https://docs.databricks.com/en/admin/users-groups/index.html | SCIM sync, service principals, groups |
| Service principals | https://docs.databricks.com/en/admin/users-groups/service-principals.html | Automation identities, token management |
| Workspace settings | https://docs.databricks.com/en/administration-guide/workspace-settings/index.html | Feature flags, defaults, notifications |
| Notification destinations | https://docs.databricks.com/en/admin/account-settings/notification-destinations.html | Slack/email/PagerDuty alerts |

---

## Cost Governance

| Source | URL | Notes |
|--------|-----|-------|
| Account usage & billing | https://docs.databricks.com/en/admin/account-settings/usage.html | DBU consumption, cost dashboards |
| Budgets | https://docs.databricks.com/en/admin/account-settings/budgets.html | Budget alerts by workspace/tag |
| Cost monitoring (system tables) | https://docs.databricks.com/en/admin/system-tables/billing.html | `system.billing.usage` |
| Query cost attribution | https://docs.databricks.com/en/sql/admin/query-cost-attribution.html | Per-query cost breakdown in DBSQL |
| DBU pricing | https://www.databricks.com/product/pricing | Public DBU rates by tier and cloud |
| Serverless billing | https://docs.databricks.com/en/serverless-compute/index.html | Serverless cost model vs provisioned |
| Cluster policies | https://docs.databricks.com/en/administration-guide/clusters/policies.html | Constrain cluster configs to control spend |

---

## Performance Governance

| Source | URL | Notes |
|--------|-----|-------|
| Lakehouse monitoring | https://docs.databricks.com/en/lakehouse-monitoring/index.html | Data quality and drift monitoring on tables |
| Query profile | https://docs.databricks.com/en/sql/user/queries/query-profile.html | Visual query plan, bottleneck identification |
| Query history | https://docs.databricks.com/en/sql/admin/query-history.html | Cross-warehouse query log |
| Liquid clustering | https://docs.databricks.com/en/delta/clustering.html | Replaces static partitioning |
| Delta optimizations | https://docs.databricks.com/en/delta/optimizations/index.html | OPTIMIZE, Z-ordering, compaction, bloom filters |
| Photon engine | https://docs.databricks.com/en/compute/photon.html | Vectorized execution |
| DLT (Lakeflow) pipelines | https://docs.databricks.com/en/dlt/index.html | Declarative ETL with built-in observability |

---

*Last updated: March 2026. Companion: `intel/external-intel.md` · `intel/internal-intel.md`*
