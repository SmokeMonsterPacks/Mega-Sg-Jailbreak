# Mega Sg Jailbreak

Custom "*Jailbreak*" firmware for the [Analogue Mega
Sg](https://www.analogue.co/pages/mega-sg/) that allows loading 
ROMs from the SD Card slot, and an expanded featureset.

## Updating Firmware

Format a 2GB (or larger) SD card as
[FAT32](https://en.wikipedia.org/wiki/FAT32) (FAT16 and exFAT are not
supported). In Windows, you must use a tool for cards larger than
32GB, such as
[fat32format](http://www.ridgecrop.demon.co.uk/index.htm?guiformat.htm).

Place the firmware file
[msg_firmware_verJBX.Y.bin](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/releases/download/)
into the root directory of your SD card.  Be sure that there is only
one firmware file there.  Insert the card into your Mega Sg and power
on. The firmware will be flashed to the console. This process may take
a few minutes.

While the firmware is flashing the LED will turn red and flicker,
followed by a considerable pause and HDMI signal blackout.  Do not
power off.  The main menu will boot when it has finished. Delete the
firmware file from your card after flashing.

The Mega Sg is protected from bricking as a result of firmware
updates, but please still follow the above precautions to be safe.

## Organizing ROMs

Create a folder called `MEGADRIVE` at the root of your SD card, and
drop your folders and subfolders of ROMs inside (see [SmokeMonster's
database](https://github.com/SmokeMonsterPacks/EverDrive-Packs-Lists-Database)
for a curated [list of valid Megadrive
ROMs](https://github.com/SmokeMonsterPacks/EverDrive-Packs-Lists-Database/blob/master/EverDrive%20Pack%20SMDBs/Mega%20EverDrive%20SMDB.txt)).
The system will search for ROMs in the `/MEGADRIVE/` folder first, or
the root directory of the SD card if there is no `/MEGADRIVE/` folder.
The maximum number of files (ROMs and subfolders) that can be placed
in a given folder is around 300-500, depending on the length of the
filenames.

## Running ROMs

Select **browse SD card** from the main menu.  Hit **enter** on a
filename to run it, or if it's a subfolder, it will enter said folder.
The menu hotkey will return to the file menu from the game.

## Saves

NEVER insert or remove cartridges while your Mega Sg is powered
on. Doing so may risk damaging the console and/or losing saves. It is
good practice to backup saves before updating firmware.

When a game is exited to the menu, it will prompt you to save. Return
to the file menu and save your progress before powering down.


## Changelog
- [JBX.X](https://github.com/SmokeMonsterPacks/Super-NT-Jailbreak/releases/download/v6.4/snt_firmware_verJB6.4.bin) 2019-0X-XX Initial release :heart:

## Known Issues


## Cores Supported

`Genesis/Megadrive`

## Problem Reporting and Community Chat

The custom firmware is not coded by
[SmokeMonsterPacks](https://github.com/SmokeMonsterPacks) or
[frederic-mahe](https://github.com/frederic-mahe), but please do
report problems here at GitHub for support. Priority will be given to
jailbreak-specific problems (using ROMs through the SD card slot
rather than through the cartridge slot). Feel free to also submit issues 
for non-jailbreak related problems. You can join the [Classic Gaming
Discord](https://discord.gg/EX57xnF) to chat or troubleshoot 
in #analogue-mega-sg

Use at your own discretion. We are not responsible for any damage or
data loss caused by custom firmware installation or use.
