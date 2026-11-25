# SEAF: Planetary Operations

A single-player, top-down 2D sci-fi military game about ordinary SEAF soldiers fighting to reclaim hostile worlds. Built as a browser game with PC and mobile controls.

## Current status
- **Latest build:** v0.7 — Combat Foundation & Squad AI
- **Development status:** Early prototype; browser gameplay testing remains incomplete
- **Platform:** Browser (HTML/CSS/JavaScript)
- **Perspective:** Top-down, fully 2D

## Gameplay loop
Manage a forward base, select an operation, deploy with squadmates, complete objectives, return to extraction, and use rewards to expand your base.

## Current prototype systems
- SEAF blue-grey forward base with pale concrete structures, blue identification panels, yellow safety markings, detailed perimeter and gate, engineered roads, transport apron, motor pool, reserved service zones, full-base camera framing and footprint-aware construction
- Overhead Pelican-inspired transport staged on a marked landing apron; vehicle artwork is original canvas illustration
- Zoomable/pannable base camera and plot-based construction
- Resources: supplies, components, requisition, intel
- Recruitment and squadmates; each Barracks increases squad capacity by two, from the existing eight-person baseline up to twelve
- Logistics and storage: Supply Depots increase supply/component capacity; mission rewards are capped by available storage with overflow reported
- Three missions: Clear the Area, Supply Recovery, Relay Sabotage
- Combat foundation with distinct squad formation spacing, HOLD/FOLLOW orders, cover collision and destructible barricades
- Three enemy archetypes, visible health/ammunition HUD, 30-round service rifle and interaction-based objectives
- Desktop keyboard/mouse and mobile touch controls
- Main menu with three local campaign save slots
- Legacy single-save migration into Campaign Slot 1

The v0.7 combat update adds visible squad spacing, HOLD/FOLLOW commands, battlefield cover and three enemy archetypes. The v0.6 transport artwork is an original top-down Pelican-inspired fan-game silhouette; vehicle artwork is stylized canvas illustration, not imported game models.

## Controls
**Desktop:** WASD/arrows move, mouse aim, left click fire, R reload, E interact, Q toggle squad HOLD/FOLLOW.
**Mobile base:** pinch to zoom, drag to pan, and tap an open building plot to place a selected structure. **Mobile deployment:** joystick movement, FIRE auto-aim, RELOAD, INTERACT, HOLD/FOLLOW squad order, RETREAT.

## Development notes
The v0.7 release expands combat and squad AI while preserving campaign saves, logistics, base construction and resource rules. Test squad spacing, cover, HOLD/FOLLOW controls and combat readability on desktop and mobile.

See [CHANGELOG.md](CHANGELOG.md) for version history and [docs/ROADMAP.md](docs/ROADMAP.md) for planned milestones.
