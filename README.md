# Clinexa Planning

Planning and architecture documentation for **Clinexa**. This repository holds product and system design only — not application source code.

## Purpose

Use this repo as the single place for Clinexa’s planning artifacts: requirements, architecture, domain designs, and delivery guidelines. The PRD anchors decisions; the rest of `docs/` expands them. Implementation lives in other repositories; keep every document consistent with the PRD.

## How to use this repository

- Treat [`docs/00-product-requirements-document.md`](docs/00-product-requirements-document.md) as the **single source of truth**. All other planning docs must derive scope, terminology, and business rules from the PRD.
- Use [`MasterPrompt.md`](MasterPrompt.md) as the **master prompt** to generate task prompts for authoring each numbered document under `docs/`. Update the “Today's task” target file, then run the prompt; do not invent scope outside the PRD.
- When updating any document, keep related docs aligned (requirements, architecture, APIs, security, and domain specs).
- Do **not** add implementation code here unless explicitly requested.
- Prefer linking to the numbered doc that owns a topic instead of duplicating detail in this README.

## Documentation status

The documentation set is **scaffolded and work in progress**. The PRD is complete as the baseline; numbered files under `docs/` (01–24) are authored from it using prompts derived from `MasterPrompt.md`. This README is a navigation entry point only.

## Documentation index

### Source of truth

| Doc | Description |
| --- | --- |
| [00 — Product requirements document](docs/00-product-requirements-document.md) | Single source of truth for product scope, rules, and planning decisions |
| [MasterPrompt.md](MasterPrompt.md) | Master prompt template for generating each planning document from the PRD |

### Foundations

| Doc | Description |
| --- | --- |
| [01 — Project overview](docs/01-project-overview.md) | Product vision, scope, and high-level context |
| [02 — Business requirements](docs/02-business-requirements.md) | Business goals, constraints, and success criteria |
| [03 — Functional requirements](docs/03-functional-requirements.md) | What the system must do |
| [04 — Non-functional requirements](docs/04-non-functional-requirements.md) | Performance, reliability, scalability, and related qualities |
| [05 — System architecture](docs/05-system-architecture.md) | Overall system structure and major components |

### Users and product

| Doc | Description |
| --- | --- |
| [06 — User personas](docs/06-user-personas.md) | Primary user types and their goals |
| [07 — User journeys](docs/07-user-journeys.md) | End-to-end flows for key user goals |
| [08 — Role permissions](docs/08-role-permissions.md) | Roles, access control, and authorization boundaries |
| [09 — Feature roadmap](docs/09-feature-roadmap.md) | Planned features and delivery sequencing |

### Technical design

| Doc | Description |
| --- | --- |
| [10 — Database design](docs/10-database-design.md) | Data model and persistence design |
| [11 — API design](docs/11-api-design.md) | API surface, contracts, and conventions |
| [12 — Authentication flow](docs/12-authentication-flow.md) | Sign-in, session, and identity flows |
| [13 — Security](docs/13-security.md) | Security controls, threats, and compliance posture |
| [14 — Notifications](docs/14-notifications.md) | Notification channels, triggers, and delivery |
| [15 — Payment flow](docs/15-payment-flow.md) | Payment and billing flows |
| [16 — Store architecture](docs/16-store-architecture.md) | Store / commerce domain architecture |

### Surfaces and domains

| Doc | Description |
| --- | --- |
| [17 — Patient portal](docs/17-patient-portal.md) | Patient-facing portal planning |
| [18 — CRM](docs/18-crm.md) | CRM capabilities and workflows |
| [19 — Mobile app](docs/19-mobile-app.md) | Mobile application planning |
| [20 — UI design system](docs/20-ui-design-system.md) | UI patterns, components, and design standards |

### Delivery

| Doc | Description |
| --- | --- |
| [21 — Development guidelines](docs/21-development-guidelines.md) | Engineering practices and conventions |
| [22 — Testing strategy](docs/22-testing-strategy.md) | Test approach, levels, and quality gates |
| [23 — Deployment](docs/23-deployment.md) | Environments, release, and deployment approach |
| [24 — Future features](docs/24-future-features.md) | Longer-term ideas outside the near-term roadmap |

## What this README does not cover

Tech stack choices, schemas, API contracts, user-journey detail, and domain rules belong in their dedicated docs above — not here.
