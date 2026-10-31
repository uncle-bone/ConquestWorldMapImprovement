# Conquest World Map Improvement — Conquest Reborn

Current release: **v0.15.2**, a compatibility hotfix on the v0.15.0 feature base for the WoW 3.3.5a-based Conquest Reborn client.

> **[⬇ Download ConquestWorldMapImprovement v0.15.2](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases/download/v0.15.2/ConquestWorldMapImprovement-0.15.2-Compatibility.zip)** · [Release notes](https://github.com/uncle-bone/ConquestWorldMapImprovement/releases/tag/v0.15.2)

The release package contains the addon folder and original license notices. The v0.15.2 hotfix corrects the default map-priority setting and limits a legacy Mapster 1.3.9 anchor correction to its known offset. It preserves external zoom provider enablement and the original license files. Questie-X 1.6.9 remains a target for in-game verification; certified integration is not claimed.

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
