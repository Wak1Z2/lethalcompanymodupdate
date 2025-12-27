# 1.1.0

- Updated to v73
- Removed staticnetcodelib dependency
- Added config to hide cursor when performance report is on screen

# 1.0.10

- Uploaded code to github

# 1.0.9

- Removed the staticnetcodelib dependency
- Added a config for avatars on the performance report
- Added Coroner support

# 1.0.8

- Removed LobbyCompatibility as a dependency
- Added BounceSmoothness config
- Updated DeathVoiceSensitivity to 10
- Updated BounceSmoothness to 12

# 1.0.7

- Removed LobbyCompatibility as a hard dependency

# 1.0.6

- Removed LethalCompany_InputUtils as a dependency

- Removed MoreCompany as a dependency

- Added LobbyCompatibility as a dependency

# 1.0.5

- Forgot to add some dependencies

# 1.0.4

**Bundle loading & cleanup**
- Call "bundle.Unload(false)" in "OnDestroy" to free memory.

**Shared frame‐end yield**
- Cache a single "WaitForEndOfFrame" instance for the end-screen coroutine instead of allocating a new one each loop.

**Object pooling for notes**
-  Use a "GetOrCreate" helper to reuse note UI objects (activate/deactivate) rather than destroy+instantiate on every update.

**Throttled death-screen updates**
-  Only run expensive logic in "DeathScreen.Update" every 0.1 s, and only recalc the grid layout when the number of boxes actually changes.

**Bulk avatar uploads**
-  Load Steam avatar data in one raw block ("LoadRawTextureData"), with a per-pixel fallback, then apply once—no pixel-by-pixel loops on the main thread.

**Added config for voice sensitivity**
-  Allow scaling the bounce animation in the death-screen UI via a configurable multiplier.

**AvatarTexture tracking**
-  Added a new "AvatarTexture" field to track the avatar texture for each spectator box, enabling cleanup when the box is removed.

**Cleanup on UI removal**
-  Updated "RemoveSpectateUI" to dispose of textures and reset layout data when the UI is cleared.

**Spectator box destruction**
-  Destroy associated textures whenever spectator boxes are removed and recalculate layout only when boxes change.

**Improved avatar loading**
-  Introduced "DestroySpectatorBox" and improved avatar loading to prefer raw data and minimize per‑pixel copying.

**Smoothing for avatar bounce**
- Avatars will now bounce more smoothly


# 1.0.3

- Added death spectating UI
- Added names under the profile pictures
- Added config for disabling/enabling performance report fix, death spectating UI, and text under the profile image

# 1.0.2

- Removed "Some of the equippable items" from the planned list in the readme
- Added "Remove the not needed assets in the asset bundle" to the planned list in readme

# 1.0.1

- Removed Coroner as a dependency