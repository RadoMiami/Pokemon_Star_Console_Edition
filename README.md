# Pokemon Star v0.2: Console Edition


Taking Pokemon Star v0.2, made by Rusyaas and turning it into a console-playable state.
WARNING: If you have already downloaded Pokemon Ultra Moon (not using a cart), make (ABSOL)UTELY SURE that you delete Ultra Moon when the guide tells you to. Otherwise, bad things may happen.

# Prerequisites #

1. A homebrewed 3DS on the latest version of Luma3DS (If you haven't homebrewed your 3DS yet, follow 3ds.guide to join the party.)
2. Your 3DS SD Card must have at least 8GB of space.
3. A PC with at least 12GB of space. (The rom hack won't take all this space for long, it will be reclaimed soon afterwards.)
4. An SD to USB adapter so you can actually use the SD card on your computer. (Or if you have an SD card slot on your PC, that works too)
5. GodMode9, Checkpoint, and HackingToolkit9DS or DotNet3dsToolkit. (You should have the first two, the third is at https://github.com/Asia81/HackingToolkit9DS-Deprecated-/releases).


# Extract A Clean a083 Garc From A Rom #

Get some form of a Pokemon Ultra Moon or Ultra Sun ROM. Download and install a rom from that site, rip a rom, just get the ROM somehow. However, I highly recommend supporting the devs and downloading Ultra Moon off of the eShop or buying an Ultra Moon cart if you don't have it or Ultra Sun. Those methods tell Game Freak that you like USUM, and hope they do more games like that in the future. :D

## eShop Method (Recommended) ##
1. Download the game off the eShop. (In this instance, make sure you have 8GB of free space before continuing!)
2. Boot into GodMode9.
3. Go into [A:] SYSNAND SD, then /title/.
4. Press R+A while highlighting the 00040000 folder, then select "Search for titles".
5. Scroll down the list until you see Pok??mon Ultra Moon or Pok??mon Ultra Sun. (Number to left ends in 001B5100 and 001B500 respectively!)
6. Select "TMD file options..."
7. Select "Build CIA (standard)" (This will take some time.)

## Use A Cartridge (Also Recommended) ##
1. Boot into GodMode9 by holding Start upon boot. If you see multiple options, select GodMode9.
2. Insert your cart, then find 00040000001B5100_v00.3ds or 0040000001B5000_v00.3ds in [C:] GAMECART.

## Download A .3ds ROM (Unrecommended) ##
1. Find the .3ds rom somewhere and move it to your 3DS. (Blatant piracy isn't cool, so I can't help you with this one. Downloading it will take some time, depending on your internet speed.)
2. Move the .3ds rom to your 3DS and enter GodMode9.
3. AFter finishing the next steps, delete the ROM.

After doing one of the three, follow one of the below depending on which game it is.

## Get a083 Garc (Ultra Moon) ##

1. Mount the .3ds/.cia file by selecting NCSD/CIA image options, then select Mount image to drive.
2. Push A, then select content0.game/romfs/a/0/8.
3. Select the file named "3", then select Copy to 0:/gm9/out. (This will take some time.)
4. Turn off your 3DS.



## Get a083 Garc (Ultra Sun) ##

1. Mount the .3ds/.cia file by selecting NCSD/CIA image options, then select Mount image to drive.
2. Push A, then select content0.game/romfs/a/0/8.
3. Select the file named "2", then select Copy to 0:/gm9/out. (This will take some time.)
4. Turn off your 3DS, then move the file to your computer.
5. Download patches.zip from this Github.
6. Apply the usonly.xdelta patch using xdelta. (https://www.romhacking.net/utilities/598/)
7. Rename the file to "3", then move the now patched file back to your 3DS.


# Patching a083 with xDelta #
1. Get xDelta patcher from above (https://www.romhacking.net/utilities/704/) and apply the Stars_083_v0.x.xdelta patch to the a083 garc (named "3") extracted from a legitimate Ultra Moon copy (or converted from Ultra Sun) earlier.
2. Keep track of your newly patched garc, it should be 473,143kb. 


# While You Wait... #
While you're waiting to get your a083 garc, download Pokemon Star from that site. (If you already have it, skip this.) (Search "pokemon star rom", and you'll eventually find what you need.) Both will take a while, so it's better to knock them both out now.


# Creating The Rom #
1. After downloading HackingToolkit9DS, run SetupUS.exe first, or it may not work.
2. After it finishes, trim your Pokemon Star rom on your PC using something like NDSTokyoTrim.
3. Put the trimmed Pokemon Star rom on your 3DS, then mount the image.
4. Go into content0.game, but this time copy the romfs folder, exefs folder, and extheader.bin file to 0:/gm9/out on your SD card.
5. Replace the romfs/a/0/8/3 file with the one you got from the previous steps.
6. Turn off your 3DS, then put the spliced together romfs folder, untouched exefs folder, and  back onto your computer.
7. In the folder where you installed HackingToolkit9DS, there should be an ExtraTools folder (For convinence sake, put the folders there.
8. Replace the banner and icon files in the exefs folder from the ones in the exefs.zip file posted on the Github, and rename the file .code file in the exefs folder to .code.bin. (Weird things happen if you don't.)
9. Run the tool 3DS Builder Mod.
10. Select the romfs folder that you spliced together, the exefs folder, and the extheader.bin file. (If you know what you're doing, modify them to your liking.)
11. Put in a serial number (CTR-P-STAR works just fine.) and name the output rom. (pkmnstar.3ds works just fine.)
12. Wait for it to build, then move it to your 3DS. 
13. Select "NCSD image options", then choose "Build CIA from file", then pray to your deity of choice that it works. (This will take some time. If there's an error, make sure that you didn't forget any steps. (If you see an ETA, it's a good sign!)
14. Delete the ROM that you built. (DO NOT DELETE THE CIA!)
15. If you got Ultra Moon by downloading it off the eShop, backup the save file through Checkpoint and delete the game

# Creating The Rom With DotNet3dsToolkit #
1. Download evandixon's DotNet3dsToolkit from https://github.com/evandixon/DotNet3dsToolkit/releases/tag/1.4.6.
2. Run DotNet3dsToolkit from ToolkitForm.exe and dump your acquired *Pokemon Stars* rom from the steps above. (Make sure your output directory is a clean folder!)
3. Replace the code and banner files in ExeFS making sure to add .bin as an extension, take your patched a083 garc from above and replace the existing a083.
4. Rebuild with DotNet3dsToolkit making sure to select build, and adding the extension ".cia" to whatever you choose to name it.
5. Install using FBI or custom-install (https://github.com/ihaveamac/custom-install/releases/tag/2.0). (Make sure to backup your save!!!)

# Installation & Cleanup #
1. If you picked the correct deity, or got super lucky, then this went of without a hitch! As Gamechamp3000 said in her first video about a low-shot run of Octo Expansion, "Turns out all you needed to conquer death was a spoonful of elbow grease and a freighter loaded with pain and suffering!"
2. Delete the USUM .cia/.3ds file and the downloaded pokemon star .3ds file if you haven't already.
3. Reboot your 3DS, then install and delete the .cia Pokemon Star file with FBI. (For convenience, back up the CIA file to your computer beforehand.)
4. Update if it asks you to, then fire up the game. If you see Kukui instead of Wicke, you messed up somewhere. The text from anytime after the opening cinematic should be the same, but the models will unfortunately still be the originals. Fixing them will be a major undertaking, assuming I even go down that route.


# Migrating from Citra #
1. Boot the game on your 3DS at least once.
2. Select your Pokemon Star save file from Citra, then copy it over to 3ds/Checkpoint/saves/0x01B51 Pokemon Ultra Moon.
3. Restore the Citra save file using Checkpoint


# Returning to Vanilla #
1. Make a backup of your Pokemon Star save with Checkpoint. Name it something like "PkmnStarSave".
2. Delete Pokemon Star from your 3DS.
3. If you play the digital version of UM, redownload it.
4. If you play the digital version of UM, load the backup of your Ultra Moon save.

# Credits #
Nintendo - Publisher of Ultra Sun and Ultra Moon

Game Freak - Developer of Ultra Sun and Ultra Moon

Rusyaeffy - Developer and Publisher of Pokemon Star

RadoMiami - Writer of this guide

AquaSamurott - Fixing a083 garc for console. (Didn't ask them to do this, but they just kinda announced it on New Year's Eve.)

# Changelog #
v0.1 (10/31/20): First sucessful experiment.
Banner and icons: Replaced.
Modded a083 garc: Probably still broken.
Thinking about trying to fix a083 garc: Some day...

v0.1.1 (11/1/20): Added US support via an xdelta patch.

Still v0.1.1 (12/31/20): AquaSamurott begins fixing a083 garc. Never asked them to do so, but glad they're doing it nonetheless.\

v0.1.2 (3/25/21): First prerelease of fixed a083. 
