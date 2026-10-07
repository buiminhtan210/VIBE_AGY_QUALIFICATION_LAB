# Project Brief

## Project

- Project ID: `Q001`
- Name: `VIBE_AGY_QUALIFICATION_LAB`
- Owner: VIBE CODE qualification governance
- Canonical Project Path: `D:\VIBE_CODE_WORKSPACE_BASELINE\80_PROJECTS\VIBE_AGY_QUALIFICATION_LAB`
- Repository: `https://github.com/buiminhtan210/VIBE_AGY_QUALIFICATION_LAB`

## Upstream / Domain Source

- Domain/project: VIBE CODE runtime qualification
- Handoff: `PACK-03B0_QUALIFICATION_LAB_CANONICAL_PROJECT_BOOTSTRAP`
- Domain decision owner: VIBE CODE Orchestrator

## Problem / Desired Outcome

Maintain one reusable Canonical VIBE Project for synthetic qualification of
universal runtime provisioning, Antigravity adapters, Universal Safe Runner,
runtime overlays, and future compatible runtimes.

## Primary User

VIBE CODE maintainers and authorized runtime-qualification operators.

## User Journey

1. Use this accepted Canonical Project identity as the qualification source.
2. Open a separately authorized runtime-lane Pack.
3. Provision and qualify the runtime outside this canonical checkout.
4. Preserve the canonical repository as runtime-neutral project authority.

## Decision Needs

- Is the candidate runtime lane derived from the exact accepted project base?
- Do shared adapters and Safe Runner work without per-project runtime files?
- Can results return through the canonical VIBE governance path?

## Inputs

- Synthetic static fixture under `prototype/`.
- VIBE CODE policies, profiles, and runtime provisioning records referenced by an
  authorized Pack.

## Outputs

- Deterministic qualification evidence produced by later runtime Packs.
- No production or business output.

## Constraints

- Synthetic data only.
- No MISA data, CPGS data, personal/confidential data, credentials, or secrets.
- No external CDN, remote asset, JavaScript dependency, framework, or package
  installation for the static fixture.
- Canonical Project remains runtime-neutral.

## Non-scope

- Production/business functionality.
- Antigravity installation, settings, permissions, project creation, or runtime
  lane provisioning.
- Canonical VIBE CODE System, Skills, Safe Runner, or runtime adapter copies.

## Proposed Architecture

A minimal static HTML fixture plus durable project context and `.vibe` execution
state. Runtime-specific infrastructure is created only in a separate execution
lane under separate authority.

## Acceptance Criteria

- Canonical Q001 identity and repository are coherent.
- Static qualification fixture is dependency-free and visibly identifies the lab.
- Required project and `.vibe` files are present and readable.
- No vendor-specific runtime deployment files or secrets exist.

## Risks / Assumptions

- Runtime qualification remains pending until a later authorized Pack.
- A future runtime may require explicit UI authorization; that does not change this
  project's canonical identity.
