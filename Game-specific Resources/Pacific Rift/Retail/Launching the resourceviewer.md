# Launching the resourceviewer
- Unpack \PS3_GAME\USRDIR\ms2.psarc.
- Make a folder called overrides in USRDIR.
- Copy fonts.rpk, global.rpk, post.rpk and the scripts folder into the overrides folder, along with any RPKs you want to load.
- Open \PS3_GAME\USRDIR\overrides\scripts\ and delete everything apart from host.lua.
- Delete everything from host.lua. This helps to launch the resourceviewer faster.
- Run resourceviewer_atg.self directly using your terminal, passing the filenames of RPKs you want to load as launch parameters seperated by spaces:
  - RPCS3:
    - Windows: .\rpcs3.exe [PATH_TO_GAME]\PS3_GAME\USRDIR\resourceviewer_atg.self [RPKs]
      - If your game version is not 1.00, this may not open the resourceviewer. You can either downgrade your game to 1.00, or a simple workaround is to copy overrides and resourceviewer_atg.self to a seperate directory (e.g. Desktop) and run the program from there.
    - Linux: -
    - macOS: -
  - PS3:
    - Target Manager

## Controls
- Look around: Left Stick
- Pan: L2 + Left Stick
  - Left/Right are inverted.
- Zoom: Right Stick Up/Down
