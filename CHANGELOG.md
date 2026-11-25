# Changelog

All notable changes to SEAF: Planetary Operations will be recorded here.

## v0.3 — Base Technical Update

### Added
- Zoom in/out controls and a reset-camera control for the forward base.
- Touch pinch-to-zoom and drag-to-pan camera gestures on the base map.
- Expanded base-map world area with camera bounds.
- Highlighted construction plots and a translucent building placement preview.
- Tap/click-to-place construction with grid snapping; construction costs are charged only after a valid plot is selected.
- Cancel placement control.

### Changed
- Building placement now gives the player control over the selected plot instead of immediately choosing a location automatically.
- Building footprints were reduced slightly to create more room between structures.
- Existing base saves migrate their building coordinates into the expanded map on first load.
- Base ground markings are now deterministic rather than being randomly redrawn every frame.

### Fixed
- Building placement no longer falls back to a random position when all standard plots are occupied.
- Main access lanes are kept clear of construction plots.
- Camera panning is separated from tap-to-place so dragging across the map does not accidentally construct a building.

### Testing
- JavaScript syntax and static interaction checks passed in the generated source.
- Repository contents were re-fetched after publishing to verify the version and key controls.
- A fresh in-browser and iPhone playtest of v0.3 is still required; the user's earlier playtest covered the previous build.

## v0.2 — Gameplay Fixes & Quality of Life

### Added
- Extraction zone and return-to-extraction requirement after mission objectives are completed.

### Changed
- Mobile firing now auto-aims at nearby hostiles.
- Relay sabotage uses discrete interaction damage instead of continuous damage while holding interact.

### Fixed
- Touch controls are gated to mobile/touch-style screens so they do not overlay desktop gameplay.
- Squad casualty handling no longer mutates the squad array during collision iteration.
- Touch firing releases safely if the pointer is lifted outside the fire button.

### Testing
- JavaScript syntax check passed.
- Static checks for the main v0.2 changes passed.
- Full browser gameplay testing was not completed during v0.2 development.

## v0.1 — Foundation (prototype; initial build created outside repository)

### Added
- Basic top-down battlefield and direct soldier control.
- Basic enemy behavior and combat.
- Two AI squadmates.
- Mission framework: Clear the Area, Supply Recovery, and Relay Sabotage.
- Base construction, recruit flow, and resource systems.
- Desktop and touch controls.
- Local save/load.
