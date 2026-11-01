# Conquest World Map Improvement — Conquest Reborn

**Current release:** v0.15.2 compatibility hotfix · **Client:** Ascension Conquest Reborn (WoW 3.3.5a)

[Download the latest release](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases/latest) · [Compatibility tracking](COMPATIBILITY.md)

## About

Conquest World Map Improvement enhances the Conquest Reborn world map with a scrollable, zoomable map interface, custom map presentation, and integration points for quest tracking and other map-based addons. This repository maintains a **compatibility-focused build** of the original project for players using a larger collection of customized Conquest of Azeroth addons.

The aim is to let players keep their existing UI, quest, map, and rare-tracking addons enabled rather than requiring them to choose between features.

## Features

- Scrollable and zoomable world-map interface with original map artwork.
- Map presentation and quest/navigation integration inherited from the original addon.
- Compatibility safeguards for other world-map zoom providers.
- Integration targets for Questie-X quest markers, LootCollector discoveries, and other map pin sources.
- Compatibility targets for Blizzard UI, DragonUI, and ElvUI-CoA.
- Original third-party copyright and license notices preserved.

## v0.15.2 compatibility changes

- Prevents the addon from automatically disabling external map zoom addons, including Magnify.
- Corrects the default map-priority/conflict setting.
- Restricts a legacy Mapster 1.3.9 map-anchor adjustment to its specific known layout.
- Retains the original world-map assets and features.

**Important:** These are implemented safeguards, not a certification that every combination has been tested in-game. In particular, Questie-X **v1.6.9** and the latest Mapster-CoA/Magnify, LootCollector, SilverDragon, Zygor-CoA, and ElvUI-CoA releases still require combined runtime verification.

## Installation

1. Download the v0.15.2 compatibility ZIP from [Releases](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases).
2. Extract the included `ConquestWorldMapImprovement` addon folder into your Conquest Reborn `Interface/AddOns` directory.
3. Replace the older version of that folder. Keep your other addons installed.
4. Enable the addon at character selection and check the world map, zoom controls, quest markers, rare markers, and waypoints.

## Compatibility policy

The goal is to work alongside **all current World of Warcraft addon repositories** maintained under [uncle-bone](https://github.com/uncle-bone), including Mapster-CoA/Magnify, Questie-X, LootCollector, Zygor-CoA, SilverDragon, SexyMap-CoA, ElvUI-CoA, DBM-CoA, AtlasLoot-CoA, WeakAuras-CoA, Details, BoneUI, Cell-CoA, Nameplates, Refactor-CoA, MRT-CoA, UnclePlus-CoA, UncleTranslate-CoA, and NovaInstanceTracker.

CWMI should not silently disable another addon or overwrite its saved settings. Overlapping zoom and map ownership behavior must be handled safely. See [COMPATIBILITY.md](COMPATIBILITY.md) for outstanding compatibility work.

## Development and attribution

**Compatibility maintainer:** Uncle Bone · [GitHub](https://github.com/uncle-bone)

This is a compatibility-focused continuation of a third-party addon, **not a claim of original authorship**. Preserve all original author credits, license notices, and legally required third-party attributions included with the addon. No upstream affiliation is implied.

Please include your Conquest Reborn client build, addon versions, and any Lua errors when reporting compatibility problems.
