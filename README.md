# Judicial Decision Support — Frontend (Prototype)

This repository contains a mobile-first React + TypeScript frontend prototype that demonstrates an accessible, auditable, human-in-the-loop UI for judicial workflows.

Quick start (dev):

```bash
npm install
npm run dev
```

Testing:

```bash
npm test
# E2E
npm run e2e
```

What this deliverable includes:
- Responsive case list & detail views
- AI Insights panel with model metadata and "AI recommendation" labels
- Provenance modal linking to source snippets and signed URLs
- RBAC-aware action bar requiring explicit rationale for consequential actions
- Immutable audit log viewer
- API contract docs, deployment notes, accessibility & bias assessment
- HTML prototype in `/prototype` mimicking key flows

Notes: This is a frontend-focused deliverable. Backend endpoints (signed URLs, explanations, audit logs) must be provided by the server described in `docs/api.md`.
