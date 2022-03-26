# How to launch the campaign

## For RPCS3 on Windows, you can use this Lua script with Cheat Engine
```
openProcess('rpcs3.exe')
debugProcess()

debug_setBreakpoint(0x336CA3B58,1,bptWrite)

function debugger_onBreakpoint()

  local check = readQword(0x336CA3B49)

  if (check==7957705705567118692) then
    writeBytes(0x336CA3B49,0x69, 0x6E, 0x74, 0x72, 0x6F, 0x76, 0x69, 0x64, 0x65, 0x6F, 0x2E, 0x67, 0x75, 0x69, 0x00)
    return 0
  else
    return 1
  end
end
```

## For all other platforms
- Launch the game and go to `0x36CA3B6A`.
- Once text has generated around it, set a breakpoint on write on that address.
- Keep running the process until `demo-sonylogo.gui` / `64 65 6D 6F 2D 73 6F 6E 79 6C 6F 67 6F 2E 67 75 69` appears before it.
- Replace this with `introvideo.gui.` / `69 6E 74 72 6F 76 69 64 65 6F 2E 67 75 69 00`. It's important that you use the null character.
- Remove the breakpoint and resume the process. You should now be greeted with the 'Press X Button' screen.
