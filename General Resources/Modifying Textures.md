# Modifying Textures

## This method is for the PS3 games only.

- First get the texture you want to edit. There are two ways of doing this:
    - **This method is only possible on RPCS3.** Rip the texture with RenderDoc ([video tutorial](https://youtu.be/TvdxSIbPz0w)).
    - Use the RPK unpacker to unpack the RPK. Go through the list of resulting files from largest to smallest, converting each one with the raw texture converter with offset `0x1B` until you find the texture you want to edit.
- Once you've got the source texture, open it in a hex editor and copy 30-ish bytes starting from `0x80`.
- Open the RPK in the hex editor and search for the bytes you just copied. You should now have the location of the raw DDS data in the RPK.
- Edit your texture and save it as DDS, with the same metadata as your source texture. You can use Compressonator to help with this.
- Open your edited texture in the hex editor, and select everything from `0x80` to the end.
- Copy it, and paste it in the same place as the original texture data in the RPK, replacing it.
- If the filesize is different, go to the 4 bytes immediately before the texture data. They form an unsigned integer, adjust that number to the size of the raw texture in bytes.
- If the resolution is different, go to the `EVOSBIG `/ `45 56 4F 53 42 49 47 20` before the texture, and skip 20 bytes. The next 2 bytes form an unsigned short which is the resolution in the x-axis. The 2 bytes after that form another unsigned short which is the resolution in the y-axis.
- Save the RPK, and you're done.
