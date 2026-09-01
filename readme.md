# Hi, I'm Mariano Sagua

### Full Stack Engineer · TypeScript · Next.js · Node.js · PostgreSQL · Applied AI

I build and run production SaaS end to end — frontend, backend, data modelling, authentication, payments, testing and CI/CD.

For the past **2.5 years** I've worked in a **two-developer team** shipping two live products in **EdTech** and **FinTech**, and I was the **sole developer on one of them from the first commit**. That means I own features from the data model through to the deploy, and I do the unglamorous half too: migrating identity providers without losing user data, re-platforming vector search, and building pipelines that refuse to ship when tests fail.

Based in **Buenos Aires, Argentina** · open to **remote international opportunities**.

---

## Featured Work

### Invertilo — FinTech SaaS · [invertilo.com.ar](https://invertilo.com.ar)

**Next.js 16 · React 19 · TypeScript · Deno · Supabase · PostgreSQL · OpenAI · Clerk · MercadoPago**

Sole developer since the first commit — product, architecture, data model and deployment.

- Serverless backend of **16 Deno Edge Functions** on Supabase
- PostgreSQL hardened with **65 Row Level Security policies** across **34 versioned migrations**
- AI analysis engine on GPT-4o-mini with domain prompts, **JSON-schema-constrained output** and validation before persistence
- **Compensating transaction** on paid model calls: consumed credits are restored automatically when the provider or the write fails
- End-to-end monetization with MercadoPago — checkout, signed webhooks, transaction reconciliation, automatic credit provisioning
- **Zero-data-loss identity migration** from Supabase Auth to Clerk: idempotent sync preserving user IDs, records and payment history, with a dry-run mode
- Portfolio backtesting over historical price series, interactive charts (Chart.js / Recharts) and PDF / CSV export

### Estudialo — EdTech SaaS · [estudialoweb.com](https://estudialoweb.com)

**Next.js 16 · React 19 · TypeScript · Node.js · Express · TypeORM · PostgreSQL · pgvector · OpenAI · LangChain · Clerk · Docker**

Founding frontend developer, co-owner of the backend.

- Frontend grown from the first commit to **57 routes** across public, authenticated and admin areas — **migrated from a Vite/React SPA to Next.js App Router**
- Internal admin back-office used daily by the business: ~20 screens for catalog, content, instructors, webinars, registrations and per-course analytics, with RBAC
- Modular REST API — **47 endpoints, 39 TypeORM entities, 25 versioned migrations**, documented with Swagger
- **Semantic search re-platformed from an in-memory FAISS/HNSWLib index to pgvector inside PostgreSQL** (IVFFLAT), so embeddings survive deploys, restarts and backups
- AI learning paths with OpenAI + LangChain, per-plan depth and graceful degradation when the provider fails
- Microlearning system: staged microcourses, AI-generated PDF theory, graded evaluations, progress tracking and badges
- Credit-based freemium model with concurrency-safe initialization
- Catalog ingestion automated with Puppeteer in Docker — keeps **770+ course records** in sync while preserving manually curated data
- **Authentication owned twice over**: SSO on self-hosted Keycloak (OAuth 2.0 + PKCE, JWT/JWKS, RBAC), then a tested, idempotent migration of legacy production users to **Clerk + Resend**, executed from CI
- CI/CD on GitHub Actions: lint, type-check, **85% coverage thresholds**, build and Playwright E2E on every PR; auto-deploy to a self-hosted VPS runner with PM2, dry-run migrations and a post-deploy health check
- Production log observability with Loki + Promtail + Grafana

---

## Tech Stack

### Frontend
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React_19-20232A?logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js_16-000000?logo=nextdotjs&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?logo=tailwindcss&logoColor=white)
![Radix UI](https://img.shields.io/badge/Radix_UI-161618?logo=radixui&logoColor=white)
![Redux](https://img.shields.io/badge/Redux_Toolkit-764ABC?logo=redux&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-433E38)

### Backend
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?logo=express&logoColor=white)
![Deno](https://img.shields.io/badge/Deno-000000?logo=deno&logoColor=white)
![REST API](https://img.shields.io/badge/REST-API-0A66C2)
![Webhooks](https://img.shields.io/badge/Webhooks-signed-0A66C2)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?logo=swagger&logoColor=black)

### Data
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?logo=supabase&logoColor=white)
![TypeORM](https://img.shields.io/badge/TypeORM-FE0803?logo=typeorm&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-PostgreSQL-4169E1)
![RLS](https://img.shields.io/badge/Row_Level_Security-4169E1)

### AI
![OpenAI](https://img.shields.io/badge/OpenAI-412991?logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757)
![Codex](https://img.shields.io/badge/Codex-111111)

### Security & Authentication
![Clerk](https://img.shields.io/badge/Clerk-6C47FF?logo=clerk&logoColor=white)
![OAuth 2.0](https://img.shields.io/badge/OAuth_2.0_+_PKCE-3C3C3D)
![JWT](https://img.shields.io/badge/JWT-000000?logo=jsonwebtokens&logoColor=white)
![RBAC](https://img.shields.io/badge/RBAC-3C3C3D)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?logo=keycloak&logoColor=white)

### Testing & Delivery
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?logo=vitest&logoColor=white)
![Supertest](https://img.shields.io/badge/Supertest-6E9F18)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white)
![PM2](https://img.shields.io/badge/PM2-2B037A?logo=pm2&logoColor=white)
![Grafana](https://img.shields.io/badge/Loki_%2B_Grafana-F46800?logo=grafana&logoColor=white)

> Keycloak is listed as prior production experience — Estudialo's SSO ran on a self-hosted Keycloak with a custom Keycloakify theme until it was migrated to Clerk in 2026.

---

## How I Work With AI

**Claude Code and Codex are my primary development environment**, with repo-level configuration committed alongside the code so the setup is reproducible for the team.

I own what they produce. The safety net is deliberate: strict TypeScript, lint and type-check gates, enforced coverage thresholds and E2E on every pull request, and dry-run migrations before any schema change reaches production. Architecture, validation and code quality stay under engineering control — the model accelerates the work, it doesn't decide it.

---

## What I Focus On

- Production SaaS architecture that a two-person team can actually maintain
- Clean REST APIs and relational data models with versioned migrations
- Authentication, authorization and application security
- Third-party integrations that stay correct when the other side fails
- Testing and delivery pipelines that block bad releases
- Integrating AI where it adds real product value — and validating what it returns

---

## Languages

- **Spanish:** Native
- **English:** B2 / Upper-Intermediate — I read, write and document in English daily

---

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mariano_Sagua-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/marianosagua)
[![GitHub](https://img.shields.io/badge/GitHub-marianosagua-181717?logo=github&logoColor=white)](https://github.com/marianosagua)
[![Email](https://img.shields.io/badge/Email-marianosagua4343%40gmail.com-EA4335?logo=gmail&logoColor=white)](mailto:marianosagua4343@gmail.com)
