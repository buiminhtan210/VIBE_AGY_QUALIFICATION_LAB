# Project Context

## Current architecture

- Canonical, runtime-neutral Git repository.
- Dependency-free static browser fixture at `prototype/index.html`.
- Project governance and execution state in the root documents and `.vibe/`.

## Important modules / entry points

- `prototype/index.html` — reusable browser qualification target.
- `PROJECT_BRIEF.md` — mission and boundaries.
- `.vibe/CURRENT_STATE.md` — current project readiness.

## Data model / key entities

- Canonical Project ID: `Q001`.
- Project name: `VIBE_AGY_QUALIFICATION_LAB`.
- Qualification fixture: static, synthetic-only HTML.

## External services / APIs

None. The fixture has no network or third-party dependency.

## Environment / dependencies

No package installation or build tool is required. An optional local static HTTP
server may be used for browser QA.

## Important terminology

- Canonical Project: durable source-of-truth repository under `80_PROJECTS`.
- Runtime Lane: separately authorized execution infrastructure outside this
  canonical project.
- Qualification: bounded verification, not production acceptance.

## Known constraints

- Synthetic-only; no production/business data or confidential material.
- Runtime-neutral canonical tree; no vendor-specific deployment artifacts.

## Commands

- Run: `python -m http.server 8000 --directory prototype`
- Test: inspect static HTML and run the bounded browser QA authorized by the active
  qualification Pack.
- Lint: not configured.
- Build: not required.

## Domain Authority / Source of Truth

- Domain owner: VIBE CODE Orchestrator.
- Canonical source: this repository plus the controlling VIBE CODE Pack/policies.
- Accepted business rules: there is no business domain; qualification is
  synthetic-only.

## Domain knowledge location

No external domain knowledge is required.

## Things an AI agent must not assume

- `RUNTIME_LANE_REQUESTED` means a runtime is provisioned or qualified.
- Antigravity settings, permissions, or runtime roots may be changed without a
  separate Pack.
- Runtime-generated state belongs in this canonical repository.
