# Conquest World Map Improvement — Conquest Reborn

This repository tracks compatibility work for **Conquest World Map Improvement** (upstream version **0.15.0**) on the WoW 3.3.5a-based Conquest Reborn client.

## Scope
Maintain compatibility with **all** World of Warcraft addons under [downingwow](https://github.com/downingwow), with special attention to Mapster-CoA / Magnify, Questie-X, LootCollector, SilverDragon, Zygor-CoA, ElvUI-CoA, DragonUI, SexyMap-CoA and Leatrix Plus. Also regression-check DBM-CoA, Details, WeakAuras-CoA, AtlasLoot-CoA, UnclePlus-CoA, Cell-CoA, Nameplates, BoneUI, MRT-CoA and other repository addons.

## Compatibility rules
- Never disable, overwrite, or rewrite a user's other addons to resolve a map conflict.
- Preserve Mapster/Magnify functionality while enabling CWMI zoom and marker rendering; coordinate viewport ownership safely.
- Keep map POIs, quest objectives, rare/chest/worldforged pins, tooltips and waypoints aligned while panning and zooming.
- Feature-detect integration APIs rather than relying on one exact addon version.
- Keep original copyright notices and license attribution intact.
- Support Blizzard UI, DragonUI, and ElvUI-CoA.
- Test against latest source builds; repository inclusion is not proof of successful runtime testing.

**Current status:** compatibility audit in progress. This repository has not yet been populated with the original 0.15.0 source/assets; the original archive is the development baseline. No compatibility fixes are claimed as released yet.
