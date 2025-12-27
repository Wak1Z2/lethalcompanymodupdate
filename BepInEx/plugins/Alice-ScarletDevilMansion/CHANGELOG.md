### 2.3.3
Updated for v73

### 2.3.2
Fixed map radar for interior.

### 2.3.1
Increased bounds for all dungeon variants to decrease failure chance\
Larger rooms now try to spread their doorways around\
Added new broken doorways for certain rooms\
Scarlet Basement now prefers to generate downwards\
Hallway lights are brighter

Fixed some issues with hallway visuals and error spamming\
Fixed some issues with Maids and Revenants in multiplayer\
Fixed issues pertaining to moons with high amounts (6+) of fire exits

### 2.3.0
Redid dungeon generation. All dungeons generate hallway tiles more often, have longer main paths, and shorter branching paths.\
Retextured and redid the hallway rooms\
Added new stair rooms\
Redid all void rooms

Added some new visual effects to the portraits and void\
Added some sound effects for using the jukebox

Adjusted hitbox of the maid's dropped knife to match her full body initially\
Fixed blood from the maid and her knife to not be weirdly shiny white

### 2.2.2

Fixed me serializing stuff that I really shouldn't be. May stop certain crashes

### 2.2.1

Fixed crashing lol bad dev forgot to include some .pngs

### 2.2.0

Updated for LLL 1.4.0\
Added new dungeon variant\
Added new scrap item\
Separated configs into the main mod and each of the individual dungeon's generation

Void rooms with missing paths are slightly easier\
Enlarged 2F library rooms\
Added a bit more space to the 1F library rooms\
Added collision to the christmas trees\
Fire exits will no longer spawn close to each other\
Hallway rooms: removed some tiles, reduced some of the blood spam, added decorations

Fixed revenant slowly down even when you aren't looking at it\
Fixed vent effects and sounds to work\
Knights and Revenants now play a summoning effect when they spawn on props\
Knights no longer trigger vent effects\
Revenants now spawn at a vent instead of on the maid if no props exists\
Fixed loot interaction with CodeRebirth's Gal enemies


### 2.1.0

Updated for v69\
Added more config fields for scrap items and enemies\
Added christmas trees to mayor\
Each main path will generate a minimum of one fire exit and painting if possible\
Slightly shrinked the size of the vanilla dungeon\
All critical damage mechanics renamed to "marked for death." Being marked for death by any mechanic twice will kill the player regardless of the source.\
Revenant properly slows down when being stared down\
The code to inject items/enemies when SDM dungeon loads has been changed. May cause bugs please let me know if they occur\
Added new portrait art

### 2.0.0

Updated for v65/66\
Two new outside rooms with an open sunroof\
Added visual effects to the dungeon if the moon has certain weather effects\
Dungeon "sunlight" will decrease over time\
The v62 enemies should destroy Scarlet doors now\
Undefined enemies (future or modded) should open Scarlet doors by default now\
Updated the red anger effect to be less red\
Made the mayor pillars float higher in the air

### 1.3.0 - 1.3.27

<details> 
  <summary>
  Updates
  </summary>

Added many variant rooms\
Added void rooms\
Added new treasure rooms\
Added clock prop to main entrance\
Added destroyable doors\
Added spike traps to dungeon\
Added jukebox with Touhou beats to Servant's Quarter rooms\
Redone dungeon brightness, item and map hazard spawn locations\
Added ink/blood stains throughout the mansion floor\
Expanded mayor entrance tile, removed basement\
Shrunk all 1F libary rooms\
Lights now have a chance of flickering and dying

Updated dungeon generation to prefer branch tiles that make multiple connections to encourage looping paths

Added new enemy variant for Butler and new weapon from said enemy\
Added new scrap item, shattered decorative crystal (can combine with flashlights)\
Added new scrap item, doll snowglobe\
Added new scarlet key (it's just red) to help with visibility\
Updated knight to match the coilhead's new v60 behaviour\
Knight enters a brief cooldown after hitting a player

Added config to add unique enemy spawns during the bedroom dungeon event\
Added configs for dungeon enemies and items spawn weights\
Added config for demonic painting\
Added config to use either SDM or vanilla fire exits\
Moved some of the configs to LLL

Dungeon lights turn red during certain dungeon events\
Added special colouring to enemies that spawn from the painting event\
Portraits stare at you when you aren't looking

Added Mimics compatibility\
Added FacilityMeltdown compatibility
Added ReservedFlashlightSlot compatibility\
Added ReservedKeySlot compatibility\
Added Coroner compatibility\
CullFactory mod is now manatory\
LethalConfig's entries will have a different shade of red if my preset settings auto-change its values

Updated mod for my new API\
Added Sanguine (moon) to the interior's spawn list\
Added Scarlet Devil Mansion (moon) to the interior's spawn list

</details>

### 1.2.0 - 1.2.12

<details> 
  <summary>
  Updates
  </summary>

Added new dungeon event\
Added basement to mayor starting room\
Added bedroom and servant quarter variant rooms\
Many many internal code and design changes to reduce the load times by abouy 90% on average\
Removed garden tile (temporarily). Added unpolished fire exits throughout the dungeon\
Added rotateable frames to the hallways\
Added new functionality to decorative crystal item\
Added config presets. Automatically set to default. Contains two distinct presets for 4+ lobbies are 1-3 smaller lobbies\
These config presets make the map much smaller\
Fixed scrap spawn prefering to spawn on the upper floors\
Added many new networked configs\
Switch from BinaryFormatter to OdinSerializer\
Fixed issues with unofficial Korean patch

</details>

### 1.1.0 - 1.1.12

<details> 
  <summary>
  Updates
  </summary>

Added support for LLL\
Detailed the hallway rooms and added new ones\
Added lethal company's lighting onto the dungeon (somehow?)\
Added new enemy variant\
Added new scrap item\
Fixed enemy pathing issues\
Spray cans now work, thanks SkullCrusher my beloved\
Added wall lights to hallway rooms as a possible spawn\
Added chandelier lights to most rooms as a possible spawn\
Added networked config to modify the spawn chance of light sources\
Added networked config to modify much of the dungeon generation values and scrap count

</details>

### 1.0.1 - 1.0.4

<details> 
  <summary>
  Updates
  </summary>

Detailed the mayor starting room\
Added three detailed kitchen variants\
Made more drastic changes to make the map much less spread out, AKA map is smaller

</details>
