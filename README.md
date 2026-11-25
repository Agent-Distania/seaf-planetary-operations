# SEAF: Planetary Operations

A single-player, top-down 2D sci-fi military game about ordinary SEAF soldiers fighting to reclaim hostile worlds. Built as a browser game with PC and mobile controls.

## Current status
- **Latest build:** v0.6 — Transport & Logistics
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
- Recruitment and squadmates; each Barracks increases squad capacity by two, up to eight
- Logistics and storage: Supply Depots increase supply/component capacity; mission rewards are capped by available storage with overflow reported
- Three missions: Clear the Area, Supply Recovery, Relay Sabotage
- Top-down deployment combat
- Desktop keyboard/mouse and mobile touch controls
- Main menu with three local campaign save slots
- Legacy single-save migration into Campaign Slot 1

The v0.6 transport artwork is an original top-down Pelican-inspired fan-game silhouette; the Bastion remains a fixed-casemate tank destroyer with a shortened barrel. Vehicle artwork is stylized canvas illustration, not imported game models.

## Controls
**Desktop:** WASD/arrows move, mouse aim, left click fire, R reload, E interact.
**Mobile base:** pinch to zoom, drag to pan, and tap an open building plot to place a selected structure. **Mobile deployment:** joystick movement, FIRE auto-aim, RELOAD, INTERACT, RETREAT.

## Development notes
The v0.6 release adds functional storage limits and Barracks personnel capacity while preserving existing save data and construction costs. New storage capacity is derived from constructed Supply Depots, so older saves do not need a data conversion. Static source checks were performed; test the Pelican's scale and all base panels on desktop and mobile.

See [CHANGELOG.md](CHANGELOG.md) for version history and [docs/ROADMAP.md](docs/ROADMAP.md) for planned milestones.
