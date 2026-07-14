# Milestones

Milestones for Frontier Company should be lightweight and organized around playable validation chunks. They are not rigid production phases or calendar commitments.

## Current milestone: Production foundation

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

## Candidate next milestone: First playable chunk definition

### Goal

Define the smallest playable experience that can test whether Frontier Company's core strategic promise is understandable and worth pursuing.

### Includes

- A concise playable goal.
- The minimum player decision loop needed for validation.
- Explicit exclusions to prevent scope creep.
- A verification checklist for the playable chunk.

### Excludes

- Final balance.
- Large content sets.
- Full campaign structure.
- Long-term architecture beyond what the chunk requires.

## Candidate later milestone: First Unity validation scene

### Goal

Create a minimal Unity scene or prototype space that can validate the first playable chunk.

### Includes

- Only the assets, scripts, and scene structure required for the validation target.
- Clear notes about what is temporary versus durable.

### Excludes

- Production art requirements.
- Full UI polish.
- Broad simulation coverage.

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
