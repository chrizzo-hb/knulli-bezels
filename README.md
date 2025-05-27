# KNULLI Bezels

A compilation of bezels to be used with [KNULLI](https://knulli.org).

KNULLI is an open-source custom firmware (CFW) for **handheld** retro gaming devices. It is a fork of [Batocera](https://batocera.org).

This bezel set is maintained as a **multi-resolution bezel set** to be used with KNULLI. Since **KNULLI Firefly**, the CFW allows to use sets of bezels for multiple different resolutions ([read more here](https://github.com/knulli-cfw/distribution/pull/131)). Multi-resolution bezel sets allow the users to **choose a single bezel set** which will **work just as well** on the **built-in screen** of the handheld device as it does on a **16:9 TV set** when the device is plugged via HDMI.

To keep it lightweight, balanced, and consistent, this bezel pack contains

* **System-specific bezels** only (no game-specific bezels)
* **Hardware- and box-art focused designs** to take you back memory lane
* **Gridless** bezels only, no CRT effects
* **16:9 bezels** mostly adopted directly **from Batocera**
* **3:2 bezels** mostly adopted **from Batocera** with priority of **maxing out screen size** over integer scaling
* **1:1 bezels** with priority of **maxing out screen size** over integer scaling
* **4:3 bezels** with priority of **maxing out screen size** over integer scaling
* **No 4:3 bezels** for systems which were **designed for 4:3 screens**
  (Some games, e.g., games for SEGA Game Gear or Nintendo Entertainment System (NES), have a resolution which corresponds to an aspect ratio of 10:9 or 8:7. However, the actual screens the systems have been played on had an aspect ratio of 4:3 - [the pixels were stretched!](https://misterfpga.org/viewtopic.php?p=13816&sid=deab7f52c41ae361889bbe5b0986eee5#p13816) This bezel set does **not** aim for pixel-perfect integer scaling but for the aspect ratio of the original **screens**. Hence, there will be no bezels for 4:3 systems on 4:3 screens.)

Most of the bezel decorations in this set have **not** been created by myself. I only maintain this collection as a service to the retro-gaming community (and also for my own personal needs). You will find a detailed list of the sources of all the different bezels below.

## Installation

The KNULLI bezel set `default-knulli` comes **pre-installed** with KNULLI since the **Firefly** version. However, if the pre-installed version of the bezel set is outdated or if you wish to modify it to your liking, you can manually install it on your KNULLI device:

* **[Download](https://github.com/chrizzo-hb/knulli-bezels/archive/refs/heads/main.zip)** the bezel pack from this GitHub repository
* **unpack** the bezel pack (e.g., with [7Zip](https://www.7-zip.org/))
* **enable** the bezel pack on your KNULLI device by
    * **copying** the **entire folder** `default-knulli` to your KNULLI device into the `decorations` folder
    * **selecting** *DEFAULT-KNULLI* in the *Decorations* subsection of the *Game Settings*
    * (If you need any help with setting up the bezel set, do not worry, the KNULLI website has a [section on Bezel decorations](https://knulli.org/configure/customization/bezel-decorations/))

### Customization

If you like the pre-installed version of  `default-knulli` on your KNULLI device but would like to customize a little bit by replacing specific bezels, try the following:

* On your KNULLI device, select *DEFAULT-KNULLI* in the *Decorations* subsection of the *Game Settings*
* Create a new folder `default-knulli` inside your `decorations` folder
* Create a new folder `systems` inside the `default-knulli` folder
* Create a new folder `games` inside the `default-knulli` folder
* Put your preferred system- or game-specific bezel `png` files into the respective folder
* Mind the naming pattern:
    * `<system>-<aspect ratio>.png` for bezels with a specific aspect ratio, e.g. `mame-4_3.png` for a 4:3 aspect ratio 640x480 screen
    * `<system>-<rotation>-<aspect ratio>.png` for bezels for rotated games with a device-specific resolution, e.g. `mame-90-4_3.png` for running games which are rotated by 90° on a 4:3 aspect ratio 640x480 screen
* Add a corresponding `info` file for every bezel, e.g. `mame-4_3.info` for `mame-4_3.png`
    * `width` and `height` set the total screen resolution
    * `top`, `bottom`, `left`, and `right` are directional offsets from the respective borders of the screen
    * See example below

```
{
   "width":720,
   "height":480,
   "top":6,
   "left":48,
   "bottom":8,
   "right":51,
   "opacity":1.0000000,
   "messagex":0.220000,
   "messagey":0.120000
}
```

### Example: Replacing the GBA bezel decoration with a GBA SP variant

While the default GBA bezel works fine for most devices, users of clamshell devices, e.g., the Anbernic RG35XX SP, obviously prefer a GBA SP variant for their handhelds. Consequently, `default-knulli` comes with an SP variant for 4:3 displays.

You can use the customization options as explained above to **override** the default GBA bezel with a GBA SP bezel:

* On your KNULLI device, select *DEFAULT-KNULLI* in the *Decorations* subsection of the *Game Settings*
* Create a new folder `default-knulli` inside your `decorations` folder
* Create a new folder `systems` inside the `default-knulli` folder
* download the [gba-4_3.png](https://github.com/chrizzo-hb/knulli-bezels/blob/main/default-knulli-sp/systems/gba-4_3.png) bezel image from this repository
* download the [gba-4_3.info](https://github.com/chrizzo-hb/knulli-bezels/blob/main/default-knulli-sp/systems/gba-4_3.info) bezel info file from this repository
* Copy both files to your new `decorations/default-knulli/systems` folder
* Make sure to **rename** `gba-alt-4_3.png` to `gba-4_3.png`!

Now launch a GBA game and be amazed that your original GBA bezel has been replaced by the SP variant!

## Contribution

If you want to propose additions or changes to this bezel set, feel free to hand in a pull request anytime! However, please be aware that any bezel that might not match the overall theme of the set might be rejected. If you hand in a pull-request, make sure to add licensing information and links to the sources of the proposed bezels.

## License

All works in this repository are published under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/), unless they are covered by a different license. You will find links to the original sources, authors, and licenses in the sections below.

## 16:9 bezels

All 16:9 bezels have been adopted from [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel) and have been published under the [LGPL v3 License](https://www.gnu.org/licenses/lgpl-3.0.html), except for the bezels by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/).

## 3:2 bezels

All 3:2 bezels have been adopted from [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel) and have been published under the [LGPL v3 License](https://www.gnu.org/licenses/lgpl-3.0.html), except for the bezels listed below.

| System | Filename | Source |
| ------ | -------- | ------ |
| Amiga | `amiga-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Amiga 500 | `amiga500-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Atari 2600 | `atari2600-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Atari 5200 | `atari5200-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Atari 7800 | `atari7800-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| C64 | `c64-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Dreamcast | `dreamcast-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Game Gear | `gamegear-3_2` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| Gameboy | `gb-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Gameboy Color | `gbc-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Atari Lynx (horizontal) | `lynx-3_2` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), adapted and converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| Atari Lynx (vertical)| `lynx-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Master System | `mastersystem-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Mega Drive | `megadrive-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Megaduck | `megaduck-3_2` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| N64 | `n64-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| NeoGeo | `neogeo-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| NeoGeo CD | `neogeocd-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| NES | `nes-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| NeoGeo Pocket | `ngp-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| NeoGeo Pocket Color | `ngpc-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| PC Engine | `pcengine-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| PC Engine CD | `pcenginecd-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Pico-8 | `pico8-3_2` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| PlayStation Portable | `psp-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| PlayStation | `psx-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Saturn | `saturn-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| ScummVM | `saturn-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Sega 32x | `saturn-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Sega CD | `saturn-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| SG-1000 | `saturn-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| SNES | `snes-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| SNES MSU-1 | `snes_msu-1-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Supervision | `supervision-3_2` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| Virtual Boy | `virtualboy-3_2` | Overlay by [antiKk](https://github.com/antiKk/muOS-Overlays), converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| Wonderswan | `wswan-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Wonderswan (vertical) | `wswan-90-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Wonderswan Color | `wswanc-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Wonderswan Color (vertical) | `wswanc-90-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| X68000 | `x68000-90-3_2` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |

## 4:3 bezels

All bezels have been upscaled by [chrizzo-hb](https://github.com/chrizzo-hb) to 1024x768.

| System | Filename | Source |
| ------ | -------- | ------ |
| Default (vertical) | `default-90-4_3`, `default-270-4_3` | by [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 640x480 scale for vertical aspect ratio |
| FBNeo (vertical) | `fbneo-90-4_3`, `fbneo-270-4_3` | by [fabricecaruso](https://github.com/fabricecaruso) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 640x480 scale for vertical aspect ratio |
| MAME (vertical) | `fbneo-90-4_3`, `fbneo-270-4_3` | by [fabricecaruso](https://github.com/fabricecaruso) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 640x480 scale for vertical aspect ratio |
| Gameboy | `gb-4_3` | Perfect DMG-EX (no grid) by [mugwomp93](https://github.com/mugwomp93) |
| Gameboy Advance | `gba-4_3` | Perfect GBA (no grid) by [mugwomp93](https://github.com/mugwomp93) |
| Gameboy Advance SP | `gba-4_3` | Perfect GBA SP by [C1PH3RR](https://www.youtube.com/watch?v=3YU-_ZPXFhE), adopted by [chrizzo-hb] |
| Gameboy Color | `gbc-4_3` | Perfect GBC (no grid) by [mugwomp93](https://github.com/mugwomp93) |
| Atari Lynx (horizontal) | `lynx-4_3` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| Atari Lynx (vertical)| `lynx-4_3` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Megaduck | `megaduck-4_3` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| NeoGeo Pocket | `ngp-4_3` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| NeoGeo Pocket Color | `ngpc-4_3` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| Pico-8 | `pico8-4_3` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| PlayStation Portable | `psp-4_3` | Overlay by [chrizzo-hb](https://github.com/chrizzo-hb) |
| Pokemon Mini | `pokemini-4_3` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| Supervision | `supervision-4_3` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| Virtual Boy | `virtualboy-4_3` | Overlay by [antiKk](https://github.com/antiKk/muOS-Overlays), converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| WonderSwan | `wswan-4_3` | Overlay by [antiKk](https://github.com/antiKk/muOS-Overlays), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| WonderSwan Color | `wswanc-4_3` | Overlay by [antiKk](https://github.com/antiKk/muOS-Overlays), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |

## 1:1 bezels

| System | Filename | Source |
| ------ | -------- | ------ |
| Default (vertical) | `default-90-1_1`, `default-270-1_1` | by [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 720x720 scale for vertical aspect ratio |
| MAME | `fbneo-1_1` | by [gonejack](https://github.com/gonejack/rgb30) |
| FBNeo (vertical) | `fbneo-90-1_1`, `fbneo-270-1_1` | by [fabricecaruso](https://github.com/fabricecaruso) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 720x720 scale for vertical aspect ratio |
| MAME | `mame-1_1` | by [gonejack](https://github.com/gonejack/rgb30) |
| MAME (vertical) | `mame-90-1_1`, `mame-270-1_1` | by [fabricecaruso](https://github.com/fabricecaruso) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 720x720 scale for vertical aspect ratio |
| Amiga | `amiga-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Amiga 500 | `amiga500-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Amiga 600 | `amiga-600-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Amiga 1200 | `amiga-1200-600-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Amiga CD32 | `amigacd32-1200-600-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Amiga CDTV | `amigacdtv-1200-600-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Atari 2600 | `atari2600-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Atari 5200 | `atari5200-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Atari 7800 | `atari7800-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Atari Lynx | `lynx-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Atari Lynx (vertical) | `lynx-90-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| C64 | `c64-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| DOS | `dos-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Dreamcast | `dreamcast-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Famicom Disk System | `fds-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Gameboy | `gb-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width |
| Gameboy Advance | `gba-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Gameboy Color | `gbc-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width |
| Game Gear | `gamegear-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width |
| Master System | `mastersystem-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) |
| Mega Drive | `megadrive-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| N64 | `n64-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| NeoGeo | `neogeo-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| NeoGeo Pocket | `ngp-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width |
| NeoGeo Pocket Color | `ngpc-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width |
| NES | `nes-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| PC Engine | `pcengine-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width and PC Engine |
| PC Engine CD | `pcenginecd-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width and PC Engine CD |
| PlayStation | `psx-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| PlayStation Portable | `psp-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb) |
| ScummVM | `scummvm-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Sega 32X | `sega32x-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Sega CD | `segacd-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| SG-1000 | `sg1000-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| SNES | `snes-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| SNES MSU-1 | `snes_msu-1-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Virtualboy | `virtualboy-1_1` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb) |
| WonderSwan | `wswan-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| WonderSwan (vertical) | `wswan-90-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| WonderSwan Color | `wswan-90-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| WonderSwan Color (vertical) | `wswan-90-90-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| X68000 | `x68000-1_1` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
