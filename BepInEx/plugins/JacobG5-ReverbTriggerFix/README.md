# This is an experimental release and may have problems!
If this mod provides a significant enough performance lift I will continue to update it.

If it's negligible I will probably deprecate it.

## What does this do?
In a similar vain to [VanillaMoonsLagFix](https://thunderstore.io/c/lethal-company/p/EugeneWWolf/VanillaMoonsLagFix) I am making changes to reverb triggers in hopes of performance improvement. 

[VanillaMoonsLagFix](https://thunderstore.io/c/lethal-company/p/EugeneWWolf/VanillaMoonsLagFix) works by completely disabling many of the reverb triggers on Artifice, Rend, Dine, and March.

This works because the reverb triggers in Lethal Company do a lot of checks on every object within their bounds every frame to test if they're something they need to interact with. This also means on maps like Artiface the game spends every single frame checking everything inside the bounds of all the triggers. Every stair step, railing, building, door, switch, EVERYTHING is having these checks run on it every game tick.

Rather than disabling unnecessary reverb triggers, this mod changes their exclusion layer to everything but Players, Enemies, and PlayerRagdolls. (Those are the only things the triggers interact with in vanilla.) By doing this the game no longer wastes resources calculating things on the terrain and map props and only checks when something it needs to interact with is within its bounds.

This method has the added benefit of not removing map sound cues and still applies reverb changes for entering/exiting parts of the map like buildings or garages. It also should inherently be compatible with all modded moons. It will patch all reverb triggers in a level after the dungeon generation finishes.

## AudioReverbPresets
Whenever the game needs to reference AudioReverbPresets it does so by running `UnityEngine.Object.FindObjectOfType<AudioReverbPresets>()`

This is a problem because that method searches every gameobject in the loaded scene tree to locate objects with the AudioReverbPresets script. 

This mod replaces most of the calls for that method with a call to a different method that saves that object to memory and returns it if it still exists. The AudioReverbPresets object is part of a level's scene tree so when loading a new scene it should notice the reference is invalid and save the new AudioReverbPresets object for future use over the course of the round.

## Experimental Feature (OnTriggerEnter)
While this is ***disabled by default***, I got curious about changing reverb triggers to only apply their checks when something enters their trigger colliders rather than checking everything inside of them every frame. On paper, this could help performance even further. In practice, I ran into some problems. That's why I've set it to an experimental toggle in the mod's config.

If you decide to enable this feature you will encounter some bugs. It's not game-breaking, but there will probably be some errors thrown in your logs with it enabled. 

The 0.3.0 update should increase stability with this feature enabled. I still want to caution it will probably have some issues.
