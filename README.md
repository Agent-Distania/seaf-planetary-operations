# SEAF: Planetary Operations

A single-player, top-down 2D sci-fi military game about ordinary SEAF soldiers fighting to reclaim hostile worlds. Built as a browser game with PC and mobile controls.

## Current status
- **Latest build:** v0.8.26 — Upright Patrol Head Placement
- **Development status:** Early prototype; browser gameplay testing remains incomplete
- **Platform:** Browser (HTML/CSS/JavaScript)
- **Perspective:** Top-down, fully 2D

## Gameplay loop
Manage a forward base, select an operation, deploy with squadmates, complete objectives, return to extraction, and use rewards to expand your base.

## Current prototype systems
- SEAF blue-grey forward base with pale concrete structures, blue identification panels, yellow safety markings, detailed perimeter and gate, engineered roads, transport apron, motor pool, reserved service zones, full-base camera framing, pedestrian service paths, low-profile path lighting, drainage grates, marked road crossings including the motor-pool access lane, a detailed modular HQ forecourt, eight animated SEAF base staff on non-combat routes with upright screen-aligned bodies, helmets always above the torso, and visor indicators turned toward their travel direction, and footprint-aware construction; redesigned Barracks, Supply Depot, Medical Station, Radar Station and Engineering Depot
- Overhead Pelican transport with wingtip VTOL engines and expanded apron
- Expanded 1,600 × 1,400 battlefields with branching industrial roads, varied ground zones, separated Automaton facilities and mission-specific combat sectors
- Automaton Fabricators, Detector Towers, communications arrays, power sites, command bunkers, defence positions and supply compounds with dedicated top-down silhouettes
- Infantry barbed wire that can be crossed but damages units on entry; anti-vehicle obstacles remain deferred until vehicle movement is implemented
- Zoomable/pannable base camera and plot-based construction
- Resources: supplies, components, requisition, intel
- Recruitment and squadmates; each Barracks increases squad capacity by two, from the existing eight-person baseline up to twelve
- Logistics and storage: Supply Depots increase supply/component capacity; mission rewards are capped by available storage with overflow reported
- Three missions: Clear the Area, Supply Recovery, Relay Sabotage
- Combat foundation with distinct squad formation spacing, HOLD/FOLLOW orders, cover collision and destructible barricades
- Three Automaton archetypes — compact humanoid Trooper, forward-set Brawler and broad bipedal Devastator — with separated heads, torsos, arms and legs, faction-consistent armour profiles and role-specific movement/engagement behaviour
- SEAF personnel silhouettes with more readable helmets, torso armour, packs, limbs and unit identifiers
- Editable Automaton Threat Database with field descriptions, observed behaviour, identification notes and SEAF assessments
- Top-down Codex field-reference previews rendered from the same Automaton sprites used in live combat, over a battlefield scene
- Refined SEAF building foundations and shared visual identity details; more legible, type-specific Automaton installations
- Visible enemy health bars, ammunition HUD, 30-round service rifle and interaction-based objectives
- Desktop keyboard/mouse and mobile touch controls
- Main menu with three local campaign save slots
- Legacy single-save migration into Campaign Slot 1

The v0.8.26 patrol-sprite pass keeps each ambient staff figure upright on screen so the helmet remains above the torso even on horizontal routes; a small visor indicator turns toward the route direction. The v0.8.25 pass moved the helmet closer to the torso, but did not prevent whole-sprite rotation from putting it beside the body on horizontal paths. The v0.8.24 infrastructure pass adds a marked pedestrian crossing across the motor-pool access road, curb-ramp details at base crossings, and modular paving around the HQ forecourt. The v0.8.23 base-staff pass makes each ambient pedestrian face the direction their route leads, turns them toward the next path segment during corner pauses, and replaces the pack-like sprite shape with a centered, rounded head and clearly separated body and limbs. The v0.8.12 battlefield pass reduces clutter, adds randomized obstacle placement and road checkpoints. The v0.8.10 cleanup removes the rear leg/foot plates from the Automaton silhouettes for a cleaner overhead read. The v0.8.9 Automaton model pass rebuilds the shared Trooper, Brawler and Devastator sprite painter around recognizable bipedal humanoid proportions; the live battlefield and Codex use the same revised models. The v0.8.6 Codex recognition pass adds overhead field-reference previews that use the exact in-game Automaton sprite painter over the battlefield terrain. The v0.8.5 Operations Expanded visual pass established the editable Automaton Threat Database, identifies the three prototype enemy roles as Trooper, Brawler and Devastator, refines Automaton and SEAF top-down silhouettes, and improves the shared presentation of SEAF facilities and hostile installations. Combat roles and stable runtime identifiers are preserved. It does not expand the battlefield or add patrols; those remain part of Operations Expanded, Part II: Battlefield Overhaul and later encounter work. The v0.8.1 patch fixes the startup error that prevented the campaign save-slot menu from appearing. The v0.6 transport artwork is an original top-down Pelican-inspired fan-game silhouette; vehicle artwork is stylized canvas illustration, not imported game models.

## Controls
**Desktop:** WASD/arrows move, mouse aim, left click fire, R reload, E interact, Q toggle squad HOLD/FOLLOW.
**Mobile base:** pinch to zoom, drag to pan, and tap an open building plot to place a selected structure. **Mobile deployment:** joystick movement, FIRE auto-aim, RELOAD, INTERACT, HOLD/FOLLOW squad order, RETREAT.

## Development notes
The v0.7 release expands combat and squad AI while preserving campaign saves, logistics, base construction and resource rules. Test squad spacing, cover, HOLD/FOLLOW controls and combat readability on desktop and mobile.

See [CHANGELOG.md](CHANGELOG.md) for version history and [docs/ROADMAP.md](docs/ROADMAP.md) for planned milestones.

- Separate Automaton and SEAF Codex tabs, with initial friendly personnel entries and overhead field previews.

- Refined overhead silhouettes for Automaton and SEAF personnel, with Codex field previews matching the in-game visual style.
