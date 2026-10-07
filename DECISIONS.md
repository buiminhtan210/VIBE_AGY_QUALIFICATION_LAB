# Project Decision Log

## DEC-001 — Runtime-neutral synthetic qualification lab

- Date: 2026-10-07
- Status: Accepted

### Context

VIBE CODE needs a reusable project for validating runtime provisioning, adapters,
Safe Runner, overlays, and future compatible runtimes without using CPGS or other
production/business projects.

### Decision

Use Q001 as a dependency-free, synthetic-only Canonical Project. Keep all
runtime-specific deployment files outside the canonical checkout and require a
separate Pack for every runtime lane.

### Why

This isolates qualification risk, protects business projects, and preserves the
boundary between canonical project authority and replaceable runtime execution
infrastructure.

### Consequences

- The canonical repository contains only stable project context and static fixture.
- `.agents/`, `.claude/`, runtime context, overlays, and Safe Runner copies are
  forbidden here.
- Installed-runtime PASS must come from a later qualification Pack.

### Revisit when

A canonical policy change requires a different reusable qualification topology.
