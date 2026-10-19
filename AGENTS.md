# Realms of the Shattered Crown — Agent Instructions

## Project
An original retro fantasy RPG built with Unreal Engine 5.
Visual style:
- Angled top-down, tile-based overworld.
- First-person pseudo-3D grid-based dungeons.
- Turn-based combat and classic RPG progression.

## Human authority
The human developer is the game director.
Do not make major design or architecture changes without approval.

## Before working
1. Read Docs/GAME_DESIGN.md.
2. Read Docs/ARCHITECTURE.md.
3. Inspect the existing project before modifying files.
4. Explain your planned changes before large or risky edits.

## Development rules
- Prefer Blueprints for beginner-friendly gameplay.
- Use C++ only when justified and approved.
- Keep overworld and dungeon presentation separate.
- Share one authoritative character state, inventory and combat model.
- Use small, testable increments.
- Never silently overwrite another agent's work.
- Do not modify the same Unreal asset concurrently.
- Do not delete assets or alter project settings without approval.
- Preserve a working project after every milestone.

## Git rules
- Check git status before editing.
- Never discard uncommitted user changes.
- Use a separate branch or worktree for independent coding tasks.
- Do not push, merge, reset or rewrite history without approval.
- Report modified files, tests performed and known limitations.

## Deliverables
For every task, report:
1. What changed.
2. Which files changed.
3. How to test the result in Unreal.
4. Known bugs or unfinished work.
5. Whether human editor setup is required.

## Current milestone
Build a tiny playable prototype:
- Tile-based overworld movement.
- First-person grid-based dungeon.
- One basic monster encounter.
- Shared health and character state.

Do not build the full game yet.
