# SAP Business Technology Platform

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
