## Mariano Sagua

Full stack engineer in Buenos Aires. I build and operate production web products end to end — data model, APIs, interface, security and deployment.

At GBFlux I work across two live platforms: a FinTech product for AI investment analysis and an EdTech platform with AI-generated learning paths.

### Selected work

**Invertilo** — FinTech · [invertilo.com.ar](https://invertilo.com.ar)

Serverless TypeScript APIs on PostgreSQL under row-level security. Payments run on signature-verified, idempotent webhooks, with a compensating transaction that restores credits when a paid model call or the write that follows it fails. Production identity migrated with no data loss.

**Estudialo** — EdTech · [estudialoweb.com](https://estudialoweb.com)

Node.js and Express REST API on PostgreSQL with TypeORM. Learning paths generated through function calling with strict JSON schemas, semantic search on embeddings in pgvector, and an assessment layer that scores evaluations, limits attempts and gates progression. Unit, integration and end-to-end tests run on every pull request.

### How I work

Claude Code and Codex are part of my daily environment, with their configuration committed alongside the code. What they produce is mine to defend: strict TypeScript, lint and type gates, coverage thresholds on critical modules, end-to-end tests, and dry-run migrations before any schema change reaches production.

Most of my work sits close to failure — webhooks that arrive twice, providers that fail mid-operation, migrations that run while people are using the app.

### Stack

TypeScript · React · Next.js · Node.js · Express · Deno · PostgreSQL · Supabase · TypeORM · pgvector · OpenAI · LangChain · Docker · GitHub Actions · Vercel

### Contact

[LinkedIn](https://www.linkedin.com/in/marianosagua) · marianosagua4343@gmail.com

Spanish (native) · English (B2)

Both products are live. Happy to walk through the decisions behind any of the work above.
