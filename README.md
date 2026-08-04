# SAP Business Technology Platform

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

Cloud platform with REST APIs for application development, integration, data management, AI services, and analytics across the SAP ecosystem. SAP BTP unifies AI agents, applications, and data across SAP and third-party landscapes with secure, API-ready integrations.

- **Website:** https://www.sap.com/products/technology-platform.html
- **Documentation:** https://help.sap.com/docs/btp/sap-business-technology-platform/sap-business-technology-platform
- **API Hub:** https://api.sap.com/products/SAPCloudPlatform/apis/REST
- **GitHub:** https://github.com/SAP
- **Pricing:** https://www.sap.com/products/technology-platform/pricing.html
- **Status:** https://www.sap.com/about/trust-center/cloud-service-status.html
- **Blog:** https://community.sap.com/t5/technology-blog-posts-by-sap/bg-p/technology-blog-sap

## APIs

- **Core Services API** — Manage global accounts, subaccounts, directories, and entitlements
- **Authorization and Trust Management (XSUAA)** — OAuth 2.0 authentication and JWT token management
- **Destination Service API** — Connectivity destination configuration for SAP and third-party systems
- **Integration Suite API** — Cloud integration, API management, and event mesh capabilities
- **AI Core API** — AI/ML model training, deployment, and inference
- **Service Manager API** — Service instance and binding lifecycle management
- **Alert Notification Service API** — Event-driven alerts and monitoring notifications

## Authentication

SAP BTP APIs use OAuth 2.0 with the XSUAA (Extended Services for UAA) service as the authorization server. The client credentials grant type is used for service-to-service communication. Tokens are typically valid for 12 hours and should be cached to minimize token requests.

## Pricing

SAP BTP offers consumption-based pricing with the following account types:

- **Trial** — Time-limited free access for evaluation
- **Free Tier (PAYG/BTPEA)** — No-expiry free access to 90+ services within paid account types
- **Pay-As-You-Go** — No minimum commitment, billed monthly based on usage
- **SAP BTP Enterprise Agreement (BTPEA)** — Enterprise subscription with annual commitment and full service catalog access

See [plans/sap-btp-plans-pricing.yml](plans/sap-btp-plans-pricing.yml) for full pricing details.

## Rate Limits

Rate limits are enforced per-service and configurable through SAP Integration Suite API Management. HTTP 429 responses indicate rate limit exceeded. Token caching and destination caching are recommended best practices to reduce API call volume.

See [rate-limits/sap-btp-rate-limits.yml](rate-limits/sap-btp-rate-limits.yml) for service-level details.

## FinOps

Cost management is performed through the SAP BTP Cockpit and SAP for Me portal. Monthly balance statements provide consumption transparency. Key cost drivers include API call volume, compute hours, data storage, AI inference, and user licensing for applicable services.

See [finops/sap-btp-finops.yml](finops/sap-btp-finops.yml) for FinOps guidance.
