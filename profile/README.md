<div align="center">

<img src="./assets/banner.svg" alt="SIDIGS Microservices — Sekolah Jadi Mudah" width="100%" />

**English** · [Bahasa Indonesia](./README.id.md)

### The engineering home of SIDIGS — one platform that runs a whole school.

From admissions to report cards, attendance to the canteen till: SIDIGS connects
foundations, schools, teachers, students and parents in one integrated ecosystem.

<a href="https://sidigs.com"><img src="./assets/btn-website.svg" alt="sidigs.com" height="44" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-architecture"><img src="./assets/btn-architecture.svg" alt="Architecture" height="44" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-service-template"><img src="./assets/btn-template.svg" alt="Service Template" height="44" /></a>

</div>

## 🏫 What we build

SIDIGS is a digital school platform used by **foundations, schools and families** across Indonesia.
This organization holds its next generation: independent, domain-focused services behind a single
gateway, and one web app with a dedicated workspace for every role.

<img src="./assets/features.svg" alt="What we build: academic, assessment, finance, people, school services, communication" width="100%" />

## 🧭 Architecture

<img src="./assets/architecture.svg" alt="Architecture: the Web App reaches the API Gateway, which routes to the core and domain services" width="100%" />

**Principles we hold to**

- 🧩 **One domain, one service, one database** — services own their data and talk through signed service-to-service calls.
- 🚪 **A single front door** — every request passes the API Gateway: identity, tenant resolution, permissions and feature flags.
- 🔐 **Security by default** — token-based identity (JWKS), per-route permissions, encrypted credentials, validated input at every boundary.
- 📱 **Mobile first** — most of our users are on phones; every page must work at 375 px.
- 🧪 **Tested rules** — money, scoring and access rules live in small, unit-tested modules.

## 🗂️ Repositories

<div align="center">

<img src="./assets/repos/group-front.svg" alt="FRONT END & EDGE" width="100%" />

<a href="https://github.com/sidigs-microservice/sidigs-web-app"><img src="./assets/repos/sidigs-web-app.svg" alt="sidigs-web-app: Next.js · every role" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-api-gateway"><img src="./assets/repos/sidigs-api-gateway.svg" alt="sidigs-api-gateway: routing · auth · flags" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-attendance-ingress-service"><img src="./assets/repos/sidigs-attendance-ingress-service.svg" alt="sidigs-attendance-ingress-service (in development): RFID · device attendance" width="49%" /></a>

<img src="./assets/repos/group-core.svg" alt="CORE SERVICES" width="100%" />

<a href="https://github.com/sidigs-microservice/sidigs-iam-service"><img src="./assets/repos/sidigs-iam-service.svg" alt="sidigs-iam-service: accounts · auth · chat" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-organization-service"><img src="./assets/repos/sidigs-organization-service.svg" alt="sidigs-organization-service: foundations · schools" width="49%" /></a>

<img src="./assets/repos/group-domain.svg" alt="DOMAIN SERVICES" width="100%" />

<a href="https://github.com/sidigs-microservice/sidigs-academic-service"><img src="./assets/repos/sidigs-academic-service.svg" alt="sidigs-academic-service: classes · attendance · report cards" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-exam-service"><img src="./assets/repos/sidigs-exam-service.svg" alt="sidigs-exam-service: question bank · CBT · scoring" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-finance-service"><img src="./assets/repos/sidigs-finance-service.svg" alt="sidigs-finance-service: bills · e-money · accounting" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-hr-service"><img src="./assets/repos/sidigs-hr-service.svg" alt="sidigs-hr-service: staff · attendance · payroll" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-content-service"><img src="./assets/repos/sidigs-content-service.svg" alt="sidigs-content-service: letters · announcements · files" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-infrastructure-service"><img src="./assets/repos/sidigs-infrastructure-service.svg" alt="sidigs-infrastructure-service: library · clinic · facilities" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-canteen-service"><img src="./assets/repos/sidigs-canteen-service.svg" alt="sidigs-canteen-service: merchants · point of sale" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-registration-service"><img src="./assets/repos/sidigs-registration-service.svg" alt="sidigs-registration-service: school onboarding" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-pkl-service"><img src="./assets/repos/sidigs-pkl-service.svg" alt="sidigs-pkl-service (in development): internships (PKL)" width="49%" /></a>

<img src="./assets/repos/group-platform.svg" alt="PLATFORM & DOCS" width="100%" />

<a href="https://github.com/sidigs-microservice/sidigs-platform"><img src="./assets/repos/sidigs-platform.svg" alt="sidigs-platform: local runtime · seeds · tooling" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-service-template"><img src="./assets/repos/sidigs-service-template.svg" alt="sidigs-service-template: starter for every new service" width="49%" /></a>

<a href="https://github.com/sidigs-microservice/sidigs-architecture"><img src="./assets/repos/sidigs-architecture.svg" alt="sidigs-architecture: decisions · source of truth" width="49%" /></a>
<a href="https://github.com/sidigs-microservice/sidigs-api-collection"><img src="./assets/repos/sidigs-api-collection.svg" alt="sidigs-api-collection: API collections · testing" width="49%" /></a>

</div>

## 🛠️ Tech stack

<img src="./assets/tech.svg" alt="Tech stack. Backend: TypeScript, Node.js, NestJS, Better Auth. Frontend: Next.js 16, React, Tailwind CSS v4, Lucide. Data: MySQL 8.4, Prisma, Redis, BullMQ. Quality and CI: Jest, Vitest, ESLint, GitHub Actions." width="100%" />

## 🔄 How we work

<img src="./assets/workflow.svg" alt="Workflow: Linear ticket, branch, pull request, CI checks, review, merge" width="100%" />

- 📋 **Linear** is where work is planned and tracked. GitHub Issues are not used.
- 🔍 **Every change is reviewed** through a pull request before it is merged.
- 🤖 **GitHub Actions** run lint, tests, builds and security checks on every pull request.
- 🔒 **No secrets in code** — configuration comes from the environment, never from the repository.
- 📐 **Significant decisions are written down** in [`sidigs-architecture`](https://github.com/sidigs-microservice/sidigs-architecture).

---

[<img src="./assets/footer.svg" alt="SIDIGS Engineering — sidigs.com" width="100%" />](https://sidigs.com)
