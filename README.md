# Conquest World Map Improvement — Conquest Reborn

Current release: **v0.15.1**, a compatibility-only update on the v0.15.0 feature base for the WoW 3.3.5a-based Conquest Reborn client.

> **[⬇ Download ConquestWorldMapImprovement v0.15.1](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases/download/v0.15.1/ConquestWorldMapImprovement-0.15.1-Compatibility.zip)** · [Release notes](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases/tag/v0.15.1)

The release package contains the addon folder and original license notices. The v0.15.1 compatibility report says it no longer disables Mapster/Magnify or ConquestMapZoom, leaves LootCollector's embedded zoom initialization untouched, feature-detects required LootCollector functions, and retains a conservative zoom-canvas guard.

**Runtime testing with all custom addons is still required.** See [COMPATIBILITY.md](COMPATIBILITY.md) for the compatibility scope and remaining checks.

## Scope

Maintain compatibility with **all** World of Warcraft addons under [uncle-bone](https://github.com/uncle-bone), with special attention to Mapster-CoA / Magnify, Questie-X, LootCollector, SilverDragon, Zygor-CoA, ElvUI-CoA, DragonUI, SexyMap-CoA and Leatrix Plus. Also regression-check DBM-CoA, Details, WeakAuras-CoA, AtlasLoot-CoA, UnclePlus-CoA, Cell-CoA, Nameplates, BoneUI, MRT-CoA and other repository addons.

## Compatibility rules

- Never disable, overwrite, or rewrite a user's other addons to resolve a map conflict.
- Preserve Mapster/Magnify functionality while enabling CWMI zoom and marker rendering; coordinate viewport ownership safely.
- Keep map POIs, quest objectives, rare/chest/worldforged pins, tooltips and waypoints aligned while panning and zooming.
- Feature-detect integration APIs rather than relying on one exact addon version.
- Keep original copyright notices and license attribution intact.
- Support Blizzard UI, DragonUI, and ElvUI-CoA.
- Test against current source builds; repository inclusion is not proof of successful runtime testing.
