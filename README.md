# STACK (stack-takeoff)

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
