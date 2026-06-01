Please read ALL of the intructions below before applying overlays and/or shaders. Note the Game Boy Pocket-specific instructions at the end.

*Credits: 
- All LCD grids by 1playerinsertcoin (https://www.reddit.com/user/1playerinsertcoin/submitted/)
- Non-integer scale 720x720 NGP and NGPC bezel designs by KugelFanger*

### Applying the Overlays

Due to the logic Knulli uses to select overlays and the associated naming conventions, I've divided my overlays into four mutually exclusive decoration sets (integer scale with grids, integer scale without grids, non-integer scale with grids, non-integer scale without grids). Coverage of devices/consoles is haphazard, and each of the four collections includes different combinations of systems (availability just depends on what overlays I've made so far). I suggest configuring on a system-by-system basis using the Per System Advanced Configuration menu so you can use other collections for missing systems (see the Knulli wiki for instructions on how to do this: https://knulli.org/configure/customization/bezel-decorations/#system-bezel-decorations).

Note that some systems have alternate versions included (denoted with hopefully self-explanatory suffixes). If you wish to use one of the alternate versions, simply delete or rename the main version and remove the suffix from the filename of your chosen version. For example, if you want to use the SP version of the 640x480 GBA overlay, you could first rename gba-640x480.png to gba-640x480_no_sp.png (or whatever) and then rename gba-640x480_sp.png to gba-640x480.png.

### Shader Preset for Grid Overlays

I've created a simple shader preset for use with my GBP, GBC, and NGPC grid overlays that applies the sharp-shimmerless and pixel transparency shaders. For all other systems, it just applies sharp-shimmerless. If you want to give it a try, simply extract the shaders folder to /userdata or the root of SD2 (depending on whether you have a 1 or 2 card setup), then follow the directions in the Knulli wiki (https://knulli.org/configure/customization/shaders/). As with my overlays, I recommend configuring on a system-by-system basis using the Per System Advanced Configuration menu so you can use other shaders for missing systems (unless, of course, you want to apply sharp-shimmerless to everything).

Shader download link:
https://github.com/mugwomp93/Knulli_Customization/blob/main/overlays/mugwomp93-grids-shaders.zip

### Game Boy Pocket Overlays

The Game Boy Pocket overlays are designed to work with the Special 4 (TI-83 Legacy) internal palette. To use this palette, do the following:

   1. Press Start at the main Knulli Menu
   2. Select Game Settings
   3. Select Per System Advanced Configuration (at the very bottom)
   4. Select Game Boy
   5. Navigate to Colorization and select Special 4 (TI-83 Legacy) (near the bottom)
   6. Use the B buton to back out to the main menu

If you want to use my sharp-shimmerless/pixel transparency shader preset with the GBP overlays, make sure to rename the png for the shader version of the overlay that's most relevant for your device as per the instructions above (i.e., rename gb-###x###_pixel_transparency_shader_version.png to gb-###x###.png). The colors of the shader and non-shader versions of these overlays are slightly different to account for the effect of the pixel transparency shader.*