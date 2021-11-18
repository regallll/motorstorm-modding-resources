# How to launch the campaign
- Launch the game and go to `0x36CA3B6A`.
- Once text has generated around it, set a breakpoint on write on that address.
- Keep running the process until `demo-sonylogo.gui` / `64 65 6D 6F 2D 73 6F 6E 79 6C 6F 67 6F 2E 67 75 69` appears before it.
- Replace this with `introvideo.gui.` / `69 6E 74 72 6F 76 69 64 65 6F 2E 67 75 69 00`. It's important that you use the null character.
- Remove the breakpoint and resume the process. You should now be greeted with the 'Press X Button' screen.
