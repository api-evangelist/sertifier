# Sertifier (sertifier)

Sertifier is a digital credential and certificate/badge management platform that lets organizations design, issue, verify, and analyze verifiable digital credentials (Open Badge-style certificates and badges) at scale. Beyond the web application, Sertifier exposes a REST Credential API (base `https://b2b.sertifier.com`, authenticated with a private `secretKey` header and an `api-version` header) so backend systems and LMS/CRM integrations can programmatically manage designs, credential details, email templates, campaigns, recipients, and custom attributes, and issue and publish credentials the instant a learner completes a course. Sertifier has issued more than 10 million credentials across 70+ countries.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sertifier/refs/heads/main/apis.yml)

## Tags

- Digital Credentials
- Certificates
- Badges
- Open Badges
- Verifiable Credentials
- Credentialing
- EdTech

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## APIs

### Sertifier Campaigns API

Create, retrieve, update, delete, and search credential campaigns - the container that binds a Design, a credential Detail, and an Email Template. Add recipients and issue credentials into a campaign (addCredentials), then send or schedule delivery. The primary programmatic path for automating certificate creation.

- **Human URL:** [https://sertifier.docs.apiary.io/](https://sertifier.docs.apiary.io/)
- **Base URL:** `https://b2b.sertifier.com`

#### Tags

- Campaigns
- Issuance
- Credentials

#### Properties

- [Documentation](https://help.sertifier.com/sertifier-api-quickstart)
- [API Reference](https://sertifier.docs.apiary.io/)
- [OpenAPI](openapi/sertifier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sertifier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sertifier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sertifier Credentials API

Retrieve, update, delete, search, and publish individual issued credentials, and generate a downloadable PDF link for a credential by its ID or certificate number. Each published credential resolves to a permanent, verifiable credential URL.

- **Human URL:** [https://sertifier.docs.apiary.io/](https://sertifier.docs.apiary.io/)
- **Base URL:** `https://b2b.sertifier.com`

#### Tags

- Credentials
- Certificates
- Publishing

#### Properties

- [Documentation](https://help.sertifier.com/credentials-complete-guide)
- [API Reference](https://sertifier.docs.apiary.io/)
- [OpenAPI](openapi/sertifier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sertifier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sertifier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sertifier Designs API

Retrieve, delete, search, and copy the visual designs applied to certificates and badges. Designs are authored in the Sertifier web application; the API references, duplicates, and lists them for use inside campaigns.

- **Human URL:** [https://sertifier.docs.apiary.io/](https://sertifier.docs.apiary.io/)
- **Base URL:** `https://b2b.sertifier.com`

#### Tags

- Designs
- Templates
- Branding

#### Properties

- [Documentation](https://help.sertifier.com/credential-design-complete-guide)
- [API Reference](https://sertifier.docs.apiary.io/)
- [OpenAPI](openapi/sertifier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sertifier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sertifier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sertifier Credential Details API

Create, update, retrieve, and search credential Details - the descriptive metadata printed on a credential (title, description, attached skills, criteria). Includes a skills-library search. Details become immutable once credentials are sent.

- **Human URL:** [https://sertifier.docs.apiary.io/](https://sertifier.docs.apiary.io/)
- **Base URL:** `https://b2b.sertifier.com`

#### Tags

- Details
- Skills
- Metadata

#### Properties

- [Documentation](https://help.sertifier.com/credentials-complete-guide)
- [API Reference](https://sertifier.docs.apiary.io/)
- [OpenAPI](openapi/sertifier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sertifier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sertifier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sertifier Email Templates API

Retrieve, delete, search, and copy the email templates used to deliver finished credentials to recipients. Templates are referenced by a campaign to send the completed certificate or badge.

- **Human URL:** [https://sertifier.docs.apiary.io/](https://sertifier.docs.apiary.io/)
- **Base URL:** `https://b2b.sertifier.com`

#### Tags

- Email Templates
- Delivery
- Notifications

#### Properties

- [API Reference](https://sertifier.docs.apiary.io/)
- [OpenAPI](openapi/sertifier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sertifier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sertifier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sertifier Recipients API

Add, update, delete, and search the recipients (learners) who receive credentials. Recipients can be added individually via the API or in bulk in the web application, and are the audience a campaign issues credentials to.

- **Human URL:** [https://sertifier.docs.apiary.io/](https://sertifier.docs.apiary.io/)
- **Base URL:** `https://b2b.sertifier.com`

#### Tags

- Recipients
- Learners
- Contacts

#### Properties

- [Documentation](https://help.sertifier.com/how-do-i-add-recipients)
- [API Reference](https://sertifier.docs.apiary.io/)
- [OpenAPI](openapi/sertifier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sertifier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sertifier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sertifier Attributes API

Create, update, delete, and search custom attributes - the reusable key/value fields (for example score, cohort, or completion date) merged into a credential Design and Email Template when issuing credentials.

- **Human URL:** [https://sertifier.docs.apiary.io/](https://sertifier.docs.apiary.io/)
- **Base URL:** `https://b2b.sertifier.com`

#### Tags

- Attributes
- Custom Fields
- Personalization

#### Properties

- [API Reference](https://sertifier.docs.apiary.io/)
- [OpenAPI](openapi/sertifier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sertifier.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sertifier.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sertifier Webhooks API

**MODELED** - Sertifier documents inbound webhook/REST automation (for example receiving LMS completion events and via no-code tools such as Zapier and n8n), but a first-party outbound webhook subscription REST resource is not published in the Credential API reference. Endpoints here are honestly modeled, not confirmed.

- **Human URL:** [https://help.sertifier.com/api-key-integrations](https://help.sertifier.com/api-key-integrations)
- **Base URL:** `https://b2b.sertifier.com`

#### Tags

- Webhooks
- Events
- Modeled

#### Properties

- [Documentation](https://help.sertifier.com/api-key-integrations)
- [OpenAPI](openapi/sertifier-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/sertifierco)
- [Website](https://sertifier.com)
- [Documentation](https://docs.sertifier.com/)
- [Plans](plans/sertifier-plans-pricing.yml)
- [Rate Limits](rate-limits/sertifier-rate-limits.yml)
- [Fin Ops](finops/sertifier-finops.yml)
- [Blog](https://sertifier.com/blog/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
