# Change Scope

## Mode

SYSTEM_MAINTENANCE — bounded Canonical Project creation

## Active Project

`Q001 / VIBE_AGY_QUALIFICATION_LAB`

## Allowed Read

- this project
- exact canonical sources named by PACK-03B0
- Project Registry and PACK-03P result

## Allowed Write

- exact project bootstrap files in this repository
- PACK-03B0 commits and push on `main`
- Q001 Project Registry row and PACK-03B0 evidence outside this repository

## Read-only

- `00_SYSTEM/VIBE_CODE/`
- `80_PROJECTS/_PROJECT_TEMPLATE/`
- `80_PROJECTS/CPGS_HUMAN_WORKSPACE/`
- historical PACK00 through PACK03P evidence

## Forbidden

- secrets or credentials
- destructive Git/history actions
- runtime clone, `.agents/`, `.claude/`, runtime context, or runtime overlay
- Antigravity settings, permissions, or project actions
- unrelated refactor or repository mutation

## Exceptions

None.
