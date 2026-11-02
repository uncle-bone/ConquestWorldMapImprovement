# Conquest World Map Improvement — Conquest Reborn

**Latest development build:** v0.15.14-dev · **Current stable release:** v0.15.11 · **Client:** Ascension Conquest Reborn (WoW 3.3.5a)

> **[Download](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases/latest)**

[Releases](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases) · [Compatibility tracking](COMPATIBILITY.md)

## About

Conquest World Map Improvement adds world-map zoom, terrain and exploration controls, quest-journal support, and optional addon integrations for Conquest Reborn. This compatibility-focused build is designed to work alongside Mapster and other customized CoA addons.

## v0.15.14-dev — ElvUI and Mapster compatibility

- Fixes ElvUI backdrop suppression when Mapster controls zoom.
- Checks viewport position to keep the CWMI toolbar anchored within the map window.
- Preserves ElvUI map-coordinate positioning when Mapster controls zoom, plus existing DragonUI and Mapster integrations.

This development build needs in-game verification with ElvUI-CoA and Mapster-CoA running together.

## Features

- World-map zoom and presentation with the included map artwork.
- Terrain and exploration controls.
- Quest journal integration and optional integrations with other addons.
- Compatibility safeguards for overlapping map and zoom behavior.

Combined addon compatibility should be checked in-game with your own addon setup.

## Installation

1. Download the ZIP above.
2. Extract its `ConquestWorldMapImprovement` folder into your Conquest Reborn `Interface/AddOns` directory, replacing the older folder.
3. Keep your other addons and their saved settings in place.

## Compatibility

CWMI is intended to coexist with Mapster-CoA/Magnify, Questie-X, LootCollector, SilverDragon, Zygor-CoA, ElvUI-CoA, and other UI and map addons. It should not silently disable another addon or overwrite its saved settings. See [COMPATIBILITY.md](COMPATIBILITY.md) for compatibility tracking.

## Attribution

**Compatibility maintainer:** Uncle Bone · [@uncle-bone](https://github.com/uncle-bone)

This is a compatibility-focused continuation of a third-party addon, not a claim of original authorship. Original author credits, license notices, and required third-party attribution are preserved. No upstream affiliation is implied.

Please include your Conquest Reborn client build, addon versions, and any Lua errors when reporting compatibility problems.
