# Modifying Textures

## This method is for the RPK files in the PS3 games only ([video tutorial](https://youtu.be/4SSGGfZDP5c)).

- First get the texture you want to edit. There are two ways of doing this:
    - **This method is only possible on RPCS3.** Rip the texture with [RenderDoc](../General%20Resources/List%20of%20Tools.md#:~:text=debugging%20on%20PC.-,RenderDoc,-%2D%20Graphics%20debugging%20on) ([video tutorial](https://youtu.be/TvdxSIbPz0w)).
    - Use the RPK unpacker to unpack the RPK. Go through the list of resulting files from largest to smallest, converting each one with the raw texture converter with offset `0x1B` until you find the texture you want to edit. For Pacific Rift, the [Known texture metadata](../Game-specific%20Resources/Pacific%20Rift/Retail/Known%20texture%20metadata.md) table will help greatly.
- Edit your texture and save it as DDS, with the same metadata as your source texture. Make sure you don't overwrite your source texture. You can use [Compressonator](../General%20Resources/List%20of%20Tools.md#:~:text=them%20easily%20viewable.-,Compressonator,-%2D%20useful%20DDS%20tools) to help with this as well as the [Known texture metadata](../Game-specific%20Resources/Pacific%20Rift/Retail/Known%20texture%20metadata.md) table for Pacific Rift.
- Now, you need to replace the texture in the RPK. There are two ways of doing this:
    - Use [SIs_TexSwap](../General%20Resources/List%20of%20Tools.md#:~:text=RPCS3%20%2D%20PS3%20emulator.-,SIs_TexSwap,-%2D%20Small%20program%20which) and select the source texture, new texture and RPK when prompted.
    - **This method is more complicated and involves the use of a [hex editor](../General%20Resources/List%20of%20Tools.md#:~:text=010%20Editor%20%2D%20Hex%20editing.%20HxD%20is%20a%20good%20free%20alternative.). Only use this if the first method fails:**
        - Open the source texture in your hex editor and copy 30-ish bytes starting from `0x80`.
        - Open the RPK in the hex editor and search for the bytes you just copied. You should now have the location of the raw DDS data in the RPK.
        - Open your edited texture in the hex editor, and select everything from `0x80` to the end.
        - Copy it, and paste it in the same place as the original texture data in the RPK, replacing it.
        - If the filesize is different, go to the 4 bytes immediately before the texture data. They form an unsigned integer, adjust that number to the size of the raw texture in bytes.
        - If the resolution is different, go to the `EVOSBIG `/ `45 56 4F 53 42 49 47 20` before the texture, and skip 20 bytes. The next 2 bytes form an unsigned short which is the resolution in the x-axis. The 2 bytes after that form another unsigned short which is the resolution in the y-axis.
        - Save the RPK, and you're done.
