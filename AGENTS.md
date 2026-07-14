# AGENTS.md

## Project identity

Frontier Company is a compact, pausable, systems-driven strategy game being developed in Unity by a solo developer. The player builds and controls a small organization operating inside a changing regional ecosystem.

The project prioritizes ownership, company identity, meaningful risk, systemic interaction, contextual strategy, emergent consequences, bounded campaigns, finishable scope, and early testability.

## How agents should work in this repository

- Read `README.md` and the files in `docs/` before making project-shaping changes.
- Treat `docs/vision.md`, `docs/current-state.md`, `docs/decisions.md`, and `docs/milestones.md` as source-of-truth constraints.
- Make small, reversible changes that fit a solo Unity project.
- Do not invent detailed gameplay systems, balance rules, resources, factions, map structures, campaign rules, or content taxonomies unless the user has explicitly decided them.
- If a request appears to require a structural, architectural, or design-direction change, propose a short plan before editing.
- Planning is not required for small mechanical edits, documentation maintenance, or narrow implementation tasks that fit existing decisions.
- Prefer clarity over abstraction. Avoid process overhead that would be more suitable for a larger team.

## Documentation responsibilities

- Update `docs/current-state.md` when implementation reality changes.
- Update `docs/decisions.md` when a durable decision is accepted, opened, or rejected.
- Update `docs/milestones.md` when milestone status or playable-chunk priorities change.
- Use living notes for exploration, but promote only stable outcomes into the source-of-truth docs.

## Living notes workflow

Living notes may be added later under `docs/notes/` when useful. They are for rough thinking, observations, experiments, and questions. They are not source-of-truth until summarized into one of the core docs.

When converting notes into decisions:

1. Identify the concrete question or tension.
2. Move durable conclusions into `docs/decisions.md` as accepted, open, or rejected entries.
3. Update `docs/current-state.md` only if the note describes something that is now true in the repository.
4. Update `docs/vision.md` only if the note changes a stable project constraint.
5. Keep raw notes short and disposable.

## Unity expectations

- Preserve standard Unity project structure.
- Avoid unnecessary third-party dependencies.
- Treat serialized scenes, prefabs, and assets carefully.
- Do not assume a gameplay architecture before it has been decided.
- Testing strategy is currently undecided; do not introduce a test framework without approval.

## Verification expectations

When making changes, report what was inspected or tested. If Unity Editor checks or automated tests cannot be run in the environment, say so explicitly.
