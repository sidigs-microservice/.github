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

<table>
<tr><th colspan="2" align="left">🌐 Front end &amp; gateway</th></tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-web-app"><b>sidigs-web-app</b></a><br/><sub>Web app with a workspace for every role</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-api-gateway"><b>sidigs-api-gateway</b></a><br/><sub>Routing, identity, tenancy, permissions, feature flags</sub></td>
</tr>
<tr><th colspan="2" align="left">🔑 Core services</th></tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-iam-service"><b>sidigs-iam-service</b></a><br/><sub>Accounts, authentication, notifications, chat</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-organization-service"><b>sidigs-organization-service</b></a><br/><sub>Foundations, schools, partners, branding</sub></td>
</tr>
<tr><th colspan="2" align="left">🧩 Domain services</th></tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-academic-service"><b>sidigs-academic-service</b></a><br/><sub>Students, classes, curriculum, attendance, report cards</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-exam-service"><b>sidigs-exam-service</b></a><br/><sub>Question banks, CBT runtime, scoring</sub></td>
</tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-finance-service"><b>sidigs-finance-service</b></a><br/><sub>Billing, payments, e-money, savings, accounting</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-hr-service"><b>sidigs-hr-service</b></a><br/><sub>Staff, staff attendance, payroll, performance</sub></td>
</tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-content-service"><b>sidigs-content-service</b></a><br/><sub>Correspondence, announcements, documents, uploads</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-infrastructure-service"><b>sidigs-infrastructure-service</b></a><br/><sub>Facilities, library, clinic, laundry, boarding school</sub></td>
</tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-canteen-service"><b>sidigs-canteen-service</b></a><br/><sub>Merchants and canteen point of sale</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-registration-service"><b>sidigs-registration-service</b></a><br/><sub>School registration and onboarding</sub></td>
</tr>
<tr><th colspan="2" align="left">🧰 Platform &amp; docs</th></tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-platform"><b>sidigs-platform</b></a><br/><sub>Local runtime, config, seeds, developer tooling</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-service-template"><b>sidigs-service-template</b></a><br/><sub>Starting point for every new service</sub></td>
</tr>
<tr>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-architecture"><b>sidigs-architecture</b></a><br/><sub>Architecture decisions, the source of truth</sub></td>
<td width="50%" valign="top"><a href="https://github.com/sidigs-microservice/sidigs-api-collection"><b>sidigs-api-collection</b></a><br/><sub>API collections for testing and integration</sub></td>
</tr>
</table>

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
