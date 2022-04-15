# Recommended Tools

## All games
- [Cheat Engine](https://www.cheatengine.org) - Memory editing and debugging on PC.
- [010 Editor](https://www.sweetscape.com) - Hex editing. [HxD](https://mh-nexus.de) is a good free alternative.
- [Raw texture previewer/converter](https://forum.xentax.com/viewtopic.php?t=16461) - Calculates headers from raw DDS data to make them easily viewable.
- [Compressonator](https://gpuopen.com/compressonator/) - useful DDS tools including the ability to inspect and modify metadata.

## PS3 games only
- [RPCS3](https://rpcs3.net) - PS3 emulator.
- [SIs_TexSwap](https://cdn.discordapp.com/attachments/578652989166845965/963114233921425478/SIs_TexSwap.exe) - *Small program which makes texture swapping automatic. You provide it the original texture you've extracted, the texture you want to inject, a file you want to make the swap in - and it does the job. It doesn't check if the files you've provided it are correct or not, but it does automatically make a backup of a target file in case you've picked something wrong.*
- [QuickBMS](http://aluigi.altervista.org/quickbms.htm) + [aluigi's RPK Unpacker](http://aluigi.org/bms/driveclub.bms) - Unpacks RPKs; the script is built for Driveclub but works fine with Motorstorm. It only (inaccurately) dumps the data between each EVOSBIG (EVOSLITL in the case of Driveclub) which we could already do anyway with a hex-editor, so it's not that useful (also cannot repack the files), but it's a start, since it at least automates the process.
- [NetCheat](http://netcheat.gamehacking.org/ncUpdater/ncUpdateDir.zip) - Memory editing on PS3.
- [ProDG Target Manager and Debugger](http://www.mediafire.com/file/ov227kvod21am8n/ProDG_v4.20.1.exe/file) - Debugging on PS3.
- [Ghidra](https://ghidra-sre.org) + [Ps3GhidraScripts](https://github.com/clienthax/Ps3GhidraScripts) - Helps to reverse engineer PS3 executables.

## Pacific Rift and Apocalypse only
- [PSArcTool](https://github.com/periander/PSArcTool) - Extracts and repacks .psarc files. Use the official [Sony SDK's PSARC Tool](https://disk.yandex.ru/d/iK9rk8jXieqLdw) as a fallback. `psarc.exe -h` for help.

## Pacific Rift only
- [RAD Video Tools](http://www.radgametools.com/bnkdown.htm) - Converts to and from the Bink Video .bik format.

## Arctic Edge only
- [PPSSPP](https://www.ppsspp.org) - PSP emulator.
- [PCSX2](https://pcsx2.net) - PS2 emulator.
- [QuickBMS](http://aluigi.altervista.org/quickbms.htm) + [Acewell's Arctic Edge .PAK Extractor](https://forum.xentax.com/download/file.php?id=15764) - Unpacks .PAK files but cannot repack them.
