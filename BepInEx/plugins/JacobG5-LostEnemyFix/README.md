![AAAAAAA ERRORS!!!!](https://i.imgur.com/ZXNPXMS.png)

# Lost Enemy Fix
This mod throws more meaningful errors when an EnemyAi fails to path on Navmesh and kills enemies that throw too many of these errors.

If you play with modded moons, enemies, or interiors. You may have at some point experienced:
 
`[Error  : Unity Log] "SetDestination" can only be called on an active agent that has been placed on a NavMesh.`

This error can be thrown for several reasons, making it sometimes hard to track the exact source. This could be from a modded enemy being set up wrong, incorrectly placed AI nodes, or blocked navmesh in any modded interior or moon. When this error is thrown this mod will additionally log the EnemyType, position, target destination, enemy behavior state, and if it is outside or inside the facility.

![Giant Deleted](https://i.imgur.com/N2NR2wv.gif)

## The Fix

In order to fix this lag and console spawn this mod will kill enemies that throw this particular error.

This is configurable:

`Aggressive` Kills an enemy after it has thrown ONE SetDestination Error.

`Reasonable` *(Default)* Kills an enemy after it has thrown several SetDestination Errors.

`Off` Leaves Vanilla behavior. (Console will be spammed)

### With This Mod: (Aggressive Setting)
![One Error And Cleanup](https://i.imgur.com/qr7AH1W.png)

### Without This Mod:
![Many Errors](https://i.imgur.com/ddwEQji.png)

and it keeps going...

### Note:
This mod replaces the call to an EnemyAI's Agent with a custom method.
If the vanilla error persists creating lag, the culprit is likely a modded enemy that overrides or completely replaces the navigation method of the vanilla EnemyAI. This mod will fix all vanilla enemies and modded enemies that inherit from the vanilla EnemyAI.

## Credits
Programming by JacobG5 (Me)

Nikki - Paid me to make this. & made icons.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/C0C810N5LV)