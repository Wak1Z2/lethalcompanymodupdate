# v1.5.4
- Doppler effect fix now applies to spectating jetpacking players as well
# v1.5.3
- [Lobby Compatibility](https://thunderstore.io/c/lethal-company/p/BMX/LobbyCompatibility/) integration
# v1.5.2
- Fixed critical audio from [Jetpack Warning](https://thunderstore.io/c/lethal-company/p/Hamunii/JetpackWarning/) not playing
# v1.5.1
- Fixed the player being "dragged with the ship" if you fly away from it while it is landing
# v1.5.0
- Hopefully fixed the bug where the jetpack "drops inputs" when clicking (shakes the screen, but doesn't activate thruster)
- Fixed the jetpack's broken proximity warning (the beeping) logic
- Crashes at lethal speed now take into account modded HP values
# v1.4.5
- Fixed the jetpack exploding in mid-air if you are wearing a belt bag
# v1.4.4
- Reverted player collision change from v1.4.1
# v1.4.3
- Fixed a NullReferenceException when the jetpack explodes mid-flight
# v1.4.2
- Simplified some patches
# v1.4.1
- Minor refactor allowing players to crash into other players at high speeds
- Reduced how much vertical momentum is transferred when dropping the jetpack
- Some config fixes
# v1.4.0
- Added config setting to control when the jetpack explodes in mid-air from high speeds
  - Can be turned off completely
  - Can be enabled only at certain heights (new default, like "BecomeFirework" from v1.2)
  - Can be enabled always (like vanilla)
- Fixed several interactions between tulip snakes and jetpacks
  - Now tulip snakes flapping their wings won't spontaneously disable the jetpack
  - Tulip snakes will continue to move you if you turn the jetpack off while they are still flapping
- Added config setting that allows launching yourself by dropping the jetpack mid-flight.
# v1.3.0
- v56 compatibility
# v1.2.1
- Fixed jetpacks becoming unusable in v50
# v1.2.0
- Added "BecomeFirework" setting ;)
- Fixed the Doppler effect distorting the audio of your local jetpack
# v1.1.0
- Fixed the "inverted battery" bug (battery now only drains when the jetpack is turned on)
# v1.0.0
- Initial release