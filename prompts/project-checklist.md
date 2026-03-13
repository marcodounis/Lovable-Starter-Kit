# Lovable Project Day-Zero Checklist
**Version: March 2026**  
Use this checklist for **every single new project**.  
It takes 45–60 minutes and turns any idea into a fully documented, tested, deployable app with perfect consistency.

Copy this file into your `lovable-starter-kit` repo (or pin it in Notion) and tick the boxes as you go.

## Prerequisites (do these once per workspace)
- [ ] Workspace Knowledge is already pasted and saved (see `workspace-knowledge.md`)
- [ ] You have the full `prompts/` folder open (GitHub or local clone)
- [ ] Lovable GitHub sync is ready (connect your GitHub account in settings)

## Step-by-Step Checklist

### Phase 0: Start the Project
- [ ] Create a **new project** in Lovable.dev
- [ ] Give it a clear name (e.g. “client-portal-v1”)
- [ ] Immediately open **Project Knowledge** (left sidebar) — leave it open

### Phase 1: Foundation (Template 0)
- [ ] Copy and paste the entire content of `prompts/00-foundation-kickoff.md`
- [ ] Replace **[APP_NAME]** and **[ONE-SENTENCE DESCRIPTION]**
- [ ] After it finishes: type “Add this to Project Knowledge”
- [ ] Verify PRD and user journeys appear in Project Knowledge

### Phase 2: Tech Stack & Architecture (Template 1)
- [ ] Paste `prompts/01-technology-stack.md`
- [ ] After it finishes: type “Add this to Project Knowledge”
- [ ] Confirm the Mermaid architecture diagram rendered correctly

### Phase 3: Sequence Diagrams (Template 2)
- [ ] Paste `prompts/02-sequence-diagrams.md`
- [ ] After generation: type “Add this to Project Knowledge”
- [ ] Go to the newly created `/docs/sequence-diagrams` page and confirm diagrams are embedded

### Phase 4: Test Cases (Template 3)
- [ ] Paste `prompts/03-test-cases.md`
- [ ] After it finishes: type “Add this to Project Knowledge”
- [ ] Confirm `/docs/test-strategy` page was created

### Phase 5: Full Technical Documentation (Template 4)
- [ ] Paste `prompts/04-technical-documentation.md`
- [ ] After it finishes: type “Add this to Project Knowledge”
- [ ] Confirm the `/docs` folder now contains API docs, principles, architecture, mobile strategy, etc.

### Phase 6: Unit Tests (Template 5)
- [ ] Paste `prompts/05-unit-tests.md`
- [ ] Switch to **Agent Mode** and let it generate + run the tests
- [ ] Confirm test dashboard page exists and tests pass (85%+ coverage)

### Phase 7: Deployment & Playbook (Templates 6 + 7)
- [ ] Paste `prompts/06-deployment.md`
- [ ] Paste `prompts/07-future-playbook.md` (right after)
- [ ] After both finish: type “Add this to Project Knowledge”
- [ ] Sync project to GitHub (click the GitHub button in Lovable)
- [ ] Create `/docs/deployment` and `/docs/playbook` pages

### Final Polish & Launch
- [ ] Run Agent Mode once more: “Audit the entire codebase against the PRD, architecture, and Workspace Knowledge. Fix any issues.”
- [ ] Turn on **Test environment** and publish a preview link
- [ ] Add custom domain (if ready) or share the preview
- [ ] Commit the first version with message “Day-Zero foundation complete”
- [ ] Star this checklist and mark the project as “Ready for feature development”

## One-Shot Alternative (for tiny projects)
If you want everything in one prompt instead of 8 steps:
1. Paste `prompts/full-foundation-one-shot.md`
2. Still do the “Add to Project Knowledge” and GitHub sync steps above.

## Quick Reference
- All prompts live in `/prompts/`
- Global rules are in Workspace Knowledge
- Documentation lives at `/docs` inside your app
- GitHub repo is your source of truth

**You are now finished.**  
Your project has:
- Complete requirements
- Architecture + diagrams
- Full test suite
- Professional documentation
- Production deployment ready
- Future-proof playbook

Bookmark this checklist — you will use it on every project forever.

---
Made with ❤️ for speed and consistency.  
Last updated: March 2026
