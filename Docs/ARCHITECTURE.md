# Technical Architecture

## Engine
Unreal Engine 5. Blueprint-first implementation.

## Modules
- Core: game state, input, shared interfaces and transitions.
- Overworld: tile map, movement, camera and exploration.
- Dungeon: grid navigation and pseudo-3D rendering.
- RPG: character stats, combat, inventory and items.
- Quests: quest progress and rewards.
- Save: persistent player and quest state.
- UI: health, messages, menus and combat presentation.

## Shared state
Maintain one authoritative source for character stats,
inventory, equipment, gold and quest progress.

Changing between overworld and dungeon views must not
reset the player's RPG state.

## Dungeon renderer
Start with a fixed tile grid and a custom raycasting-style
perspective renderer. Keep map data and rendering separate.

## Data
Use Blueprint structures, enumerations, Data Assets or
Data Tables where appropriate for tiles, items, monsters
and quests.

## Testing
Each module must have a reproducible test procedure.
Test the overworld and dungeon independently before
integrating them.

## Integration
Only integrate reviewed changes.
Avoid simultaneous editing of the same Unreal assets.
Keep a known-good Git commit at each milestone.
