## A lot of these descriptions are incomplete, they will be amended in future. Also, many of these files are actually useless, and they will be removed in time.

| File extension | Description
|:-:|:-
| .aci | Plaintext, specifies actions initiated by the action button.
| .aeb | Renamed **.smp**.
| .aec | Related to audio.<br><br>**Magic:**<br>`45 56 4F 53 42 49 47 20 41 45 43`<br>`EVOSBIG AEC`
| .aes | Contains **.aec**’s within it.<br><br>**Magic:**<br>`45 56 4F 53 42 49 47 20 41 45 53`<br>`EVOSBIG AES`
| .aid | Unknown, related to levels.
| .ain | Plaintext, related to levels.
| .ait | Plaintext, related to object triggers.
| .ams | *AniMationS file*; renamed **.rpk** related to GUI animations.
| .audionode | Plaintext, specifies locations of audio effects within levels.
| .avl | Plaintext, related to levels.
| .brain | Related to AI.
| .bridge | Plaintext, related to levels.
| .cam | Some are plaintext, others are not. Specifies the camera animation path used by the benchmark system.
| .camerawidget | Plaintext, related to levels.
| .cps | Renamed XML related to levels.
| .crv | Plaintext, related to levels.
| .crvb | Related to levels.
| .custom | Renamed XML related to events.
| .def | Plaintext, defines the name of the item.
| .flw | Plaintext, related to gui.
| .gag | Related to AI punches/insults/etc?
| .gags | Renamed XML related to gags in events.
| .gan | Renamed XML related to levels.
| .gpl | Related to splines.
| .graph | Unknown, only used by surfaces.graph.
| .gui | *Graphical User Interface file*; some are plaintext, others are renamed **.rpk**s.
| .gvl | Plaintext, related to levels.
| .gvlsrc | Plaintext, related to levels.
| .jump | Plaintext, related to levels.
| .lang | Contains localisation for strings. The start of the file is binary, but the rest of it is plaintext.
| .list | Plaintext, but uses null characters. Only used by text_langs.list.
| .mng | Audio post-processing effects. Filters are always 84 bytes, compressors are always 116 bytes, and all the reverb effects are 112 bytes. The other audio effects vary in size.<br><br>**Header:**<br>`4D 55 4C 54 00 00 00 XX XX XX XX XX XX XX XX XX`<br>`MULT...*********`<br><br>The type of audio effect is defined in the space:<br><br>**Compressor**<br>`30 46 44 5F 43 4F 4D 50 00`<br>`0FD_COMP.`<br><br>**Filter**<br>`10 46 49 4C 54 00 00 00 00`<br>`.FILT....`<br><br>**EQ**<br>`60 45 51 00 00 00 00 00 00`<br>\``EQ......`<br><br>**Reverb**<br>`2C 54 44 5F 52 56 45 52 42`<br>`,TD_RVERB`
| .nam | Plaintext, specifies sound associations for certain events (e.g. ambient sounds for tracks).
| .nvl | Plaintext, related to levels.
| .nvlsrc | Plaintext, related to levels.
| .packman | Renamed XML related to AI pace in events.
| .pck | Related to shaders.
| .reward | Plaintext, specifies rewards (e.g. when a certain Festival rank is reached).
| .rpk | [010 Editor Binary Template](https://github.com/Nenkai/010GameTemplates/blob/main/Evolution%20Studios/RPK_ResourcePack.bt) by [Nenkai](https://github.com/Nenkai). Intended for Driveclub but still works to an extent with MotorStorm.
| .rpv | Related to levels.
| .sad | Unknown, only used by ms_surfaces.sad.
| .smp | Contains multiple MP3 files seperated by `MSF MSF` / `4D 53 46 20 4D 53 46`.
| .spl | *SPLine file*; related to splines.
| .spugraph | Unknown, only used by surfaces.spugraph.
| .spvs | Related to levels.
| .stp | Plaintext, defines start points in a track.
| .ticket | Renamed XML related to events.
| .trg | Plaintext, defines shadowbounds-triggerboxes in a track.
| .trophy | Plaintext, related to trophies.
| .vfl | Related to levels.
| .vsb | Contains information on how to play sounds (e.g. pitch data). Not a VSampler SoundBank file; can’t be opened by any programs that can open real VSBs.<br><br>**Magic:**<br>`56 53 42 20 00 00 00 05`<br>`VSB ....`
| .wall | Related to levels.
| .wth | Plaintext, related to levels.
