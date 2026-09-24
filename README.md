# Pac-Man World 2: Re-PAC Archipelago

## Requirements
* Legitimate Steam copy of Pac-Man World 2: Re-PAC on PC
  * We are only supporting the most current game version; if you've downpatched your game, you may encounter problems until you revert to the latest patch
* MelonLoader Installer **v4.3.0**: https://melonwiki.xyz/#/README (this is used to install and run mods)
* Latest release of PMW2RPArchipelagoClientMod (this is the mod that actually provides archipelago support to this game)
* **For seed and options generation:** Latest release of the PMW2RP APWorld
* **Optional**: Archipelago Launcher: https://archipelago.gg/tutorial/Archipelago/setup_en
  * Currently, you will not be alerted in-game when you receive items. I strongly recommended connecting with a Text Client alongside the game to keep track of what is happening in your multiworld
 
The client mod and APWorld can be found [at the latest release in this repository!](https://github.com/DThaiPome/PMW2RP-Archipelago-Central/releases/latest) The components in this release will always be compatible with each other.

## Getting Started (Setup)
### 1. Melon/Mod Installation
* Launch the MelonLoader Installer and use it to install MelonLoader to Pac-Man World 2: Re-PAC. Select MelonLoader v0.7.3.
* Navigate to the game install directory. Place **PMW2RPArchipelagoClientModStandalone.dll** into the **Mods** folder.

The next time you launch the game, it may take some time to startup, and may also close and re-open itself. This is a normal part of MelonLoader's initial setup, and should only happen once.

### 2. Connecting To A Multiworld
The first time you launch the game without configuring a connection, the game will fail to connect and a configuration file will be created for you.

* Navigate to the game install directory. Open **UserData**, then edit the **ap_connection.ini** file in a text editor. If you don't see this file, just make it yourself.
* Fill out the fields with connection details for your multiworld. **Remember, you will need to configure this every time you want to connect to a different multiworld!**
Example:
```
# The multiworld server domain
domain=archipelago.gg
# The multiworld port
port=38281
# The name of your player slot in the multiworld
slot=DThaiPome_PMW2RP
# The multiworld password (leave this blank if there is no password)
password=
```
* Save this file, then launch the game. Once the game finishes booting up, you should be connected successfully. You can check the Melon logs window for a success line, or see if any errors occurred.

### 3. Start The Game
Once you've completed the above setup and are connected successfully, you are free to create a new save file and play :)

**REMEMBER, DON'T CHANGE SAVE FILES WHILE CONNECTED!** Loading another save file may unintentionally clear locations. It is safest to stick to one save file for the duration of the multiworld session.

## About This AP Implementation
To get started with configuring and generating your seed, see the example options YAML file in this repo. That file also explains many of the items and locations.

### What is randomized?
You can configure your seed to gate the following behind random item checks:
* Pac-Man's moveset
* World/Level access
* Types of fruit that appear in levels (Fruit Switches)

### What kinds of locations can you clear to earn items?
* Reaching a level's goal
* Completing missions
* Collecting gashapon capsules and galaxians
* Beating gold medal time trial times

### How do you beat the seed?
Depending on your settings, either by defeating Spooky for the first time, or by clearing the level Flying Dark Shadow.

### When I receive items in this game, what does it look like?
Currently, we have no dedicated in-game tracking for items received or owned. I recommend using a text client with this game to keep track of your progress.

Here are some things that do appear in game:
* Levels cleared, either cleared by you or cleared remotely, will appear as such in the world map.
* Levels unlocked will appear if you zoom out on the map.
  * All levels may appear unlocked until you zoom out. Ignore this, it's a side effect of some patches that enable full map navigation. Use the zoomed-out UI as the source of truth.
  * If a level does not appear unlocked when it should be, try entering and exiting Pac-Village. Or, try navigating over the level with your cursor, you may be able to enter it even if it looks locked.
* Galaxians collected in a level will immediately appear collected permanently, even if you leave or restart a level without reaching the goal.
* All Golden Fruit that you receive will appear in Pac-Village under the Golden Tree.
* Pac-Knight Era keys that you receive will appear in the world map near their respective gates.
* Missions and time trials cleared in-game or remotely will appear as such in the world map.

These things will not always appear in game, and you may want to use a text client to track them:
* Gashapons will appear collected if you reach a level's goal. Use a text client to track specific gashapons.
* There is no visible way to track your current moveset, but moveset items you receive will become active immediately. So if you're ever wondering what Pac-Man can or can't do, just try it :)
* Fruit switches also have no visible tracking. If you receive a fruit switch while playing a level, you may need to restart the level to see the respective fruit appear.

## This AP implementation is currently in development!
We will be adding features, fixing bugs, and cleaning things up over time. Reach out to us in the AP Discord server if you have any questions or concerns! We have a thread in the future games channel.

Maintained by DThaiPome and DepressingChild
