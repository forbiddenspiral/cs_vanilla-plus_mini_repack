# Changelog

v0.6 - 04/25/2024

- Gameplay Adjustments:
  - Restored default grid cell size to match vanilla game.
  - Reverted weapon names to vanilla.
  - Added Sleeping Bag feature: Allows players to sleep anywhere in the Zone using this item.
  - Increased vodka's radiation cure by ~40% based on user feedback.

v0.5 - 04/01/2024

- Weight and Movement:
  - Increased weight limit before fatigue from 30kg to 35kg (matches vanilla COP and offers a more vanilla gameplay experience).
  - Increased maximum weight for movement from 50kg to 60kg (aligns with vanilla values across all three STALKER games).
- Player Character Properties (Aligned with COP):
  - Matched the healing value to slightly restore health when injured using the value found in COP. This is for a more balanced approach across all three games.
  - Adjusted bleeding value to the more balanced level found in COP.
  - Wound healing rate when bleeding now aligns with the more balanced value from COP.

v0.4 - 03/18/2024

- Restored more vanilla behavior for medical items and food. Changes:
  - Using medical items no longer penalizes stamina.
  - Food no longer restores stamina.
- Made red hit marks invisible on HUD from mutants and NPCs (optional feature).
- Added to SRP Modifier a new configuration (disabled by default):
  - NPCs have the ability to turn off flashlights if they spot enemies.
- Enabled the previously mentioned ability for NPCs.

v0.3 - 03/11/2024

- Enabled moving faster through water (from (WIP) SRP v1.1.5).
- Improved inventory icon for medical supplies to look more like COP (from PRP).
- Fixed medkit revive functionality for downed NPCs.
  - Resolved an issue where medkits occasionally failed to revive downed NPCs.
  - This bug primarily affected non-critical gameplay but is now fixed.

v0.2 - 03/09/2024

- Updated mini-addon InGameSubs for SRP v1.1.4 to v0.3.

v0.1 - 03/02/2024

- Enabled no enemy map spots and showing only ally map spots.
- Enabled no intro movies.
- Enabled restoring pistol ironsights aiming.
- Enabled smaller inventory grids.
- Enabled no weapon sway on strafe.
- Enabled real weapon names.
- Enabled reasonable machine gun nest lethality.
- Enabled reduced grenade spam.
- Enabled user configuration patch.
- Enabled reduced head bobbing.
- Reduced max_item_mass (weight limit before fatigue) from 50kg to 30kg.
- Reduced max_walk_weight (maximum weight for movement) from 60kg to 50kg.
- Enabled stopping disk I/O icon from flashing at the lower right corner of the HUD.
- Enabled no enemy minimap spots.
- Hidden grenade indicator on HUD.
- Muted NPC detection sounds on PDA.
- Hidden NPC counter number on HUD.
- Hidden ammo counter on HUD.
- Hidden distance task counter on HUD.
- Made crosshair smaller.
- Removed some elements on minimap and HUD:
  - Minimap:
    - Direction of current objective.
    - Red hit shoot mark.
  - HUD:
    - NPC counter indicator.
- Disabled tagging NPCs through the binoculars.
- Disabled sound notification of detected NPCs through the binoculars.
- Tweaked SRP hide/restore HUD feature:
  - Disabled feature by default.
  - HUD instantly reappears in-game upon restoring, removing the need to return from the main menu.
  - HUD instantly disappears in-game upon hiding, removing the need to return from the main menu.
- Integrated SRP Modifier with basic functionalities:
  - Added ability to enable/disable HUD from the main menu.
  - Automated alife.ltx installation.
  - Implemented basic alife.ltx tweaks.
- Removed nightvision from suits with closed-cycle breathing system as in COP (only SEVA suit).
- Enabled ZRP flashlight beam.
- Fixed the scope (and binocular) views when running the game in 16:9 resolutions (included optional patch when running the game in DX10 and DX11).
- Implemented mini-addon InGameSubs for SRP (added subs and PDA messages to the English sounds used in-game that don't have).
- Removed 1s timeout effect to some PDA messages.
- Implemented Medicine Mod for SRP compatibility and addressed audio issues:
  - Adapted Medicine Mod for seamless integration with SRP.
  - Fixed minor audio inconsistencies related to consumable items.
  - Added long usage and sound effects for all consumable items.
- Fixed incorrect weapon animation when using the exoskeleton with the Gauss Rifle.
- Added optional LuaJIT library to improve performance.
- Updated inventory icon to exoskeleton (icon from COP).
- Allowed sprinting with SVD and RG-6 as in COP.
- Changed icon and message on PDA when an emission occurs.
- Improved inventory icons for some weapons (icons from PRP).
- Fixed Professor name inconsistency in CS text files. Changes Professor Beanpolev's name to Professor Kalancha in Clear Sky English text files for consistency with Call of Pripyat.
