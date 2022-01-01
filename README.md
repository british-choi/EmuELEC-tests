# EmuELEC TESTS 

The files included in this repository are meant to be a TEST (beta) version of EmuELEC that might contain erros/bugs/issues!    
While we do our best to test every change some changes might break your installation!  
**DO NOT INSTALL IF YOU DO NOT FEEL COMFORTABLE DEALING WITH POTENTIAL BUGS**  
For stable releases visit: https://github.com/british-choi/EmuELEC  
For support: join us at discord: https://discord.gg/cbgtJTu A new forum has been open for emuelec: https://emuelec.org


## CHANGELOG


# 4.4k-TEST-20211231

General
* retrorun: Fix that hotkey do not input alone
* Retroarch: Bump to 02898a4 (v1.9.14)
* fbneo: Bump to 73164d2 (support dsno's 20211124 romset)
* mame2003-plus: Bump to 99432c7
* flycast: Bump to e9bc945
* flycastsa: Bump to 0bb6fed
* genesis-plus-gx: bump to 6f782a3
* genesis-plus-gx-wide: Bump to fa71a16
* emuelec-emulationstation: Bump to e0e8d09

Ports Update
* VVVVVV: Bump to a345cf9
* sdlpop: Bump to d7ea0f6
* tyrquake: Bump to 423a217
* cdogs-sdl: Bump to 683b10d (v1.2.0)
* hurrican: Bump to 446b7a1
* nxengine-evo: Bump to e4b46c6
* devilutionX: Bump to a4bc8fe 

# 4.4k-TEST-20211120
General
* Retroarch: Bump to 02898a4 (v1.9.13.2)
* retrorun: Modify OSH PB Controller for RG351P/V
* libgo2: Support Analog stick for RG351P
* emuelec-emulationstation: Bump to de0dbd2
* ap6xxx-aml: Bump to 2b3ff5b
* WIP: Experimental HDD loading retry
* mount_romfs.sh: Fix missing then
* autostart: Mount roms earlier
* emuelec_autostart.sh: Fixed the problem that restore could not be done when using 2nd memory
* Create folders for karaoke, gmloader
* SDL_GameControllerDB: Update SAULABI & DragonRise Inc. joystick DB
* gptokeyb: Bump to 0f10087

Ports Update
* abuse: change source and bump to eaeb893
* devilutionX: Bump to a6f17fe (v1.3.0) with korean font
* VVVVVV: Bump to 0c1f756
* sdlpop: Bump to 6701645
* nxengine-evo: Bump to 1764184
* nxengine: Bump to 3680353
* cdogs-sdl: Bump to 33872a6 (Version 1.1.1)

Core Update
* hypseus-singe: Bump to a40eae9 (v2.6.16)
* Dosbox-svn: bump to 8e70e6e
* dosbox-pure: Bump to 01f2f5f (v0.20)
* pocketcdg: Bump to 6667414
* EasyRPG: Bump to 69aaeb2 (0.7.0 "Sword")
* fbneo: Bump to 5f9836a (support dsno's fbneo 20211027 roms)
* mame2003-plus: Bump to bc21f6a
* pcsx_rearmed: Bump to 9cc1b6c
* prosystem: Bump to f8652c7
* fmsx-libretro: Bump to 01731fc
* gambatte: Bump to b0c79f0
* swanstation: Bump to b6f76ff
* Solarus: Use gptokeyb for control on RG351P/V
* pcsx_rearmed: Bump to 589bd99
* Yabasanshiro: Bump to 2848d50 
* flycast: Bump to ae670ea
* ppsspp: Bump to b6e7fe1
* mupen64plus-nx-alt: Bump to 018ee72
* dolphinSA: Bump to 735fd60
* flycastsa: Bump to cc208ce
* Bump some emulators and cores


# 4.3k-TEST-20210907

* Add Abuse to ports NOTE: WIP controls
* Add Nxengine-evo to ports (support korean language)
* Add Streets of Rage Remake
* Fix Retroarch display of CJK characters
* Fix SFC not scraping
* Updated most emulators and cores
* Create folders for fbneo consoles

Amlogic-ng: 

* Add RTL8761 Bluetooth Support (#698)
* Include ssv6xxx-aml drivers

# 4.3k-TEST-20210825

* Fix Stadia Gamepad. Thanks to amuzulo#1322 
* Fix RA uses correct time zone
* Fix issue with lzdoom loading .doom files and sound on mods
* Update some sound packages
* Fix es_systems.cfg: Add extensions to c64/c128 and Amiga (#677)
* Add Cdogs-sdl to ports
* Bump Retroarch to v1.9.8
* Bump fbneo to 8ffe131 (support dsno's korean hack 8/22)
* Bump dosbox-pure to v0.15
* Bump devilutionX to 966cae8
* Bump VVVVVV to 749a885
* Bump mame2003-plus to d7dd8e7
* Bump neocd_libretro to 323f102

# 4.3k-TEST-20210801

* Fix create /storage/roms/amstradgx4000 on boot
* Cleanup es_systems.cfg remove and add some extentions
* Add Hurrican port (Handhelds currently have no working controls) 
* Atomiswave: Remove workaround for nvmem
* Bump Retroarch to 1.9.8
* Bump dosbox-pure to v0.14
* RG351V: Fix LCD streak issue

# 4.3k-TEST-20210723
General:

* Add Flycast Stand Alone 
* Add Alternate version of Mupen64plus-nx
* Replace old filemanager for 351Files
* Fix Amstrad GX4000


# 4.3k-TEST-20210713

General: 

* Fix Autoupdate
* Fix no backup restore if EEROMS was set to fat32
* Fix no external ROMS if EEROMS was set to fat32
* Fix typo on Parallel N64 32b core name
* Unify Brightness between ES and RA
* Fix advmame.sh: unset DISPLAY for Amlogic and Amlogic-ng
* Fix SuperTux2: Fix sed in launch script
* Fix vertical mode not respecting index ratio
* Fix Connect to WiFi on first boot if using es_defaults.txt
* Fix volume resets to 98% using AV
* Fix Do not redirect stdout/stderr to /dev/null in maxperf and normperf. (#661)
* Fix Do not update ppsspp assets
* emuelecRunEmu.sh: remove hardcoded bin path, this allows to use most of the binaries/scripts be called from `/emuelec/bin` or `/usr/bin` in that order
* Add Megadrive MSU to es_systems.cfg
* Add fceumm-mod libretro core to play some additional NES ROM hacks. (#658)
* New Packages: Box64, Box86, GL4es, Axe11, libglu (for future use)
* Bump most cores and emulators to current versions
* Bump fbneo to 886e424 (include korean hack)
* Bump SDLPoP to v1.22
* Bump sonic2013 to c3be493
* Bump soniccd to 129cd86
* Bump devilutionX to 72e888c
* Bump Retroarch to 1.9.6
* Bump ppsspp to eb0f0d3 (fix some korean character is broken in settings)
* Bump VVVVVV to 95ffc3a

Amlogic-ng: 

* Add preliminary support for Raxda Zero (But not support korean version)



# 4.2k-TEST-20210605
General:
- Hypseus replaced by Hypseus-singe
- Fix latest test missing libs
- Bump RigelEnfgine to fix a bug
- bump Retroarch to v1.9.3
- Switch Duckstation name to Swanstation
- Rework 32bit core detection on emuelecRunEmu.sh
- Yabasanshiro: Revert back to 7ae0de7 as it gives much better performance
- Added freej2me Java games emulator, it accepts .jar files and they should go into /storage/roms/freej2me. Internet is required only on first run to download the Java JDK.
- Update most cores and emulators to latest versions
- Add ee_fstype to set the EEROMS partitions to the desired file system, between FAT32 (default), EXT4, EXFAT and NTFS (read the warning about using NTFS). Instructions coming soon to Wiki/forum
- Fix OGG background music
- Update setres.sh and advmame.sh for resolution 1280x1024p60hz (PR #600)
- Fix drastic game saves & save states erased when resetting scripts & binaries to default (PR #595)
- Add Potator a Watara Supervision emulator core (not tested)
- gptokeyb bump and fix missing trigger actions
- Crystal bump to latest
- emuelec-emulationstation bump to latest

Amlogic-ng:
- Enable qca6174 drivers (Fixes issues #611)

Odroid Go Advance/Super & RG351P/V:
- Update U-boot and Kernel
- Use gptokeyb for controls on Solarus
- Fix reboot while charging
- Fix retrorun reversed analogs
- Introduce RetroRun, available for Flycast for the moment



# 4.1k-TEST-20210418
General:
- Use gptokeyb as a fake keyboard for OpenBOR
- Bump Retroarch to 1.9.1
- Bump mpv to v0.33.1
- Bump amiberry to v4.1.2

Additions:
- Added Chocolate-Doom with support for mods
- Added Amstrad GX4000

Fixes:
- Fixed OpenBor would not work after playing one game
- Fixed DevilutionX character voices were wrong
- ARM32 interpreter is now symlinked so no need for patchelf
- Fix some TimeZones not displaying/working correctly
- Fixed Drastic controller for RG351P



# 4.1k-TEST-20210321
General:
- Bump Genesis-plus-gx and Genesis-plus-gx-wide to support FM music
- Use DinguxFileManager as default on all platforms
- Use gptokeyb as a fake keyboard for OpenBOR
- Support Korean language for TvTextView
- Bump mpv to v0.33.0

Additions:
- Added gptokeyb to enable video controls on all devices with SDL support!
- Replace jslisten with gptokeyb to kill emulators
- Added easyrpg to es_systems.cfg
- Added Ecwolf with support for mods
- Added supermariowar to ports, on the first run a fake keyboard will be used, make sure you set your gamepad and restart the game, if you need to run the fake keyboard again delete /emuelec/configs/smw/nofakekeyb and run the game again.
- Added Flycast 32bit as core option for Dreamcast/Atomiswave/Naomi

Fixes:
- Fixed some errors messages were not wrapped and could not be read



# 4.1k-TEST-20210306
General:

- Emulationstation: While in a game list, pressing X will move to a random game, holding X will mark it as favorite (thanks to @lethal-guitar)
- Bump PPSSPPSDL to v1.11
- Bump Duckstation to abb7631
- Pico-8: Allow saving favorite carts, include binary in backup
- Update Sonic 1 and 2 so that they work with multiple gamepads
- Bump most emulators and cores to newest git hash (check commits for specifics)
- Bump Crystal theme which now includes a new panel (boxart)
- Enable bezels on OGS, not fully tested yet

Additions:

- Added Chocolate-Doom
- Added SuperTux and SuperTuxKart to ports
- Added Imagemagick (mainly for screenshot manipulation from CLI)
- Added logos to the ports (Thanks to Dim!)
- Added minecraft logos
- Added vertical aspect ratio option to OGA/S
- Added uchardet for mpv (korean smi is ok)

Fixes:

- Removed unused scripts, and fixed many small issues with scripts
- Fixed many script that were causing hangups or other issues
- Fixed gamecontrollerdb.sh it will now replace the UUID from the one in the db, this fixes weird controllers that use the same UUID as others (but are not the same)
- Fixed an issue with unicode characters not displaying correctly on the EEROMS partition (CN, JP, etc)
- Fix SonicCD Gamepad for the OGS
- Fix Pico-8 disappearing splore file
- Fix Scummvm game scan
- Fix brightness not restored after reboot on OGA/S, thanks to @miwasp, fixes issue #470
- Fixed issue with OGA/S OC not beeing applied correctly (this does not solve the random lockups on some devices)
- Fix backup/restore issues
- Fixed Retroach video recording
- Fixed Eduke not running when having lots or ROMS in ES, by enabling swap (much testing needed!)
- Fixed an issue with ES not playing .ogg music files in BGM
- 

## IMPORTANT!

This version includes a big change on how binaries and scripts are stored, basically to deal with the issue of people not reading how to properly update and since I am getting tired of answering the same question over and over again, lets just move all binaries and scripts to RO /usr/bin, this will force update all of these and make updating much simpler.

If you use custom scripts /emuelec/bin and /emuelec/lib are still in the path so you will have to deal with it accordingly.

All configurations regarding emuelec will still be handled in /emuelec/config

#### Note that this is probably not final, I still need to do a lot of testing, but keep that in mind if you want to update



# 4.1k-TEST-20210221
- Emulationstation: While in a game list, pressing X will move to a random game, holding X will mark it as favorite (thanks to @lethal-guitar)
- Fixed many script that were causing hangups or other issues
- Fixed gamecontrollerdb.sh it will now replace the UUID from the one in the db, this fixes weird controllers that use the same UUID as others (but are not the same)
- Fixed an issue with unicode characters not displaying correctly on the EEROMS partition (CN, JP, etc)
- Added SuperTux and SuperTuxKart to ports
- Fix SonicCD Gamepad for the OGS
- Fix Pico-8 disappearing splore file
- Added Imagemagick (mainly for screenshot manipulation from CLI)
- Bump PPSSPPSDL to v1.11
- Bump Duckstation to abb7631
- Fix Scummvm game scan
- Fix brightness not restored after reboot on OGA/S, thanks to @miwasp, fixes issue #470
- Removed unusued scripts, and fixed many small issues with scripts
- Fixed issue with OGA/S OC not beeing applied correctly (this does not solve the random lockups on some devices)
- Added Chocolate-Doom
- Bump Dosbox-pure to v0.10
- Added DinguxCommander for OGS
- Bump mpv to 4dcaf70
- Bump fbneo to 9538dca with korean hack patch (thanks to @DsNo)
- Bump emulationstation to a63ba0c
