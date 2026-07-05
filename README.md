# STACK (stack-takeoff)

STACK Construction Technologies makes cloud-based preconstruction software for on-screen takeoff and estimating, used by contractors across most trades (website: [stackct.com](https://www.stackct.com/)).

**API access model:** STACK exposes a real, documented REST API (v2) - but access is gated. You must be a STACK customer on an **API-Enabled Subscription** (or an approved software partner) to obtain credentials. Authentication is **OAuth 2.0**, offered as **two-legged** (client-credentials, server-to-server on an account you control) and **three-legged** (authorization-code, acting on behalf of a user) flows. Tokens are issued by a per-tenant authorization server; the API base follows the pattern `https://{server}/api/v2`, where `{server}` is the host provided with your API credentials. Access tokens are valid for 8 hours, authorization codes for 5 minutes, and refresh tokens for 90 days.

The full endpoint reference sits behind an access request. The API surface documented here is **modeled from STACK's public developer overview, authentication guide, and tutorials** - it is not sourced from an official machine-readable OpenAPI document. Only calls published in STACK's own Developers Reference are officially supported.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/stack-takeoff/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/stack-takeoff/refs/heads/main/apis.yml)

## Tags

- Construction
- Preconstruction
- Takeoff
- Estimating
- Construction Technology
- Partner API

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

> Endpoints below are **modeled** from STACK's public developer docs and tutorials. Exact paths, request/response shapes, and available operations are confirmed only after you obtain API access from STACK.

### STACK Projects API

Create and update projects and organize their contents in folders - the top-level container that takeoffs, plans, and estimates hang off of.

- **Human URL:** [https://www.stackct.com/developers-docs/](https://www.stackct.com/developers-docs/)
- **Base URL:** `https://{server}/api/v2`

### STACK Plans & Files API

Upload plan sets and supporting documents into project folders, read file metadata, update file properties, and download plans.

- **Human URL:** [https://www.stackct.com/developers-docs/](https://www.stackct.com/developers-docs/)
- **Base URL:** `https://{server}/api/v2`

### STACK Takeoffs API

Create takeoffs on a project, list a takeoff's pages, set page scale, and retrieve measured quantities. On-screen takeoff is STACK's core workflow.

- **Human URL:** [https://www.stackct.com/developers-docs/](https://www.stackct.com/developers-docs/)
- **Base URL:** `https://{server}/api/v2`

### STACK Estimates API

Create, update, and retrieve estimate proposals - turning takeoff quantities into priced line items and a bid.

- **Human URL:** [https://www.stackct.com/developers-docs/](https://www.stackct.com/developers-docs/)
- **Base URL:** `https://{server}/api/v2`

### STACK Items & Assemblies API

Manage items and assemblies attached to takeoffs and retrieve their quantities and costs, so partner tools can pull takeoff/estimating data into invoices, purchase orders, or a separate estimating system.

- **Human URL:** [https://www.stackct.com/developers-docs/](https://www.stackct.com/developers-docs/)
- **Base URL:** `https://{server}/api/v2`

### STACK Reference Data API

Read-only lookup endpoints for cost types, states, and countries used when constructing projects and estimates.

- **Human URL:** [https://www.stackct.com/developers-docs/](https://www.stackct.com/developers-docs/)
- **Base URL:** `https://{server}/api/v2`

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/stack-construction-technologies)
- [Website](https://www.stackct.com/)
- [Documentation](https://www.stackct.com/developers-docs/)
- [Authentication](https://www.stackct.com/developers-docs-authentication/)
- [Request API Access](https://www.stackct.com/developers/)
- [Plans](plans/stack-takeoff-plans-pricing.yml)
- [Rate Limits](rate-limits/stack-takeoff-rate-limits.yml)
- [Fin Ops](finops/stack-takeoff-finops.yml)
- [Blog](https://www.stackct.com/blog/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
