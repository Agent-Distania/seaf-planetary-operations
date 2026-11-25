# Changelog

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
