## Nutcracker Massacre Crosshair

very small mod that implements the custom crosshair i made for my unreleased Nutcracker Massacre mod. the crosshair is a simple unity ui sprite that i stole from the in-game assets (as shown in the mod icon) and changes color depending on what you're looking at. if anything goes wrong ping me in the [Unofficial Lethal Company Community](https://discord.gg/nYcQFEpXfU) or DM me on discord `@swaggies`.

### Colors
| Color | Description |
| :---: | :---------: |
| Green | Grabbable object (items and scrap) |
| Aqua | Interactable object (such as the ship lever) |
| Dark Aqua | Disabled interactable object (such as a locked door) |
| Red | Killable enemy |
| Dark Red | Invinicible enemy |
| Gray | surface within reach distance |
| White | default color |

*please note that the red highlighting doesnt indicate that you can reach the enemy with a weapon, it only means the enemy is within your grabbing distance*

### Tooltips
in the mod's config you can enable custom tooltips which overwrites and colors the little text that appears under your crosshair based on context. by default this is off.
- for items and scrap, it will show the item's name, scrap value (if available), current battery charge (if available), and current ammo stock for shotguns.
- for interactable objects, most of them are just their default tooltips but some common ones have been modified:
  - for the ship lever, it will display what moon you are landing on while in orbit. on a moon, it will show a timer indicating when the ship will leave automatically.
  - for the terminal, the amount of credits you have will be shown.
  - for entrances/exits, the "near activity detected" indicator will now show up more reliably, and can now detect outdoor enemies from inside as well.
- for enemies, it will show the enemies name (ONLY IF you are able to scan the enemy), and how much health it has.
  - keep in mind health may be desynced depending on who's host or the owner of the enemy. it hasnt been too bad in my experience but it can definitely happen.
  - some invincibile enemies may show health since they are marked as "can die" in the games code

tooltips that provide an advantage over vanilla clients (such as showing enemy HP) can be disabled by changing the "Enable CSA Tooltips" option in the config.

### Compatibility
should support every version of lethal from 35 onward. completely client-sided. this will *potentially* conflict with mods that change the crosshair but will likely overwrite it and should be generally fine, idk though i havent tested. :3