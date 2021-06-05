# EmuELEC TESTS 

The files included in this repository are meant to be a TEST (beta) version of EmuELEC that might contain erros/bugs/issues!    
While we do our best to test every change some changes might break your installation!  
**DO NOT INSTALL IF YOU DO NOT FEEL COMFORTABLE DEALING WITH POTENTIAL BUGS**  
For stable releases visit: https://github.com/british-choi/EmuELEC  
For support: join us at discord: https://discord.gg/cbgtJTu A new forum has been open for emuelec: https://emuelec.org


## CHANGELOG
### 4.2k-TEST-20210605
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
##
### 4.1k-TEST-20210418
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
##
### 4.1k-TEST-20210321
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
##
### 4.1k-TEST-20210306
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
##

### 4.1k-TEST-20210221
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
