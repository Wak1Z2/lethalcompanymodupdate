### v0.0.2
- Added configs options
    - You can set any of these config options to true to turn on this mod's potential fixes, set any option to false to make this mod not interfere.
    - The only tweaks turned off by default are the isEditor globalTimeSpeedMultiplier toggle, to prevent potential desyncs or cheating, and the ModelReplacementAPI's first-person arm-jitter, since this should now be fixed by the mod itself, I believe.
- Fixes:
    - The ship's monitor will now correctly draw a line from the watched player to the mineshaft elevator button if they're underground
    - The spectate camera's flashlight available through SpectateEnemies will no longer have a cookie, preventing the debug console errors and other flashlights not properly turning on
- Changes:
    - The Landmines' new AudioSource now uses the AudioMixerGroup of the original AudioSource, dunno what changes but can't hurt right
    - Moved the list of tweaks from the ReadMe to the Wiki's List of Fixes page
- Updated dependency on BepInExPack to v5.4.2304

### v0.0.1
- First upload, including the Wiki's Artifice disabled AudioSource, Landmines audio spatializer, Spike Traps null AudioClip, isEditor globalTimeSpeedMultiplier, playDelayedMusicCoroutine, AnimatedObjectTrigger null-check, and ModelReplacementAPI's first-person arm-jitter