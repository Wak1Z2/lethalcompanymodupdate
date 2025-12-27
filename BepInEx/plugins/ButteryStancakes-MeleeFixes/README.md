# Melee Fixes
Fixes bugs with the shovel, kitchen knife, and shotgun:
- Fixed shovel sometimes becoming unusable if a player died while holding it mid-swing.
- Fixed hit effects (shovel bounce, knife blood spray) sometimes playing even if your swing misses, providing poor feedback.
- Whenever a melee weapon plays a hit sound, it calls an expensive search function that can cause lag or frame drops on less powerful computers.
  - It now references a cached instance of the required object, which should help combat remain more smooth and fluid.
- [Damage should now be handled more consistently when firing the shotgun at multiple enemies](https://thunderstore.io/c/lethal-company/p/Zaggy1024/NutcrackerFixes/)
- Fixed duration of ear-ringing effect when a shotgun is shot in point-blank range (usually, because you are the one holding it)