# SEAF: Planetary Operations

A single-player, top-down 2D sci-fi military game about ordinary SEAF soldiers fighting to reclaim hostile worlds. Built as a browser game with PC and mobile controls.

## Current status
- **Latest build:** v0.4 — Base Visual Overhaul
- **Development status:** Early prototype; browser gameplay testing remains incomplete
- **Platform:** Browser (HTML/CSS/JavaScript)
- **Perspective:** Top-down, fully 2D

## Gameplay loop
Manage a forward base, select an operation, deploy with squadmates, complete objectives, return to extraction, and use rewards to expand your base.

## Current prototype systems
- Redesigned SEAF forward base with top-down facility artwork, perimeter security, roads, Pelican-style transport apron, motor pool, reserved service zones, full-base camera framing and footprint-aware construction
- Zoomable/pannable base camera and plot-based construction
- Resources: supplies, components, requisition, intel
- Recruitment and squadmates
- Three missions: Clear the Area, Supply Recovery, Relay Sabotage
- Top-down deployment combat
- Desktop keyboard/mouse and mobile touch controls
- Main menu with three local campaign save slots
- Legacy single-save migration into Campaign Slot 1

The v0.4.1 motor-pool vehicle silhouettes were redrawn to better match the supplied overhead Bastion tank-destroyer and SEAF exosuit references. Canvas silhouettes are still stylized stand-ins, not imported game models.

## Controls
**Desktop:** WASD/arrows move, mouse aim, left click fire, R reload, E interact.
**Mobile base:** pinch to zoom, drag to pan, and tap an open building plot to place a selected structure. **Mobile deployment:** joystick movement, FIRE auto-aim, RELOAD, INTERACT, RETREAT.

## Development notes
The v0.4 visual overhaul uses original canvas-drawn top-down facility artwork and preserves the main menu, three local campaign slots, camera controls and placement workflow. JavaScript syntax and static footprint checks passed; test the new artwork and construction spacing on desktop and mobile.

See [CHANGELOG.md](CHANGELOG.md) for version history and [docs/ROADMAP.md](docs/ROADMAP.md) for planned milestones.
