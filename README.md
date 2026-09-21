# Pac-Man World 2: Re-PAC Archipelago

## Requirements
* Legitimate Steam copy of Pac-Man World 2: Re-PAC on PC
  * We are only supporting the most current game version; if you've downpatched your game, you may encounter problems until you revert to the latest patch
* MelonLoader Installer **v4.3.0**: https://melonwiki.xyz/#/README
* Latest release of PMW2RPArchipelagoClientMod
* Archipelago MultiClient .NET 6.7.1: https://github.com/ArchipelagoMW/Archipelago.MultiClient.Net/releases/tag/v6.7.1
* **For seed and options generation:** Latest release of the PMW2RP APWorld
* **Optional**: Archipelago Launcher: https://archipelago.gg/tutorial/Archipelago/setup_en
  * Currently, you will not be alerted in-game when you receive items. I strongly recommended connecting with a Text Client alongside the game to keep track of what is happening in your multiworld

## Getting Started (Setup)
### 1. Melon/Mod Installation
* Launch the MelonLoader Installer and use it to install MelonLoader to Pac-Man World 2: Re-PAC. Select MelonLoader v0.7.3.
* Navigate to the game install directory. Place **PMW2RPArchipelagoClientMod.dll** into the **Mods** folder. Place Archipelago.MultiClient.Net.dll into the **UserLibs** folder.

The next time you launch the game, it may take some time to startup, and may also close and re-open itself. This is a normal part of MelonLoader's initial setup, and should only happen once.

### 2. Connecting To A Multiworld
The first time you launch the game without configuring a connection, the game will fail to connect and a configuration file will be created for you.

* Navigate to the game install directory. Open **UserData**, then edit the **ap_connection.ini** file in a text editor. If you don't see this file, just make it yourself.
* Fill out the fields with connection details for your multiworld. **Remember, you will need to configure this every time you want to connect to a different multiworld!**
Example:
```
# The multiorld server domain
domain=archipelago.gg
# The multiworld port
port=38281
# The name of your player slot in the multiworld
slot=DThaiPome_PMW2RP
# The multiworld password (leave this blank if there is no password)
password=
```
* Save this file, then launch the game. Once the game finishes booting up, you should be connected successfully. You can check the Melon logs window for a success line, or see if any errors occurred.

### Start The Game
Once you've completed the above setup and are connected successfully, you are free to create a new save file and play :)

**REMEMBER, DON'T CHANGE SAVE FILES WHILE CONNECTED!** Loading another save file may unintentionally clear locations. It is safest to stick to one save file for the duration of the multiworld session.
