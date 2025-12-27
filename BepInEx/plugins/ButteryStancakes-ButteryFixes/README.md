# Buttery Fixes
A collection of miscellaneous vanilla-compatible bug fixes that were too small to release as individual mods.

## List of Changes
For a full list, please consult the [Changelog](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/ButteryFixes/changelog/) tab. Below is just a summary of the most important changes

<details>
<summary>General</summary>

**Host only**
- Fixed ordered items remaining inside the dropship after you are fired or the challenge moon resets, giving you a free "head start"
- The dropship's inventory will now be remembered when rehosting a save
  - Only applies if the file was both saved & loaded with this mod active
- Cruiser fixes
  - Fixed items being lost in orbit when dropped inside of an already magnetized Cruiser
  - Cruiser is lost when fired or between challenge moon attempts
- Fixed bee hives not randomizing their price correctly

**Client-side**
- Fixed music being permanently disabled (erroneously) under certain circumstances
- Fixed some v70 manor rooms not going dark when the breakers are turned off
- Ladder fixes
  - Stamina no longer drains if you try to sprint while climbing
  - You no longer climb slower/faster if you were moving up/down a slope
- "CRITICAL INJURY" popup on HUD now only displays when you have actually been critically injured (limping, unable to sprint)
- The endgame stats screen now shows the correct amount of scrap in the level
- The casualties/bodies recovered screen now displays accurate fee percentages
- Fixed scanning while driving the Cruiser
- Data chips will now disappear for all players after being picked up
- Fixed TZP effects and mineshaft echo persisting after you are fired or change save files

</details>

<details>
<summary>Entities</summary>

**Host only**
- Fixed Forest Keepers instantly chasing players on sight due to a logical error in their stealth mechanics
- Fixed Old Birds still spawning after all "dormant" Old Birds on the moon wake up (causing them to instantly appear in a random location)
- Fixed Old Birds not adding to outdoor power or their maximum spawn count (of 20) if they are woken up by unplugging the apparatus.
- Fixed the broken "global clock" for nutcrackers (they are now more likely to "inspect" in sync with each other)
- Fixed hoarding bugs and baboon hawks acting strangely if you disconnect mid-day and then host a game again
- Fixed bracken enraging on players immediately when shot by a nutcracker

**Client-side**
- Fixed Old Birds' stomps and dying Forest Keepers hurting you while you are inside the ship
- The Kidnapper Fox won't kill you in the ship, unless it has recently been attacked/stunned by a player
- Fixed slimes still dealing damage while "tamed" by a boombox if they haven't been "angered" by attacking them at least once
- Fixed eyeless dogs getting stuck in aggro when making a lot of noise in one spot
- Restored some missing text in the bestiary

</details>

<details>
<summary>Items</summary>

**Host only**
- Fixed conductivity across several items (toilet paper is no longer conductive, cookie mold pans are now conductive, etc. Configurable)

**Client-side**
- Flashlight fixes
  - Fixed multiple flashlights in your inventory preventing pocketed lights from shining
  - Fixed flashlights turning themselves on when stored with default keybinds
- Fixed certain items being audible when they hit the floor no matter where you are on the map
  - This affected large axles, plastic fish, easter eggs, bee hives, zap guns, sticky note, and clipboards
- Fixed kitchen knives not showing "Value: $35" on scan until the save file is reloaded
- Fixed whoopie cushions showing a red cube on the "Scrap collected" screen
- Fixed boombox pitch being incorrect if you charge it after it reaches low battery

</details>

## Config

### Compatibility
- `PatchLadders` - Whether or not to patch ladders, disable this if you use any mod that adds sprinting on ladders as a feature
  - [Fast Climbing](https://thunderstore.io/c/lethal-company/p/Inoyu/Fast_Climbing/), [BetterLaddersFixed](https://thunderstore.io/c/lethal-company/p/Lunxara/BetterLaddersFixed/), [BetterStamina](https://thunderstore.io/c/lethal-company/p/FlipMods/BetterStamina/), and [GeneralImprovements](https://thunderstore.io/c/lethal-company/p/ShaosilGaming/GeneralImprovements/) all offer this (and probably others)
- `AutoCollect` - When boarding the ship, all scrap in your inventory should display as collected on the HUD, not just the item you are currently holding. If you run into issues with inventory mods or item desync, turn this off and see if it makes a difference.
- `EndOrbitEarly` - Clients will end "ship phase" as soon as the lever is pulled, like the host.
  - In vanilla, this interaction is bugged and clients only end orbit phase after the ship's doors open.
  - This usually doesn't cause issues, but can have disastrous consequences for Sapsuckers (which become unable to damage clients) and eggs (which hatch instantly) under certain circumstances.
  - This setting might cause unexpected side effects for any potential mods that assume vanilla's behavior, but I think this is very unlikely to be the case.

<details>
<summary>Host only</summary>

- `RandomizeDefaultSeed` - Randomizes the seed when starting a new save file instead of always defaulting to 0. This will change starting weather, discounts, and decor rotation.
- `MakeConductive` - Disables non-conductive vanilla items being made conductive by this mod, if you are used to vanilla properties
- `FixGiantSight` - Fixes the bug with Forest Keeper line-of-sight that allows them to instantly chase players when spotting them, at any distance.
  - Their "memory" of players is meant to decay when that player is not visible, but due to a logical error, this only works if at least one other player is visible to the giant.
  - Even so, the latter usually doesn't work in vanilla, since their memory increases (past 100%) the entire time they are chasing you.
  - If you have [Fair Giants](https://thunderstore.io/c/lethal-company/p/LegoMaster3650/FairGiants/) installed for this purpose, they will both apply their effects, and giants will be "extra stupid." Use one or the other
- `MaskHornetsPower` - Enables mask hornets contributing 2 to the indoor power level. (This behavior is unused in vanilla due to their special spawn conditions)
  - Leaving this option disabled lets additional monsters spawn to replace dead butlers, like vanilla
- `FixJumpCheese` - Jumping/landing while moving near dogs alerts them, preventing an exploit where you can move past them silently at sprinting speed.
- `KeysAreScrap` - Keys can finally be sold for $3, but they get deleted if your entire team dies. **This also prevents belt bags from storing keys!**
- `FixHivePrices` - Bee hive prices finally randomize correctly (different hives cost different amounts)
- `UnlimitedOldBirds` - Disables both of the fixes made to Old Birds spawning, so it matches vanilla's behavior.
  - This allows Old Birds to continue spawning after all the ones present on the map have "woken up." This *will* cause them to appear out of thin air! (They do not have a proper spawning animation for this situation)
  - This also makes Old Birds that spawn from apparatus not add to power count or spawn caps, meaning they do not affect natural outdoor spawns.
- `LimitSpawnChance` - Prevents certain enemies with ramping spawn chances (baboon hawks, nutcrackers, mimics, etc.) from exceeding the max spawn weight and dominating enemy spawns.
  - For example, Rend already has nutcrackers set to 100 spawn weight (the "maximum" value for all vanilla levels)
  - However, nutcrackers gradually increase their spawn chances as more spawn (with 2 nutcrackers on the map, the 3rd has ~1.05x spawn chance, and so forth)
  - This multiplier allows nutcrackers to exceed 100 weight, which doesn't seem to be intended

</details>

<details>
<summary>Client-side</summary>

- `GameResolution` - Change game resolution (featuring "high" and "low" settings unused in vanilla)
  - Leave on `DontChange` for vanilla resolution, or automatic compatibility with other resolution mods
- `RestoreFilmGrain` - Restores the film grain effects from earlier versions of the game (seen in v4-v30)
  - `MenusOnly` only applies this to the title screen and pause menu
  - `Full` restores it for everything (SYSTEMS ONLINE, flashbangs, fear, etc.)
- `MusicDopplerLevel` - Reduce or entirely disable the pitch distortion of music players when moving around
- `ShowApparatusValue` - Replaces "???" text when scanning the apparatus with its actual value.
- `ScanImprovements` - Some miscellaneous improvements to the \"scan\" terminal command and radar.
  - When in orbit or at The Company, the scan will display the number of items you have on the ship and how much they total.
  - Fixed incorrect prices being displayed for apparatus, bee hives, shotguns, and kitchen knives.
  - Butlers' knives now display a scrap icon on the radar (and display their price in a terminal scan) before its owner is killed.
- `FixFireExits` - Rotates fire exit teleporters so you are always facing forward when using them.
- `LockInTerminal` - When using the terminal, you will no longer be able to move your head, and typing should be available with less delay.
  - This also locks the camera when charging items, pulling the ship's lever, or sitting in the armchair.
- `RestoreArtificeAmbience` - Restores Artifice's unused night-time ambience track.
  - It gets progressively louder as the clock approaches midnight.
  - The track is fully implemented and completely unique to Artifice, but does not play in-game due to a missing flag.
  - I am unsure if this was a mistake or done intentionally. But it sounds cool, so give it a try
- `DisableLODFade` - Disables LOD crossfade, which is broken in vanilla due to its visual style.
  - This does not completely prevent "pop in" when approaching objects, but does help minimize its frequency.
  - It now only happens once, where it used to happen twice
- `AlterBestiary` - Restores some removed text and corrects some typographical errors in bestiary entries.
- `AdjustCooldowns` - Increases cooldown on some items and interactable furniture for consistency and overlap prevention.
- `TheGoldenGoblet` - Renames "Golden cup" to "Golden goblet" :^)

</details>

## Recommendations
If you want a largely bug-free vanilla experience, I strongly suggest checking out all of the mods below (they all work great when used together):
- [Lobby Control](https://thunderstore.io/c/lethal-company/p/mattymatty/LobbyControl/) by [mattymatty](https://thunderstore.io/c/lethal-company/p/mattymatty/)
- [Additional Networking](https://thunderstore.io/c/lethal-company/p/mattymatty/AdditionalNetworking/) by [mattymatty](https://thunderstore.io/c/lethal-company/p/mattymatty/)
- [Matty's Fixes](https://thunderstore.io/c/lethal-company/p/mattymatty/Matty_Fixes/) by [mattymatty](https://thunderstore.io/c/lethal-company/p/mattymatty/)
- [LethalFixes](https://thunderstore.io/c/lethal-company/p/Dev1A3/LethalFixes/) by [1A3](https://thunderstore.io/c/lethal-company/p/Dev1A3/)
- [Pathfinding Lag Fix](https://thunderstore.io/c/lethal-company/p/Zaggy1024/PathfindingLagFix/) by [Zaggy1024](https://thunderstore.io/c/lethal-company/p/Zaggy1024/)
- [ReverbTriggerFix](https://thunderstore.io/c/lethal-company/p/JacobG5/ReverbTriggerFix/) by [JacobG5](https://thunderstore.io/c/lethal-company/p/JacobG5/)
- [Spider position fix](https://thunderstore.io/c/lethal-company/p/Fandovec03/SpiderPositionFix/) by [Fandovec03](https://thunderstore.io/c/lethal-company/p/Fandovec03/)
- [Melee Fixes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/MeleeFixes/) by me
- [Jetpack Fixes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/JetpackFixes/) by me
- [Enemy Sound Fixes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/EnemySoundFixes/) by me
- [Weed Killer Fixes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/WeedKillerFixes/) by me
- [Barber Fixes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/BarberFixes/) by me
- [Mask Fixes](https://thunderstore.io/c/lethal-company/p/ButteryStancakes/MaskFixes/) by me