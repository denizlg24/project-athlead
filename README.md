# project-dvco

> A modern platform for leaders and teams to set goals, track progress, and share wins — built for simplicity, transparency, and motivation.

## 🚀 Overview

This project aims to create a **leadership and team performance platform** where users can define objectives, share updates, give feedback, and recognize achievements in an engaging, collaborative way. The focus is on real communication and progress — not vanity metrics.

## 🧱 Architecture

* **Frontend:** [Next.js](https://nextjs.org/) (App Router, Server Components, TailwindCSS)
* **Backend:** [NestJS](https://nestjs.com/) with [tRPC](https://trpc.io/)
* **Database:** PostgreSQL (via Prisma ORM)
* **Infra:** Turborepo + Docker + optional microservices for scalable modules
* **Auth:** NextAuth.js (OAuth, credentials, or SSO)
* **Messaging:** WebSockets (real-time updates)

The setup is flexible — small teams can start with a single repo, while larger orgs can scale out each service independently.

## 📦 Monorepo Structure

```
/project-dvco
 ├── apps/
 │   ├── web/        # Next.js frontend
 │   └── api/        # NestJS backend
 ├── packages/
 │   ├── ui/         # Shared UI components
 │   ├── trpc/       # Shared API types & procedures
 │   └── config/     # Shared configs (ESLint, Tailwind, etc.)
 └── docker/         # Docker setup and service configs
```

## 🧭 Local Development

```bash
git clone https://github.com/denizlg24/project-dvco.git
cd project-dvco
pnpm install
pnpm dev
```

Make sure Docker is running if you’re using the containerized setup.

## 🧩 Project Management

We’re using **GitHub Projects (Board View)** with the following workflow:

* **Ideas / Requests:** New feature suggestions.
* **To Do:** Features or bugs ready for dev.
* **In Progress:** Actively being developed.
* **Review:** Ready for testing or feedback.
* **Done:** Completed and merged.

## 🧠 How to Contribute

If you’re not coding but want to suggest a new feature or report a bug, use the issue templates in the **Issues** tab. They’re designed to guide you through describing what you want clearly.
