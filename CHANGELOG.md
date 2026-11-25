# Changelog

All notable changes to SEAF: Planetary Operations will be recorded here.

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
- Full browser gameplay testing remains incomplete; headless browser launch timed out.

## v0.1 — Foundation (prototype; initial build created outside repository)

### Added
- Basic top-down battlefield and direct soldier control.
- Basic enemy behavior and combat.
- Two AI squadmates.
- Mission framework: Clear the Area, Supply Recovery, and Relay Sabotage.
- Base construction, recruit flow, and resource systems.
- Desktop and touch controls.
- Local save/load.
