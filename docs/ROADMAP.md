## v0.8.27 — Shoulder-Seated Patrol Heads (implemented)
- Reduced and centered ambient patrol helmets so they sit into the shoulders rather than reading as separate capsule shapes.
- Turned the full body silhouette to match the current route direction, keeping the head centered on the body's forward axis.
- Preserved the eight staff, four routes, walking animation and all other base/gameplay systems.


## v0.8.26 — Upright Patrol Head Placement (implemented)
- Kept ambient SEAF patrol figures upright on screen so helmets remain above torsos on both vertical and horizontal routes.
- Turned the visor indicator toward the current direction of travel instead of rotating the whole sprite.
- Limited the change to non-combat base staff; deployed squad sprites and battlefield artwork remain unchanged.


## v0.8.25 — Patrol Head-to-Torso Alignment (implemented)
- Moved ambient SEAF patrol helmets back so they visibly overlap the upper torso instead of projecting ahead of the body.
- Kept the head centered on the route-facing axis and retained direction-matched walking.
- Limited the change to non-combat base staff; deployed squad sprites and battlefield artwork remain unchanged.


## v0.8.24 — Integrated Forecourt & Pedestrian Circulation (implemented)
- Added a marked pedestrian crossing at the east-side walkway and motor-pool access-road intersection.
- Added curb-ramp and tactile edge details to marked pedestrian crossings.
- Added modular paver seams and corner inlays to the exposed HQ forecourt perimeter.
- Preserved the base map, construction plots, building footprints, staff routes, parked model artwork and game systems.


## v0.8.23 — Base Personnel Orientation & Silhouette Fix (implemented)
- Rebuilt ambient base-staff sprites with centered rounded heads at the leading end of the body, compact torsos, attached arms and separated walking legs.
- Removed the side-mounted shape that made the figures resemble backpacks.
- Matched each sprite's facing direction to its route movement vector and turned staff toward the next segment during corner pauses.
- Preserved the four routes, eight staff positions, base layout, campaign saves and deployment systems.


## v0.8.22 — Living Base Personnel (implemented)
- Added eight ambient SEAF base staff who walk four looping routes along the existing service paths.
- Added simple directional and walking animation with corner pauses and placed-building clearance checks.
- Personnel animate only while the Forward Base screen is open and remain separate from recruitable deployment squadmates.
- Preserved base layout, building construction, save data and mission systems.


## v0.8.21 — Base Access & Site Infrastructure Polish (implemented)
- Added narrow pedestrian footpaths alongside the main service roads and central access lanes.
- Added short footpath links, low-profile lights, drainage grates and marked pedestrian crossings.
- Preserved the map dimensions, building plots, all facility artwork, parked model artwork, campaign saves and gameplay systems.


# Development Roadmap

## v0.8.20 — SEAF Facility Visual Overhaul (implemented)
- Redesigned the Barracks, Supply Depot, Medical Station, Radar Station and Engineering Depot as distinct modular SEAF facilities.
- Expanded support-building footprints and construction pads to improve top-down readability.
- Preserved the base world dimensions, construction grid, costs, save format, HQ and defensive emplacement artwork.


## v0.8.19 — Expanded Forward Command HQ (implemented)
- Expanded the central SEAF Forward Command HQ across nearly the full compound pad.
- Removed the roof star and lettering; moved the HQ name to a separate ground-mounted sign in front of the entrance.
- Updated the logical building footprint to match the enlarged structure.


## v0.8.18 — Forward Command HQ Redesign (implemented)
- Rebuilt the central Command Post as a modular SEAF Forward Command facility with a raised operations core, paired support wings, communications mast, identity plate and formal forecourt entrance.
- Preserved its original 108 × 82 logical footprint and all campaign/building systems.


## v0.8.17 — Command Forecourt Cleanup (implemented)
- Removed the four diagonal construction plots surrounding the central Command Post forecourt.
- Preserved all other construction plots and existing building placement behavior.


## v0.8.16 — Symmetrical Motor Pool Layout (implemented)
- Recentered the apron and inner border around the existing two-bay centerline.
- Aligned the access road to the central service aisle.
- Balanced service cabinets and inspection markers across both sides.
- Mirrored the yard edge seams, bollards and service lights.
- Left parked model art and positions unchanged; no vehicle implementation added.


## v0.8.15 — Base Service Yard Details (implemented)
- Added a marked service-access walkway to the motor-pool apron.
- Added drainage grates in the aisle between the existing bays.
- Added subtle edge seams, safety bollards and service lights around the yard perimeter.
- Kept parked model artwork, dimensions and positions unchanged.


## v0.8.12 — Battlefield Variety & Road Checkpoints (implemented)
- Rotated SEAF infantry another 180 degrees.
- Reduced ground debris marks and obstacle clutter.
- Added randomized checkpoint road-control barriers while preserving passable lanes.
- Randomized light clutter sites between deployments; objectives and key facilities remain fixed.


## v0.8.11 — Infantry Facing Alignment (implemented)
- Corrected SEAF infantry sprite rotation so their visual forward direction matches movement/aim vectors rather than the gun-side axis.
- Kept squad number labels upright.
- Gameplay movement and combat behavior unchanged.


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

## v0.8.8 — Infantry Visual Refinement (implemented)
- Refined overhead Automaton and SEAF infantry silhouettes for greater in-game recognition.
- Codex previews use the refreshed visual models.


## v0.8.9 — Automaton Model Rework (implemented)
- Rebuilt the Trooper, Brawler and Devastator as clearly recognizable bipedal humanoid silhouettes from the overhead camera.
- Gave the Trooper a compact body with a separate head, torso, arms and two legs.
- Rebuilt the Brawler around a readable close-assault humanoid shape with distinct paired limbs.
- Preserved the Devastator's heavy mass while making its head, torso, paired arms and two legs immediately recognizable.
- Kept live-combat models and Codex field previews synchronized through the shared sprite painter.
- Preserved enemy identifiers, combat behaviour, spawn settings, campaign saves and controls.


## v0.8.10 — Rear Leg Silhouette Cleanup (implemented)
- Removed rear leg/foot plate shapes from Trooper, Brawler and Devastator sprites to simplify their overhead silhouettes.
- Kept their front-facing heads, torso, arm details, rear pack and combat rotation intact.
- Codex previews continue to use the same shared sprite painter.
