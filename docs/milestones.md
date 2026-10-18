# Milestones

Milestones for Frontier Company should be lightweight and organized around playable validation chunks. They are not rigid production phases or calendar commitments.

## Completed milestone: Production foundation

### Goal

Create a small documentation and agent-guidance foundation that supports solo Unity development, design clarity, and future Codex implementation work.

### Includes

- Root `AGENTS.md` for agent instructions.
- Updated `README.md` as the repository entry point.
- `docs/vision.md` for stable project identity and constraints.
- `docs/current-state.md` for factual repository state.
- `docs/decisions.md` for accepted, open, and rejected decisions.
- `docs/milestones.md` for lightweight playable-chunk direction.

### Excludes

- Detailed gameplay systems.
- New Unity scenes.
- New scripts.
- Detailed testing framework decisions.
- Detailed Unity setup instructions before Unity Hub import is complete.
- Architecture decisions not yet required by a playable chunk.

### Verification

- All foundation files exist.
- Each foundation file has a distinct responsibility.
- Core docs can be used as source-of-truth constraints by Codex.
- Current-state claims match the repository.
- No detailed undecided gameplay systems are invented.

## Current milestone: Basic interaction proof

### Goal

Create the smallest possible Unity interaction that confirms the project can accept a player choice, change a value, communicate the result, and reset cleanly.

### Includes

- One scene.
- One clearly labeled player choice.
- One small, visible state value.
- Immediate feedback showing how the choice changed that value.
- A simple reset or replay path.
- Temporary implementation where that keeps the proof easy to change.

### Excludes

- A complete or representative gameplay loop.
- Real-time progression, pause controls, ticks, or an event-driven simulation framework.
- A regional ecosystem, company simulation, economy, campaign, or content taxonomy.
- Production architecture, final UI, production art, balance, or polish.

### Verification

- A player can understand the available choice without explanation.
- Making the choice causes exactly one readable state change.
- The result is visible immediately.
- The interaction can be reset and repeated in seconds.
- No system is added solely to support anticipated later gameplay.

## Candidate next milestone: Tiny decision loop

### Goal

Turn the proven interaction into one short before-choice-after cycle that asks a meaningful but deliberately narrow question.

### Includes

- A starting state.
- A small number of understandable options.
- One immediate consequence per option.
- A clear end state and replay path.

### Excludes

- Continuous time or tick scheduling unless the decision specifically cannot be tested without it.
- Multiple interacting simulations.
- Content breadth or long-term progression.

## Candidate later milestone: Time-model validation

### Goal

Test the smallest slice of RTWP and simultaneous tick behavior only after the untimed decision loop is understandable.

### Includes

- Only the timing, pause, and resolution behavior required for one already-proven decision.
- Clear observation of when state changes occur.

### Excludes

- A general-purpose event framework unless the prototype demonstrates a concrete need for one.
- Broad simulation, complete scheduling, or final timing values.

## Candidate later milestone: First systemic interaction prototype

### Goal

Validate one meaningful interaction between company choices and the regional ecosystem.

### Includes

- A narrow systemic interaction.
- Observable cause and effect.
- Enough feedback for the player or developer to understand the result.

### Excludes

- Complete economy model.
- Complete campaign model.
- Large content expansion.
