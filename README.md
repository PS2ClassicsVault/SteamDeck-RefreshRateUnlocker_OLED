# SteamDeck Refresh Rate Unlocker
This repository contains the instructions and scripts on how to unlock the Steam Deck OLED under SteamOS to use up to 100Hz refresh rate for the display (do not confuse this with FPS). \
Discord user dan2wik for the idea on overclocking the display panel to 100Hz!

## NOTE: 
**This script is only for the OLED model, if you wish to use the script from the LCD models please see the original [Github](https://github.com/ryanrudolfoba/SteamDeck-RefreshRateUnlocker)**
**This script is experimental and i only modified this script for testing purposes, if you wish to test it, this script is based off the original script by ryanrudolfoba.**

## What does this script do?!?
1. The script checks if the gamescope-session is using the default values 40,60Hz refresh rates.
2. If it's the default values, the script will create a backup of the file and then "patches" accordingly to what the user has chosen.
3. The script creates a folder called ~/1RefreshRateUnlocker that contains additional helper scripts. Do not delete this folder!
4. The script checks the gamescope-session every startup if it needs to be "patched" and applies the patch if needed.
5. There is an uninstall script if end-user wants to revert any changes made.

## Prerequisites for SteamOS
1. sudo password should already be set by the end user. If sudo password is not yet set, the script will ask to set it up.

## Installation Steps
**IF YOU ARE USING AN OLDER VERSION OF THIS SCRIPT, UNINSTALL IT FIRST!**
**IF YOU WANT TO SWITCH FROM 30,60 to 40,70 etc etc, MAKE SURE TO UNINSTALL FIRST AND THEN RE-RUN THE SCRIPT!**
**[CLICK HERE FOR STEPS ON HOW TO UNINSTALL THE OLD VERSION](https://github.com/ryanrudolfoba/SteamDeck-RefreshRateUnlocker/tree/7ccbc1a4e32f4244b27bf8dd15daaf39f307031a#how-to-uninstall)**
1. Go into Desktop Mode and open a konsole terminal.
2. Clone the github repo. \
   cd ~/ \
   git clone https://github.com/PS2ClassicsVault/SteamDeck-RefreshRateUnlocker_OLED.git
3. Execute the script! \
   cd ~/SteamDeck-RefreshRateUnlocker \
   chmod +x install-RefreshRateUnlocker.sh \
   ./install-RefreshRateUnlocker.sh
   
4. The script will check if sudo passwword is already set.\
![image](https://user-images.githubusercontent.com/98122529/225724178-364284ac-f504-4798-b5e5-a03001dda5da.png)

   a. If the sudo password is already set, enter the current sudo password and the script will continue to run. Once you see this screen then the install is done!\
![image](https://user-images.githubusercontent.com/98122529/225747904-d0352779-40ef-4dfb-afad-c473b2a9bc5b.png)

   b. If wrong sudo password is provided the script will exit immdediately. Re-run the script and enter the correct sudo password!\
![image](https://user-images.githubusercontent.com/98122529/225724539-d73dc9ce-c468-49d1-8d2c-83276bfc34bb.png)
         
   c. If the sudo password is blank / not yet set, the script will prompt to setup the sudo password. Re-run the script again to continue.\
![image](https://user-images.githubusercontent.com/98122529/225725477-33f8ffaa-13a1-452e-b993-aceb3192726f.png)


5. Make your selection.\

6. Once the install is done, reboot the Steam Deck for changes to take effect.
         
7. After reboot, the custom refresh rate will be available. It can be set as high as 100Hz!\


## How to Uninstall
1. Go into Desktop Mode and launch RefreshRateUnlocker Toolbox icon from the desktop.

2. Select the option called Uninstall and press OK.

3. Once the uninstall is done, reboot the Steam Deck for changes to take effect.
         
4. After reboot, the refresh rate will be back to the default 90Hz.\


## Known Issues
1. When taking a screenshot in-game, the screen will momentarily go blank as it toggles to 60Hz, and then goes back to the custom refresh rate once the screenshot is done.

