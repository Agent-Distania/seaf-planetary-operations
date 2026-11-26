# Development Roadmap

## v0.3 — Base Technical Update (implemented)
- Main menu and three local campaign save slots
- Zoom in/out, reset camera, touch pinch-to-zoom and drag-to-pan
- Expanded base map, highlighted building plots and placement preview
- Tap/click-to-place construction with grid snapping
- Save migration for existing building coordinates

## v0.4 — Base Visual Foundation (implemented)
- Detailed top-down terrain, fortified perimeter, access gate and connected roads
- Central SEAF command compound and transport landing apron
- Original top-down artwork for all seven existing building types
- Dedicated motor pool and vehicle-service area
- Reserved construction plots around the motor-pool yard and transport landing apron
- Footprint-aware construction placement and save-compatible existing buildings

## v0.5 — SEAF Blue-Grey Base Visual Overhaul (implemented)
- Rebuilt ground, roads, perimeter, gate, forecourt and landing-apron surface treatments
- Established blue-grey structural surfaces, blue identification panels, white details and restrained yellow safety markings
- Reworked all seven building silhouettes, motor-pool bays, construction pads, watch posts and utility props
- Updated menu, panels, buttons and base-map interface to match the SEAF visual identity

## v0.5.1 — Motor Pool Silhouette Refinement (implemented)
- Removed the exosuit's rear legs/feet and helmet-like front block
- Removed light-grey muzzle tips from the exosuit rotary gun and Bastion cannon
- Changed the Bastion into a fixed-casemate tank destroyer with its gun mount integrated into the rear chassis

## v0.6 — Transport & Logistics (implemented)
- Added top-down Pelican-inspired transport art on the landing apron
- Shortened the Bastion fixed cannon barrel by approximately 25%
- Added supply/component storage capacities and a Logistics & Storage panel
- Made Supply Depots increase resource storage and mission rewards respect available capacity
- Preserved the existing eight-person base squad capacity; each Barracks adds two, up to twelve
- Preserved campaign saves without a schema migration

## v0.7 — Combat Foundation & Squad AI (implemented)
- Added two-row follow formation, assigned squad positions, spacing/separation and obstacle-aware movement
- Added squad HOLD/FOLLOW orders for desktop and mobile
- Added battlefield rocks, walls, destructible barricades and movement/projectile collision
- Added line-of-sight checks, enemy target selection and three enemy types: Scout, Raider and Heavy
- Improved soldier silhouettes, squad numbering, health bars, muzzle flashes, impacts and damage feedback
- Updated the service rifle to a 30-round magazine and improved the combat HUD
- Added explicit supply-cache interaction and moved extraction to the far side of the battlefield

## v0.8 — Pelican VTOL & Battlefield Installations (implemented)
- Move the Pelican's VTOL engine nacelles to the outer ends of its wings, with the engines visibly mounted at the wing tips
- Expand and reshape the landing apron to fit the corrected Pelican footprint, keeping clear approach and parking space
- Redesign enemy installations around the enemy faction's own armor, structure and lighting colors rather than neutral SEAF-looking grey props
- Make each enemy installation recognizable from directly overhead by its silhouette and visible equipment
- Communications array: prominent dish mounted on top, with a supporting mast/base, control housing and associated antenna equipment
- Add other purpose-readable hostile installations as mission needs require, such as power/generator facilities, command/control structures, defensive positions and supply compounds
- Give installations meaningful battlefield footprints that affect routes, cover, sightlines and objective approaches
- Expand the combat arena as needed for larger installations, roads, perimeter space and more than one approach route; do not force new facilities into the current 1,000 × 1,000 map
- Add varied battlefield layouts and objective placement around these installations
- Revisit battlefield structure, friendly and enemy visual designs as a coordinated art pass; preserve clear SEAF/enemy faction distinction
- Test structure readability, squad movement, combat flow and mobile performance on desktop and mobile (playtest pending)

## Operations Expanded — development series

### Part I — Enemy Overhaul (implemented in v0.8.2–v0.8.6)
- Replace the generic shared enemy token with clearly differentiated top-down silhouettes for Scout, standard Trooper and Devastator
- Give enemy roles distinct armor mass, equipment, hostile red/oxide identity and readable optics
- Add overhead Codex field-reference previews using the same enemy sprite painter and battlefield terrain as live combat
- Establish separate durability, movement and engagement profiles so each visual type communicates its combat role
- Make ranged enemies prioritize SEAF targets they can see, with a fallback target for movement when cover blocks every friendly
- Preserve the existing arena, missions, campaign saves, base systems and controls

### Part II — Battlefield Overhaul (implemented in v0.8.5)
- Expanded the battlefield to 1,600 × 1,400 with bounds-aware camera and movement handling
- Added Foundry District, Automaton Supply Yard and Signal Station mission sectors with tailored cover and structure placement
- Added Automaton Fabricator and Detector Tower silhouettes, plus communications, power, command, defence and supply installations
- Rebuilt terrain with branching roads, varied ground regions, service pads, gravel/scorched patches and dispersed cover
- Added passable infantry barbed wire that damages units crossing it without blocking movement or sight
- Added forward obstacle probing to help squad and enemy movement steer around solid cover
- Preserved mobile controls, mission objectives, existing campaign saves and base systems
- Dragon's teeth and Czech hedgehogs remain deferred until vehicle movement exists; patrols and roaming encounter systems remain follow-on work

### Follow-on — Patrols & Encounter Systems (planned after Part II)
- Add patrol routes, stationary guards, installation defenders, reinforcements and investigation behavior
- Build patrol and encounter placement around the expanded terrain and revised navigation/line-of-sight systems
- Add more varied battlefield encounters and mission approaches

## v0.9 — Base Operations & Services (planned)
- Add useful functions to the Medical Station, Radar Station and Engineering Depot
- Introduce vehicle readiness and maintenance
- Expand logistics only where gameplay systems need additional space

## v0.10 — Combat & Progression Expansion (planned)
- Add weapon selection, specialist equipment and ammunition resupply
- Expand squad commands and enemy behaviors
- Add stratagem-style support and reinforcement systems

## v0.11 — Planetary Exploration (planned)
- More varied mission environments, exploration events and points of interest

## v0.12 — Missions & Campaign (planned)
- Mission chains, campaign progression and more meaningful operational choices

## v0.13 — World & Enemy Expansion (planned)
- Broader enemy roster and planetary world details

## v0.14 — Polish (planned)
- UI, accessibility, balance, performance and bug fixing

## v1.0 — Planetary Campaign (planned)
- Coherent campaign loop with expanded progression and stable systems

## v0.8.7 — Personnel Codex (implemented)
- Added faction tabs for Automaton and SEAF records.
- Added SEAF Soldier and Squadmate entries with overhead visual previews.
- Codex entries are separated by faction for future roster expansion.
