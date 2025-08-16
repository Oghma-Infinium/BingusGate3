
![](https://raw.githubusercontent.com/Oghma-Infinium/BingusGate3/refs/heads/main/images/Banner.png)

<p align="center">
  [ Installation |
  <a href="javascript:;">Gameplay Guide</a> |
  <a href="https://github.com/Oghma-Infinium/BingusGate3/blob/main/CHANGELOG.md">Changelog</a> |
  <a href="https://loadorderlibrary.com/lists/bingus-gate-3">Load Order</a> |
  <a href="javascript:;">FAQ</a> |
  <a href="https://ko-fi.com/aljoxo">Ko-fi</a> | 
  <a href="https://www.patreon.com/aljoxo">Patreon</a> ]
</p>

---

**Modlist Support: [Waking Dreams](https://discord.gg/4WwqfK5yHg)**

<header>
    <h1>Contents</h1>
</header>

- [Introduction](#introduction)
  - [System Requirements](#system-requirements)
- [Installation](#installation)
  - [Pre-Installation](#pre-installation)
    - [Installing Microsoft Visual C++ and .NET](#installing-microsoft-visual-c-and-net)
    - [Pagefile and Crash Prevention](#pagefile-and-crash-prevention)
    - [Setting Shader Cache Size (NVIDIA Users Only)](#setting-shader-cache-size-nvidia-users-only)
    - [Obtaining the Game](#obtaining-the-game)
    - [Reinstalling Baldur's Gate 3](#reinstalling-baldurs-gate-3)
      - [Additional Steam Setup](#additional-steam-setup)
      - [Additional GoG Setup](#additional-gog-setup)
  - [Wabbajack Installation](#wabbajack-installation)
    - [Installing Wabbajack](#installing-wabbajack)
    - [Downloading and Installing Bingus Gate 3](#downloading-and-installing-bingus-gate-3)
  - [Problems with installation](#problems-with-installation)
- [Post-Installation and Optional Setup](#post-installation-and-optional-setup)
  - [Antivirus Exceptions](#antivirus-exceptions)
  - [Post-Installation Issues and Troubleshooting](#post-installation-issues-and-troubleshooting)
- [Playing the List](#playing-the-list)
  - [Before Starting a New Campaign](#before-starting-a-new-campaign)
  - [Starting a New Campaign and Difficulty Settings](#starting-a-new-campaign-and-difficulty-settings)
  - [Starting a Multiplayer Campaign](#starting-a-multiplayer-campaign)
- [Updating the modlist](#updating-the-modlist)
- [Removing the Modlist](#removing-the-modlist)
- [Issues](#issues)
- [Credits and Thanks](#credits-and-thanks)

# Introduction

Bingus Gate 3 is a modlist for Baldur's Gate 3 (who could have guessed). Bingus Gate 3 is built for **Patch 8** of Baldur's Gate 3.

A full list of the mods used in this modlist can be viewed [here](def).

You can find a summary of all relevant gameplay changes and notable mods on the [Gameplay Guide](def).

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg

## System Requirements

>[!WARNING]
>
>- An SSD is **required** to the play the modlist.
>- Only Windows 10 or 11 operating systems are supported. Windows LTSC, special variants, lightened editions or any other modified variant **WILL NOT WORK.** I am unsure at this time about Linux installations.

For system specs / hardware requirements, see the **Recommended** system requirements for Baldur's Gate 3.

Downloads Size: ~18 GB
Install Size: ~22 GB
Temporary Files: ???
**Total**: ~40 GB

# Installation

Installing Bingus Gate 3 is relatively easy and, if you have Nexus Premium, will be a simple waiting game. If you are updating the modlist, you can safely skip to the [updating section](#updating-the-modlist).

## Pre-Installation

These steps are only required for installing the modlist for the first time. Additionally, many of these steps may be covered in other modlist installs, for new users I suggest reading through here regardless.

### Installing Microsoft Visual C++ and .NET

 1. Install [Visual C++ x64](https://aka.ms/vs/17/release/vc_redist.x64.exe).
 2. Install [.NET Runtime 9.X.X Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/9.0).
 3. Install [.NET 6.0 Runtime Desktop x64](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-6.0.30-windows-x64-installer).

>[!WARNING]
>If you already have Visual C++ installed, please make sure you install it again and use the `Repair` option to get the latest version of the redistributables. **Do NOT skip this step or MO2 and the game may fail to launch.**

### Pagefile and Crash Prevention

>[!NOTE]
>While I am uncertain as of this time if pagefiles in Baldur's Gate 3 are as important as they are in modded Skyrim, I suggest setting one if you have the available space.

**To set up a Pagefile:**

 1. Press `Win Key + R`
 2. Type `sysdm.cpl ,3` and hit `ENTER`
 3. Navigate to **Performance** and click the box `Settings...`
 4. Click the **Advanced** tab at the top
 5. Under **Virtual Memory** click the box `Change...`
 6. Uncheck `Automatically Manage` if it is checked
 7. Select your disk drive, ideally your fastest solid state drive
 8. Click `Custom Size:`
 9. In the box next to **Initial Size (MB)**, type `20480`
 10. In the box next to **Maximum Size (MB)**, type `20480`
 11. Click `Set`.
 12. Click `OK`.
 13. Click `Apply`.
 14. Click `OK`.
 15. **Restart your PC**.

>[!TIP]
> Your pagefile does not need to be on the same drive as your Wabbajack install or Steam/GoG install of the game.

### Setting Shader Cache Size (NVIDIA Users Only)

>[!IMPORTANT]
>For NVIDIA users, it is recommended to boost the size of the shader cache. These settings have been shown to improve stability, while it may not be entirely necessary, it is still recommended.

**To do this:**

- Right-click on your desktop and select `NVIDIA Control Panel`
- Navigate and click `Manage 3D Settings`
- Scroll down the **Global Settings** tab until you see **Shader Cache Size**
- Double-click `Driver Default` to the right of **Shader Cache Size** and select `10 GB`
- Click `Apply` in the bottom right hand corner
- Exit out of the application
![](https://raw.githubusercontent.com/iAmMe27/Tahrovin/main/img/ShaderCache.png)

### Obtaining the Game

A legally obtained copy of Baldur's Gate 3 is required to play the modlist. While a Steam global copy is the safest, and what the list has been tested with, any copy of Baldur's Gate 3 should work.

### Reinstalling Baldur's Gate 3

It is highly recommended to have a clean installation of Baldur's Gate 3 before installing the modlist, this is to decrease the likelihood of any issues caused by unwanted or outdated `modsettings.lsx` or Mod.io subscriptions from previous playthroughs.

1. Cleaning the installation
 - **Option A**: **Nuke BG3**, unstall the game completely.
 - **Option B**: **Verify integrity of game files**, this will often remove non-vanilla files in the installation folder and will take a much shorter time.
2. Regardless of the option that was chosen above, navigate to your `%localappdata%\Larian Studios` folder and delete the `Baldur's Gate 3` folder.
 - This should take care of any errant files left over from previous playthroughs that could potentially cause issues with the list and is especially important for preventing data mismatches that will block multiplayer.
3. If installed previously, remove the BG3 Script Extender if it was previously installed manually (delete this file if it exists: `~\Baldurs Gate 3\Root\bin\DWrite.dll`). This should already have been removed if the installation was nuked.
4. After reinstalling, launch the game (vanilla from your app of choice) and reach the main menu once to generate all of the necessary folders and filepaths that MO2 and BG3MM require. When you reach the main menu, quit and continue this ReadMe.

#### Additional Steam Setup

>[!WARNING]
>If you have your Steam Library in Program Files, read [this article](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) by LostDragonist. Locations such as Desktop, Documents, Downloads, OneDrive, etc. *will* cause issues with installing and playing the list.

 1. Change Baldur's Gate 3 so it does not [automatically update](https://help.steampowered.com/en/faqs/view/71AB-698D-57EB-178C#disable).
 2. Right click on Baldur's Gate 3 and click on properties, untick the `Enable Steam Overlay while in-game.`.
 3. While in the properties, navigate to the Language tab and set the Language to `English`.

#### Additional GoG Setup

I do not have any experience with GoG at this time. I will flesh out this section in the future if required.

## Wabbajack Installation

### Installing Wabbajack

Once you have completed the pre-installation section, follow these steps to install Wabbajack:

1. Create an empty folder named `Wabbajack` on the root of your drive, such as `C:\Wabbajack` for example.
    > - **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), in your Skyrim's Steam folder, or in any folders related to the modlist itself (the downloads or install folder).**
    > - The `Wabbajack` folder does not need to be on an SSD, but it makes installing faster. You can set this location to be on an HDD for the sake of saving space.

2. Download the [latest version of Wabbajack](https://github.com/wabbajack-tools/wabbajack/releases/latest/download/Wabbajack.exe) and place the `Wabbajack.exe` file inside the Wabbajack folder you created in Step 1.

3. Double-click the `Wabbajack.exe` file that is now inside your Wabbajack folder to set up the program.

>[!IMPORTANT]
>The list requires Wabbajack version **4.0.0.0 or later**. Installing the modlist on older versions of Wabbajack will result in issues.

### Downloading and Installing Bingus Gate 3

>[!CAUTION]
>**A legal copy of Baldur's Gate 3 is required.** Pirated copies of the game will cause the installation to fail and even if you manage to somehow get around Wabbajack's built-in piracy prevention measures, BG3SE does not work with the cracked exes.  

Downloading and installing Bingus's Gate 3 can take a while depending on your internet connection, PC specs, and if you have Nexus Premium. Without Premium, you will need to manually click the **Slow Download** button for each mod.

To install Bingus Gate 3, complete the following steps.

 1. Download the `Bingus Gate 3.wabbajack` file from the pins in the **#bingusgate-general** channel of the [discord](https://discord.gg/4WwqfK5yHg).
 2. Place the downloaded file inside of the `downloaded_mod_lists` folder within your Wabbajack root folder (e.g., `C:\Wabbajack`).
 3. Open Wabbajack and click `Browse lists`.
 4. In the top right corner of the Wabbajack App, click `Install from disk`.
 5. Navigate to the `downloaded_mod_lists` folder and select `Bingus Gate 3.wabbajack`.
 6. Set the `Installation Location` to a folder such as `C:\BingusGate3`.
    > - **DO NOT place it in Program Files, User folders (such as Desktop, Documents, Downloads, OneDrive, etc.), or in your Baldur's Gate 3 Steam folder**
    > - The `Downloads Location` does not need to be on an SSD, but it makes installing faster. You can set this location to an HDD for the sake of saving space.
 7. Press the `Install` button.
 8. Turn on your favorite show or a nice long video essay as Wabbajack does its thing. Alternatively read through this readme again.
 9. If the installation is successful, then rejoice and move onto [post installation](#post-installation-and-optional-setup). If the installation is unsuccessful, follow the tips below or the [discord server](https://discord.gg/4WwqfK5yHg) for support.

## Problems with installation

It is possible that you may encounter an error with Wabbajack when installing. Some common issues are listed below.

<Details>
<summary>Wabbajack couldn't find my game folder!</summary>

Either buy the game or re-read the [Pre-Installation](#pre-installation) section.  

</Details>  

<Details>
<summary>My antivirus reports a virus with the program or modlist!</summary>

Windows 10/11 may automatically quarantine a key file which is needed for Mod Organizer. You can fix this by [adding an exclusion for Mod Organizer in windows defender](#antivirus-exceptions).  

</Details>

<Details>
<summary>Sanity check error extracting file:</summary>

Wabbajack will sometimes have issues extracting files if they use special characters. If you encounter this issue in a Wabbajack log, please try the steps down below:

 1. Press `Win Key + R`.
 2. Type `intl.cpl` and hit `ENTER`.
 3. Navigate to *Administrative* and click `Change system locale...`.
 4. Change the *Current system locale:* to `English (United Kingdom)`.
 5. **Uncheck** `Beta: Use Unicode UTF-8 for worldwide language support`
 6. Click `OK`
 7. **Restart your PC** and rerun the Wabbajack installer.

</Details>  

<Details>
<summary>Wabbajack is crashing during the installation!</summary>

If you find yourself struggling to run Wabbajack without it crashing, freezing up, or blue-screening your PC, please try lowering Wabbajack's resource usage with these steps:

 1. Open Wabbajack.
 2. Click the **Settings** button in the bottom left corner of the Wabbajack window.
 3. Under the **Performance** box, lower each number for each category to half of what it is currently set.
 4. Continue Installation.

>[!TIP]
> It is suggested to have a program installed on your PC that can open `.json` files, like [Notepad++](https://notepad-plus-plus.org/) or [Visual Studio Code](https://code.visualstudio.com/)

</Details>  

# Post-Installation and Optional Setup

## Antivirus Exceptions

>[!WARNING]
>Antivirus programs are notorious for false flagging [MO2's Virtual File System](https://stepmodifications.org/wiki/Guide:Mod_Organizer/Advanced), which can and will cause crashes and other problems. Antivirus programs like BitDefender, Norton, and Webroot are especially aggressive, and you will need to fully remove them from your PC in order to actually launch the game through MO2. It is 2024, Windows Defender and being smart online is more than adequate to protect yourself from malicious software.

If you use Windows Defender, it is advised that you set up an exception for the modlist.

<Details>
<summary>Setting up Windows Defender Exceptions:</summary>

 1. Press the Windows Key.
 2. Type "Windows Defender" in the search bar and select "Windows Security".
 3. Click on "Virus & threat protection" in the left pane.
 4. Click the "Manage settings" option under "Virus & threat protection settings".
 5. Scroll down to "Exclusions" and click "Add or remove exclusions".
 6. Windows Defender will prompt you with a run as administrator screen, just hit yes.
 7. Click the "Add an exclusion" button at the top and choose "Folder".
 8. Navigate to your Install folder for the list and click "Select Folder".
 9. **(OPTIONAL)** You can repeat these steps for the other executables:
    - ModOrganizer.exe (`[Path to Modlist]\ModOrganizer.exe`)

</Details>  

## Post-Installation Issues and Troubleshooting

TBD

# Playing the List

## Before Starting a New Campaign

 1. Head over to your modlist installation folder (e.g. `C:\BingusGate3`), locate an executable named `ModOrganizer.exe`, and launch it.
   >[!IMPORTANT]
   >If you installed Bingus Gate 3 to a **different storage device** than where you installed Baldur's Gate 3 itself and the game fails to launch, ensure that Root Builder is set to `Copy` and not `Link` (MO2 Puzzle Piece Icon > Root Builder > Root Builder).
 2. At the top right, you should be able to switch between the DX11 nad Vulkan version of the game. The DX11 version is suggested.
 3. Hit `Run` on the `Play Baldur's Gate 3` executable in MO2.
   >[!CAUTION]
   >**FOR THE LOVE OF AO, DO NOT CLICK THE UNLOCK BUTTON!**
 4. Once you have arrived to the Main Menu, verify all your mods have loaded by clicking on the `Mod Manager` button (under `Multiplayer`) and navigating to `Installed`. If you see a long list of mods (and `Memory Used` value ~20GB), then you should be good to go!
 5. Return to Main Menu and navigate to `Options` and then `Video` and ensure that your **Animation Level of Detail** is set to **High**.
   >[!WARNING]
   >You must change **Animation Level of Detail** to **High** in your `Video` settings, otherwise any heads added or changed by mods will suffer from visual bugs and animation issues. All other graphic settings can be adjusted according to your PC specs.

## Starting a New Campaign and Difficulty Settings

Please do not use existing campaigns on Bingus Gate 3, as you will likely encounter issues (or more likely won't be able to load them). When starting a new campaign, please utilize **Custom Difficulty** in order to have the intended experience, while **Honor Mode** should work fine, I do not recommend it for a modded playthrough.  

In order to have the appropriate and intended settings that the list was balanced for, please view the images below:

>[!NOTE]
>Remember to set the **Ruleset** to **Honour Ruleset**, this setting cannot be changed mid-campaign, and many combat-related settings will not work as intended without Honor Mode's changes to enemies, mechanics, and game rules.

![](https://raw.githubusercontent.com/Oghma-Infinium/BingusGate3/main/images/DifficultySettings.png)

The settings:
 - **Ruleset**: Honour Ruleset
 - **Single Save**: Disabled
 - **Enemy Aggression**: Tactician
 - **Character Power**: Tactician
 - **Enemy Loadouts**: Tactician
 - **Additional Combat Mechanics**: Tactician
 - **Proficiency Bonus**: 0
 - **Enemy Critical Hits**: Enabled
 - **No Death Saving Throws**: Disabled
 - **Disable Free First Strikes**: Enabled
 - **Camp Cost Multiplier**: 1.5 (Recommended 1.5 - 2.0)
 - **Short Rest Full Heal**: Disabled
 - **Trade Price Modifier**: 3 (Recommended 3.0 - 4.0)

The remaining settings (such as Multiclassing, etc.) can be set according to personal preference.

## Starting a Multiplayer Campaign

This section of the guide is ripped 1:1 from [Listonomicon's](https://www.nexusmods.com/baldursgate3/mods/15237) [install instructions](https://ajaxxxxxxxx.github.io/docs/1listo/Install/#13-multiplayer). This section of Listonomicon's install guide was originally written by Kmnder and edited by Ajax, I have tweaked it slightly for Bingus Gate 3.

>[!CAUTION]
>Failing to follow these instructions will lead to problems (e.g., Honor Mode ruleset not being applied, mod version mismatches, etc.) and you will not receive the intended experience.

 1. After installing Bingus Gate 3, if enabling custom or optional mods, the host should generate a fresh `ModsCache.json` and `ModSettings.lsx` and share it with all other players to guarantee BG3 loads the same mods, in the same order.  
     i. To generate a new `ModsCache.json` and `ModSettings.lsx`, navigate to the **Profiles** folder in your MO2 directory (e.g., `C:\BingusGate3\profiles`).  
     ii. Select the Mod Organizer 2 profile you intend to play multiplayer with (e.g., `Bingus Gate 3`).  
     iii. Delete the `ModsCache.json` and `ModSettings.lsx` files.  
     iv. After deleting these files, launch the game in order for a new set of files to be generated.  
 2. All players should start a new game with the same Custom Game rules as listed [above](#starting-a-new-campaign-and-difficulty-settings).
 3. The host should then create the real character that they intend to play while all other players should create a dummy character.  
     - For dummy characters, do not bother making any real choices as you will not be playing these characters. Simply click through character customization so that you can start on the Nautiloid.
 4. Once everyone has loaded into their game, the host should invite all other players. At this point, everyone (besides the host) should be prompted to make their real characters for the campaign.
 5. **When continuing a Multiplayer Campaign**, ensure that everyone (besides the host) loads into their dummy save. Once everyone has loaded in, the Host can then invite everyone to the same game.
     > Kmnder: "I've invited through clicking Multiplayer+ and then Steam inviting. But it has worked 100% of the time so far."

# Updating the modlist

Versioning for the list will adhere to the following format: `MAJOR.MINOR.PATCH`.

- `MAJOR`: Any release with a number change here will be considered a major update as at least 1 area of the list was massively overhauled. These updates with **NEVER** be save safe.
- `MINOR`: Any release with a number change here will be considered a minor update, these updates will **not** be save safe, unless otherwise specified.
- `PATCH`: Any release with a number change here will be considered a patch, these updates should be save safe and will be used primarily for bugfixes.
- In some rare cases, a fourth number will be used to designate a `HOTFIX`. These will only be utilized in cases where the list is recompiled with no other changes.

Updating is like installing the list. Simply make sure your paths are the same and tick the `overwrite installation` button. Please keep in mind any mods you have added will be deleted when updating. To make sure that Wabbajack does not delete your added mods upon updating, prefix your mods with `[NoDelete]`.

>[!IMPORTANT]
>Saves can be continued across **Save-Safe** updates. Updates will be indicated whether or not they are **Save-Safe** on the [Changelog](https://github.com/Oghma-Infinium/BingusGate3/blob/main/CHANGELOG.md). It is suggested that you backup your saves before updating if you plan on continuing them.

# Removing the Modlist

Simply delete the Bingus Gate 3 folder. Congratulations, you have uninstalled Bingus Gate 3.

# Issues

Please check the [FAQ](https://github.com/Oghma-Infinium/BingusGate3/blob/main/Documentation/FAQ.md) first if you have any issues.

# Credits and Thanks

- *YOU* for reading this.
- [Bingus](https://next.nexusmods.com/profile/bingusthecatto) for making the bulk of the baseline of the modlist.
- [aljo](https://next.nexusmods.com/profile/aljoxo) for configuring the gameplay portions of the modlist.
- [iAmMe27](https://ko-fi.com/iamme27) for general modding, documentation, and WJ assistance.
- The [Waking Dreams](https://discord.gg/4WwqfK5yHg) Helpers for their time and effort playtesting, providing feedback, and support assistance.
- Everyone who participates in playtesting and provides feedback during development builds.
- [JustThatKing](https://next.nexusmods.com/profile/JustThatKing), [jdsmith2816](https://next.nexusmods.com/profile/jdsmith2816/about-me), and [Total](https://github.com/NotTotal) for their feedback and assistance when I started modding.
- Bethesda Game Studios for Skyrim and the Creation Kit.
- [Halgari](https://www.nexusmods.com/skyrimspecialedition/users/17252164) and the WJ Team for the amazing platform that is Wabbajack.
- [Ajax](https://next.nexusmods.com/profile/Applejaxc) for [Listonomicon Again](https://www.nexusmods.com/baldursgate3/mods/15237) and the [Most Comprehensive Combat Extender Config for UNSO](https://www.nexusmods.com/baldursgate3/mods/15626), which this list is shamefully derivative of.
- [BaldursGoonsack](https://next.nexusmods.com/profile/BaldursGoonsack) and [Syrchalis](https://next.nexusmods.com/profile/Syrchalis) as their mods make up much of the core of the gameplay and rebalancing within the list.
- All other mod authors whose work is included, this list would not be possible without the greater modding community.
- Mgde12, D1Z4STR, 半蔵 内倉, Kepler, Hencoat, nostalgic.wave, EnragedHamster, unclemestor, snowpeachcherry, Charlie Kriech, Durgenage, Pacifist Fist, Don Maker, Russell Collins, Oresh, Danimals, Monko, Anehum, hildocean, The Unattested Wombat, Ola Nordman, Regista433, Jaron Scotland, King_Sheogorath, TheRyge, Shakes, highchae, Robbie, cowbellhero55, Geero, JAYDENCITO, Nehellena, Mysthey, Echo, Scott MacLeod, Exanima, Thundertube, LELUGOLELU, ravenlake, Paultinich, icaruscien, Oracraen, Lykk3, VillainousJ, Micheal Hamm, netwolff, Nico, G1Broheim, sweeper240, calcteacher, Ark, Zenity, Zolleu, medmen, jaimey19, Redwyne, Thrash Wizard, Baumalein, Serge, lorifey, TripleDoubleRuss0, De Wijswolf, FightForge, NaNo0408, DrukenReaps, Yunoronio, Diseenith, Adam Wasiura for support on [patreon](https://www.patreon.com/aljoxo).
- adorion1981, aexilkv, Alex H., AlphaGhost47, ambo, Ananta, annakins, Atlas, bigmact, Blade, BlueBeagle, Bubborus, Chef Nicnaq, Child_of_Sithis, Danimals, derbaer, derkaenaz, DevZan, Don Maker, doombot117, E2J, Elendil, EnragedHamster, FalseRealism, Felivath, Forsaken Jing, freshr, FutureWorld, Gous, Gremlin, hedich, Hencoat, Jeremy, Joey, JoeyFlow, JollyTheRancher, Julian, JXEYES, Kannon555, kanpeki, Kathie Murphy, Kiqing, Lunaros, Maelstrom, Makk, Mgde12, Mike, Modux, Monko, nana, Nehellena, netwolff, orca, paulogrupp, Psyguyy, Recklessness, rezthe0one, Rick, Roxiie, SaddestNoddles, shallow_green, skylion, SkullManEXE, Soloist, Steve, Stryn, Tamanaki, TazerReloaded, thefrogwithnoname, thepotion, Thomas Brack, Tom Curran, tyler, tyrotoxism, Victoriam, Won Pham, WoWZaton, Xtremza, Zhijia, and zidan for their support via [Ko-fi](https://ko-fi.com/aljoxo).
