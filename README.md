# Mega Sg Jailbreak

Custom "*Jailbreak*" firmware for the [Analogue Mega
Sg](https://www.analogue.co/pages/mega-sg/) that allows loading ROMs
from the SD Card slot, and an expanded featureset.

## Updating Firmware

Format a 2GB (or larger) SD card as
[FAT32](https://en.wikipedia.org/wiki/FAT32) (FAT16 and exFAT are not
supported). In Windows, you must use a tool for cards larger than
32GB, such as
[fat32format](http://www.ridgecrop.demon.co.uk/index.htm?guiformat.htm).

Place the firmware file
[msg_firmware_verJB7.3.bin](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/blob/master/firmware/msg_firmware_verJB7.3.bin)
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

An empty folder structure is included in [MSG JB
Filesystem.zip](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/blob/master/firmware/MSG%20JB%20Filesystem.zip)
Drop your ROMs into these subfolders and they will be automatically
entered when the corresponding core is loaded (see [SmokeMonster's
database](https://github.com/SmokeMonsterPacks/EverDrive-Packs-Lists-Database)
for curated [lists of
ROMs](https://github.com/SmokeMonsterPacks/EverDrive-Packs-Lists-Database)).
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

- [JB7.3](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/blob/master/firmware/msg_firmware_verJB7.3.bin) 2019-04-01 Initial release :heart:
  - includes all fixes from official firmware v4.3
  - [PDF user guide](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/blob/master/Mega%20Sg%20Unofficial%20Jailbreak%20Supplement%20JBv7.3.pdf) with documentation

## Known Issues


## Cores Supported

- `Genesis/Megadrive`
- `Master System` and `SG-1000`
- `Game Gear`
- `ColecoVision`

## Other Features

- Sega CD BIOS loading
- ColecoVision Super Game Module and Super Banking
- and much more!

## Problem Reporting and Community Chat

The custom firmware is not coded by
[SmokeMonsterPacks](https://github.com/SmokeMonsterPacks) or
[frederic-mahe](https://github.com/frederic-mahe), but please do
report problems here at GitHub for support. Priority will be given to
jailbreak-specific problems (using ROMs through the SD card slot
rather than through the cartridge slot). Feel free to also submit
issues for non-jailbreak related problems. You can join the [Classic
Gaming Discord](https://discord.gg/EX57xnF) to chat or troubleshoot in
#analogue-mega-sg

Use at your own discretion. We are not responsible for any damage or
data loss caused by custom firmware installation or use.
