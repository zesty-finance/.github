# Zesty Finance

Personal finance that's genuinely exciting and genuinely credible. Built for people who take their financial future seriously but refuse to be bored by it.

## What We're Building

Zesty Finance is a modern personal finance platform designed for engaged, forward-thinking users. We believe finance tools shouldn't feel cold, legacy, or compliance-driven — money should feel like it's working as hard as the person using it.

## Architecture

Zesty Finance is composed of three packages:

| Package | Description | Stack |
|---|---|---|
| **zesty-finance-shared** | Shared schemas, types, and constants | TypeScript, Zod v4 |
| **zesty-finance-api** | REST API and authentication server | Express.js, PostgreSQL, Kysely, better-auth |
| **zesty-finance-ui** | SSR-capable web application | React 19, TanStack (Router + Start + Query), Mantine, Vite |

All packages run on **Node.js 24** with **TypeScript 6** and **ES Modules**.

## Core Capabilities

- **Authentication** — Email/password, Google OAuth, and Apple OAuth with email verification and password reset flows
- **Account Management** — Profile, avatar, username, email, password, and subscription settings
- **CMS** — Page types, versioned pages, and policy management with acceptance tracking
- **Admin Dashboard** — Account management, content publishing, and platform analytics
- **Authorization** — Role-based access control with admin and user roles

## Tech Highlights

- **Type-safe from database to UI** — Zod schemas in the shared package validate API requests and power form validation across the stack
- **SSR with streaming** — TanStack Start handles server-side rendering with query prefetching
- **better-auth** — Session management, OAuth providers, and custom plugins for sign-up acceptance flows
- **Kysely** — Type-safe SQL query builder with UUIDv7 primary keys
- **Mantine v8** — Component library with custom theme, SCSS modules, and responsive layouts

## Contributing

Each package has its own repository, CI pipeline, and documentation. See the individual package READMEs for setup instructions and development guides.
