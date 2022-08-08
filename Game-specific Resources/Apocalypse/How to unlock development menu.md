# How to unlock development menu

## If you are on game version 1.00 with RPCS3, use the 'Enable Dev Menu' patch. For all other cases, follow this method
- Unpack ms3patchv0106.psarc (or whatever your game is updated to; if 1.00 then unpack ms3.psarc).
- Uncomment and then remove the ignoreinbuild tags from these, found in carrier_menus.xml:
![Screenshot_1](https://user-images.githubusercontent.com/87031973/183462997-65e0d9c5-44ae-4310-b478-19cf61d693ba.png)
![Screenshot_2](https://user-images.githubusercontent.com/87031973/183463002-0fbffe90-9139-4eba-a520-ded04041413d.png)
- Remove this ignoreinbuild tag from skin.xml:
![Screenshot_3](https://user-images.githubusercontent.com/87031973/183463283-280266f6-54d2-410d-a390-bbe94acf78eb.png)
- Repack these files into the PSARC.
