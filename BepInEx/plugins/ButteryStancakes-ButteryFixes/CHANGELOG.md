# v1.15.6
- Fixed head cam still being visible on radar after a player is eaten by the monster at the company building
  - Also fixes `NoBodyNoSignal` not applying to the same conditions
- Fixed various shenanigans with floating corpses and water
- Corrected an infamous typo with `TheGoldenGoblet` which was mistakenly implemented as a "Golden cup"
# v1.15.5
- Hotfix for conflict with [FurnitureLock](https://thunderstore.io/c/lethal-company/p/mattymatty/FurnitureLock/)
# v1.15.4
- Added `NoBodyNoSignal` setting
- Some fixes to the "exit line" on the radar:
  - Fixed line dots not scrolling visually
  - Fixed line "contorting" strangely when targeted player is moving around the map
  - Line now displays when targeting a "masked"
- Fixed a tutorial pop-up about storing furniture, which previously didn't work for the host
- Cached a couple of references to the Cruiser in the sapsucker AI (thanks [Scandal](https://thunderstore.io/c/lethal-company/p/ScandyTeam/))
# v1.15.3
- Fixed gift boxes having increased spawn chances ever since v70
  - [Zeekerss confirmed in Patreon chat](https://discord.com/channels/750645598293590077/974101195545280542/1424081957288935555) that this was a mistake (somehow the code from v69 Jolly was accidentally added back)
  - v1.14+ assigned this bonus weight to Zed Dog (which was also given boosted spawn chances in v70) instead, but I've removed that now (as Zed Dog boosts were reverted in v73)
- Fixed new v73 scrap having visible effects while pocketed
# v1.15.2
- Added an experimental `EndOrbitEarly` setting
  - Enabling it will cause clients to end orbit phase as soon as the lever is pulled (like the host) instead of after the doors open
  - This should fix some desync (most notably with Sapsucker eggs insta-hatching)
  - Might cause unexpected behavior with other mods if they expect vanilla's incorrect behavior, but I'm not currently aware of any examples
- Keys will now still use their special icon on the radar when using `KeysAreScrap`
  - You still need to use [BagConfig](https://thunderstore.io/c/lethal-company/p/mattymatty/BagConfig/) to store keys in a belt bag with this setting on. I don't plan to change this, sorry
# v1.15.1
- Compatibility with [Drop Ship Delivery Cap Modifier](https://thunderstore.io/c/lethal-company/p/DrinkableWater/DropShipDeliveryCapModifier/)
# v1.15.0
- Finally added an `AdjustCooldowns` setting
  - Sorry for the stubbornness on this one
- Entering the ship should now auto-collect all items in your inventory, not just what you're holding in your hand
  - This change is (somewhat) experimental
  - If you notice any issues arising with items or scrap collection, turn off `AutoCollect` and see if it helps
- Tried to fix some desync between "most profitable" statistic when collecting scrap with the Cruiser
- Fixed "Items missed!" dropship message only displaying for host
- Fixed "Store item" text for microwave door
- Added `AlterBestiary` setting to block changing bestiary entries
- Fixed "Value:" text being allcaps on bee hives and eggs
# v1.14.7
- Fixed a potential error v1.14.6 would have thrown for custom interiors
# v1.14.6
- Fixed several v70 manor tiles not properly adapting to the breaker box
- Fixed fridge costing $150 instead of the displayed $225
- Microwave is no longer silent after loading a save
- Removed auto-compatibility for [Fast Climbing](https://thunderstore.io/c/lethal-company/p/Inoyu/Fast_Climbing/), [BetterLadders](https://thunderstore.io/c/lethal-company/p/e3s1/BetterLadders/), and [BetterStamina](https://thunderstore.io/c/lethal-company/p/FlipMods/BetterStamina/)
  - Please disable the `PatchLadders` config setting instead, if you use a ladder sprinting mod
# v1.14.5
- Re-upload because I forgot the DLL :\
# v1.14.4
- Fixed turrets shooting you from inside walls/bookshelves
- Adjusted landmines and radar boosters so they should be more visible on the v70+ radar
- Rewrote the code for the microwave to address some problems
  - Fixed errors when opening the microwave near the fridge
  - Fixed desync between animation, audio, and items spinning
- Adjusted colliders for microwave and fridge
  - Fixed items being grabbable through the body of the microwave
  - Fixed items being placed under the plate in the microwave
  - Fixed items being placed "through" the fridge instead of on the shelves
- Fixed some misplaced invisible colliders on the greenhouse tile
- Fixed some missing collision on Experimentation
- Fixed the "exit line" sometimes getting stuck on the radar but not updating
- Fixed some bugs with pop-up advertisements
  - Fixed incorrect discount being displayed on items for clients
  - Fixed suit ads failing to display
- Fixed incompatibility with [NoLostSignal](https://thunderstore.io/c/lethal-company/p/Tomatobird/NoLostSignal/)
# v1.14.3
- Fixed contour map sometimes not appearing (after v71) on moons that have one
- Fixed error spam from Giant Sapsucker in multiplayer
# v1.14.2
- v72 compatibility (Removed redundant fixes)
  - Gift box randomization
  - Clock/candy spawn groups
  - Sapsucker error spam
- Fixed two sets of arms being visible for the local player on the ship camera
# v1.14.1
- v71 compatibility (Removed redundant fixes)
  - Radar booster ad fix
  - March/Titan/Embrion radar performance
  - Global audio for weed killer
- Fixed some problems with my patch relating to "No signal!" screen
- Fixed radar's exit path being unreliable for players in mineshafts
- Fixed some small bugs with sapsucker eggs (no longer inspectable, marked as outside scrap, etc.)
- Fixed your own corpses not having the correct badges on your client
- Fixed challenge moons sometimes still displaying Embrion's name on the monitor
# v1.14.0
- v70 compatibility
- Playermodel patches are now enabled by default and can be disabled by a setting
  - In previous versions, these were automatically disabled when using [ModelReplacementAPI](https://thunderstore.io/c/lethal-company/p/BunyaPineTree/ModelReplacementAPI/).
  - I still recommend disabling these if you run into issues with that or similar mods
- Fixed clocks and candy being unable to spawn (and reducing total scrap counts)
- Fixed bonus spawn chance being applied to gift box instead of Zed Dog
- Fixed gift box contents not being properly randomized
- Fixed "No signal!" screen getting stuck and/or not appearing when it's supposed to
- Fixed performance issues when watching radar on March, Titan, and Embrion
- Fixed corpses created by Giant Sapsucker:
  - Fixed excessive error spam
  - Fixed broken "explosion" physics for body parts (splattery!)
  - Corpse now wears the correct suit
- Fixed dropped items not synchronizing their rotation for other players (most notable for radar booster "headcam")
- Dropped items now make noise alerts for all clients (fixes inconsistent detection behavior for some enemies)
- Fixed door unlock sound playing twice
- Fixed radar booster's giant blue circle on advertisement pop-up
- Fixed issue with grabbing items out of the microwave
- Electric chair now burns corpses
- `LockInTerminal` setting now applies to sofa chair
# v1.13.3
- Completely removed fire exit optimizations
  - I suggest trying [EntranceTeleportOptimizations](https://thunderstore.io/c/lethal-company/p/mattymatty/EntranceTeleportOptimizations/) instead for better support
- Corrected some typos in Hygrodere's bestiary entry
- Re-removed Sigurd sections from Old Birds' bestiary, unless you have Vain Shrouds scanned or spawned on your save file
  - The Vain Shroud entry has a similar timeline contradiction that was never corrected
# v1.13.2
- Changes to optimizations from v1.11.0 to prevent "wrong warp" on using fire exit
- Dormant Old Birds can now be scanned on both sides of their body
# v1.13.1
- [Lobby Compatibility](https://thunderstore.io/c/lethal-company/p/BMX/LobbyCompatibility/) integration
- Fixed some issues with the Cruiser key in first person
# v1.13.0
- Renamed `RestoreFilmGrain` settings to be more intuitive (this might reset your chosen value, sorry)
- Added `RestoreArtificeAmbience` setting
- Expanded `ScanOnShip` setting (now `ScanImprovements`)
  - Butlers' now display a scrap icon on the map before they are killed
  - Fixed incorrect prices being displayed on scanner for kitchen knives, bee hives, shotguns, and the apparatus
- Added `DisableLODFade` setting (thx [dopadream](https://thunderstore.io/c/lethal-company/p/dopadream/))
- Fixed incorrect information being displayed when typing "upgrades" in terminal
- Fixed out-of-bounds "Main entrance" scan node on Gordion
# v1.12.2
- Fixed `RestoreFilmGrain` setting not working if you have [More Company](https://thunderstore.io/c/lethal-company/p/notnotnotswipez/MoreCompany/) cosmetics enabled, and don't have [Emblem](https://thunderstore.io/c/lethal-company/p/Darkbrewery/Emblem/) installed
- Fixed enemy spawns being incorrect on challenge moons (only fixed when `LimitSpawnChance` setting is used)
- Fixed a potential issue with placing items on shelves in multiplayer (thanks [FlipMods](https://thunderstore.io/c/lethal-company/p/FlipMods/))
# v1.12.1
- `FixGiantSight` setting
  - This will fix the infamous bug with Forest Keepers instantly chasing players (even if they are spotted for only a single frame, at any distance)
  - If you use [Fair Giants](https://thunderstore.io/c/lethal-company/p/LegoMaster3650/FairGiants/), you should disable this setting to avoid making them extra stupid
- Fixed items growing when dropped in the Cruiser and shrinking when dropped in the elevator
- Fixed red foliage turning green (at long distances or in spectator mode)
- Restored bloom effect on title screen from v30 (if `RestoreFilmGrain` is used)
  - Note that, at this time, the film grain setting DOES NOT WORK if you use [More Company](https://thunderstore.io/c/lethal-company/p/notnotnotswipez/MoreCompany/), unless you disable cosmetics
- Added `AlsoRadar` setting to `RestoreFilmGrain`
  - This will apply scanlines to the radar camera
  - Zeekerss disabled this prior to v9 (which had all the other effects still enabled)
- Added a bonus `TypeGordion` setting
# v1.12.0
- Added a setting to restore film grain effects from earlier versions of the game (v4, v9)
- Fixed out-of-bounds text on terminal when having more than $999 credits
- Added a bonus `FilterDecor` setting
- Fixes to slime "spreading" behavior (Thanks [Zaggy1024](https://thunderstore.io/c/lethal-company/p/Zaggy1024/)!)
- Further tweaks to item pickup sounds
- Some updates to compatibility with external mods
# v1.11.2
- Added a bonus `LockInTerminal` setting
- Fixed Forest Keeper ambience playing in Foggy weather at distances where you weren't in vision range
# v1.11.1
- Migrated shotgun fixes (except shell animations) to [Melee Fixes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/MeleeFixes/)
- Earth Leviathans no longer trigger collision with each other (fixed potential lag?)
- Fixed potential error spam from baboon hawks
- Fixed badges not appearing on corpses that aren't wearing the bee/bunny suits
# v1.11.0
- Migrated all mask and mimic fixes to [Mask Fixes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/MaskFixes/)
- More major performance optimizations (please let me know if you encounter any weird issues after this update)
  - Patched all enemies that interact with the Cruiser to avoid performing an expensive search
  - Patched entrance doors to reduce potential lag spikes when entering/exiting the building
# v1.10.20
- Orange suit now displays "Change: Orange suit" on the rack
- Corpse fixes
  - Meteors no longer spawn Tragedy-masked bodies
  - Fixed bee/bunny suit parts being visible on webbed bodies
- Minor performance optimizations
# v1.10.19
- Fixed music not playing more than once per session (thanks [SimonTendo](https://thunderstore.io/c/lethal-company/p/SimonTendo/) for discovering the root cause of this issue)
# v1.10.18
- Fixed Cruiser seat bugs
  - Now you can use the scanner while seated
  - No longer immune to death pits while seated
- Fixed terminal model not being visible on the ship's internal security camera
# v1.10.17
- Fixed typo in store description
- Fixed welcome mat price again
# v1.10.16
- Stormy weather redirects target to items outside of the ship a bit more aggressively (to minimize reduction in "difficulty" from v1.10.15)
# v1.10.15
- Fixed stormy weather constantly re-targeting items that are already inside the ship
- Offense displays video reel on the monitor again
# v1.10.14
- Fixed a problem with the bestiary when rehosting
- Fixed a rendering issue with the ship radar's "camera flash" animation
# v1.10.13
- Reupload of v1.10.12
# v1.10.12
- Migrated Rend/Adamance cabin door fix to [Enemy Sound Fixes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/EnemySoundFixes/)
# v1.10.11
- Fixed bugs with how hives are priced
# v1.10.10
- Reattempted fix for [Touchscreen](https://thunderstore.io/c/lethal-company/p/TheDeadSnake/Touchscreen/)
# v1.10.9
- Fixed mineshaft echo persisting forever if you die in the caves
- Planets are no longer visible in orbit (migrated this feature to [Chameleon](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/Chameleon/))
- Fixed buggy keyboard interactions with the belt bag UI
- Fixed compatibility with [Touchscreen](https://thunderstore.io/c/lethal-company/p/TheDeadSnake/Touchscreen/) and [Ordered_Custom_Boombox](https://thunderstore.io/c/lethal-company/p/Hackattack242/Ordered_Custom_Boombox/)
# v1.10.8
- Dust pan is now conductive
- Fixed compatibility with the birthday hat (if you have it enabled in [Classic Suit Restoration](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/ClassicSuitRestoration/))
- Fixed glowing eyes on Tragedy mimics
# v1.10.7
- Hotfix for compatibiilty with [Celestial Tint](https://thunderstore.io/c/lethal-company/p/sfDesat/Celestial_Tint/)
# v1.10.6
- The external security camera is now a bit busier when in orbit:
  - Now you can see the planet and moon the ship is parked at, like earlier versions of the game.
  - Fixed the particle effect when the ship is moving through space, so it now works every time you reroute (not just the first time)
- Hotfixed the Halloween fog event being more frequent than it's supposed to be
# v1.10.5
- Fixed a potentially gamebreaking error with the jump cheese patch
- Removed some unnecessary compat code
# v1.10.4
- Fixed raindrops on helmet during Flooded weather
- Some visual fixes for the birthday hat
# v1.10.3
- Some improvements to external mod compatibility
# v1.10.2
- Removed some redundant fixes (as of latest patch)
- Fixed the cabin doors using the wrong sounds on Rend and Adamance
- Fixed Teeth not being collected when magnetizing the Cruiser
- Consistency tweaks to item sounds
- Old Birds and Forest Keepers no longer interfere with items (soccer balls & whoopee cushions) when they are inside the ship
- Fixed throwables (stun grenades, easter eggs, etc.) falling through catwalks and other metal gratings when thrown
- Fixed some enemy line-of-sight issues on Dine
- Spike traps no longer spawn inside of the elevator
# v1.10.1
- Hotfix for stormy weather patch sometimes(?) causing an exception on startup
# v1.10.0
- Removed some redundant fixes implemented in v64
- Fixed stormy weather not targeting items as of v64
- Soccer ball fixes
  - Fixed soccer ball being impossible to scan
  - Fixed soccer ball making you invisible to nutcrackers
- Fixed Old Birds being immune to the Earth Leviathan (new bug since v60)
- Spray paint cans ordered during the same round can now have different colors
- Fixed maneater opening doors while held by the player
- Fixed some surface lights turning off on Dine or Artifice when power goes out
- Fixed players endlessly tracking blood if they are critically injured right before end-of-round recovers their HP
# v1.9.0
- Migrated some features to [Chameleon](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/Chameleon/), a new mod
  - Removed `FancyEntranceDoors` setting
  - Removed snow-recolored boulders
- Fixed Forest Keepers' sight timers being unclamped
- Fixed some interior bugs when landing on March after visiting any previous moon
- Maybe fixed fancy lamps spawning underneath tables?
- Fixed a certain prop in the manor blocking item grabs
- Players who die in the ship get auto-collected :-)
- Fixed some factory rooms having unpaintable floors
- Fixed water droplet rendering in the caves when standing underneath them
# v1.8.1
- Reverted door haunt behavior to vanilla
- Further improvements to player animations when scrolling items (thx again [pacoito](https://thunderstore.io/c/lethal-company/p/pacoito/))
- Fixed audio echo persisting permanently if you quit to main menu while inside a mineshaft
- Enemies won't kick the soccer ball out of the ship as it's leaving
- The dog ship patch from v1.3.1 should now apply when the ship door is open as well
- Reduced several console logs to "Debug" level for better filtering
# v1.8.0
- Some improvements to player animation consistency when scrolling through the hotbar. Thanks [pacoito](https://thunderstore.io/c/lethal-company/p/pacoito/)!
- Cruiser fixes
  - Items placed into the back of a magnetized Cruiser now get auto-collected
    - Fixed items inside a magnetized Cruiser sometimes being lost in orbit
  - Cruiser no longer carries over when fired or after completing a challenge moon attempt
- Fixed Earth Leviathan killing players that are inside the ship
- Fixed compass showing on radar when observing a dead body (even inside the building)
- Fixed haunted doors being increasingly more frequent in multiplayer (the more people using this mod, the better it'll work)
- Fixed dead enemies kicking the soccer ball
- Fixed some items showing unusually high or low random value on the terminal's "scan" command
# v1.7.2
- Fixed softlock when landing on March
# v1.7.1
- Fixed fancy doors persisting between days regardless of interior type
- Fixed maneater AI breaking when they get crushed by a spike trap as a baby
# v1.7.0
- v61 compatibility
  - Removed redundant fixes
  - Doppler setting now applies to elevator jingle
  - Fixed conductivity of v60 items
- `FancyEntranceDoors` now changes the entrance appearance based on the currently active interior (for all vanilla levels)
# v1.6.2
- Fixed Cruiser engine alerting dogs twice in a single tic
- Dogs now hear the Cruiser radio when it is turned on
# v1.6.1
- "Reduced" setting now further reduces the Doppler effect on the Cruiser radio
- Fixed Experimentation having the wrong weather on screen immediately after being fired
- Fixed Old Birds not adding to spawn cap or power count when they wake up from the apparatus being unplugged
  - This does not apply if you enable the `UnlimitedOldBirds` setting
- Added a warning if using [Lethal Quantities](https://thunderstore.io/c/lethal-company/p/BananaPuncher714/LethalQuantities/) without enabling `UnlimitedOldBirds`
- Fixed mimics rolling their sprint chance *per player* (instead of just once) when attacked
- Added smoke particles to all burnt corpses (previously just Old Bird blowtorch and Cruiser explosions)
# v1.6.0
- Added a config setting to replace the main entrance doors with fancier ones on Rend, Dine, and Artifice
- Disabled several unused out-of-bounds objects on vanilla levels (possible performance boost?)
- Added a config setting to re-enable "killing" Old Birds with the Cruiser
- Added a config setting to allow Old Birds to keep spawning after all dormant ones have woken up
  - Also fixed enemy spawns sometimes being skipped after all Old Birds wake up, if you don't enable this setting
- Added a config setting to limit the spawn weight of entities to 100 (on vanilla maps)
- Added a config setting to fix the ship icon not displaying next to the compass radar
- Cozy lights and disco ball no longer interrupt firing sequence
# v1.5.7
- Hotfix for compatibility with Old Bird in [Everything Can Die]
# v1.5.6
- Fixed Artifice fire exit still facing the wrong way (oopsie)
- ScanOnShip will now display items inside the Cruiser
- Fixed destroyed Cruiser still showing health meters when sprayed with weed killer
# v1.5.5
- Kidnapper Fox won't kill players inside the ship unless it has been damaged/stunned
- Tried to fix vanilla's XP reset bug
- Fixed "[Near activity detected!]" not working with "masked" for clients
- Some improvements to spray paint hit detection so it paints more clearly
  - My changes will be skipped if you are using [BetterSprayPaint](https://thunderstore.io/c/lethal-company/p/taffyko/BetterSprayPaint/), which does the same things but better
- Additional fixes for end-of-round screen
  - Fixed apparatus not actually being tracked in previous patch
  - Butlers now add their knife's value to the scrap total even if they aren't killed
  - Fixed letter grade calculation
- Teleported bodies now get automatically collected
- Randomly spawning boulders now match the aesthetic of snow planets better
- Player bodies are now coated in blood when they die to butlers or spike traps
# v1.5.4
- Hotfix for a potential incompatibility with custom moons
# v1.5.3
- Fixed keys still adding to the value counter on the HUD when they aren't marked as scrap
- Fixed the welcome mat price being inconsistent between $40 and $50
- End-of-round scrap display now shows the correct numbers
- The "Ship" scan node now moves with the ship (while landing, or taking off)
- Fixed flashlight beams not showing up when other players were using them (due to some 1.5.2 code)
- Fixed extension ladders not always beeping before they close
- Weed killer is now inspectable
- Fixed landmines still making the trigger sound when whacked with a shovel after they explode
- Tried to fix some bugs with fog on Experimentation when using the jetpack
# v1.5.2
- Fixed flashlights turning each other off if you have multiple in your inventory
- Fixed laser pointers shining through walls when pocketed
- Config setting to rotate fire exit teleporters so you are always facing forward 
- Miscellaneous fixes to each moon
  - Dine: The pit outside of fire exit kills you instead of getting you stuck at the bottom forever
  - Experimentation, Offense, Adamance, Embrion, Titan: Fixed factory ambience not emitting from the main building
# v1.5.1
- Fixed items auto-collecting for clients at the start of each round
- Migrated tulip snake fixes to [Jetpack Fixes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/JetpackFixes/)
# v1.5.0
- v56 compatibility
  - Removed several redundant fixes added to vanilla in v56
  - If you purchase the Cruiser and rehost it will be reloaded into the dropship
  - Fixed Old Birds' AI breaking when getting hit by the Cruiser
  - Fixed survival kit not giving you the right items
- Config setting to re-roll starting seed
  - This will change the shop rotation, discounts, and weathers each time you create a new save file
- Config setting to scan items on the ship when using terminal in orbit
- Player corpse fixes
  - Now wear accessories (for bee & bunny suit, badges, stickers)
  - Fixed helmet using an old texture
  - Fixed legs wearing the wrong suit when you get snipped
  - All forms of explosive deaths now cause your corpse to appear burnt
  - Destroying the Cruiser no longer "melts" your corpse, just burns your suit
- Fixed hum from breaker box when power is turned off by scripted events
- Fixed dying giants crushing players inside the ship when they fall over
- Fixed eyeless dogs getting stuck attacking permanently after hearing too many sounds in one spot
- Miscellaneous fixes from [GeneralImprovements](https://thunderstore.io/c/lethal-company/p/ShaosilGaming/GeneralImprovements/) (if you have both installed, GI's versions will be prioritized)
  - Fixed landmines not disappearing on ship radar or scanner after detonating
  - Fixed discounts not being displayed for the host when starting/loading a game
  - Fixed "MONITORING: Player" text not displaying username until switching the camera for the first time
  - Terminal now lets you order items in groups of 12, not 10
# v1.4.1
- Hotfix for [More Company](https://thunderstore.io/c/lethal-company/p/notnotnotswipez/MoreCompany/) compatibility
# v1.4.0
- Data chips now disappear for all players once they have been picked up
- Fixed bee antennae and bunny ear shadows (they now attach to your helmet and animate as you move)
- Fixed a logic error with the tinnitus effect from a shotgun being fired nearby
- Fixed some enemy variables not resetting when you quit mid-day and rehost
  - Fixes hoarder bugs aggroing automatically without stealing items from them
  - Fixes baboon hawks trying to reach an inaccessible nesting point
- Mimic fixes
  - Mimics stop moving on the map screen after they die
  - Mimics imitate player appearance much closer
    - Badges now update to match the player they converted (Intern, Employee, Leader, etc.)
	- Costume attachments (like from bee and bunny suits) now appear properly
    - Tragedy masks will no longer turn into Comedy when it attaches to your face
    - Tragedy mimics now actually wear Tragedy (previously, they would wear Comedy, but make Tragedy's crying noises)
- Fixed whoopie cushion displaying a red box on the scrap collection screen
- Fixed snare fleas and tulip snakes opening doors while attached to a player's head
# v1.3.1
- Added a config setting to patch the jump cheese for eyeless dogs
- Fixed eyeless dogs killing you through the ship walls
  - Right now, only applies while the door is closed
- Some nutcracker fixes
  - Fixed nutcracker tiptoe for clients (in case you aren't using [LethalFixes](https://thunderstore.io/c/lethal-company/p/Dev1A3/LethalFixes/) already)
  - Nutcrackers tiptoe after 2 shots at any player (previously 2 shots for host, 3 shots for all other players)
  - Fixed nutcrackers not retaliating against players when taking damage if they finish reloading and no players are in sight
- The shotgun can now only hit a maximum of 10 enemies in a single shot (vanilla limit)
  - It will still scan for 50 targets to prevent 1 monster from taking up multiple "slots"
  - If 11 or more enemies were registered, only the nearest 10 will be damaged
  - Invincible enemies are de-prioritized, so Jesters, Coil-heads, etc. won't block damaging other nearby enemies
- Mod compatibility fixes
  - Apparatus scan text should have better compatibility with mods that change its value
  - Potentially fixed a crash with model replacements
# v1.3.0
- Added a config setting to enable mask hornets taking up power level (unused in vanilla)
- Fixed "CRITICAL INJURY" text popping up on HUD sometimes when you aren't actually critically injured (limping, unable to sprint)
- Restored the effect from v49 where blood fills your visor when a masked is vomiting blood into it
- Fixed bracken aggroing on players when shot by a nutcracker
- Fixed some items making noise across the entire map when dropped
- Fixed your own rank/beta badges being visible when reeling up a shovel
- Fixed Old Birds stomping players through the ship walls
- Corrected "Apparatice" typo on scanner
# v1.2.3
- Shotgun damage fixes (inspired by [NutcrackerFixes](https://thunderstore.io/c/lethal-company/p/Zaggy1024/NutcrackerFixes/)
  - Increased the number of registered colliders from 10 to 50
  - Fixed the same enemy receiving damage multiple times from one shot
  - Fixed error when nutcracker shoots a spider
- The casualties/fines screen now shows the proper fee percentage
# v1.2.2
- Tooltip patch is safer for better compatibility with modded items
# v1.2.1
- Hotfix for dropship saving and terminal patch
# v1.2.0
- Dropship inventory is now remembered when reloading your save
- Fixed item conductivity (configurable)
- Fixed TZP effects persisting after you are fired or change save files
- Fixed shotgun visuals
- Fixed inspectability for certain items (extension ladders no longer clip into the camera)
- Fixed inspectable items not having the inspect tooltip
- Bestiary fixes
# v1.1.0
- Improved physics when using a jetpack while tulip snakes are riding you
- Fixed boombox pitch staying wrong if you recharge it on low battery
- Fixed dropped butler knives not showing "Value: $35" until reloading your save
- Fixed Doppler effect still applying to the jetpack when you are the one flying it
- Added a config setting to disable/reduce the Doppler effect for music players
- Added a config setting for the unused resolution quality settings
# v1.0.2
- [Fast Climbing](https://thunderstore.io/c/lethal-company/p/Inoyu/Fast_Climbing/) and [BetterLadders](https://thunderstore.io/c/lethal-company/p/e3s1/BetterLadders/) compatibility
- Now hides "fake helmet" shadow
# v1.0.1
- Eclipsed Rend hotfix
# v1.0.0
- Initial release