# Mega Sg Jailbreak

Custom "*Jailbreak*" firmware for the [Analogue Mega
Sg](https://www.analogue.co/pages/mega-sg/) that allows loading ROMs
from the SD Card slot, and an expanded featureset.


## Updating Firmware

As shown in this [video
walkthrough](https://www.youtube.com/watch?v=xMBruBrhnv8), format a
2GB (or larger) SD card as
[FAT32](https://en.wikipedia.org/wiki/FAT32) (FAT16 and exFAT are not
supported). In Windows, you must use a tool for cards larger than
32GB, such as
[fat32format](http://www.ridgecrop.demon.co.uk/index.htm?guiformat.htm).

Place the firmware file
[msg_firmware_verJB7.8.bin](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/blob/master/firmware/msg_firmware_verJB7.8.bin)
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
Filesystem.zip](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/raw/master/firmware/MSG%20JB%20Filesystem.zip).
Drop your ROMs into these subfolders (see [SmokeMonster's
database](https://github.com/SmokeMonsterPacks/EverDrive-Packs-Lists-Database)
for curated [lists of
ROMs](https://github.com/SmokeMonsterPacks/EverDrive-Packs-Lists-Database)).
When loading a core, the Mega Sg will automatically enter the
corresponding subfolder.  The maximum number of files (ROMs and
subfolders) that can be placed in a given folder is around 300-500,
depending on the length of the filenames.


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


## Fonts

The **System -> Font** menu allows you to select your own font in place of those which come with the console. The load font option will bring you to the file browser. If you have a directory called `/FONT/` at the root of your SD card, it will default to that directory to load a font file. The font must use an 8x8 text box and must be represented in binary in a 1-bit per pixel format. Each character will take eight bytes to represent in this format. The file must be 768 or 1024 bytes in size and use the extension .fnt. The characters in the file will have to start at ASCII 20 (space) and end at ASCII 7F (delete). Font files 1024 bytes in size will not show the first 32 characters which would be stored in the first 256 bytes of that file. A set of user-created fonts compiled by [Sho](https://archive.org/details/@zreport) is available [here](https://archive.org/details/shos-font-pack-v-3). Utilities to convert Analogue font files to/from bitmap files are available [here](https://archive.org/details/analogue-font-utilities).


## Changelog
- [JB7.8](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/blob/master/firmware/msg_firmware_verJB7.8.bin) 2021-02-22
  - Added blurring for the entire screen - enable dither blending and set blending depth to maximum
  - Added SPD HDMI packet to identify as 'Mega sg"
  - Added timing sliders for Sega CD
  - Added horizontal position slider for DAC/analog output
  - Added SMS Model 1 reset by pressing X, Y, and Z at the same time on a 6 button controller
  - Fixed non-visble top scanline in HDMI
  - Fixed graphical corruption in Paprium
  - Fixed six button controller reading for Ultracore, Paprium and other games
  - Fixed cartridge adapters failing to work properly if startup is set to "Cartridge Direct"
  - Fixed Spider Man: Web of Fire 32x cartridge not working
  - Fixed non-centered picture when horizontal/vertical position sliders are centered
  - Fixed Z80 inability to write to the cartridge bus
  - Fixed timing bug reported by krikzz
  - Fixed Coleco Super Game Module not running Penguin Adventure
  - Fixed Squish 'em Sam digitized audio

- [JB7.7](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/raw/master/firmware/msg_firmware_verJB7.7.bin) 2019-11-19
  - includes all fixes from official firmware v4.7:
      - 32X support added in DAC mode
    - Cartridge/CD audio selection fixed. Checking 'enable cartridge and CD audio' will work now regardless of the 'automatic' setting checkbox.
    - 32X is detected and will enable audio by default.
    - Chuck Rock CD is now working.
    - Many CD fixes- NHL 94, Willy Beamish, and other games now work.
    - Zesenilia demo text fixed.
    - Turbo Outrun graphics seem to be fixed.
    - Audio pitch shifting on some games in zero delay mode fixed.
    - Support for cartridge adapters added.
    - Game Gear adapter supports the tuner now.
  - plus:
    - Fixed large SMS BIOSes not working issue
    - CJ Elephant now works properly
    - Hardball 95 "SRAM error" fixed
    - Many other minor fixes

- [JB7.6](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/raw/master/firmware/msg_firmware_verJB7.6.bin) 2019-08-09
  - includes all fixes from official firmware v4.6:
    - Added DAC
    - Added light gun support with DAC
    - Fixed boot audio level
    - Fixed left side green line when HQX scalers active
    - Bubble Bobble SMS fixed
    - Added Genesis and SMS light gun support
    - Fixed CD BIOS replacement again
    - Sped up file loading

- [JB7.5](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/blob/master/firmware/msg_firmware_verJB7.5.bin) 2019-06-11
  - includes all fixes from official firmware v4.5:
    - Player 2 controller can run the menu if it is a 3 or 6 button controller, and player 1 controller is not a 3 or 6 button controller
    - Different size font files are supported. If the file is 1K or larger, the first 32 characters are cut off
    - DVI Mode added
    - Fixed scaler bug where the top scanline or two might not be visible
    - Scanlines have been totally redone. There are now more options to tweak and width is now adjustable

    (gen/md)
    - Fixed CD games that regressed in previous fw
    - Fixed Some graphic issues on *Mickey Mania CD* and others
    - Fixed bugs with Japanese Sega CDs
    - *Silpheed* and *Vay* bugs fixed
    - *Popful Mail* "CPU ERROR" fixed
    - CD bus timing improvements
    - *Pier Solar* cartridge + audio CD works and tested on US model 1, US model 2, and Japanese CD units
    - Added an option to automatically enable CD audio when CD unit plugged in
    - Fixed FM sound bug on *Streets of Rage* percussion on certain tracks
    - Fixed PSG sound bug (*Phantasy Star IV*)
    - CRAM dots option added
    - *X-Men 2* random character select on start is now random

    (sms)
    - SMS Cropping setting added to crop the left side when a game used left cut
    - Fixed PSG sound bug (*Alex Kidd in Miracle World*)
    - CRAM dots option added
    - VDP palette option added to select SMS or original TMS9918a palette for video modes 0-3
    - All 240 scanlines are now visible. Before, only 239 were visible

  - plus:
    - CD BIOS replacement works now after a reboot
    - Coleco *Gradius* mapper + flash memory supported. Use extension .CF0 for this game
    - Fixed Coleco *Jungle Hunt* / *Learning with Leeper* had stuttering scrolling
    - Coleco *Risky Rick* console detection fixed. Note: there are two versions of the game. A full version and a demo version. If the game does not let you progress to level 2, it is the demo version
    - Fixed Super Game Module AY-3-8910 write delay. This fixes the pitch of speech on *Wizard of Wor*
    - Fixed *Megaman Wily Wars* EEPROM saving

- [JB7.4](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/archive/v7.4.zip) 2019-04-16
  - includes all fixes from official firmware v4.4:
    - Sega CD - adjusted timing i.e. *Mickey Mania*
    - *Overdrive 2 demo* is 100%
    - *X-men 2* character select fixed
    - Fixed player 2 XYZ (6 buttons)
    - Allow no controller on player 2
    - SMS fixes for X7 and flash everdrive
    - You now stay in the file browser when selecting a font
    - Changed "hotkeys" to "hotkeys & controllers"
  - plus:
    - Sega CD BIOS substitution works properly now on games like *Snatcher*
    - Fixed speech on Coleco *Wizard of Wor*
    - Fixed random crashes in *Wizard of Wor* and *Majikazo*
    - Fixed graphics issue on *Juno First* and *Astrododge*
    - Fixed sprites sticking around between games
    - Added warning: CD BIOS replacer only works if fix region is turned on
    - SMS BIOS now also works for cartridges
    - Game gear buffer changed to zero delay by default
  - [PDF user guide](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/blob/master/documentation/Mega_Sg_Unofficial_Jailbreak_Supplement_JBv7.4.pdf) with documentation
  
- [JB7.3](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/archive/v7.3.zip) 2019-04-01 Initial release :heart:
  - includes all fixes from official firmware v4.3
  - [PDF user guide](https://github.com/SmokeMonsterPacks/Mega-Sg-Jailbreak/blob/master/documentation/Mega_Sg_Unofficial_Jailbreak_Supplement_JBv7.3.pdf) with documentation


## Warnings

- Sega CD Region-Free BIOS are problematic even on real hardware, so
it's recommended to use an official SCD firmware from the region 
of game you wish to boot. Also, you must use a PAL CD BIOS for PAL 
games and NTSC for NTSC.
- Clean your Sega CD's edge connector with Deoxit before reporting issues.


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
Gaming Discord](https://discord.gg/UDu5ztY) to chat or troubleshoot in
#analogue-mega-sg

Use at your own discretion. We are not responsible for any damage or
data loss caused by custom firmware installation or use.
