------------------------------------

Sky Reclamation Project (SRP) v1.1.4

------------------------------------


====================================

About:

====================================


The Sky Reclamation Project (SRP) is a community patch to address bugs that remain in S.T.A.L.K.E.R.: Clear Sky after the official patch v1.5.10. All original game content has been preserved wherever feasible. To ask a question or provide feedback, drop by the project discussion thread at the following URL:

https://www.gsc-game.com/index.php?t=community&s=forums&s_game_type=xr2&thm_page=1&thm_id=20140&page=1&sort=ASC&sec_id=22&lang=en


====================================

Is a new game required?

====================================


Yes, unless you are upgrading from SRP v1.1.3. This SRP release is compatible only with savegames created with SRP v1.1.3 or above.


====================================

Installation:

====================================


Before proceeding, ensure your game is patched to version 1.5.10. If you are unsure of this, launch the game and check the bottom left corner of the main menu. It should read: "ver. 1.5.10". Also, if playing the Steam version of the game, verify the integrity of your game cache before proceeding. Then:

1.) Paste the 'gamedata' folder from the root of the SRP archive into your game's root directory. The root directory is usually one of:

• C:\Program Files (x86)\Deep Silver\S.T.A.L.K.E.R. - Clear Sky\       (Retail version)
• C:\Program Files (x86)\Steam\steamapps\common\stalker clear sky\     (Steam version)
• C:\GOG Games\S.T.A.L.K.E.R. Clear Sky\                               (GOG version)

2.) Install any desired optional features by pasting into your game's root directory the contents of the folder named after the desired optional feature. For example, to install 'Alternative Ballistics', locate the 'Alternative Ballistics' folder and paste its contents — the 'gamedata' folder it contains — into your game's root directory. Overwrite any pre-existing files and folders when prompted.

To prevent conflicts, install any optional features desired from folder #1 before installing any from folder #2. The 'Prefilled Stashes' and 'Prefilled Randomized Stashes' features require a new game, but all other optional features can be installed at any point in the game. Note also that the 'Reduced Grenade Spam' feature will take full effect only after starting a new game, although it is safe to install at any time. Consult the documentation marked 'Optional Features' for information on each feature, including recommendations for players unsure of which features to use.


====================================

Uninstallation:

====================================


1.) Delete the 'gamedata' folder from your game's root directory.

2.) If you installed the optional 'Improved LuaJIT Library' and wish to remove it, navigate to the game's 'bin' folder and restore the original 'lua.JIT.1.1.4.dll' file from the 'SRP Original LuaJIT Backup' archive.

3.) If you installed the optional 'SweetFX v1.5.1' feature and wish to remove it, delete these files from the game's 'bin' folder: 'd3d9.dll', 'dxgi.dll', and 'injector.ini'. Then delete the following from the game's root directory: the 'SweetFX' folder, 'd3d9.fx', 'dxgi.fx', 'log.log', 'shader.fx', 'SweetFX_preset.txt', and 'SweetFX_settings.txt'.

4.) If you installed the optional 'User Configuration Patch' and wish to restore your pre-SRP user profile, navigate to your %PUBLIC%\Documents\STALKER-STCS\ directory, delete 'user.ltx', and reinstate the 'user.ltx.before_srp' file as your 'user.ltx' file by stripping away its '.before_srp' suffix.


====================================

Issues addressed:

====================================


Crash fixes:

+ Fixed instability and savegame corruption in Limansk.
+ Fixed occasional savegame corruption during the Fang basement mugging scene in the Garbage.
+ Fixed two task entity identifier leaks which could eventually destabilize the game.
+ Fixed a crash in Agroprom if Orest strays from his spot by the loner base window.
+ Fixed a crash in the Red Forest if the trader in the mine strays from his spot at the desk.
+ Fixed a crash in the Garbage if the player receives a task with Wild Napr as its target while the Flea Market is in combat.
+ Fixed a crash upon entering the Garbage if the player took Yoga's task to kill Stringov, accepted Stringov's bribe, left Stringov alive, finished the task while Yoga was offline, and did not loot Stringov's stash.
+ Fixed a crash in the Garbage if a bandit robber squad suddenly leaves for another camp during a hold-up.
+ Fixed a crash in the Garbage if the robbery scheme tries to assign the robber leader role to a mutant due to incorrect detection of squads belonging to a robbery camp.
+ Fixed a rare case of save corruption if the game attempts to load an NPC's logic before initializing the player.
+ Fixed potential crashing due to NPCs in some circumstances switching offline while their dialogue/trade/upgrade window is open.
+ Fixed potential crashing due to smart terrain overloading.
+ Fixed potential crashing during the marsh creature scene in Agroprom and in the Swamps.
+ Fixed several potential crashes caused by the game attempting to alter the attitude of a non-existing squad.
+ Fixed an occasional crash upon the game evaluating whether to assign the player a 'help' task.
+ Fixed several potential crashes caused by missing script logic sections.
+ Fixed several potential crashes caused by buggy dialog trees.
+ Fixed a potential Army Warehouses waypoint crash when mutants attack the military base.
+ Fixed a potential Cordon waypoint crash when an NPC enters the 'Bonfire in forest'.
+ Fixed a crash upon the game trying to assign a 'capture' task to a non-existing squad.
+ Fixed a crash upon attempting to load or delete an already deleted savegame.
+ Fixed a rare crash upon a squad capturing a smart terrain.
+ Fixed two rare crashes upon reloading a savegame.
+ Fixed a rare crash caused by a missing mesh.

Quest fixes:

+ Fixed Clear Sky's "Find a way to the Chernobyl NPP" task not completing.
+ Fixed the issue where any active 'defend' tasks would be cancelled upon loading a savegame.
+ Fixed the issue where the player could simultaneously pursue contradictory tasks for Yoga and Wild Napr.
+ Fixed Orest's tasks in Agroprom becoming available only on chance if the player kills the defensive bandit squad in the train tunnel before accepting Orest's request to do so.
+ Fixed Orest's "Destroy the mutant lair" task in Agroprom being activated only after the player has already killed most of the mutants that Orest assigned to be purged.
+ Fixed the issue where the "Receive the reward from Krylov" task in agroprom would not cancel if the player joins the bandits or Freedom.
+ Fixed the "Defend the stalkers in the anomalous area" task being received and immediately cancelled when the player completes the "Guard the stalkers on their way to the anomalous area" task in the Red Forest.
+ Fixed the issue where a generic 'capture' task directed toward the Devilish Encampment would be assigned simultaneously to the Red Forest task to "Guard the stalkers on their way to the anomalous area", which has the same objective.
+ Fixed the issue where failing or cancelling a 'return item' task at the Army Warehouses would make the task available again, yielding an exploit whereby the player could gain an indefinite supply of the requested item(s).
+ Fixed the Yantar "Help: Scientists' camp" task being received and immediately cancelled when the player attacks the scientists' camp.
+ Fixed the Yantar "Follow the stalker onto the hangar roof" task being completed rather than cancelled if the player does not get into position before the cooling device has been repaired.
+ Fixed Freedom's "Eliminate the potential threat at the gas station" task being cancelled when the player completes its objective.
+ Fixed Freedom's "Deliver ammo to the outpost" task being completed rather than cancelled when Chekhov informs the player that the outpost has been attacked.
+ Fixed Freedom's "Respond to the SOS signal" task being received and immediately failed whenever the player goes near the dead squad if the player initially fails the task.
+ Fixed Freedom's "Respond to the SOS signal" task being received and immediately completed after the player talks to the outpost commander if the player has already discovered the squad's fate.
+ Fixed Freedom's "Respond to the SOS signal" task sometimes failing to be assigned if the player enters the Dark Valley through the Cordon.
+ Fixed the issue where the player could bypass Freedom's "Respond to the SOS signal" task by leaving the Dark Valley before the Freedom outpost commander has finished speaking.
+ Fixed the Dark Valley task to "Find Freedom’s base" being received and immediately completed if the player has already found Freedom's base before the task becomes contemporary in the storyline.
+ Fixed the Dark Valley task to "Talk to the outpost commander" being received and immediately completed upon the player entering the Dark Valley if the player has already spoken to the outpost commander before receiving the task to find Fang.
+ Fixed Yar's 'Bring the component to the technician' task lacking a deadline despite the task briefing implying it needs to be completed before sunrise.
+ Fixed the issue where the player could delay reception of the Agroprom "Talk to the outpost commander" task (and cancellation of the "Find the stalker group’s stash" task) by bypassing its space restrictor.
+ Fixed the Limansk "Find the generator" task failing to complete when the player deactivates the generator if the player rushes to the apartment building and climbs onto the roof before the squad leader has finished the dialog which assigns the task.
+ Fixed the Limansk "Find the generator" task being received and immediately completed if the player initially bypasses its assigning space restrictor in the institute building but returns to it after deactivating the generator.
+ Fixed the Limansk "Return to the group commander" task failing to cancel when the player deactivates the generator if the player has not by then returned to speak with the squad commander.
+ Fixed the Limansk "Return to the group commander" task becoming available multiple times if the player moves outside of the squad commander's immediate proximity while he is speaking.
+ Fixed the Limansk "Destroy the machine gun nest" task being assigned to the player even if it has already been destroyed by the time the task would be contemporary.
+ Fixed an onslaught of tasks being suddenly received and completed in the Abandoned Hospital if the player kills the sniper earlier than intended.
+ Fixed the issue where the player could break the storyline at Agroprom by killing the Duty outpost commander while he is speaking or by leaving the map before he has finished.
+ Fixed the "Help the stalkers" task in Agroprom being cancelled immediately after being received if the loner faction is hostile to the player.
+ Fixed the storyline potentially breaking in saves created immediately after Sidorovich's first audio transmission to the player upon entering the Cordon.
+ Fixed the storyline breaking if the player kills every stalker in the Cordon stalker base before extracting the location of Sidorovich's loot from Khaletskiy, even after paying Sidorovich to set things right with the stalkers.
+ Fixed the storyline temporarily breaking if the player suppresses the Limansk military machine gun nest during the interval between receiving and completing the task to speak to the Clear Sky squad commander.
+ Fixed the storyline breaking if the player speaks to Forester before responding to the SOS signal in the Red Forest.
+ Fixed the issue where the dogs that spawn to attack Vasyan might fail to do so due to nearby NPC interference, hindering storyline progress.
+ Fixed the issue where the skirmish between the loners and military at the Cordon bus stop could begin prematurely, preventing the player from receiving the task to defend the loner patrol.
+ Fixed the issue where the dogs spawned for Wolf's "Help the stalker" task would not attack Drifter if the player picks up Sidorovich's loot before taking the task.
+ Fixed the issue where the player would in some circumstances fail to properly receive credit for killing the boars during the tutorial mission in the Swamp.
+ Fixed the issue where 'return item' tasks would sometimes be unavailable to the player when they should be available.
+ Fixed the issue where 'clear the road' tasks would sometimes get haphazardly cancelled or fail to be assigned when intended.
+ Fixed the issue where 'clear the road' tasks would get cancelled when they should register as complete.
+ Fixed the issue where 'capture' tasks would sometimes not register as complete or failed when they should.
+ Fixed the issue where 'capture' tasks would sometimes be offered by NPCs even for smart terrains that are already under attack or unreachable to them.
+ Fixed the issue where 'find upgrade' tasks would not cancel when they should.
+ Fixed several instances where a generic faction war task would fail when it should instead cancel.

Gameplay fixes:

+ Fixed erratic corpse cleanup behavior.
+ Fixed the broken artifact respawn system.
+ Fixed a range of NPC script logic errors.
+ Fixed a range of issues with the faction wars.
+ Fixed the buggy updating of NPC trade supplies.
+ Fixed a cover scheme bug that could make NPCs unresponsive.
+ Fixed corpse map spots haphazardly failing to appear on the minimap.
+ Fixed the issue where squads would sometimes fail to capture a camp upon reaching it.
+ Fixed the issue where squad NPCs could sometimes vanish right in front of the player.
+ Prevented NPCs dying of collision damage when spawning at the same spot as another NPC.
+ Fixed the issue where NPCs would sometimes perceive an enemy as a threat even after the enemy has been killed.
+ Fixed a range of circumstances in which Yoga's logic would break, causing all subsequent tasks from him to become unavailable.
+ Fixed the issue where Vasyan's logic could break, forcing the player to kill him to advance the storyline.
+ Fixed the issue where NPCs would sometimes fail to turn hostile or friendly to the player when they should.
+ Fixed the issue where the robbery scheme would remain active even for camps that the player has been tasked with assaulting or defending.
+ Fixed the issue where a squad NPC would not always be assigned the role of a guide when the relevant squad enters a camp for which a guide is suitable.
+ Fixed the issue where some factions would spawn well-equipped NPCs even before their resource level has increased by the amount intended as a prerequisite for doing so.
+ Fixed the issue where, upon leaving the Swamp for the first time, the player's relation to the Clear Sky faction would reset in its entirety instead of only in respect of that component of it which was yielded just by being a member of the faction.
+ Fixed a glitch which would allow the player to use a guide's services even if the player couldn't afford it, potentially leading to a situation where the player has negative money.
+ Fixed the issue where the Freedom base gate would open upon completion of the "Deliver ammo to the outpost" task instead of only after the player has found the active PDA on the dead blockpost commander's corpse, enabling the player to speak to Chekhov prematurely and break the storyline.
+ Fixed the issue where returning to the Swamps for the first time would not unlock the level changers to the Cordon if Clear Sky has regressed from total victory against the renegades, leaving the player locked into the Swamps without explanation until Clear Sky advances back to its final faction war tier.
+ Fixed the issue where the player's weapon would sometimes be intermittently holstered during a firefight at a faction base despite being an enemy to the current residents of the base.
+ Fixed the issue where the bandit base gate would get closed and locked when the base is assaulted even if not captured by bandits.
+ Fixed the issue where bandits would try to mug the player even if the player has joined their ranks.
+ Fixed the issue where the player could not drag and drop objects with the SEVA suit equipped.
+ Fixed the issue where important characters would not disappear when they are supposed to during a raid on their base either by the player or another faction.
+ Fixed the issue where Senka would occasionally rush out of the bandit base and get killed by enemies.
+ Fixed the script bugs causing the sudden unexplained deaths of Drifter and Hound.
+ Made some important characters invulnerable to prevent their accidental demise.
+ Fixed some groups of zombified stalkers using cover as if they were ordinary stalkers.
+ Fixed the bridge to Limansk in the Red Forest not aligning properly when lowered, which in rare cases would cause NPCs to never reach the other side.
+ Fixed the issue where the stalker squad overlooking the Vehicle Station in the Cordon would be blocked from raiding it with the player in exchange for payment until Valerian has tasked the player with assaulting it.
+ Fixed the Dark Valley mercenary base tunnel detonating (i) prematurely if the player wanders behind the deserted factory before receiving the task to purge the base; (ii) after it should have already gone out of commission if the player enters the relevant space restrictor for the first time only after the reward dialog with Chekhov.
+ Fixed the issues where the Dark Valley entrance hold-up (i) could occur prematurely if the player enters the Dark Valley before being tasked with chasing Fang there and (ii) would happen even after the player has reached Freedom's base if the player did not speak to the outpost commander before doing so.
+ Fixed the issue where the player's 'stashes found' statistic would rise even when emptying a stash box of items placed inside it by the player.
+ Fixed the exploit whereby the player could obtain multiple sets of stash coordinates from a corpse by re-checking it after leaving and re-entering the map wherein the corpse is located.
+ Fixed the Red Forest bridge lowering sequence becoming prematurely unlocked.
+ Fixed the issue where the stalker squad headed toward the Devilish Encampment in the Red Forest could, in rare circumstances, spawn right in front of the player.
+ Fixed the issue where the Witch Circle squad in the Red Forest would not necessarily turn hostile if the player kills the ambush squad traitor while he is still yelling for help.
+ Fixed the issue with the first Clear Sky 'return item' task where the Makarov PM on the soldier's corpse is not actually "modified" despite the task description clearly stating that it is.
+ Fixed the issue where submitting the item requested in a 'return item' task would not complete the task if the player possesses multiple units of the item when submitting it.
+ Fixed ten stash coordinates being unattainable due to programming mistakes. Most notably, Drifter now offers coordinates to a stash containing the third Cordon flash drive as a reward to the player for saving him from dogs.
+ Fixed faction reward tooltips failing to update to reflect new rewards after resuming progress from a savegame in which the player already has an outstanding reward from the relevant faction.
+ Fixed all issues where submitting a flash drive with upgrade schematics would unlock the wrong upgrade.
+ Fixed a script typo preventing the Lost Party's PDA from being transferred to Sakharov upon talking to him following completion of the task to retrieve it.
+ Fixed the issue where several varieties of weapon would not be properly identified as such when the player's inventory is checked for dialog availability purposes.
+ Fixed the issue where ammunition would not aggregate into full boxes in the inventory, making its transference to a container tedious and providing a profitable exploit for 'bring ammo' tasks.
+ Fixed the issue where non-scripted squads loaded from a savegame (as opposed to spawning into the Zone in the current game session) would not spawn inventory box items.
+ Fixed the wrong location-based multiplier being used to spawn faction equipment chest supplies for scripted squads loaded from a savegame (as opposed to spawning into the Zone in the current game session).
+ Fixed the issue where supply boxes on smart terrains controlled by online squads would generate more supplies with every game reload.
+ Fixed the issue where NPCs would drop the wrong type of ammo for some weapons.
+ Fixed mutants not behaving aggressively on patrol paths linking them to attack-targets unless aggravated by an external force (e.g. the player).
+ Fixed the issues where (i) Chekhov, Lingov, and Sakharov would not be marked as important characters on the map and (ii) the Duty outpost commander at Agroprom would be flagged as an important character even after he has become functionally generic.
+ Fixed the mechanic specialization tooltip displaying 'none' for Aydar, Yar, and Thunderov, despite all of them having a specialization.
+ Fixed the issue where squad info tooltips would fail to update properly and would, consequently, sometimes display the wrong target location.
+ Fixed several bugs pertaining to the displaying of squad map spots, including the issue where its color would react sluggishly to relationship changes to the player.
+ Mitigated the issue where the weather would sometimes inexplicably change after loading.
+ Fixed NPCs not settling into their sleeping animation at some sleep waypoints.
+ Fixed campfire NPCs sometimes not settling into their campfire idle animation.
+ Fixed sniper NPCs not settling back into their scan-for-targets state after an enemy detection timeout.
+ Fixed the start time for NPCs' heavily wounded state being saved incorrectly.
+ Fixed PSI emission hit and effector intensity doubling on save/reload.
+ Fixed the issue where crows could get stuck floating in the air upon being shot.
+ Fixed the "Life support system" upgrade for the Freedom Exoskeleton making the player bleed out faster rather than slower as intended.
+ Fixed a few instances of a mechanic not being able to upgrade a pre-upgraded variant of a weapon even if they could upgrade the base weapon.
+ Added the missing 'doesn't use shot' text to the threaded barrel upgrade tooltip for the Maverick 88.
+ Fixed the "Electronic stabilizer" upgrade for the SPAS-12 and Maverick 88 wrongly decrementing their ammo capacity by 2.
+ Fixed the "Relief backpack" upgrade for various armors wrongly incrementing the carry weight tooltip value by only 5kg instead of the 15kg actually unlocked by the upgrade.
+ Corrected the behavior of shot megaphones.
+ Fixed the issue where the player would be rejected from playing the shooting minigame if their money precisely matches the entry fee instead of exceeding it.
+ Fixed medicaments becoming more rather than less expensive at the Flea Market after liberating the concentration camp.
+ Replaced the generic masked face of the player's unarmored character model with Scar's face, as in the leather jacket armored character model.
+ Mitigated or fixed the player's character model reverting back to the default rookie jacket model upon picking up another suit or loading a savegame / changing maps, respectively.
+ Corrected the mesh, name, icon, and description of the several varieties of 7.62x54 mmR ammunition.
+ Extended GSC's implementation of rank-dependent NPC money from just Duty, Freedom, and the bandits, to all the game's factions.
+ Removed the out-of-place AK-74 from Scar's starting inventory which was introduced there by patch v1.5.09.
+ Deleted the duplicate supply box spawn at the Trailhead in the Swamp.
+ Moved the eastern Cordon-to-Garbage level changer in order to make the player less likely to accidentally walk into it.
+ Made both the inventory box in the Old Church at the Great Swamp and the downward-facing safe at the Yantar factory less tedious to access. Also spawned a wooden box underneath the former in order to prevent it from seeming to levitate.
+ Made each attribute bar length in the "Faction War" tab of the PDA reflect something sensible.
+ Made a few additional way-points available to NPCs that were not so due to bugs.
+ Made it possible to refuse payment to Garbage bandit robber squads via dialog.
+ Improved support for playing the game in a non-linear fashion.
+ Fixed the Abandoned Hospital not having a high-resolution map in the PDA.
+ Fixed a multitude of info portion and texture related console errors.
+ Fixed armor descriptions pertaining to artifact containers and upgrade possibilities.
+ Assigned unique names to some quest weapons and armors that were missing them.
+ Corrected several typos and standardized the formatting of all dialog, UI, and PDA message texts.

Dialog fixes:

+ Fixed the exploit with the Forester 'Compass' artifact submission dialog where the player could repeatedly break the dialog before being told the space anomaly coordinates and then re-enter it to receive the reward (a VSS "Vintorez") again and again an endless amount of times.
+ Fixed the following issues with the dialogue of the stalker squad overlooking the Vehicle Station at the Cordon: (i) the dialogue option to hire the squad would be available even without sufficient player funds, (ii) no money would actually be taken from the player when hiring the squad, (iii) the dialogue option to hire the squad would remain available even after the squad has already been hired, and (iv) the player could hire the squad even after already having dealt with the military presence at the Vehicle Station without the stalker squad's assistance.
+ Fixed the Uncle Yar dialog succeeding the completion of the night bloodsucker task where the player could reply to Yar's greeting only with a prompt "bye", making it impossible to e.g. submit flash drives to him.
+ Fixed the issues with the Professor Sakharov dialog where (i) he would ask the player to go see Lefty even after the player has restarted the cooling device, (ii) the player could ask for information about zombie attacks even after perpetually terminating them, and (iii) the player could ask about Lefty even before learning of him.
+ Fixed the issue where stationary squad commanders would claim hostiles are nearby when greeting the player even if only neutral/friendly factions occupy neighboring smart terrains.
+ Fixed the issue where the player could ask Major Zvyagintsev about Mitay even before learning of Mitay.
+ Fixed the issue where Sidorovich would answer only one question per game session after Scar returns him his case.
+ Fixed the issue where the player could not talk to NPCs previously involved in a hold-up.
+ Fixed the branching of some Duty member dialogs in Agroprom.
+ Fixed all buggy Cordon, Garbage, Yantar, Army Warehouses, and Limansk dialog trees.
+ Fixed all dialogue exploits made possible by the revocation of the player's ability to break out of certain dialogues being delayed.

Weapon fixes:

+ Fixed all inferable errors and inconsistencies in the weapon upgrade system.
+ Fixed the misaligned ironsight positions of all weapons in the game.
+ Synchronized the depth of field effect that occurs whenever a weapon is reloaded with each weapon's reload animation.
+ Synchronized the bore and reload sounds of all weapons in the game.
+ Added a sound for the second bore animation of the following weapons: G36, L85, LR-300, MP5, SG 550.

Graphical fixes:

+ Partly fixed the broken wet surfaces effect.
+ Fixed bullet tracers not being displayed in DX10/10.1 mode.
+ Made camo nets and fences visible on ATI/AMD based graphics cards.
+ Fixed the smoothing of the bridge to Limansk.
+ Replaced the inventory icon of the PM, PB, RPG-7, AKS-74U, and the exoskeleton to match their in-game appearance.
+ The correct HUD arm texture is now displayed for the Sunrise Suit, SEVA Suit, and the Bandit Jacket.
+ Fixed the issue where a squad commander icon would sometimes overlap with a guide icon, trader icon, or important character icon on the map.
+ Fixed the HUD bleeding icon being misaligned with its background in widescreen mode.
+ Fixed the misaligned border on secondary task map spots.
+ Fixed the incorrect 'important character' PDA map legend icon.
+ Fixed some NPCs having the wrong PDA message avatar.
+ Disabled the annoying, redundant flashing diskette icon appearing on screen every now and then.
+ Fixed the alignment of the off-center 'Game Over' text and accompanying flashing prompt in widescreen mode.
+ Fixed a few misaligned UI elements in the options menu.
+ Fixed all badly aligned weapon upgrade trees.

Audio fixes:

+ Fixed the issue where dynamic music would sometimes persist even after a battle is over and erratically fade in/out during a battle due to intermittent visibility loss.
+ Fixed the audio of an NPC's instrument-playing animation continuing to play even when the animation is interrupted by the NPC getting up intermittently.
+ Fixed the parting audio of an NPC playing prematurely upon entering the trade or upgrade screen with them.
+ Fixed the final portion of General Krylov's briefing dialog with the player being cut off following his walkie-talkie conversation with Sergeant Cheersov.
+ Fixed the issue where the player could rush out of Sakharov's bunker to meet Lefty before Sakharov has finished his first walkie-talkie conversation with him, thereby triggering a second transmission on top of the first one.
+ Fixed Father Valerian's invitation to join the stalkers playing on top of Sidorovich's 'thank you' audio upon returning the latter his case with the loot.
+ Fixed the issue where Sidorovich's voice could sometimes be randomly heard in the vicinity of the rookie village at the Cordon.
+ Fixed the issue where audible prompts from the squad commander could be heard during the Limansk square ambush even if the player is far away from the ambush location.
+ Fixed various audio transmissions to the player being initiated mid-sentence upon the player's arrival on a map.
+ Fixed the issue where a duplicate 'drop him' command would be issued by the commander of a Garbage exit bandit robber squad upon player non-cooperation.
+ Fixed the issue where a duplicate 'thank you' message would be played by the relevant squad leader in response to the player completing a 'capture', 'defend', or 'help' task.
+ Fixed the issue where the Freedom (/Duty) base megaphone would continue to play Freedom's (/Duty's) propaganda even after the base is no longer captured by Freedom (/Duty).
+ Made the Freedom base megaphone play Yar and Ashot's banter only when the player is in the vicinity of the Freedom base and not in a location where it can abruptly cut off immediately after it begins.
+ Fixed the issue where zombified stalkers would sometimes shout battle slogans as if they were ordinary stalkers.
+ Fixed the overlapping audio transmissions during the initial cutscene in the Abandoned Hospital.
+ Fixed Professor Beanpolev's overlapping greeting audio.
+ Fixed mercenaries' silent guitar playing around campfires.
+ Fixed some NPCs using the wrong voice files.
+ Fixed unlit campfires emitting a burning sound.

Other changes:

+ Restored some content left out of the game due to bugs and/or negligence (see changelog for details).
+ Added support for displaying location names on the world map.
+ Added a squad state indicator text to squad info tooltips on the world map.
+ Added the target camp owner name to 'capture' task dialog descriptions.
+ Added the target camp name to 'capture' task phase titles.
+ Enabled freeplay mode after finishing the main storyline.
+ Implemented level- and freeplay-specific autosaves.
+ Various optimizations.


====================================

Optional additional features:

====================================


• SweetFX
• Sleeping bag
• Deadlier weapons
• Smaller crosshair
• Real weapon names
• Feasible stealth
• Prefilled stashes
• No enemy map spots
• Ally map spots only
• Reduced grenade spam
• No weapon sway on strafe
• Easier Cordon machine gun
• Re-enabled pistol ironsights aiming
• NPCs do not toss weapons upon death
• Improved script engine performance
• Less frequent / disabled emissions
• Disabled developer startup videos
• Smaller inventory grids
• Transparent inventory


====================================

Advice / good to know:

====================================


• Frequently make hard-saves through the main menu and avoid relying on the quick-save feature — it is less reliable than hard-saving.

• A potentially more reliable alternative to the quick-save feature is to enter the main menu and press the 'S' key to create a quick named savegame from the currently active game session.

• Make a separate named savegame before entering Limansk; you will not be able to return to the earlier levels upon entering it until in freeplay mode.

• Keep the key bound to the 'use' command pressed down when approaching corpses to display the names of any tossed weapons in the vicinity.

• Double-click usable inventory items as a convenient shortcut to right-clicking them and selecting 'use this' from the droplist.

• Press the 'SHIFT' key as a convenient shortcut to take everything from a container or corpse when the inventory screen is open.

• Outside the PDA, press the key bound to the 'order to attack' command (default: 'K') to order a nearby friendly squad, currently on standby, to attack.

• Inside the PDA, press the key bound to the 'order to attack' command (default: 'K') to toggle displaying of location names on the world map.

• Unload the magazines of any weapons you have looted before selling them: contained ammo does not get factored into the selling price.

• Since SRP v1.0.4, saving the game refreshes the 'bring item' task available through any NPC set to offer such tasks for whom the player has not completed such a task during the preceding 24 game-hours.

• Hide/restore the HUD from the main menu using the 'F3'/'F4' keys, respectively. Scar will be impervious to damage and fatigue while the HUD is hidden, yielding a sort of 'god mode'.

• Quick-quit the game conveniently at any time by entering the main menu and then pressing the 'Q' key.


====================================

Troubleshooting:

====================================


Problems running the game? Ensure:

 • Your computer meets all the hardware requirements.
 • Your device drivers are up to date.
 • Your game is patched to version 1.5.10.
 • You have validated your game cache if running the Steam version of the game.
 • Your anti-virus software is not blocking the game from running.
 • You are running the game with administrator privileges. If you are not sure whether this is so, navigate to your game's root directory, open the 'bin' folder, right-click xrEngine.exe, and select 'Properties'. In the 'Compatibility' tab, check the box next to 'Run this program as an administrator', and then accept the changes. If this is not an option, refer to:

  https://www.gog.com/forum/stalker_series/how_do_you_run_the_game_without_admin_rights/post7

 • You have shut down all unnecessary applications before running the game. This includes monitoring utilities / overlays like MSI Afterburner and the Steam overlay.
 • You have installed the SRP correctly and are not running any other modifications --OR-- you are confident that your other modifications are merged correctly with the SRP and that they do not cause instability.

Unable to select DX10/10.1 mode in the graphics settings menu?

 • Uninstall SweetFX if you have it installed — it is known to disable DX10/10.1 support on some configurations.

Trying to run the game in DX10/10.1 mode? Getting intermittent freezes? Possible solutions:

 • Disable anti-aliasing in the game's graphics settings. It has been correlated to intermittent freezing in DX10/10.1 mode on Windows 7 64-bit with 'Update for Microsoft Windows (KB2670838)' installed.
 • Switch to DX9 mode.
 • Uninstall 'Update for Microsoft Windows (KB2670838)' if you have it installed — it is known to cause problems with the game. But beware that uninstalling it may have undesirable consequences for other applications on your PC. Research first.

Still have trouble?

 • Lower your graphical settings to the minimum, either from the main menu or manually via the user.ltx file located in your %PUBLIC%\Documents\STALKER-STCS\ folder. (See https://tweakguides.pcgamingwiki.com/ClearSky_7.html for details on the latter method.) If that helps, you can begin raising the settings one-by-one until you pin-point the problematic setting. Then simply use a value for it that works.

If the steps above do not resolve your issue, make a post on the official GSC forum, here: https://www.gsc-game.com/index.php?t=community&s=forums&s_game_type=xr2&sec_id=19. The forum members are very helpful and knowledgeable and will usually reply within a day or two. You can hasten the process by quoting the last few lines of your crash log if you have one - this will usually be located inside a compressed folder in %AppData%\XRay Engine\reports\ and will be named 'xray_<Yourname>.log'. You can also quote the lines between 'Error Reason:' and 'Registers:' in 'errorlog.log', located in the same folder.


====================================

Bugs still in the game:

====================================


• Strelok can fall off a platform at the NPP, making the game unfinishable.
• Emissions may rarely break active tasks and NPC logic.
• NPCs may occasionally get stuck in an unresponsive state. Save and reload to work around this.
• Artifacts sometimes glitch into terrain, making them unattainable.
• Weapon scope zoom upgrades are 'forgotten' when another upgrade is installed over them, or when the player reloads a savegame - the new scope zoom value does not persist.
• The AI of the military NPCs at the Cordon outpost sometimes becomes unresponsive.
• Ambient music sometimes cuts off or fails to loop until the player creates or loads a savegame.
• It is sometimes possible to talk to hostile NPCs.
• The reload animation for shotguns sometimes glitches and shows the wrong number of shells being loaded into the shotgun.
• The player's nightvision gets disabled when a new suit of armor enters the player's inventory.
• The player's character model briefly reverts back to the default leather jacket model upon picking up another suit. It returns to the correct model again a few frames later.
• Attempting to quit the game from the main menu can sometimes freeze the game on some hardware in DX10/10.1 mode.
• Controller psy-aura sounds playing before a savegame is loaded persist into that savegame. Restart the game before loading to work around this.
• Entries made to the PDA message log persist into a subsequently loaded savegame until overwritten by a new entry. Restart the game before loading to work around this.
• A squad NPC will issue squad audio prompts even if he is the sole member of the squad.
• Grenades sometimes become non-equippable. To work around this, drop one and pick it up again.
• Scar's avatar in the inventory screen may occasionally turn a red hue for no obvious reason. Restart the game to fix this.
• Forester's animation transitions are sometimes jerky.
• The trader in the Red Forest mine often levitates in the air beside his stool in a sitting position rather than being positioned on the stool itself. This is an SRP v1.0.4 regression.
• Upon entering the Dark Valley to find Fang and receiving the task to speak to the outpost commander, the mission marker on the map will always point to the north-western entrance of the Dark Valley, even if the player entered through the south-west and should therefore speak to the south-western commander.
• The emission timer text is wonky - the tooltip might display 5 hr. even when the map spot says that 21 minutes remain until an emission.
• Weapon attachment icons on primary weapons are misaligned in the inventory slot in widescreen mode.
• Graphical artifacts may appear when it rains. Restart the game to work around this.
• There are minor geometry glitches on some levels, e.g. floating reeds, trees, terrain objects, etc.
• The wet surfaces effect still does not work exactly as it should: when it is raining, (i) static stripes may appear on some surfaces (e.g. posters) fastened to an interior wall; (ii) rain may appear to pour down some interior walls; and (iii) grass / shrubbery may take on a metallic hue under some lighting conditions.
• Volumetric smoke may not appear properly or at all on some DX10-capable hardware.
• Skyboxes are visible through terrain when there is sufficient fog between the player and the terrain. The effect increases in prominence with fog density and the player's distance from the terrain.
• Hugging the wall next to Forester from the other side triggers his greeting audio due to an imprecisely aligned space restrictor.
• Attempting to exit the game while an NPC's death animation is in progress crashes the game:

  stack trace:

  0023:00000000 xrEngine.exe
  0023:06B4150B xrGame.dll, CxImage::`copy constructor closure'()
  0023:0041C7C6 xrEngine.exe, Feel::Touch::operator=()
  0023:0693A5D6 xrGame.dll
  0023:0693A905 xrGame.dll

  [error][       8]    : Not enough storage is available to process this command.

• Attempting to drop an item from a container or NPC inventory using the key bound to the 'drop' action (default: 'G') crashes the game:

  FATAL ERROR

  [error]Expression    : assertion failed
  [error]Function      : CUIActorMenu::SendEvent_Item_Drop
  [error]File          : E:\priquel\sources\engine\xrGame\ui\UIActorMenuInventory.cpp
  [error]Line          : 118
  [error]Description   : pItem->parent_id()==recipient

• At least one possible waypoint crash remains in the game:

  FATAL ERROR

  [error]Expression    : vertex || show_restrictions(m_object)
  [error]Function      : CPatrolPathManager::select_point
  [error]File          : E:\priquel\sources\engine\xrGame\patrol_path_manager.cpp
  [error]Line          : 155
  [error]Description   : any vertex in patrol path [red_smart_terrain_6_3_artefact_walker_1_walk] is inaccessible for object [sim_default_stalker_32778]

• Dying in an anomaly can occasionally crash the game:

  stack trace:

  0023:0603B4B0 xrGame.dll

  [error][       8]    : Not enough storage is available to process this command.

  Error Reason:
  ----------------------------------------
  xrEngine.exe caused ACCESS_VIOLATION in module "C:\Program Files (x86)\Deep Silver\S.T.A.L.K.E.R. - Clear Sky\bin\xrGame.dll" at 0023:0603B4B0, CDialogHolder::shedule_Scale()+2180672 byte(s)

  System Error:
  ----------------------------------------
  0x00000012 - There are no more files.


====================================

Credits:

====================================


 • Content contributions:

Alex Rinic, AMK Team, angrydog, Angus McFisticuffs, Anonymous, antifrost, Armada, Artos, Atempad,
b1ub4k, barin, BobBQ, burger, Canzah, castl, CeeJay.dk, Control volume, Danila_STALKER,
dDefinder, Decane, DerHeiligeApfel, DEXXX, Fangion, Gosuke, GSC Game World, IG2007,
InnerGround, jjwalker (Cameron Sneed), Kill_the_Strelok, Lebedev88, Lobstris, MacroN, Marked_2,
MrSeyker, notanumber (nandersen), NatVac, OGSM Team, olegj5, pavlov, PhoenixHeart, PYP,
Red7204, RoboMook, SetaKat (fluffy22), Shoker, smoq2, smrtphoneusr, SurDno, Tariq, Vandal,
vlad54rus, Xetrill

 • Useful feedback and testing:

100RadsBar, AR2R, Ceano, Charcharo, Compizfox, Crew 900, EliteHunter39, Firon, lowenz,
Marius Petran, motiv-8, Paul Jaye, RK Roadkill, Stryker7, Talrivian, TKGP, VicRattlehead