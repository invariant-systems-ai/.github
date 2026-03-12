---
description: Public T0 guardrails for org profile work in this workspace
applyTo: "**"
---

Public workspace scope is limited to:
- aiir/
- invariantsystems.io/
- org-github-profile/

Hard boundary:
- Treat this workspace as public T0 only.
- Do not reference, infer, summarize, or rely on internal repositories, private notes, private infrastructure, undisclosed product plans, patent strategy, or internal project names.
- If a task would benefit from private context, stop and say that public context is insufficient.
- Do not suggest copying text, code, terminology, or architecture from internal work into this workspace.

Operational defaults:
- Prefer local-only workflows by default.
- Do not enable or use networked Hub or integration features unless explicitly requested.
- Do not add commands, docs, or UI copy that imply private capabilities unless those capabilities are already public in this repo.
- Keep all user-facing text safe for docs, release notes, screenshots, and marketplace listing copy.

Repo-specific rules:
- If editing aiir/, read aiir/AGENTS.md first and follow it.
- Keep AIIR stdlib-only where repo rules require it.
- Preserve branding consistency across invariantsystems.io, org-github-profile, and the AIIR extension.
- Reuse existing public assets and copy before inventing new branding.

Primary goals in this workspace:
- improve customer readiness
- improve packaging and release quality
- improve documentation and public onboarding
- improve UX for public-facing features
- keep changes minimal, reviewable, and public-safe

Working style:
- Inspect relevant files first.
- Make the smallest coherent change set.
- Validate with the narrowest useful local command.
- Call out assumptions, risks, and anything not validated.
- When discussing files or behavior, stay grounded in the checked-out code.

Good default focus areas:
- AIIR extension UX and packaging
- public docs and README quality
- marketplace and release polish
- website consistency and verification UX
- org profile clarity and consistency

Avoid by default:
- private or internal workflow design
- hidden feature flags tied to private systems
- speculative enterprise claims not backed by public code or docs
- adding network behavior without an explicit opt-in
