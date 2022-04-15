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
| .cam | Some are plaintext, others are not. Specifies details of the camera panning sequence before a race.
| .camerawidget | Plaintext, related to levels.
| .cps | Renamed XML related to levels.
| .crv | Plaintext, related to levels.
| .crvb | Related to levels.
| .custom | Renamed XML related to events.
| .def | Plaintext, defines the name of the item.
| .flw | Plaintext, related to gui.
| .gag | Related to AI punches/insults/etc?
| .gan | Renamed XML, related to levels.
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
| .pck | Related to shaders.
| .reward | Plaintext, specifies rewards (e.g. when a certain Festival rank is reached).
| .rpk | Resource PacK file; proprietary Evolution Studios archive. They seem to be pretty inconsistently structured especially between games, hence why it's hard to go into detail about it.<br><br>**Header:**<br>`45 56 4F 53 42 49 47 20 00 00 00 12 52 65 73 6F`<br>`75 72 63 65 20 50 61 63 4B 20 66 69 6C 65 00 00`<br>`XX XX 00 00 00 26 45 56 4F 53 42 49 47 20 00 01`<br><br>`EVOSBIG ....Reso`<br>`urce PacK file..`<br>`**...&EVOSBIG ..`<br><br>**Basic Structure:**<ul><li>Header, then a section of 42 bytes, of which the function is unknown.<li>Filenames start at `0x5A` and are seperated by `.` / `00`. Irrelevant to the file's function, and length will obviously vary from RPK to RPK.<li>Then, the locations of the files and some other stuff from when the developers packed the file, seperated by `.` / `00`. Also irrelevant to the file's function, and length varies between RPKs.<li>After that, some unknown data (length is different for every RPK), and then the actual packed data will begin.<li>Packed data always begins with `EVOSBIG `/ `45 56 4F 53 42 49 47 20`. The following part of the structure depends on the filetype.<ul><li>For some files (one example being plaintext files such as XML) there is a section of 12 bytes of which the function is unknown, then the filesize in bytes (displayed as a 4-byte integer) and then the actual file data will follow.<li>Some other files (such as headerless DDS files) have a section of 31 bytes, then the filesize in bytes (displayed as a 4-byte integer) and then the actual file data will follow.<li>The rest of the files use other methods which I haven't figured out yet.</ul><li>At the end, a final `EVOSBIG `/ `45 56 4F 53 42 49 47 20` followed by some more unknown data (again, length is different for every RPK).
| .rpv | Related to levels.
| .sad | Unknown, only used by ms_surfaces.sad.
| .smp | Contains multiple MP3 files seperated by `MSF MSF` / `4D 53 46 20 4D 53 46`.
| .spl | *SPLine file*; related to splines.
| .spugraph | Unknown, only used by surfaces.spugraph.
| .spvs | Related to levels.
| .stp | Plaintext, defines start points in a track.
| .ticket | Renamed XML related to events.
| .trg | Plaintext, defines trigger boxes in a track.
| .trophy | Plaintext, related to trophies.
| .vfl | Related to levels.
| .vsb | Contains information on how to play sounds (e.g. pitch data). Not a VSampler SoundBank file; can’t be opened by any programs that can open real VSBs.<br><br>**Magic:**<br>`56 53 42 20 00 00 00 05`<br>`VSB ....`
| .wall | Related to levels.
| .wth | Plaintext, related to levels.
