# Recommended Tools

## All games
- [Cheat Engine](https://www.cheatengine.org) - Memory editing and debugging on PC.
- [010 Editor](https://www.sweetscape.com) - Hex editing. [HxD](https://mh-nexus.de) is a good free alternative.
- [Raw texture previewer/converter](https://forum.xentax.com/viewtopic.php?t=16461) - Calculates headers from raw DDS data to make them easily viewable.
- [Compressonator](https://gpuopen.com/compressonator/) - useful DDS tools including the ability to inspect metadata.

## PS3 games only
- [QuickBMS](http://aluigi.altervista.org/quickbms.htm) + [aluigi's RPK Unpacker](http://aluigi.org/bms/driveclub.bms) - Unpacks RPKs; the script is built for Driveclub but works fine with Motorstorm. It only (inaccurately) dumps the data between each EVOSBIG (EVOSLITL in the case of Driveclub) which we could already do anyway with a hex-editor, so it's not that useful (also cannot repack the files), but it's a start, since it at least automates the process.
- [NetCheat](http://netcheat.gamehacking.org/ncUpdater/ncUpdateDir.zip) - Memory editing on PS3.
- [ProDG Target Manager and Debugger](http://www.mediafire.com/file/ov227kvod21am8n/ProDG_v4.20.1.exe/file) - Debugging on PS3.
- [Ghidra](https://ghidra-sre.org) + [Ps3GhidraScripts](https://github.com/clienthax/Ps3GhidraScripts) - Helps to reverse engineer PS3 executables.

## Pacific Rift and Apocalypse only
- [PSArcTool](https://github.com/periander/PSArcTool) - Extracts and repacks .psarc files. Use the official [Sony SDK's PSARC Tool](https://disk.yandex.ru/d/iK9rk8jXieqLdw) as a fallback. `psarc.exe -h` for help.

## Pacific Rift only
- [RAD Video Tools](http://www.radgametools.com/bnkdown.htm) - Converts to and from the Bink Video .bik format.

## Arctic Edge only
- [QuickBMS](http://aluigi.altervista.org/quickbms.htm) + [Acewell's Arctic Edge .PAK Extractor](https://forum.xentax.com/download/file.php?id=15764) - Unpacks .PAK files but cannot repack them.
