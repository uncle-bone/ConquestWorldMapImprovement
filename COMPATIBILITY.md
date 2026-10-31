# Conquest World Map Improvement compatibility

Target: Ascension Conquest Reborn / WoW 3.3.5a. Current package: **v0.15.1**, a compatibility update on the v0.15.0 feature base. This repository tracks compatibility across the [uncle-bone addon repositories](https://github.com/uncle-bone).

## v0.15.1 source-review changes

The included `COMPATIBILITY-0.15.1.txt` reports these changes:

- Does not disable Mapster/Magnify or ConquestMapZoom.
- Leaves LootCollector's embedded zoom initialization untouched.
- Detects required LootCollector adapter functions instead of requiring exactly version 1.0.9.
- Retains conservative zoom-canvas arbitration so competing zoom engines stay enabled and CWMI yields when another engine owns the canvas.
- Retains original licenses and notices.

These are compatibility changes reported by the package; runtime testing across all custom addon combinations is still required.

## Remaining compatibility checks

- Mapster-CoA / Magnify and ConquestMapZoom: verify viewport ownership and zoom behavior when multiple engines are enabled.
- Questie-X, Zygor-CoA, SilverDragon and LootCollector: verify map pins, quest objectives, waypoints, tooltips and scaling while panning and zooming.
- ElvUI-CoA, DragonUI and Blizzard UI: verify frame skinning, anchoring and map controls.
- SexyMap-CoA, Leatrix Maps and other map overlays: verify minimap and map-button interactions.
- Regression-check DBM-CoA, Details, WeakAuras-CoA, AtlasLoot-CoA, UnclePlus-CoA, Cell-CoA, Nameplates, BoneUI, MRT-CoA and other repository addons.

## Validation status

The v0.15.1 release package is available from the [release page](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases/tag/v0.15.1). Cross-addon in-game validation remains outstanding. These docs describe compatibility targets and package-reported changes, not universal compatibility certification.
