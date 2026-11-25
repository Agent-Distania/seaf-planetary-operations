## v0.8.3 — Operations Expanded, Part I: Enemy Silhouette Refinement
*Released November 25, 2026*

### Changed
- Reworked enemy canvas silhouettes with clearer top-down mechanical shapes and role-specific armor profiles.
- Standard Trooper now has a more readable humanoid armored outline, helmet/optic, backpack and rifle silhouette.
- Devastator now has a broader reinforced profile and visibly heavier forward weapon.
- Scout retains a narrow reconnaissance silhouette with sensor details.
- Added compact type labels above enemy health bars for readability during combat.

### Verification
- Published JavaScript syntax compilation passed.
- Canvas-mock draw smoke tests passed for Scout, Trooper and Devastator.
- Not tested in live Safari/mobile browser; on-device visual review is still needed.


## v0.8.2 — Operations Expanded, Part I: Enemy Overhaul
*Released November 25, 2026*

### Added
- Replaced the shared generic enemy token with three purpose-built top-down silhouettes: a narrow, sensor-equipped Scout; an armored standard Trooper; and a substantially broader, reinforced Devastator.
- Added clearer hostile visual identity through dark mechanical frames, red/oxide armor plates, visible red optics, role-specific equipment, and health-bar sizing.
- Gave each archetype distinct durability, movement speed and preferred engagement distance so the visual roles also communicate different battlefield behavior.

### Changed
- Replaced the former Raider role with the standard Trooper and renamed the former Heavy role to Devastator; the fast Scout remains the close-range archetype.
- Ranged enemies now prefer the nearest SEAF unit with a clear line of sight. When every friendly is obscured, they retain a nearest target as a movement destination rather than stopping without a target.
- Troopers maintain a closer firing distance, while Devastators keep farther back and have a larger, slower, more durable profile.

### Preserved
- Campaign saves, save-slot migration, base construction, logistics, recruitment, missions, battlefield dimensions, squad orders, mobile controls and existing objective flows.
- The existing arena and cover layout. Map expansion, patrols, barbed wire and anti-vehicle obstacles are not part of Part I.

### Verification
- Embedded JavaScript syntax compilation passed against the published GitHub file.
- Simulated startup and Clear the Area mission test passed: eight enemies spawned as five Troopers, two Scouts and one Devastator; one combat update and one render call completed.
- Relay mission test passed: ten enemies spawned as seven Troopers, two Scouts and one Devastator.
- A targeted line-of-sight test confirmed a ranged enemy selected an unobstructed squadmate rather than a closer player obscured by cover.
- These are simulated DOM/canvas checks, not a live visual playtest in mobile Safari. The new silhouettes still need an on-device visual review for scale and readability.

### Not included
- No battlefield expansion, new building-spawn rules, patrols, new mission types or vehicle obstacles. These remain in Operations Expanded, Part II: Battlefield Overhaul and later encounter work.

# Changelog

## v0.8.1 — Save Menu Startup Fix

### Fixed
- Corrected a malformed loop in the relay objective renderer that caused a JavaScript parse error and prevented the game from initializing.
- Restored startup rendering of all three campaign save-slot cards and access to the save-slot selection screen.

### Verification
- Embedded JavaScript syntax compilation passed.
- Runtime smoke test with a simulated browser DOM confirmed initialization completes and all three save-slot cards render.
- Full interactive playtesting in mobile Safari remains pending.


## v0.8 — Pelican VTOL & Battlefield Installations

### Added
- Five distinct hostile installations: communications array with overhead dish and antennae, generator, command post, defense post and supply compound.
- Enemy structures use red/oxide industrial colors and recognizable overhead silhouettes.
- Facility footprints participate in the existing collision and cover system.

### Changed
- Pelican VTOL nacelles relocated to outer wing tips and wings widened.
- Landing apron expanded to accommodate the updated transport silhouette.

### Testing
- Static source checks completed during update.
- Desktop/mobile browser playtesting remains pending.

## v0.7 — Combat Foundation & Squad AI

### Added
- A distinct two-row squad follow formation with assigned offsets, obstacle-aware steering and repeated separation checks so deployed SEAF squadmates remain visibly spaced instead of stacking on the player.
- Squad HOLD/FOLLOW orders, available via Q on desktop and a dedicated mobile control.
- A handcrafted battlefield obstacle layout with rocks, walls and destructible barricades.
- Collision handling that keeps the player, squadmates and enemies from walking through solid battlefield cover.
- Line-of-sight checks and projectile collision against cover; destructible barricades can be damaged and destroyed.
- Three enemy archetypes with different health, movement, attack ranges and fire rates: Scout, Raider and Heavy.
- Improved top-down soldier/enemy silhouettes, visible squad identifiers, enemy health bars, muzzle flashes, impact effects and player damage feedback.
- A 30-round SEAF Service Rifle magazine, reload feedback and updated combat HUD.
- Explicit INTERACT pickup for supply caches and a southern extraction point away from the player's insertion location.

### Changed
- Squadmates now engage enemies they can see and maintain separate assigned positions while following or holding.
- Enemies select the nearest visible SEAF target instead of always attacking the player.
- Player and enemy movement respects map obstacles; projectiles stop at cover.
- Mission supply caches require deliberate interaction rather than automatic collection on contact.
- Clear-area, supply-recovery and relay missions retain their existing objective/reward structures, with the battlefield and extraction approach improved.

### Preserved
- Three local campaign save slots and legacy-save migration.
- Logistics storage capacities and overflow handling.
- Barracks squad capacity progression, recruitment and existing construction costs.
- Base map, vehicles, campaign resources and mission reward values.

### Verification
- Embedded JavaScript syntax check passed.
- Lightweight simulated-browser checks passed for mission startup, mobile/desktop squad-order controls, movement-frame rendering, save flow and squad spacing.
- Geometry checks confirmed the two squadmates remain separated from each other and from the player during simulated movement.
- Full playtesting in mobile Safari remains outstanding.


## v0.6 — Transport & Logistics

### Added
- New overhead Pelican-inspired transport artwork on the SEAF landing apron, with a tapered central fuselage, cockpit glazing, broad lifting surfaces, twin engine nacelles, paired rear exhausts and parked landing gear.
- Logistics and Storage panel showing current supplies/components against their capacity.
- Derived storage limits: starting capacity is 150 supplies and 90 components; each Supply Depot adds 100 supplies and 50 components.
- Mission reward overflow handling: supplies and components are credited only up to available storage, and any overflow is reported in the operations log and mission status.
- Functional Barracks personnel capacity: existing base capacity remains 8; each Barracks adds 2, up to 12 total.

### Changed
- Shortened the Bastion tank destroyer's fixed-casemate cannon barrel by approximately 25%, retaining the rear-integrated mount and removing any separate light muzzle cap.
- Updated Barracks and Supply Depot descriptions to communicate their actual gameplay effects.
- Resource bar now displays supplies and components as current amount / storage capacity.

### Preserved
- Existing save format and three campaign slots; capacities are calculated from built facilities, so older saves require no schema migration.
- Existing stored resources are not deleted when a legacy save is already above the new base capacity; new mission rewards are simply not credited until space is available.
- Existing eight-person recruitment baseline, building costs, limits, footprints, placement, map camera, missions and combat controls.

### Verification
- Embedded JavaScript syntax was checked after the changes.
- Static checks cover the storage-capacity rules, reward overflow path, squad-capacity progression, vehicle drawing functions and preserved save/placement hooks.
- A full visual playtest in mobile Safari has not been performed by the assistant and remains necessary.


### v0.5.1 — Motor Pool Silhouette Refinement

### Changed
- Removed the exosuit's visible rear legs/feet and forward helmet-like head block, keeping the torso, shield arm and under-arm rotary gun.
- Removed the light-grey end cap from the exosuit rotary gun so its tip reads as part of the weapon housing rather than an assault-rifle muzzle.
- Reworked the Bastion into a fixed-casemate tank destroyer silhouette with its gun mount integrated into the rear of the chassis, rather than a conventional turret.
- Removed the Bastion cannon's light-grey muzzle tip.

### Verification
- JavaScript syntax check passed after the silhouette changes.
- Real mobile visual verification remains pending.


## v0.5 — SEAF Blue-Grey Base Visual Overhaul

### Changed
- Rebuilt the base ground treatment in cool blue-grey concrete and compacted surface tones, with restrained deterministic texture and engineered expansion seams.
- Reworked roads with concrete shoulders, darker sealed lanes, pale route markings, blue-grey edging and yellow safety ticks.
- Reworked the perimeter wall, gate piers, observation posts and wall lighting around a reinforced Super Earth military-facility look.
- Rebuilt the command forecourt and transport apron with pale concrete surfaces, blue SEAF identification, white touchdown markings and yellow hazard boundaries.
- Reworked all seven facility silhouettes: Command Post, Barracks, Supply Depot, Medical Station, Radar Station, Defense Turret and Engineering Depot.
- Reworked construction pads, motor-pool service bays, electrical cabinets and the landing-transport palette to match the SEAF blue-grey identity.
- Recolored the parked Bastion and exosuit artwork to fit the same palette without changing their silhouettes or service-yard placement.
- Updated the main menu, panels, controls and base-map feedback to use a coordinated blue-grey interface theme.

### Preserved
- Existing campaign save format, three save slots and legacy-save migration.
- Existing building costs, building limits, footprints, plot reservations and placement workflow.
- Base camera, zoom, panning, touch gestures, missions, combat and mobile controls.

### Testing
- Static source checks confirmed the intended blue-grey palette and the removal of the previous olive base-ground/building color tokens.
- The published source and documentation were re-fetched to verify the v0.5 release contents.
- The embedded JavaScript parsed successfully; the expected drawing functions are present exactly once, and save slots, migration, placement rules, building costs and camera controls remain in place.
- A real mobile Safari visual playtest has not been performed by the assistant; the user should inspect the map on-device for visual scale, overlap and readability.


## v0.4.1 — Vehicle Silhouette Reference Pass

### Changed
- Reworked the motor-pool Bastion tank destroyer silhouette to read as a long tracked vehicle from overhead, with centerline fixed gun, tread runs, glacis and rear deck details.
- Reworked the SEAF exosuit overhead silhouette with a broad armored torso, separated legs, asymmetrical shield arm and under-arm rotary weapon.
- Kept the motor-pool layout and other base artwork unchanged.

### Testing
- Repository update verified. The source has not yet been run in a full browser or mobile visual test; that remains outstanding.


## v0.4.1 — Vehicle Silhouette Reference Pass

### Changed
- Reworked the motor-pool Bastion tank destroyer silhouette to read as a long tracked vehicle from overhead, with centerline fixed gun, tread runs, glacis and rear deck details.
- Reworked the SEAF exosuit overhead silhouette with a broad armored torso, separated legs, asymmetrical shield arm and under-arm rotary weapon.
- Kept the motor-pool layout and other base artwork unchanged.

### Testing
- JavaScript syntax and static function checks passed before publication; actual visual inspection in mobile Safari remains for the user.



All notable changes to SEAF: Planetary Operations will be recorded here.

## v0.4 — Base Visual Overhaul

### Added
- A detailed top-down terrain treatment with deterministic ground variation and gravel detail.
- Fortified perimeter walls, watch posts, reinforced access gate and road network.
- Central SEAF Command Compound and dedicated transport landing apron, visible in the default full-base camera view.
- Original top-down vector-style artwork for Command Post, Barracks, Supply Depot, Medical Station, Radar Station, Defense Turret and Engineering Depot.
- A dedicated motor-pool yard with original top-down heavy-vehicle and exosuit silhouettes, plus reserved construction space.
- Reserved construction space around the transport apron to keep the landing approach clear.
- Concrete construction pads and facility-specific silhouettes.
- Default camera framing and centering adjusted to show the full installation.

### Changed
- Base building models now have different visual silhouettes, roof equipment, doors, loading areas, antennae and identifying markings.
- Construction overlap checks now use each building's individual footprint instead of one generic spacing rule.
- The base heading and description now present Landing Zone Cedar as a fortified SEAF installation.

### Fixed
- Building placement highlights and previews use the selected building's footprint.
- Facility artwork is drawn after terrain and infrastructure so buildings remain visually distinct.

### Testing
- JavaScript syntax and static layout/footprint checks passed before publishing.
- Repository files were re-fetched to verify the published release.
- Live Safari/iPhone visual testing remains necessary; canvas artwork has not been physically tested on the user's device.

## v0.3.1 — Main Menu & Save Slots

### Added
- Main menu shown when the game opens.
- Three local campaign save slots, each with Continue and New Campaign actions when occupied.
- Fresh campaign creation with the original starting resources, squad and Command Post.
- Confirmation before replacing an occupied save slot.
- Automatic import of the previous single-save data into Campaign Slot 1 when that slot is empty.
- Main Menu navigation from the base, operations and deployment screens.

### Changed
- Saves now write to the currently selected campaign slot rather than a single shared save key.
- The main menu hides campaign resources and gameplay navigation until a save is selected.

### Fixed
- Starting a test campaign no longer requires manually clearing browser storage.
- Existing legacy campaign data is copied into the first slot without deleting the original legacy key.

### Testing
- JavaScript syntax and static save-slot flow checks passed.
- The repository files were re-fetched after publishing.
- Actual browser storage behavior and iPhone menu interaction still require a user playtest.

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
