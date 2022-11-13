## A lot of these descriptions are incomplete, they will be amended in future. Also, many of these files are actually useless, and they will be removed in time.

| File extension | Description
|:-:|:-
| .aci | Plaintext, specifies actions initiated by the action button.
| .aeb | Renamed **.smp**.
| .aes | Contains **.aec**’s within it.<br><br>**Magic:**<br>`45 56 4F 53 42 49 47 20 41 45 53`<br>`EVOSBIG AES`
| .ainodes | Renamed XML, related to AI behaviour within tracks.
| .ait | Plaintext, related to object triggers.
| .aps | Unknown, only used by mixtoolparamset.aps.<br><br>**Magic:**<br>`45 56 4F 53 41 50 53`<br>`EVOSAPS`
| .audionode | Plaintext, specifies locations of audio effects within levels.
| .cam | Some are plaintext, others are not. Specifies details of the camera panning sequence before a race.
| .checkpoints | Renamed XML related to AI nodes.
| .control | Plaintext, only used by editor.control. Related to GUI.
| .dec | Plaintext, related to UV mapping.
| .fnpvs | Renamed XML related to tracks.
| .gags | Renamed XML, related to events.
| .gameobjects | Renamed XML, related to events.
| .gtf | Decal files. Use the raw texture converter with offset `0x80` and DXT5 format to convert them to DDS.
| .gvl | Plaintext, related to levels.
| .ins | Plaintext, related to the livery editor.
| .jump | Plaintext, related to levels.
| .lang | Contains localisation for strings. The start of the file is binary, but the rest of it is plaintext.
| .liv | Unknown, related to liveries.<br><br>**Magic:**<br>`42 30 30 31 52 30 30 30 00 00 00`<br>`B001R000...`
| .lst | Plaintext list.
| .mng | Audio post-processing effects. Filters are always 84 bytes, compressors are always 116 bytes, and all the reverb effects are 112 bytes. The other audio effects vary in size.<br><br>**Header:**<br>`4D 55 4C 54 00 00 00 XX XX XX XX XX XX XX XX XX`<br>`MULT...*********`<br><br>The type of audio effect is defined in the space:<br><br>**Compressor**<br>`30 46 44 5F 43 4F 4D 50 00`<br>`0FD_COMP.`<br><br>**Filter**<br>`10 46 49 4C 54 00 00 00 00`<br>`.FILT....`<br><br>**EQ**<br>`60 45 51 00 00 00 00 00 00`<br>\``EQ......`<br><br>**Reverb**<br>`2C 54 44 5F 52 56 45 52 42`<br>`,TD_RVERB`
| .mode | Renamed XML, specifies parameters for gamemodes.
| .nam | Plaintext, specifies sound associations for certain events (e.g. ambient sounds for tracks).
| .npcs | Renamed XML, related to NPCs.
| .npvs | Renamed XML, related to tracks.
| .packman | Renamed XML related to events.
| .pck | Related to shaders.
| .pld | *PLantDefs file*; renamed XML, only used for plantdefs.pld.
| .reward | Plaintext, specifies rewards (e.g. when a certain Festival rank is reached).
| .rpk | [010 Editor Binary Template](https://github.com/Nenkai/010GameTemplates/blob/main/Evolution%20Studios/RPK_ResourcePack.bt)
| .sad | Unknown, only used by ms_surfaces.sad.
| .smp | Contains multiple MP3 files seperated by `MSF MSF` / `4D 53 46 20 4D 53 46`. 
| .splinefollowers | Renamed XML, related to tracks.
| .tln | *TimeLiNe file*; renamed XML file related to timelines.
| .vsb | Contains information on how to play sounds (e.g. pitch data). Not a VSampler SoundBank file; can’t be opened by any programs that can open real VSBs.<br><br>**Magic:**<br>`56 53 42 20 00 00 00 05`<br>`VSB ....`
| .vsi | Contains vehicle icons for the livery editor. They are simply raw DDS data so can be converted with the raw texture converter in DXT5 format with resolution 256x256. To convert them back to **.vsi** simply remove the DDS header (first 128 bytes).
| .wacd | Unknown.
