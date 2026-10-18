# Decisions

This file records durable project decisions. It should stay lightweight and should not become a full design document.

## Accepted

### 2026-07-14 — Unity project

- **Decision:** Frontier Company is being developed in Unity.
- **Rationale:** The project has been described as a Unity strategy game and the repository contains Unity project settings and packages.
- **Consequences:** Repository guidance should preserve standard Unity project structure and avoid unnecessary non-Unity assumptions.
- **Related docs:** `README.md`, `docs/current-state.md`


### 2026-07-14 — Real-Time with Pause time model

- **Decision:** Frontier Company should use Real-Time with Pause (RTWP), operating on a simultaneous tick-based system.
- **Rationale:** The game needs a time model that supports systemic interaction while allowing the player to pause, inspect, and make contextual strategic decisions.
- **Consequences:** Documentation should describe pause as part of the RTWP time model rather than as a loose central identity label. Future representative gameplay implementation should account for simultaneous tick resolution, but detailed timing, tick length, scheduling, and simulation architecture remain undecided. The earliest interaction prototype does not need to implement this time model.
- **Related docs:** `docs/vision.md`, `docs/current-state.md`, `AGENTS.md`

### 2026-07-14 — Solo-developer scope

- **Decision:** The project foundation should stay suitable for a solo developer.
- **Rationale:** The game is being developed by a solo developer and should remain finishable.
- **Consequences:** Avoid heavy production process, large-team workflows, and architecture that only pays off at large scale.
- **Related docs:** `docs/vision.md`, `docs/milestones.md`

### 2026-07-14 — Source-of-truth core docs

- **Decision:** Core documentation should act as source-of-truth constraints for Codex implementation work.
- **Rationale:** Codex needs durable project context to avoid inventing systems or drifting from the intended direction.
- **Consequences:** `docs/vision.md`, `docs/current-state.md`, `docs/decisions.md`, and `docs/milestones.md` should remain clear, current, and constraint-oriented.
- **Related docs:** `AGENTS.md`, `README.md`

### 2026-07-14 — Living notes can feed decisions later

- **Decision:** Living notes may be added later as rough inputs, but they are not source-of-truth until promoted into the core docs.
- **Rationale:** The project benefits from free-form thinking while still giving Codex stable constraints.
- **Consequences:** Future notes should be short, clearly provisional, and periodically summarized into accepted, open, or rejected decisions.
- **Related docs:** `AGENTS.md`

### 2026-07-14 — Playable-chunk milestones

- **Decision:** Milestones should be organized around free-flowing playable chunks rather than rigid production phases.
- **Rationale:** Playable validation fits the project's emphasis on early testability and compact solo development.
- **Consequences:** Milestones should describe goals, inclusions, exclusions, and verification instead of detailed sprint plans.
- **Related docs:** `docs/milestones.md`

### 2026-07-14 — Testing strategy deferred

- **Decision:** Testing strategy is currently undecided.
- **Rationale:** The project is still establishing its foundation, and testing should be revisited after early Unity/project structure decisions are clearer.
- **Consequences:** Do not introduce a testing framework or mandate a test workflow yet.
- **Related docs:** `AGENTS.md`, `docs/current-state.md`

### 2026-10-18 — Validate a basic interaction before a gameplay loop

- **Decision:** The first implementation target should be a basic interaction proof rather than a representative gameplay loop.
- **Rationale:** Starting with a real-time, tick-event-driven loop reaches too early into unresolved gameplay and architecture decisions. A smaller proof can validate the project's basic player-input and feedback path with less cost and fewer assumptions.
- **Consequences:** The current milestone should contain one choice, one immediate visible state change, and a reset path. RTWP, simultaneous ticks, event-driven simulation, regional systems, and durable gameplay architecture are deferred until a smaller interaction works and is easy to change.
- **Related docs:** `docs/current-state.md`, `docs/milestones.md`, `docs/vision.md`

## Open

### Basic interaction content

- **Question:** What concrete choice and visible state change should the basic interaction proof use?
- **Options:** To be chosen for clarity and implementation simplicity; it does not need to represent the final game loop.
- **Needed before:** Implementing the basic interaction proof.

### Unity import state

- **Question:** What project setup details should be documented after Unity Hub and Unity have completed their required actions?
- **Options:** To be determined after import.
- **Needed before:** Expanding setup instructions in `README.md`.

### Gameplay architecture

- **Question:** What architecture should production gameplay systems use?
- **Options:** To be determined after the basic interaction proof and a later small decision loop reveal what structure is actually needed.
- **Needed before:** Implementing durable production gameplay systems.

## Rejected

### 2026-07-14 — Heavy upfront production process

- **Rejected:** Establishing heavyweight project management, large-team production workflows, or extensive templates at the foundation stage.
- **Reason:** The project is solo-developed and should stay compact, flexible, and finishable.

### 2026-07-14 — Inventing detailed systems before validation

- **Rejected:** Defining detailed gameplay systems, balance values, content taxonomies, or simulation rules before they are needed for a playable chunk.
- **Reason:** Premature detail could constrain discovery and create false source-of-truth assumptions.

### 2026-10-18 — Tick-driven simulation as the first prototype boundary

- **Rejected:** Requiring the first prototype to establish real-time ticking, a gameplay event system, or representative simulation architecture.
- **Reason:** Those concerns are deeper than the immediate need to prove that one player action can produce a clear, inspectable result. This rejection concerns prototype order, not the accepted RTWP direction for the game.
