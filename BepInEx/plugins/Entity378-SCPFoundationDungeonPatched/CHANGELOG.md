## 4.4.0
- Updated to work with V73 of the game
- Removed unnecessary dependencies and implemented use of harmony to patch vanilla methods/functions

## 4.3.4
- Recompiled for v60+
- Changed LobbyCompatibility to be a soft dependency
- Update LLL dependency to latest

## 4.3.3
- Fix SCP 914 and apparatus room elevator ignoring items
- Update LLL dependency to latest

## 4.3.2
- Rebuilt for Lethal Company v55/56
- Minor change to compatibility handling for Piggys mod (guarantee safe calling when not present)

## 4.3.1
- Updated git repository link

## 4.3.0
- Added optional support for Piggys Variety mod (If enabled and mod is found, tesla gate rooms can spawn)
- Updated LLL dependency to 1.2.4

## 4.2.0
- Add support for enemy conversions to SCP 914
- Minor tweak to doors to try and mitigate stuck enemies

## 4.1.3
- Fix client replication issues with the apparatus room elevator

## 4.1.2
- Fix SCP 914 output items sometimes spawning on top of the output box

## 4.1.1
- Fix json typo

## 4.1.0
- Dramatically increased SCP 914 default recipe config entries and rebalanced existing entries (generally more favourable and varied outputs)

## 4.0.1
- Fix custom content configuration not being generated in LLL

## 4.0.0
- Update to 1.2.1 LLL
- Added Omega Warhead Silo room (includes apparatus)
- Made SCP-914 default to copying items instead of destroying for conversions to unknown items (more lenient for custom jsons) + logging for unknown items
- Fixed lights not flickering
- Adjusted lighting colours and brightness
- Fixed various texture UV errors
- Generation tweaks
- LobbyCompatibility dependency
Note: Configs for generation are now managed by LLL, please use that for configuration as the old configs are ignored (Recommend deleting existing config to regenerate)

## 3.0.0
*Thanks for 2 Million downloads!*
- Upgraded to latest LLL
- Added Heavy Containment (keycard gate TODO)
- 1 Extra room in Light Containment
- Fixed rooms not being able to loop back on themselves
- Changed item group patching to better support different languages
- Tweaked default config (slightly higher default rarity, made Secret Labs highly likely to be SCP Foundation)
- Option to disable default SCP 914 config
- Upped minimum dungeon size scale from 1.0 to 1.5

## 2.3.1
- Fix file structure in Thunderstore for SCP 914 recipes (no changes to mod file)
- Changes to documentation/install instructions

## 2.3.0
- Added json-based custom conversions for SCP 914

## 2.2.1
- Fix inverted logic for doors (and manually account for Thumper/Mimic door speeds)
- Fixed issue with doors opening normally networking incorrectly

## 2.2.0
- Reprogrammed doors, should be less prone to navigation issues
- Fixed 914 global audio (hopefully for real this time)
- Fixed spraypaint not working

## 2.1.0
- Fix SCP 914 locking up if an item conversion is supposed to destroy an item
- Added per-moon rarity overrides
- Uncapped rarity value
- Added Secret Labs as a default config option
- Updated config descriptions

## 2.0.2
- Fix softlock on map generation when vanilla items are removed/replaced

## 2.0.1
- Fixed SCP 914 SFX radius being far too big

## 2.0.0
- Added SCP 914
- Fixed some minor mesh issues in SCP 914 room
- Minor adjustments to doors (may help with enemies getting stuck)

## 1.5.0
- v49 compatibility
- Ported to LethalLevelLoader (with some generation tweaks and additional config options, multiple fire exit moons e.g. March are now supported)
- Added much more lighting to the start room
- Fix some navmesh issues in 914 room
- Additional navmesh tweaks to reduce occurences of scrap spawning in walls/in ceilings

## 1.4.1
- Fix collisions missing in SCP 914 room

## 1.4.0
- Added SCP 914 room (Not functional... yet)
- Adjusted dungeon generation to make smaller dungeons (plus additional tweaks to try and make generation more consistent)
- Added new config option to allow customization of the dungeon size (use with caution)

## 1.3.2
- Tweaked moon config to be more flexible and support modded moons better
- More detailed logging of processes and additional error notify messages
- Lethal Expansion incompatibility note

## 1.3.1
- Fix door desync problem
- Fix scrap possibly spawning OOB
- Fix moon config not working with latest LethalLib versions
- Slightly decreased average size of generated dungeon (NOTE: Balanced around Titan; free moons may be relatively small)

## 1.3.0
- Fixed special scrap not spawning, improved scrap spawns in general
- Dungeon flow tweaks to further improve path generation
- Increased chances for special cap rooms to spawn (173, 372, etc)
- Added Bepinex/HookGenPatcher dependencies to make dependencies clearer for manual downloaders

## 1.2.0
- Added new rooms (173 Chamber, 3-way connector)
- Added open doorways for room connectors
- Improved room meshes to help prevent enemies/scrap spawning OOB and improve navigation
- Increased lighting brightness across all rooms
- Modified dungeon generation to increase odds of more winding paths
- Removed fire escapes from catwalks in 4-way room

## 1.1.1
- Fix readonly issue with some room meshes
- Improved lighting

## 1.1.0
- Fix missing room layer information, causing enemies/hazards to ignore walls/fail to recognise floors
- Added flat stair colliders

## 1.0.1
- Fix default config

## 1.0.0
- Initial release