# Current State

_Last reviewed: 2026-10-18_

## Repository state

This repository currently contains an early Unity 2022.3.62f1 project scaffold and a lightweight documentation foundation.

Confirmed project files include:

- `Packages/manifest.json` for Unity package dependencies;
- `ProjectSettings/ProjectVersion.txt` for the Unity editor version recorded by the scaffold;
- `ProjectSettings/ProjectSettings.asset` and related Unity settings;
- `Assets/Scenes/SampleScene.unity`, the only scene currently present;
- `README.md`;
- `AGENTS.md`;
- `docs/vision.md`;
- `docs/current-state.md`;
- `docs/decisions.md`;
- `docs/milestones.md`.

## Confirmed project direction

- Frontier Company is a Unity strategy game project.
- Development is solo-developer oriented.
- The intended game is compact and systems-driven.
- The approved time model is Real-Time with Pause (RTWP), operating on a simultaneous tick-based system.
- RTWP and simultaneous ticks describe the intended game, but are deferred from the first prototype target.
- The immediate target is a basic interaction proof, not a representative first gameplay loop.
- The foundation docs should serve as source-of-truth constraints for Codex and future implementation work.
- Detailed gameplay systems are not yet decided.

## Current implementation status

No gameplay scripts, production gameplay systems, or custom gameplay scenes are currently present. The repository contains Unity's sample scene only.

An earlier prototype direction attempted to begin with a real-time, tick-event-driven gameplay loop. That direction reached too deeply into unresolved game and architecture decisions, and it is no longer the immediate target.

## Current development target

The recommended first implementation target is a basic interaction proof in a single Unity scene:

1. Present one clearly labeled player choice.
2. Apply one small state change when the choice is made.
3. Show the result immediately and unambiguously.
4. Allow the interaction to be reset and repeated quickly.

The exact fictional choice, state, and presentation remain open. The proof should use the simplest direct implementation that makes the interaction testable; it does not need to model time, ticks, pausing, a regional ecosystem, or a complete company-management loop.

## Current unknowns

- Unity Hub import and Unity-generated project actions are not yet confirmed complete.
- Testing strategy is undecided.
- Gameplay architecture is undecided.
- The specific content and presentation of the basic interaction proof are not yet defined.
