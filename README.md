# GPT-For-PR

GPT-For-PR is a Next.js 16 + TypeScript web application that serves as the foundation for a GitHub pull request review workflow manager.

## What it does today
- Supports GitHub authentication for user sign-in via OAuth.
- Provides GitHub App installation and connection management.
- Receives GitHub pull request webhooks for `opened`, `synchronize`, and `reopened` events.
- Persists repository installation and pull request metadata in PostgreSQL via Prisma.
- Exposes a protected dashboard experience for authenticated users.

## Roadmap
- Ingest support is planned for the next sprint, enabling GitHub PR data to be imported and preprocessed.
- AI review functionality will be implemented after ingest is available.

## Getting Started

First, install dependencies and run the development server:

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to view the app.

## Project details
- Framework: Next.js 16 App Router
- Language: TypeScript
- Database: PostgreSQL with Prisma
- GitHub integration: GitHub OAuth and GitHub App webhook handling
- UI: Tailwind CSS and shadcn/ui-inspired components

## Notes
- The current app includes authentication and GitHub installation flows, but AI-based review generation is not yet implemented.
- The next sprint will focus on ingesting PR data first, followed by AI review capabilities.
