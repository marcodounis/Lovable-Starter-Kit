# Lovable Global Workspace Rules (March 2026)
These rules apply automatically to EVERY new project unless explicitly overridden in Project Knowledge.

## 1. Core Principles
- Always follow Clean Architecture + Feature-Sliced Design
- Mobile-first, fully responsive (Tailwind)
- Accessibility (WCAG 2.2 AA) built-in by default
- Performance: Lighthouse 95+ on mobile
- Security: Supabase RLS + Row Level Security everywhere, never hard-code secrets
- All code must be TypeScript-strict (no `any`)

## 2. Default Technology Stack (override only if needed)
- Frontend: React 19 + TypeScript + Tailwind CSS v4 + shadcn/ui + Radix primitives + Lucide icons
- State: Zustand + TanStack Query
- Forms: React Hook Form + Zod
- Backend: Supabase (PostgreSQL + Auth + Edge Functions + Storage)
- API layer: tRPC (preferred) or typed Supabase client
- Testing: Vitest + React Testing Library + Playwright (E2E)
- Diagrams: Mermaid only (use the exact syntax Lovable renders)
- Styling: Tailwind + dark mode by default (system preference)
- Deployment: Lovable Cloud primary + Vercel/Netlify fallback (GitHub Actions)

## 3. Coding Standards
- File naming: kebab-case for folders/files (e.g. user-profile.tsx)
- Components: PascalCase, hooks: use- prefix
- No console.log in production code (use a logger)
- Every public function/component must have JSDoc
- Error handling: try/catch + user-friendly messages
- No inline styles except Tailwind
- Imports: absolute paths where possible (@/components/...)
- Max line length 100, Prettier + ESLint enforced

## 4. Testing Standards (never skip)
- 85%+ coverage on all logic
- Unit tests for every hook, utility, and complex component
- Integration tests for all Supabase calls
- E2E tests for critical user flows
- Every test must have clear name and be in __tests__ folder
- Use Vitest’s built-in test dashboard page

## 5. Documentation & Diagrams
- All diagrams: Mermaid (sequenceDiagram, flowchart, component, etc.)
- Technical docs live in /docs folder (auto-created pages)
- README.md must include: tech stack, local setup, deployment, test command
- Every major feature gets its own sequence diagram
- API docs in OpenAPI-style tables

## 6. Prompting & Agent Behaviour
- When I say “add to Project Knowledge” → immediately create/update the entry
- Always output in clean Markdown with clear headings and tables
- Use Agent Mode for audits and fixes
- Never invent new dependencies without asking
- If something is ambiguous, ask for clarification before coding

## 7. Security & Compliance Defaults
- All auth: Supabase Auth (email + magic link + social where requested)
- Rate limiting on all public endpoints
- GDPR-ready data handling
- Environment variables never committed

## 8. Deployment & CI/CD Defaults
- Branches: main = Live, develop = Test
- GitHub Actions: test → build → deploy on push to main/develop
- Custom domain ready
- Environment variables: .env.example included

## 9. Future-Proofing
- All components must be reusable and exportable
- Use Lovable’s GitHub sync from day 1
- Keep code clean enough to hand off to any developer

These rules are locked in. Reference them in every prompt with: “Follow all Workspace Knowledge rules.”
