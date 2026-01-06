# Deployment Guide

- Build: `npm run build`
- Serve behind HTTPS reverse proxy (nginx) with strict CSP headers and HSTS.
- Container example: build static assets and serve with nginx; ensure cookies set with `SameSite=Strict`, `Secure`.
- Secrets: do not store API keys in frontend. Server issues signed URLs and validates roles.
- CI: run `npm test` and `npm run build` before deploy.

Security checklist
- HTTPS only
- Content-Security-Policy restricting scripts to same-origin
- Minimal third-party scripts
- Session timeout enforced server-side
- Require re-auth and capture rationale for consequential actions
