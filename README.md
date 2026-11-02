# Conquest World Map Improvement — Conquest Reborn

**Current stable release:** v0.15.6 · **Client:** Ascension Conquest Reborn (WoW 3.3.5a)

> **[⬇ Download ConquestWorldMapImprovement v0.15.6](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases/download/v0.15.6/ConquestWorldMapImprovement-0.15.6.zip)**

[Releases](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases) · [Compatibility tracking](COMPATIBILITY.md)

## About

Conquest World Map Improvement enhances the Conquest Reborn world map with original artwork and compatibility-focused map controls. This build is designed to work alongside Mapster and other customized Conquest of Azeroth addons.

## v0.15.6 — Responsive Mapster toolbar

- Keeps CWMI's Settings, Terrain, and Fog controls available while Mapster is enabled.
- Adapts the toolbar to Mapster window resizing and anchors it to the visible map window.
- Leaves zoom, pan, scaling, and map positioning to Mapster.
- Preserves detailed map artwork and existing addon behavior.

This package has not been tested in-game; combined addon compatibility still needs runtime verification.

## Installation

1. Download the ZIP above.
2. Extract its `ConquestWorldMapImprovement` folder into your Conquest Reborn `Interface/AddOns` directory, replacing the older folder.
3. Keep your other addons and their saved settings in place.

## Compatibility

CWMI is intended to coexist with Mapster-CoA/Magnify, Questie-X, LootCollector, SilverDragon, Zygor-CoA, ElvUI-CoA, and other UI and map addons. It should not silently disable another addon or overwrite its saved settings. Overlapping map ownership behavior must be handled safely. See [COMPATIBILITY.md](COMPATIBILITY.md) for compatibility tracking.

## Attribution

**Compatibility maintainer:** Uncle Bone · [@uncle-bone](https://github.com/uncle-bone)

This is a compatibility-focused continuation of a third-party addon, not a claim of original authorship. Original author credits, license notices, and required third-party attribution are preserved. No upstream affiliation is implied.

Please include your Conquest Reborn client build, addon versions, and any Lua errors when reporting compatibility problems.
