# Compatibility scope (source audit)

Target: Ascension Conquest Reborn / WoW 3.3.5a. Baseline archive: ConquestWorldMapImprovement-0.15.0.zip. All **21 other repositories** on downingwow's GitHub are in regression scope (plus this repository). Relevant projects: NovaInstanceTracker, Questie-X, DBM-CoA, LootCollector, MRT-CoA, ElvUI-CoA, Zygor-CoA, SilverDragon, BoneUI, Details, CoA-Research (data only), Cell-CoA, Nameplates, AtlasLoot-CoA, CoA-Item-Search (data/tool), WeakAuras-CoA, UnclePlus-CoA, Refactor-CoA, UncleTranslate-CoA, SexyMap-CoA, VeilForge-CoA (graphics), and Mapster-CoA.

## Source-confirmed compatibility blockers in upstream 0.15.0

1. `Compatibility.lua`: default `manageConflicts=true` and `ManageStandalone()` invokes `DisableAddOn` against `Magnify-WotLK` and `ConquestMapZoom`, including when already loaded. This violates coexistence. Default and behavior must change so CWMI never disables another addon; where concurrent zoom is unsafe, provide a visible warning and explicit in-game choice about zoom-controller ownership, without changing other addon settings.
2. `Compatibility.lua`: `GetConflict()` unconditionally blocks if Magnify-WotLK is loaded or an unknown WorldMapScrollFrame exists. Need interface-specific safe arbitration; don't blindly claim universal simultaneous zoom controllers are safe.
3. `Compatibility.lua`: embedded LootCollector zoom handling assumes exact `2.2.0`, changes `OnFirstLoad` and can hide its frame. Replace with feature-driven adapter and reversible ownership logic.
4. `LootCollectorCompat.lua`: `GetProviders()` returns unless version is exactly `1.0.9`. Validate actual module contracts in the user's latest LootCollector, not an old version string.
5. `MapsterCompat.lua`: `MapSizeChanged()` includes a Mapster 1.3.9-specific anchor workaround. Test against latest Mapster-CoA implementation and Magnify integration.
6. Questie-X, Zygor-CoA, SilverDragon and LootCollector map pins/POIs/waypoints must remain aligned at 1x to maximum zoom, pan, full/mini map and UI reload.
7. Check ElvUI-CoA, DragonUI and Blizzard frame skinning/anchoring, Leatrix map controls, SexyMap-CoA minimap buttons, and interactions with the rest of the user's addons.

## Validation status

These are **code-inspection findings and targets, not confirmed working fixes**. The GitHub repo was initially empty; source/assets must be imported and tested before publishing a compatible release. No original author attribution/license files should be removed.
