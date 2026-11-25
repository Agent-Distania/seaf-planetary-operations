# SEAF: Planetary Operations

A single-player, top-down 2D sci-fi military game about ordinary SEAF soldiers fighting to reclaim hostile worlds. Built as a browser game with PC and mobile controls.

## Current status
- **Latest build:** v0.3.1 — Main Menu & Save Slots
- **Development status:** Early prototype; browser gameplay testing remains incomplete
- **Platform:** Browser (HTML/CSS/JavaScript)
- **Perspective:** Top-down, fully 2D

## Gameplay loop
Manage a forward base, select an operation, deploy with squadmates, complete objectives, return to extraction, and use rewards to expand your base.

## Current prototype systems
- Forward base, zoomable/pannable camera, and plot-based construction
- Resources: supplies, components, requisition, intel
- Recruitment and squadmates
- Three missions: Clear the Area, Supply Recovery, Relay Sabotage
- Top-down deployment combat
- Desktop keyboard/mouse and mobile touch controls
- Main menu with three local campaign save slots
- Legacy single-save migration into Campaign Slot 1

## Controls
**Desktop:** WASD/arrows move, mouse aim, left click fire, R reload, E interact.
**Mobile base:** pinch to zoom, drag to pan, and tap an open building plot to place a selected structure. **Mobile deployment:** joystick movement, FIRE auto-aim, RELOAD, INTERACT, RETREAT.

## Development notes
The v0.3.1 main-menu and three-slot save system has passed JavaScript syntax and static save-flow checks. Campaigns are stored locally in the current browser/device; test slot loading and new-campaign confirmation before relying on the saves.

See [CHANGELOG.md](CHANGELOG.md) for version history and [docs/ROADMAP.md](docs/ROADMAP.md) for planned milestones.
