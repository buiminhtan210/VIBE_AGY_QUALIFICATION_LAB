# Change Scope

## Mode

`SYSTEM_MAINTENANCE`

## Active Project

`Q001 / VIBE_AGY_QUALIFICATION_LAB`

## Active authorized phase

`PACK-04B1_CHATGPT_PLATFORM_DEPLOYMENT_CLOSEOUT_AND_DURABLE_SYNC`

## Allowed read

- Q001 project governance and `.vibe` state.
- PACK-04A, PACK-04B0, and orchestrator-supplied PACK-04B deployment evidence.
- Exact current canonical ChatGPT deployment fingerprints.
- Execution Lane and Runtime Capability registries for readback only.
- Protected roots for pre/post fingerprinting only.

## Allowed write

- `.vibe/CURRENT_STATE.md`
- `.vibe/CURRENT_PACK.md`
- `.vibe/CHANGE_SCOPE.md`
- `.vibe/HANDOVER.md`
- `.vibe/VERIFICATION_LOG.md`
- Exactly one normal local commit on `main` with the scoped `.vibe` delta.

## Read-only / protected

- `00_SYSTEM/VIBE_CODE/`
- `90_WORKSPACE/PROJECT_REGISTRY.md`
- `90_WORKSPACE/EXECUTION_LANE_REGISTRY.md`
- `90_WORKSPACE/RUNTIME_CAPABILITY_REGISTRY.md`
- `D:\VIBE_AGENT_RUNTIME\ANTIGRAVITY\VIBE_AGY_QUALIFICATION_LAB`
- `D:\LOCAL_WORKSPACE_CPGS`
- published Agent Return bundle
- ChatGPT and Antigravity platform/settings state

PACK evidence under
`90_WORKSPACE/SYSTEM_MAINTENANCE_TASKS/VIBE_UNIVERSAL_PROJECT_RUNTIME_PROVISIONING_01/`
is written separately by the SYSTEM_MAINTENANCE orchestrator and is not part of
the Q001 Git commit.

## Forbidden

- push, fetch, pull, merge, reset, clean, rebase, amend, force, history rewrite,
  or branch switch;
- product/fixture/root-governance changes outside the five `.vibe` files;
- runtime, Antigravity, settings, permission, CPGS, registry, bundle, or platform
  mutation;
- Resident Knowledge upload or Project Instructions deployment;
- fresh-session/fresh-account validation;
- SYSTEM KNOWN GOOD or PACK-04 completion claim.

## Stop point

Stop after the local PACK-04B documentary commit and clean/ahead-one verification.
Manual GitHub Desktop push and exact remote readback are required before PACK-04C
fresh-session validation opens.
