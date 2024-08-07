# SteamDeck Refresh Rate Unlocker OLED
This repository contains the instructions and scripts on how to unlock the Steam Deck OLED under SteamOS to use up to 100Hz refresh rate for the display (do not confuse this with FPS). \
Discord user dan2wik for the idea on overclocking the display panel to 100Hz!

## NOTE: 
**This script is only for the OLED model, if you wish to use the script from the LCD models please see the original [Github](https://github.com/ryanrudolfoba/SteamDeck-RefreshRateUnlocker)**

**This script is experimental and i only modified this script for testing purposes, if you wish to test it, this script is based off the original script by ryanrudolfoba, do not expect results i am doing this on my own**

**Please support the original developers work!, i do not need your donations so please support the origivsal dev [here](https://github.com/ryanrudolfoba/SteamDeck-RefreshRateUnlocker)**

## What does this script do?!?
1. The script checks if the gamescope-session is using the default values 40,90Hz refresh rates.
2. If it's the default values, the script will create a backup of the file and then "patches" accordingly to what the user has chosen.
3. The script creates a folder called ~/1RefreshRateUnlocker that contains additional helper scripts. Do not delete this folder!
4. The script checks the gamescope-session every startup if it needs to be "patched" and applies the patch if needed.
5. There is an uninstall script if end-user wants to revert any changes made.

## Prerequisites for SteamOS
1. sudo password should already be set by the end user. If sudo password is not yet set, the script will ask to set it up.

## Installation Steps
1. Go into Desktop Mode and open a konsole terminal.
2. Clone the github repo. \
   cd ~/ \
   git clone https://github.com/PS2ClassicsVault/SteamDeck-RefreshRateUnlocker_OLED.git
3. Execute the script! \
   cd ~/SteamDeck-RefreshRateUnlocker_OLED \
   chmod +x install-RefreshRateUnlocker.sh \
   ./install-RefreshRateUnlocker.sh
   
4. The script will check if sudo passwword is already set.\

   a. If the sudo password is already set, enter the current sudo password and the script will continue to run. Once you see this screen then the install is done!\

   b. If wrong sudo password is provided the script will exit immdediately. Re-run the script and enter the correct sudo password!\
         
   c. If the sudo password is blank / not yet set, the script will prompt to setup the sudo password. Re-run the script again to continue.\

5. Make your selection.\

6. Once the install is done, reboot the Steam Deck for changes to take effect.
         
7. After reboot, the custom refresh rate will be available. It can be set as high as 100Hz!


## How to Uninstall
1. Go into Desktop Mode and launch RefreshRateUnlocker Toolbox icon from the desktop.

2. Select the option called Uninstall and press OK.

3. Once the uninstall is done, reboot the Steam Deck for changes to take effect.
         
4. After reboot, the refresh rate will be back to the default 90Hz.


## Known Issues
1. When taking a screenshot in-game, the screen will momentarily go blank as it toggles to 90Hz, and then goes back to the custom refresh rate once the screenshot is done.
2. 100Hz will not be displayed in the QAM even when turning off Unified Frame Limit Management, however turning off the framelimit helps.
3. Applications will still report 90Hz regardless, this needs additional assitance to get this script to function properly, but the system seems more resposive with this script installed.

