## 2.0.4

* Fixed furniture not appearing when disabling furniture being always available.
* Fixed chairs being visually invisible.

## 2.0.3

* Migrated to use DawnLib.

## 2.0.2

* Updated to use latest netcode patcher.

## 2.0.1

* Fixed readme/description furniture listing, wtf did I do.

## 2.0.0

* Moved pocket rooms to its own mod (and improved how they work, and added more).
* Added 4 sittable chairs. Style toggleable in config.
* Added 3 more beds. All beds can now have style/type configured.
* Added 2 toggleable standing lamps.
* Added 1 floor piano that you can manually press or step on to play notes to impress yourself!
* Added 1 crib for people who want cozy place for the bAbIeS.
* Added 3 open-shelves. May add config to interchange with cabinets, workshops, etc.
* Walls, doors (and their different styles), and gates can now be interchanged between each other in config.
* Walls and doors can also have materials and shared material colors changed.
* Increased wall slots to 15.
* Slightly increased wall length.
* Added configs to enable/disable every individual grouping of furniture.
* Fixed moveable posters being invisible.
* Added example furniture images in description/readme.
* Added luck values to readme/description.
* Don't TLDR me istg

## 1.1.4

* Changed pocket room's teleport to custom script to break less.
* Fixed material change.

## 1.1.3

* Fixed issue preventing leaving moons.

## 1.1.2

* Fixed some storage furnitures not properly assigned network objects.
* Slight script and patching rework. Some patches no longer apply when certain furnitures are disabled.

## 1.1.1

* Added networking to sync item parenting in animated bed drawers (untested multiplayer).
* Changes to portable fire exit (untested multiplayer).
* Changed Filter0 to AC0 to prevent terminal command incompatibility.

## 1.1.0

* Added Speaker1 and Alarm0-3 moveable ship objects.
* Added Poster0-5 as moveable ship posters. Affected by ship poster-changing mods
* Slightly adjusted positions for moveable Screen0, and Speaker0.

## 1.0.1

* Potential fix for multiplayer fire exit bug when using buyable ship fire exit (untested multiplayer).
* Slightly adjusted moveable Screen0 position.

## 1.0.0

* Added buyable ability to move certain ship objects: charger coil, small screen above door panel, main speaker, and air filter.
* Migrated Item Furniture's aquarium to here.
* Set certain fire exit component to inactive when in orbit to combat frame drops when not landed (effectiveness untested).
* Changed fire exit type config to be more intuitive (and fixed incorrect labelling).

## 0.4.2

* Added outwardly facing collider to pocket room.
* Fixed being considered "left behind" when being inside pocket room while leaving a planet (tested).

## 0.4.1

* Added beehive minimum and maximum value config.
* Moved pocket room location from -100 to +150 height.

## 0.4.0

* Added "pocket room" door teleport furniture item to prove glitch wrong. (Experimental and a little janky as of now! Can be disabled. Cannot normally bring ship furniture inside it unless using mods like FurnitureLock.)
* Added more detailed README/description.
* Shortened furniture names for less conflicting/convoluted buying.

## 0.3.2

* Fixed default starting chance for presents spawning under the tree without ornaments, being 56% chance per hour.
* Lowered default ornament influence from +8% to +5%.

## 0.3.1

* Fixed XMAS tree to ACTUALLY spawn presents based on how many items are decorating it (was broken since day 1).

## 0.3.0

* Added XMASTree0 with configurable chance to spawn presents on timed moons depending on how many items are placed on the tree.
* Migrated, optimized, and improved Fireplace0 and Counter0 from Item Furniture to here. Counter can now be opened and store items.
* Fixed config to change furniture store-type to add decor to shop rotation.

## 0.2.2

* Added config to change furniture store-type.
* Added config to disable walls (will do more lAtEr).

## 0.2.1

* Changed tree and fern foliage textures to be double-sided.
* Fixed fern LoD distance.
* Fixed client desync causing duplicate bee hives on trees

## 0.2.0

* Added outdoor tree furniture with configurable percent chance to spawn beehives randomly when landed on non-company moon (4 spawnpoints per tree).
* Added outdoor bench table.
* Added potted ferns (subject to change, more to come!)
* Added config option for portable fire exit to choose between one-way only enter, only exit, or both (works as fully normal fire exit).
* Improved twin bed's drawers to open further, and to parent items into the animated part (items move with the drawer!)
* ID correction for certain furniture items.
* Fixed wider cabinet not spawning inside the ship for non-wider ships.

## 0.1.2

* Re-added fire exit unlockable registry.

## 0.1.1

* Removed experimental furniture duplication system (caused major furniture bugs with not loading furniture for clients).

## 0.1.0

* Added working fire exit as a furniture item (only works on next landing after buying, not during. Can be disabled in config)
* Added twin bed with side cabinets.
* Added sectionable walls as furniture items.
* Added 3 sectionable door variants as furniture items.
* Added experimental and currently buggy duplicate furniture item registry, including for vanilla items. Can be set in config. (Positions and rotations do not save on reload, partially works with FurnitureLock, do NOT change on an existing saves!)
* Added config options to customize prices for furniture items in this mod.
* Added v65+ luck values to furniture items.
* Moved changelog to its own section.

## 0.0.0

* Added Workshop station (Workshop1). Can be used to place items like the storage shelf, including 2-handed items. Items can also be placed on the wall.
* Added Work Table (WorkTable1). Basically the workshop station, but only the bottom part.
* Added Wide Cabinet (WideCabiner). Identical to the vanilla cabinet, except lime green, no doors, wider, and can store 2-handed items.
* Added Metal Gate (MetalGate). This is just a wider version of the cruiser's back door, as a furniture item. Can be opened and closed.
