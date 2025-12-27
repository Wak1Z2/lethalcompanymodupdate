# 1.12.4

### Rrajigar Mines
- The Elevator in the pit room is less jank and conveys items.

# 1.12.3

### Rrajigar Mines
- Fixed the holes into the Void in the Main Entry room.

# 1.12.2

### Rrajigar Mines
- Now Zeranos Compatible.

# 1.12.1

### Skaarj Outpost
- Now Zeranos Compatible.

# 1.12.0

### General
- A bunch of stuff and various objects from Unreal to decorate interiors with.
- Refactored default weights, EGypt, Skelahs Moons, and Beanies moons added.

### Chizra Temple
- Reduced the Audible Distance of Wind SFX in rooms with a Death Pit.

### Skaarj Outpost
- The Laser Trap halls SFX are no longer Global.
- Improved the Look of Fire Exits.

# 1.11.1

### General
- Fixed Scrap Oddities.

# 1.11.0

### General
- Interiors updated for V70.

### Skaarj Outpost
- Fixed a few longstanding Pathing issues.

# 1.10.1

### Rrajigar Mines
- Turrets can no longer fire through closed crates.
- Very Minor optimizations.

### Skaarj Outpost
- Fixed missing sound references on lights.
- Filesize optimization.
- Removed Turret Spawns from the Laser Hall room.

# 1.10.0

### General
- Reworked the Default weights.

### Rrajigar Mines
- A bit more extensive normal mapping.
- Lighting improvements.
- Tag changes to various rooms for consistency reasons.
- The hinge bridge is properly tagged and on the Room Layer.
- Fixed a Lights position.
- Emergency Lights above doors light up properly again.
- Fixed a bunch of Lights not spawning properly.

### Chizra Temple
- More extensive normal mapping.
- The ritual event is properly synced.
- Snow falls from the ceiling if the Weather is Snowfall or Blizzard from Lethal Elements.
- Ambient Sound effects are quieter, with larger radii.
- Cavernous wind blowing from death pits don't have Doppler effects anymore.
- Fixed the Wonky UVs in the Diamond pool room.
- Lighting Improvements.

### Skaarj Outpost
- More extensive normal mapping.
- 1 new tile, The 'Intruder discouragement room'.
- Minor Lighting improvements in hallways and doors.

### Nali Haven
- More extensive normal mapping.
- Minor Lighting changes.
- Fixed the Texture on Wall Lamps.
- Added a longer delay before elevators start moving.

# 1.9.5

### Rrajigar Mines
- Patched a hole in the Large Pillar room.
- Toned down the normal mapping on Brick materials.

# 1.9.4

### General
- Updated LLL Dependencies.
- Added Lunar Lights, Realestudios' Vulcan9 port, Prominence, Starlancers moons and Frostfall to the Default moon weight presets.

### Rrajigar Mines
- Experimental changes to the interiors presentation.

### Nali Haven
- Carpets are now on the Room Layer.

# 1.9.3

### General
- Added Generics Moons to the Default moon weight presets.
- Updated Rrajigars Readme.
- Updated Skaarj Outposts Readme.

### Chizra Temple
- Rain falls from the open ceilings when the weather is Rainy, Stormy, or Flooded.

# 1.9.2

### Rrajigar Mines
- Fixed a missing icon when climbing the ladder in the two-level room.

# 1.9.1

### Nali Haven
- Elevator buttons have the correct hand hover sprite.

# 1.9.0

### General
- Project Reimporting neccesitated fixing a multitude of broken references, I've forgotten what's been changed, added and fixed.

# 1.8.5

### Skaarj Outpost
- If played on moons tagged with 'Atomic', the pale white and green lights become Green and Yellow.
- Fixed some incorrectly configured Klaxon Spawners.
- Hallway Blocker lights have a subtle glowing light.

# 1.8.4

### General
- Fixed the Transparencies in various materials broken with the last update.

# 1.8.3

### General
- Filesize optimization

### Rrajigar Mines
- The Two Level rooms Navmesh has been fixed.

### Nali Haven
- The double Elevator room is supposed to have Lamps in it, This has been fixed.

# 1.8.2

### Rrajigar Mines
- Added Rosies moons to the list of default Weights
- Revamped the Dungeon Tilesets, Many rooms are now marked as unique, and some are weighted higher depending on if they're on the main path or branching.
- Fire Exits no longer spawn in the cave room.

### Chizra Temple
- Added Rosies moons to the list of default Weights

### Skaarj Outpost
- Added Rosies moons to the list of default Weights

# 1.8.1

### General
- Updated internal LLL dependencies.

# 1.8.0

### General
- New Screenshots that better reflect the current state of the Interiors.

### Rrajigar Mines
- Added JLL as a dependecy.
- depending on the moon tag, The rock and lava textures, and light colors change depending on the Moons tag. Currently supported tags are Rocky, Canyon, Tundra, Ocean, and Asteroid-14.
- Lights are even brighter with further range.
- Doors have pneumatic opening and closing sounds from Unreal.
- Door Frames have proper room tags, preventing some oddities.
- The Rocky floors are rougher and not flat surfaces.
- Patched up a lot of holes in the tiles geometry.
- Raised the Lava surface in the Lava Hallway room. This is so if the liquid in the room doesn't instantly kill, it is high enough to drown in.
- Increased the total Light count in larger Rooms.
- Changed the position of the Main Entrance light.
- Texture changes to bricks.

### Chizra Temple
- Changed the tag and Layer on Doorframes.
- Fixed the longstanding issue of doors being ever so slightly misaligned in their frames.
- New Sounds for doors from Unreal.
- Interior ambience in some rooms.

### Skaarj Outpost
- If Klaxons are enabled, they begin playing when the Apparatus is pulled.
- Doors have pneumatic opening and closing sounds from Unreal.
- Pillars have been placed in the Entry room, these are to help mitigate cheap shot kills from turrets pointing into the room.

### Nali Haven
- New Sounds for doors from Unreal.

# 1.7.14

### Nali Haven
- Fixed doors spawning in entryways.
- Crystal lights are more indigo colored like they used to be.

# 1.7.13

### Chizra Temple
- Darker regions of Chizras water texture are more transparent.

# 1.7.12

### General
- Overhaul of default weights.

### Rrajigar Mines
- Adjusted the position of the Main Entrance slightly, this should help the Code Rebirths Shockwave gal pathfind her way outside.

### Chizra Temple
- Some floors with shallow water have been tagged with 'Puddle'.

# 1.7.11

### General
- Materials are now GPU instanced, this should squeeze a bit more performance when used.

### Chizra Temple
- In my feverish attempts to fix the lag, I axed the lighting quality even though it wasn't the cause, this has been rectified, as well as being made slightly prettier.
- The Trial of Combat was broken, It should be fixed now.

# 1.7.10

### Rrajigar Mines
- Lava is brighter and lights rooms with it better.
- Fixed some error spam with lights.
- Falling in Lava Does not leave recoverable bodies and makes appropriate burning sounds.
- Lights in the storage room, and cave room, and control room are brighter.
- The Main entrance Light is brighter and has a larger radius.
- Fixed a buried Crate.
- Removed or reduced the volumetrics from several lights.
- Removed the Unreal Content tag since LLL dungeon matching doesn't work.
- Reduced dungeon length (9-10 => 9-9)
- Reduced Branch count. (26-32 => 26-30)
- Dynamic dungeon size restrictor change to 1.8, equivalent to Rends dungeon size.

### Nali Haven
- Restored a simplier version of the elevators.
- Brightened the Crystal lights.

# 1.7.9

### Chizra Temple
- 1 New tile, the chamber of combat.
- 2 new items, one unutilized.
- The ritual of combat can be attempted for a sizeable prize. This can be disabled in the config.

### Skaarj Outpost
- Fixed a room boundary that caused room clipping in rare instances.

# 1.7.8

### Nali Haven
- The elevators broke in V65, so they have been temporarily replaced with ladders while I fix them.

# 1.7.7

### General
- Updated JLL version used and dependencies to 1.7.4.

### Rrajigar Mines
- widened the navmesh blocker in doors to prevent fringe cases of monsters slipping through them.
- Slightly brightened emergency door lights.
- Slightly increased the range and brightness of Cave Lights.

### Chizra Temple
- Lighting rework.
- Lag fixed for good.
- Fire exits will actually generate again.

# 1.7.6

### Chizra Temple
- Removed the particle effects from torches, replaced them with meshes.
- Lighting changes.
- Some optimizing.
- Dynamic dungeon size restrictor change to 1.8, equivalent to Rends dungeon size.

# 1.7.5

### Chizra Temple
- Potential fix for 1 way wall generation but for real this time.
- Toned down the Fire Particle effects on torches every so slightly for performance optimization.
- Added a dynamic dungeon size restrictor of 2.0.

# 1.7.4

### Chizra Temple
- Potential fix for 1 way wall generation occurences.

### Skaarj Outpost
- Added JLL as a dependecy.
- Lasers are more lasery looking.
- If played on USC Vortex, the pale white and green lights become red and blue.
- Added Klaxons playing throughout the facility. These are turned off by default.
- Added Lithium to the list of default moon matches.

# 1.7.3

### Chizra Temple
- Tag based modifiers Have been split into individual options, you can toggle the ones you want and don't want.
- Increased the starting points Y coordinate, this is for Fray Compatibility.

# 1.7.2

### Chizra Temple
- Tag based modifiers have a config option. this is enabled by default.

# 1.7.1

### Chizra Temple
- Added JLL as a dependecy.
- If played on moons tagged with Haunted or Argon, the torch light turns a ghastly purple.
- If played on moons tagged with Tundra, the skylights take a lighter blue hue and freezes water.
- If played on moons tagged with Canyon or Wasteland, the skylights take an Ochre hue.
- Fixed a pool collider.
- Fixed certain rooms being see through under the right conditions.

# 1.7.0

### Skaarj Outpost
- Lighting overhaul.
- Added boxes to the hangar to make it feel less empty.
- Made the fire exit Light brighter.
- Removed the connector Hall lights.
- Removed Security door spawns, The Laser gates are now this interiors versions of them. They also only generate in the Holding Cell rooms and X-Room near the end of the dungeon.
- rebalanced connector door weights.
- Laser gates no longer kill, but they Hurt a lot.
- Fire Exits should no longer spawn in the first quarter of the dungeon.
- Removed the lights from the Generator for Performance.
- Added a standard Dynamic Dungeon limiter of 1.9.
- Laser gates play a noise when they game end you.

### Nali Haven
- 1 New tile, The multi elevator room.
- Adjusted Elevator room Weight.
- Both elevator room tiles are now unique and only generate once.
- Elevator off mesh links are now one way, Enemies will not be able to magically scale the vertical wall and jumpscare you.
- Lamp Light properties have been changed to have a wider radius.
- Crystal lights are brighter, and have a larger radius.
- Window lights are brighter.
- Adapted the Mineshaft elevators.
- Added a standard Dynamic Dungeon limiter of 1.85.
- Increased bedroom weight on end caps.
- Increased the weight of the Power room deeper in the dungeon.
- Adjustments to Blocker decoration weights.
- Lamps have a hard cap of 16.
- The Diagonal hall should generate again, I don't know why it disappeared.
- Carpets can sometimes be found in hallways.

# 1.6.10

### Rrajigar Mines
- Cave Nodes for the Man Eater.
- Lava Light should be brighter everywhere.
- Turbo Charged the Lumens on everything.

### Chizra Temple
- Cave Nodes for the Man Eater.

# 1.6.9

### Rrajigar Mines
- Lights above doors now light up when the power is off, they're dim but cast a wide range.
- Added a custom Security Door. I have confirmed these are compatible with VEGA.

# 1.6.8

### Rrajigar Mines
- Added Cracks in floors with lava flows, these are for aesthetics and to provide light when the power is out.
- Removed Unused Meshs to reduce File Size.
- Added security doors, they spawn very rarely.

### Chizra Temple
- Fixed a pool.
- Changed the way the generation generates slightly, and the branching properties.
- Potential fix for blocked off main dungeon paths.

### Skaarj Outpost
- New Entrance Tile
- dungeon length increased. (10-11 => 11-12) It should be the same length in practice however.
- Added security doors, they spawn very rarely.

### Nali Haven
- Removed Fray and Cambrian from the Moon preset list, increased Temper to 100.
- Decreased Rockwell Weight to 50.

# 1.6.7

### Rrajigar Mines
- Fixed several incorrectly assigned crate.

### Nali Haven
- Fixed an oversight with blocker placements in the big lirbabrury room.

# 1.6.6

### Nali Haven
- Added Rockwell to the list of moon Presets.

# 1.6.5

### General
- New Icons to better represent the dungeons contents.

### Rrajigar Mines
- Lowered the min/max dungeon length (10-11 => 9-10)
- Increased Branching count (24-29 => 26-32)

# 1.6.4

### Rrajigar Mines
- Fixed the weird Main Entrance Light texture.

### Chizra Temple
- Disabled the Water triggers in some rooms to prevent inescapable situations you couldn't resolve through drowning.

# 1.6.3

### Rrajigar Mines
- Fixed an incorrect texture assignment.

### Nali Haven
- Fixed the entry teleporter placement in the alternate entry room.

# 1.6.2

### General
- Crunched File sizes into a singularity, all 4 interiors packed together went from 21 MB to 9 MB.
- Updated the Readme and moon weights.

# 1.6.1

### Rrajigar Mines
- Added 2 new tiles, these are Asymetrical in design and should spice up dungeon generation.
- Added an item, the Tarydium Crystal. Currently unused.
- Fixed some missing seams.

### Chizra Temple
- Added 2 new Asymetrical tiles to add Dungeon variety.
- Replaced scrap denial zones in water, They were removed unintentionally when I replaced kill zone with Water zones.

### Skaarj Outpost
- Added 1 new Asymetrical tile to give the Dungeon more variety.
- Changed how Laser Gates Work.
- Fixed a potential Laser gate desync.

### Nali Haven
- Added an alternative entry room. Very rarely the one unused can appear as a basic room.
- Further increased Bedroom Tile weight.
- Generation Changes.

# 1.6.0

### General
- Ported to V60
- Ported to LLL V.1.3.9

### Rrajigar Mines
- Brightened the Fire Exit Light.
- Lights above doors have a more easily distinguishable color from Fire Exit Lights.
- Changed the Storage room and Cave rooms Crate Layout.
- Removed a Hazard spawn point from the Control room.
- Fixed erroneously placed AI nodes in the Control room.
- Brightened the Main Entrance Light.
- Adjusted the Entry rooms components, hopefully lowering the chances of Main Entry Spawn failure.
- Added a bunch of Lights to the lower floor in the Huge Pillar Connector room.

### Chizra Temple
- Removed Kill Triggers from all Water Rooms, Replaced with Water Volumes. You will still need Assistance to Escape if trapped however.
- Someone Left a rope ladder in the Ceremony Hall.
- Water is slightly more transparent.

### Skaarj Outpost
- Reduced the chance of the entry room having a door.
- Fixed misplaced AI nodes.

### Nali Haven
- Added a Breaker box spawn to Elevator rooms.
- Fixed an incorrectly tagged Carpet.
- The Treasure room should spawn more frequently in the last third, and usually never in the first third.

# 1.5.4

### Rrajigar Mines
- Enemies can traverse the mini bridge in one of the lava room tiles when it's raised now.
- changed the dirt pile tags, they should sound like dirt when stepped on now.
- Items should spawn in the entryroom minecart more consistently.
- Changed the light properties in the Ladder Vent 8 way.

### Skaarj Outpost
- Fixed an incorrectly tagged room.
- Fixed some wild navmesh issues in the Hangar Room.

### Nali Haven
- Fixed some missing references.

# 1.5.3

### General
- Potentially fixed missing entrance errors.

### Rrajigar Mines
- Fixed some incorrectly assigned boundaries.
- Spruced up the Hallways and removed Bloat in Hall tile variety, this should mean more unique tiles should generate more often and feel less confusing to navigate.
- Increased the chances of the Locker Room Spawning.
- 1 New Tile, the Ventilation 4-way Corridor.

# 1.5.2

### General
- Shuffled the Hazard Spawns in all dungeons.
- File Size reduction for all interiors.

### Rrajigar Mines
- The glow around Lights has been reduced and their shadows removed, The light emitted from lamps are brighter and have a larger radius.
- Fire Exit lights are brighter and more Conspiscuous.
- Added Sierra to the list of Default moon assignments.

### Chizra Temple
- Skylights are brighter.
- Water doesn't cast shadows, this should make it easier to see the death pits.
- Added Fray and Cambrian to the list of Default moon assignments.

### Skaarj Outpost
- Fire Exit lights are brighter and more Conspiscuous.
- Added Cambrian to the list of Default moon assignments.

### Nali Haven
- Reduced the min and max Lamp count. (15-20 => 14-19)
- The Lamp light above the Main Entrance is more Bluish in color and always spawns.
- Home room tiles. are more common.
- Added Fray, Cambrian, and Temper to the list of Default moon assignments.

# 1.5.1

### Nali Haven
- Adjustements to table collisions, this should hopefully stop items spawning inside tables

# 1.5.0

### General
- Updated the Mods screenshots
- Fixed a typo in the Readme.

### Rrajigar Mines
- Greatly expanded the Range Scrap and Hazards will Spawn.
- Normal Mapping!
- 1 New tile, a locker room.

### Chizra Temple
- Fixed an incorrectly configured room
- Added 2 scrap spawns to the 6 Fires Chamber.
- Expanded scrap and Hazard spawn ranges in some rooms.
- 1 shiny new Tile, A big ass bridge.

### Skaarj Outpost
- scrap and Hazard spawn ranges Increased in places.
- Adjusted the Generator room Lighting.
- 2 New Tiles, A storage bay and a fancy hallway.
- Changes to Dungeon Generation.

### Nali Haven
- Expanded scrap and Hazard spawn ranges in some rooms.
- 2 New Tile, A big Library and Diagonal Hallway.
- An unused Bar Tile has been reimplemented, so that technically means 3 new tiles?
- Reduced the door Spawning chances in Hallways.

# 1.4.0
- Dungeons have been split into individual Bundles to be released separately. I apologize for the file size increase that ensued.
- Texture property changes in all dungeons.
- Doors in Chizra are fancier looking.
- Fixed items spawning out of bounds in Chizra Temple.
- Rrajigar Doors have a small light above them, Their orientation matters.
- Fancier Lighting effects in Rrajigar Lights.
- Fixed missing Audio mixer and animation properties in some Rrajigar Lights.
- Skaarj Outpost Doors Have glowing inner panels.
- Fixed a Seam in the skaarj outpost hallway blockers.
- Fixed off-center door placement in the Holding Cells tile in Skaarj Outpost.
- Adjustments to some lights in Skaarj Outpost.
- Laser doors have a rare chance to spawn in Skaarj Outpost Hallways.
- Scrap can spawn in L-Hallways in Skaarj Outpost.
- Doors in Nali Haven are a little more shapely and less flat.
- Increased the Global Limit of Nali Haven Lamps. (9-18 => 15-20)
- Removed a lot of Mesh colliders from objects that didn't need them.

# 1.3.9
- Dungeon Entrances should play nicer with Cullfactory.

# 1.3.8
- Updated the Readme
- Removed a scrap spawn point from slope halls in Skaarj Outpost, added one instead to the default 4 way Hall. This should greatly help with loot distribution.
- Elevators in Nali Haven and Rrajigar will no longer be locked.

# 1.3.7
- Nali Chapel my beloved and hated, I have been forgetting to add a ladder to reach the second level for the last 4 patches but now it's here.
- Increased the range of the lights emitted from the Glass stained windows in the Chapel and Entry hall and removed their volumetrics in Nali Haven.
- Swapped Laser gate states in Skaarj Outpost.

# 1.3.6
- Ported to LEthal LEvel LOader V.1.3.1
- Fixes to Generation setup means entry rooms branch off more from the start. Dungeon Length of all dungeons affected increased, but the actual dungeon size will be the same.
- Adjustments to Nali Haven Size. (9-11 => 10-11) (20-24 => 20-32)
- Adjustments to Rrajigar Mine Size. (9-10 => 10-11)
- Adjustments to Outpost Branch Count. (26-30 => 28-32)
- Adjustments to Chizra Branch Count. (20-23 => 20-26)
- Disabled Volumetrics on the Hallway Light panels on Skaarj Outpost.
- Lighting Adjustments to Skaarj Outpost Entry Room.
- Fixed a Seam in the Study Room in Haven.
- Reduced the volumetrics in Haven Lights, Increased the Blue Crystal Ambient Light Count and changed their properties.
- Lamps in Haven Turn off when Unpowered.
- Skylights in Chizra have been changed to Spotlights and some of their shadows disabled, Volumetrics have been added.
- Reduced Haven Weights for Rend and Dine. (300 => 200)
- Dungeons have a unique 'Unreal' Content Tag for Lethal Level loader.

# 1.3.5
- Rrajigar and Haven should be slightly brighter on average.
- Added an additional scrap spawn point to the Sloped hall, Hangar, and Pipe Hallway in Outpost.
- Reworked Scrap spawns in Rrajigar. Where there are crates, loot is abound.
- Laser grid doorways added to Skaarj outpost, they open and close like regular doors.
- Reduced length and branching count of Nali Haven. (10-12 => 9-11) (22-25 => 20-24)
- The Chapel Rooms entrance configuration in Nali Havens has been fixed.

# 1.3.4
- Reduced the amount of doors in Chizra Temple.
- Removed some floating colliders that shouldn't be there in Rrajigar mines
- The Ladder in the Observation hall in the Skaarj outpost is more ladder shaped with a model.

# 1.3.3
- Fixed and Issue with Rrajigar mines Fire Exits.
- Vastly increased potential Fire Exit Spawn Locations on Nali Haven.
- Nali Haven Exits are spawned slightly higher to fix a potential Spawning Problem.

# 1.3.2
- Duplicate door spawns removed from Skaarj Outpost.

# 1.3.1
- Vents are important. Skaarj outpost and Rrajigar mines had none, this has been resolved.

# 1.3.0
- Fully V56 supported.
- Added the Nali Haven interior, A Stoney Mansion alternative filled with abandoned living spaces, libraries, and Homes lit by lamps and Crystal light.
- Many changes to lighting in various rooms in all Dungeons.
- Scrap placement overhaul.
- The laser grid in the Skaarj outpost Hanger room kills on contact, this was done for consistency between all laser grids.
- A lot of other stuff I'm probably forgetting.

### Important Note

Project files were borked during the update process, So I had to recreate all the Dungeon flows, Tilesets, and Archetypes from scratch. Dungeons should still feel about the same but with a subtle change in structure. If issues arise relating to this, I will try to fix them as fast as possible.

# 1.2.2 (This update was not released publicly.)
- multiple tiles across all dungeons should spawn in a way that prevents impossible 2 handed item transference.
- An elevator has been added to a tile in Rrajigar mines.
- The Death Pit room in Chizra Temple kills from gravity instead of Drowning.
- Lowered the Death Trigger in the opening Ceremony hall in Chizra Temple.

# 1.2.1
- Manifest dictated there was 2 interiors when there are 3, this has been rectified.
- Apparatus spawn points added to Rrajigar Mines and Skaarj Outpost.
- Rrajigar Mines Lighting Adjusted, Lights generally are brighter but with shorter radii.
- Lava Pools in Rrajigar Mines kill by Burning rather than Gravity now.
- Fire Exits are more common in deeper sections of Rrajigar Mines.
- Fixed Item spawns in Rrajigar Mines Cave Tiles.
- Door lines shown on the terminal and in Minimap mods should accurately reflect the state of the Door now.
- Fire Exit lights have been brightened on Skaarj Outpost and Chizra Temple.
- Added a new tile to Skaarj Outpost, The Generator Room. It will typically spawn at the end of the dungeon and contains the Apparatus.

# 1.2.0
- Added Skaarj Outpost Interior.

- Reduced the overall length of Rrajigar Mines to make it feel less Empty.
- Added a bunch of Scrap spawn points in Rrajigar Mines.
- Fixed the Bridge selection in the Lava Suspension Bridge Room in Rrajigar Mines.
- Fixed several pathing issue in Rrajigar Mines.
- Rrajigar Ladders are ladder shaped and more obvious to spot now.

- Audio bugging out should be fixed in Chizra Temple.
- Performance improvements (hopefully) in Chizra Temple.
- Reduced the Particle density in the Chizra Temple Torches.
- Fixed several pathing issue in Chizra Temple.
- The Large 8 way pillar room in Chizra Temple cannot spawn with Fire exits anymore.

- Adjusted some pick rates in the dungeon matching settings.

# 1.1.1
- Adjusted chizra temple Torch spawns
- Fixed some erroneously placed vents in Rrajigar Mines.
- All Dungeons have a Unique Stinger.

# 1.1.0
- Added Temple of Chizra Interior.
- Adjusted Rrajigar pick rates.


# 1.0.0
- Release Version