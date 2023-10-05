# MO2077 - MO2 for Cyberpunk 2077, but not in the way you're thinking.
- [MO2 for Cyberpunk?](#MO2-for-Cyberpunk?)
- [Prove It](#proof)
- [Installation](#installation)
  - [Steam/GOG Config](#steam/gog-config)
  - [Disable Overlays](#disable-overlays)
  - [Change Update Behavior](#change-update-behavior)
  - [Using Wabbajack](#using-wabbajack)
  - [Preparations](#preparations)
  - [Downloading and Installing](#downloading-and-installing)
  - [Problems with Wabbajack](#problems-with-wabbajack)
  - [Post-Installation](#post-installation)
  - [Starting the Game](#starting-the-game)
- [Updating](#updating)
- [Manual Instructions soon?](#manual-instructions)
- [In-Game Configuration](#in-game-configuration)
- [FAQ](#faq)
- [Removing the Modlist](#removing-the-modlist)
- [Credits and Thanks](#credits-and-thanks)
- [Contact](#contact)
- [Contributing](#contributing)
- [Changelog](#changelog)

# MO2 for Cyberpunk? 
It works. Really*.

Mod Organizer 2 and Cyberpunk 2077 aren't normally compatible - using MO2 on the game leads to CET and Redscript errors. We've managed to address this through a plugin called Root Builder that allows specific folders to be automatically be copied into the game folders when launching the game, and be automatically cleaned up once the game closes.
Root builder requires a specific folder structure. The archive folder of mods is MO2 deploys via its VFS,  this works in 99% of cases for mods of this type.
The other folders are copied before runtime, namely: bin, engine, r6, red4ext and Redmods. This way your game folder remains intact when not run via MO2.
This means under all practical purposes, these mods are installed manually, but with the convenience of a mod manager. 

No found exceptions as of MO2077 v1.0.7...so that's nice, tell me if you find one.

# Proof

For now I have included a couple of mods in a "Proof this works" section. Please feel free to remove them if you wish, I will be removing them from the list once I feel that point has been made. 

I will not provide support on how to mod Cyberpunk, however I will answer questions explaining why this works where MO2 generally doesn't. 
Please seek general modding support in the numerous other places where people can teach more about modding. 

# Installation

This list assumes that you have a clean install of Cyberpunk 2077. There may be unintended issues if you have multiple mods either installed manually or deployed by Vortex.
Please delete manually added files & verify game integrity before installing. For Vortex, please purge the installed mods, you will be able to redeploy them later if you choose to. 

## Steam/Gog Config

### Disable any game Overlays

The Steam/GOG Overlay can cause issues with certain mods and is
recommended to be turned off.

Steam:
Open the Properties window (right click the game in your Library->Properties),
navigate to the _General_ tab and un-tick the _Enable the Steam Overlay while in-game_
checkbox.

GOG:
Open the settings window (Cog in the top left of GOG Galaxy),
navigate to the Game Features tab and un-tick the Overlay checkbox. 


## Change Steam/GOG's Update Behavior

Cyberpunk 2077 is still being updated by CDPR. Whenever the game updates, it's quite possible
that everything can break due to these changes.

Steam:
To ensure that Steam does not automatically update the game unless you want it to, head over
to the Properties window, navigate to the _Updates_ tab and change
_Automatic updates_ to _Only update this game when I launch it_.

GOG:
To ensure that GOG does not automatically update the game unless you want it to, head over
to the Settings window, navigate to the _Game Features_ tab and turn off the checkbox for
_Auto Update Games_.

## Using Wabbajack

### Preparations

Grab the latest release of Wabbajack from [here](https://www.nexusmods.com/site/mods/403) and place the `Wabbajack.exe`
file in `X:\Wabbajack`

### Downloading and Installing

The download and installation process depends on
your system specs. Wabbajack will calculate the amount of threads it will use at
the start of the installation.

To have the highest amount of threads and thus the fastest speed, it is advised
to have the working folder on an SSD, this doesn't matter a huge deal for the modlist itself however it will matter significantly more for playing the game. 

1. Open Wabbajack
2. Load the Modlist from either Browse Modlists (selecting the Cyberpunk 2077 dropdown and unoffical checkbox) or Install from Disk (if you have downloaded the list from elsewhere).
3. Set MO2077 to install to `X:\MO2077` and downloads to `X:\MO2077\Downloads`.
   You can set a different path if you wish, but avoid system protected folders. 
4. Click the Go/Begin button
5. Wait for Wabbajack to finish

### Problems with Wabbajack

There are a lot of different scenarios where Wabbajack will produce an error.
If you do not see an installation failed warning do not worry about it. If you
feel like wabbajack is stuck or a download is hanging just restart wabbajack,
it will pick up from exactly where you left off.

Please rerun wabbajack at least twice and try to manually download the file
from first before posting about a failed download.

**Could not download x**:

If a mod updated and the old files got deleted, it may be impossible to download
them. In this case just wait till I update the Modlist.

**Wabbajack could not find my game folder**:

You need to have launched the game once before WJ will locate it. Additionally
Wabbajack will not work with pirated versions of the game. The list works with games from Steam, GOG and Epic Game Store.

Support in [CDPR Modlists Discord](https://discord.gg/YE2VzkEwEj)

## Post-Installation

### Starting the Game

Head over to the installation folder and locate an executable named
ModOrganizer.exe and launch it. Once its launched there will be a dropdown box
on the top right and a big run button next to it.

Ensure it is set to `Cyberpunk 2077` by selecting it in the dropdown
box and then hitting the run button. Due to how it is deploying the files, you may have to click "Run" twice. This is normal. 

CET is bound to the ' key. You can change it from the menu once in game if you wish. 

# Updating

If this Modlist receives an update please check the Changelog before doing
anything. Always backup your saves or start a new game after updating.

**Wabbajack will delete all files that are not part of the Modlist when updating!**

This means that any additional mods you have installed on top of the Modlist
will be deleted. Your downloads folder will not be touched! That means if you have made your own modded setup on top of the list, you should update mods *manually*.

Updating is like installing. You only have to make sure that you select the same
path and tick the _overwrite existing Modlist_ button.

# Manual Instructions

Somewhen soon tm.

# In-Game Configuration

However you want to set bindings up. You will be prompted to choose a CET binding when you first launch the game. 

# FAQ

How do I update to a later version?

- All you have to do is rerun wabbajack with the new version of the installer.
  If you have the downloads wabbajack will hash everything, download any new mods,
  and make the necessary changes in your install folder. This will remove mods you have added yourself.

Is [insert mod name here] part of the list?

- Check the modlist manifest. If there is a utilitiy that you think should be in the list, ask nicely in the discord. Do not ping me or DM me with requests. 

Will you add x mod to the list?

- Maybe?

I think I found a bug! Here are some things that are not bugs:

- Thanks! Please let me know via the discord.

# Removing the Modlist

You can just remove the MO2 folder, along with any Game Folder file mod you've installed and be done with it.

# Credits and Thanks

MO2077 - made by:
- JTK

Special Thanks

- **_YOU_** for actually reading the readme.
- Xanza - For working out the initial Root Builder mapping and implementation
- Rfuzzo - For fixing CET to work nicely with MO2's UVFS
- Delta 
- brahmax 
- Crit

Mod Authors

- And of course, where would we be without awesome mod authors? Thank you
  all for releasing the quality content that you guys do.

  **_PLEASE DO NOT FORGET TO ENDORSE THE MOD AUTHORS!_**

# Contact

Contact me in the [CDPR Modlists Discord](https://discord.gg/YE2VzkEwEj)

**DO NOT DM ME ON DISCORD. I WILL NOT PROVIDE SUPPORT FOR YOU IN DMS**. I am available for support in the linked discord server. 

# Changelog

See [Changelog](CHANGELOG.md).
