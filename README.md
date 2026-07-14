<div align="center">

# Hey there, I'm Bappi Rahman 👋

**Full Stack Engineer · Software Engineer · Technical Writer**

*Dhaka, Bangladesh 🇧🇩*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/bappi-rahman)
[![X](https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/_bappi_rahman)
[![BoringDocs](https://img.shields.io/badge/BoringDocs-7c6fff?style=flat-square&logoColor=white)](https://boringdocs.dev)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:cs.bappirahman@gmail.com)

</div>

---

## 🧑‍💻 About Me

I'm a Full Stack Engineer from Dhaka who builds production systems, developer tools, and documentation that doesn't assume you already know everything.

I started with a Diploma in Computer Science, worked as a Software Engineer at **24Studio** building internal dashboards, payment integrations, and client-facing portals — and now I'm focused on open source work and learning in public through **BoringDocs**.

I care about:
- **Shipping things that actually work** — not just demos, but deployed, load-tested, production systems
- **Writing code that's readable** — not clever for the sake of being clever
- **Explaining things clearly** — which is why I write technical documentation alongside building
- **Understanding the why** — not just copying patterns but knowing the tradeoffs behind every decision

Currently studying **B.Sc. in Computer Science & Engineering** at Northern University Bangladesh while building in public.

---

## 🔭 What I'm Building

### ⚡ [autoFlow](https://autoflow.boringdocs.dev) — Open Source Workflow Automation

> *Build workflows visually. Run them reliably. Ship to production.*

A workflow automation platform with a visual canvas editor, durable execution engine, and real-time node status updates — think a self-hostable alternative to Zapier or Make, built for developers.

**What's under the hood:**

- **NestJS + Next.js Nx monorepo** with a shared TypeScript library (`@autoflow/shared`) as single source of truth for node types and status enums across both apps
- **Durable execution engine** via Inngest — BFS reachable node calculation, topological sort, sequential executor loop with step memoization and automatic retries
- **9 node executors** — Manual Trigger, HTTP Request, Google Form, Stripe, Anthropic, OpenAI, Gemini, Discord, Slack — each following a `LOADING → validate → execute → SUCCESS/ERROR` pattern
- **Real-time node status** via `@inngest/realtime` — one pub/sub channel per node type keyed by userId, consumed by a custom `useNodeStatus` hook in the frontend
- **AES-256-GCM credential encryption** at rest — credentials decrypted only inside executors at runtime, never exposed in API responses
- **Webhook ingestion pipeline** for Google Form and Stripe triggers with secret-based routing and idempotent registration
- **Deployed to DigitalOcean** (Ubuntu 24.04, Nginx, PM2, GitHub Actions CD with SSH deploy on push to main)

**Benchmark results** (k6 load test, 100 VUs peak):

| Metric | Value |
|--------|-------|
| Min Latency | 46ms |
| Webhook Ingestion P95 | 923ms |
| Total Requests Benchmarked | 20,000+ |
| Peak Concurrency | 100 VUs |
| P99 at Peak Load | 2.36s |
| Credential Encryption | AES-256-GCM |

**Tech stack:** `NestJS` `Next.js` `TypeScript` `Inngest` `PostgreSQL` `Drizzle ORM` `BetterAuth` `Polar` `Nx` `React Flow` `Tailwind CSS` `Nginx` `GitHub Actions`

🔗 [Live](https://autoflow.boringdocs.dev) · [GitHub](https://github.com/bappirahman/autoFlow)

---

### 📚 [BoringDocs](https://boringdocs.dev) — Technical Documentation for Node.js Developers

> *The docs you wish existed when you were stuck.*

A technical documentation platform targeting Node.js and TypeScript developers. 60+ published articles written from first principles — no knowledge assumed beyond what's explicitly listed.

**What's covered:**

| Module | Articles | Topics |
|--------|----------|--------|
| SQL & PostgreSQL | 15 | Schema design, queries, indexing, Prisma, Drizzle |
| NoSQL & MongoDB | 9 | Document model, aggregation, use cases |
| Message Queues | 10 | RabbitMQ, BullMQ, Kafka, patterns |
| REST API Design | 8 | Principles, versioning, error handling, auth |
| Inngest & Event-Driven | 13 | Durable execution, steps, retries, fan-out, observability |

**Writing philosophy:**
- **Assumption-free** — every article lists exactly what you need to know before reading it
- **Analogy-first** — real-world comparisons before technical definitions
- **Runnable examples** — every concept has working code you can copy and run
- **Honest about trade-offs** — no "always use X" advice without explaining when not to

🔗 [boringdocs.dev](https://boringdocs.dev)

---

## 💼 Experience

### Software Engineer @ [24Studio](https://24studio.org)
*Nov 2025 – Apr 2026 · Dhaka, Bangladesh · Hybrid*

- Built a full-stack admin dashboard with role-based access control (RBAC), real-time data tables, and REST API integration using React, TypeScript, and React Query
- Developed a partner portal with reusable component architecture using Shadcn/ui and Tailwind CSS
- Integrated **SSLCommerz** payment gateway and built end-to-end e-commerce order management flows
- Configured Cloudflare Tunnel on Ubuntu Linux servers for secure internal service exposure
- Mentored junior engineers on software design patterns, code review, and Git workflows

---

## 🛠️ Tech Stack

**Languages**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**Backend**

![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-009688?style=flat-square&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Shadcn/ui](https://img.shields.io/badge/Shadcn/ui-000000?style=flat-square&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Drizzle ORM](https://img.shields.io/badge/Drizzle_ORM-C5F74F?style=flat-square&logoColor=black)

**DevOps & Cloud**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![DigitalOcean](https://img.shields.io/badge/DigitalOcean-0080FF?style=flat-square&logo=digitalocean&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

---

## 📊 GitHub Stats

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=bappirahman&show_icons=true&theme=radical&count_private=true&hide_border=true" height="165" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=bappirahman&layout=compact&theme=radical&hide_border=true" height="165" />
</p>

<p align="left">
  <img src="https://streak-stats.demolab.com/?user=bappirahman&theme=radical&hide_border=true" />
</p>

<p align="left">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=bappirahman&theme=react-dark&hide_border=true&area=true" width="100%" />
</p>

---

## 🌱 Currently Learning

- Advanced system design patterns for distributed systems
- Deeper TypeScript compiler internals
- Performance optimization at the infrastructure level
- Building more in public — writing, shipping, documenting

---

## 🤝 Volunteering & Leadership

- **Mentor & Developer @ 24Studio** — Guided junior developers on system design, code review practices, and Git workflows
- **ICT Secretary @ GAI Rover Scout Group** — Led technology initiatives during COVID-19 community programs; managed digital communications and internal tools

---

## 📫 Reach Me

- 📧 Email: [cs.bappirahman@gmail.com](mailto:cs.bappirahman@gmail.com)
- 🐦 X: [@_bappi_rahman](https://x.com/_bappi_rahman)
- 💼 LinkedIn: [bappi-rahman](https://linkedin.com/in/bappi-rahman)
- 🌐 Portfolio: [boringdocs.dev](https://boringdocs.dev)

---

<div align="center">

*If you're building something interesting, let's talk.*

</div>
