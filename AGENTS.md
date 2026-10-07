# Project AGENTS.md

MODE=PROJECT.

## Bootstrap

This project is managed by VIBE CODE. The current Git repository/worktree is the
Active Execution Root. Resolve the Canonical Workspace Root through the verified
runtime-specific bootstrap before non-trivial work, then read:

- `90_WORKSPACE/AGENT_BOOTSTRAP_PROTOCOL.md`
- this repository's `INTAKE_HANDOFF.md`, `PROJECT_BRIEF.md`, `CONTEXT.md`
- `.vibe/CURRENT_STATE.md`, `.vibe/CURRENT_PACK.md`,
  `.vibe/CHANGE_SCOPE.md`, and `.vibe/HANDOVER.md`
- only the canonical VIBE CODE sources required by the active task

Current Pack/state/scope authority lives in `.vibe/`, not in this file. In
`MODE=PROJECT`, the Canonical System and `90_WORKSPACE` are read-only. Write only
inside this Active Execution Root and only under the exact active Pack scope.

## Stable commands

- Run static fixture: `python -m http.server 8000 --directory prototype`
- Test: validate `prototype/index.html` as dependency-free static HTML and run the
  bounded browser QA named by the active qualification Pack.
- Lint: not configured; no application source exists.
- Build: not required; the fixture is static HTML.

## Project-specific constraints

- Qualification-only synthetic fixtures; no production or business function.
- No MISA data, CPGS data, personal/confidential data, credentials, or secrets.
- Keep the Canonical Project runtime-neutral: do not add `.agents/`, `.claude/`,
  runtime context, runtime overlay manifests, or project-local Safe Runner code.
- Runtime lane provisioning requires a separate authorized Pack.
- Do not perform destructive Git/data actions or modify unrelated projects.
- Follow `Outcome -> Spec -> Plan -> Build -> Verify` for non-trivial changes.
