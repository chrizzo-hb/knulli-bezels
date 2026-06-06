Please read ALL of the intructions below before applying overlays and/or shaders. Note the Game Boy Pocket-specific instructions at the end.

Credits: 
- All LCD grids by 1playerinsertcoin (https://www.reddit.com/user/1playerinsertcoin/submitted/)
- Non-integer scale 720x720 NGP and NGPC bezel designs by KugelFanger

### Applying the Overlays

Due to the logic Knulli uses to select overlays and the associated naming conventions, I've divided my overlays into mutually exclusive decoration sets (integer scale with grids, integer scale without grids, non-integer scale with grids). Non-integer scale versions without grids are already included in default-knulli.

Coverage of devices/consoles is haphazard, and each of the four collections includes different combinations of systems (availability just depends on what overlays I've made so far). I suggest configuring on a system-by-system basis using the Per System Advanced Configuration menu so you can use other collections for missing systems (see the Knulli wiki for instructions on how to do this:

https://knulli.org/configure/customization/bezel-decorations/#system-bezel-decorations).

### Shader Preset for Grid Overlays

I've created a simple shader preset for use with my GBP, GBC, and NGPC grid overlays that applies the sharp-shimmerless and pixel transparency shaders. For all other systems, it just applies sharp-shimmerless (useful for non-integer scale overlays). If you want to give it a try, simply change the shader preset to mugwomp93-grids as per the directions in the Knulli wiki (https://knulli.org/configure/customization/shaders/). As with my overlays, I recommend configuring on a system-by-system basis using the Per System Advanced Configuration menu so you can use other shaders for missing systems (unless, of course, you want to apply sharp-shimmerless to everything).

### Game Boy Pocket Integer-Scale Grid Overlays

The Game Boy Pocket overlays are designed to work with the Special 4 (TI-83 Legacy) internal palette. To use this palette, do the following:

   1. Press Start at the main Knulli Menu
   2. Select Game Settings
   3. Select Per System Advanced Configuration (at the very bottom)
   4. Select Game Boy
   5. Navigate to Colorization and select Special 4 (TI-83 Legacy) (near the bottom)
   6. Use the B buton to back out to the main menu

I highly recommend using my shader preset with the GBP overlays as the overlay are adapted to account for the effect of the shader preset (the pixel transparency component, specifically). To do so, follow the instructions in the shader section above. If for, some reason, you don't want to use a shader with this overlay, select the gb-integer-scale-noshader version instead. You'll still need to change the colorization to Special 4 (TI-83 Legacy).