# KNULLI Bezels

A compilation of bezels to be used with [KNULLI](https://knulli.org).

KNULLI is an open-source custom firmware (CFW) for **handheld** retro gaming devices. It is a fork of [Batocera](https://batocera.org).

This bezel set is maintained as a **multi-resolution bezel set** to be used with KNULLI. Since **KNULLI Firefly**, the CFW allows to use sets of bezels for multiple different resolutions ([read more here](https://github.com/knulli-cfw/distribution/pull/131)). Multi-resolution bezel sets allow the users to **choose a single bezel set** which will **work just as well** on the **built-in screen** of the handheld device as it does on a **16:9 TV set** when the device is plugged via HDMI.

To keep it lightweight, balanced, and consistent, this bezel pack contains

* **System-specific bezels** only (no game-specific bezels)
* **Hardware- and box-art focused designs** to take you back memory lane
* **Gridless** bezels only, no CRT effects
* **16:9 bezels** mostly adopted directly **from Batocera**
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

## Contribution

If you want to propose additions or changes to this bezel set, feel free to hand in a pull request anytime! However, please be aware that any bezel that might not match the overall theme of the set might be rejected. If you hand in a pull-request, make sure to add licensing information and/or links to the source of the proposed bezels.

## License

All works in this repository are published under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/), unless they are covered by a different license. You will find links to the original sources, authors, and licenses in the sections below.

## 16:9 (1920x1080) bezels

All 16:9 bezels have been adopted from [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel) and have been published under the [LGPL v3 License](https://www.gnu.org/licenses/lgpl-3.0.html), except for the bezels by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License].

## 3:2 (720x480) bezels

All 3:2 bezels have been adopted from [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel) and have been published under the [LGPL v3 License](https://www.gnu.org/licenses/lgpl-3.0.html), except for the bezels listed below.

| System | Filename | Source |
| ------ | -------- | ------ |
| Amiga | `amiga`, `amiga-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Amiga 500 | `amiga500`, `amiga500-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Atari 2600 | `atari2600`, `atari2600-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Atari 5200 | `atari5200`, `atari5200-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Atari 7800 | `atari7800`, `atari7800-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| C64 | `c64`, `c64-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Dreamcast | `dreamcast`, `dreamcast-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Game Gear | `gamegear-720x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| Gameboy | `gb`, `gb-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Gameboy Color | `gbc`, `gbc-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Atari Lynx (horizontal) | `lynx-720x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), adapted and converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| Atari Lynx (vertical)| `lynx-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Master System | `mastersystem-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Mega Drive | `megadrive-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Megaduck | `megaduck-720x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| N64 | `n64-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| NeoGeo | `neogeo-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| NeoGeo CD | `neogeocd-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| NES | `nes-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| NeoGeo Pocket | `ngp-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| NeoGeo Pocket Color | `ngpc-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| PC Engine | `pcengine-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| PC Engine CD | `pcenginecd-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Pico-8 | `pico8-720x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| PlayStation Portable | `psp-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| PlayStation | `psx-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| SNES | `snes`, `snes-720x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |

## 4:3 (640x480) bezels

| System | Filename | Source |
| ------ | -------- | ------ |
| Default (vertical) | `default-90-640x480`, `default-270-640x480` | by [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 640x480 scale for vertical aspect ratio |
| FBNeo (vertical) | `fbneo-90-640x480`, `fbneo-270-640x480` | by [fabricecaruso](https://github.com/fabricecaruso) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 640x480 scale for vertical aspect ratio |
| MAME (vertical) | `fbneo-90-640x480`, `fbneo-270-640x480` | by [fabricecaruso](https://github.com/fabricecaruso) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 640x480 scale for vertical aspect ratio |
| Gameboy | `gb-640x480` | Perfect DMG-EX (no grid) by [mugwomp93](https://github.com/mugwomp93) |
| Gameboy Advance | `gba-640x480` | Perfect GBA (no grid) by [mugwomp93](https://github.com/mugwomp93) |
| Gameboy Advance SP (alternative) | `gba-alt-640x480` | Perfect GBA SP (no grid) by [mugwomp93](https://github.com/mugwomp93) |
| Gameboy Color | `gbc-640x480` | Perfect GBC (no grid) by [mugwomp93](https://github.com/mugwomp93) |
| Atari Lynx (horizontal) | `lynx-640x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| Atari Lynx (vertical)| `lynx-640x480` | by [Duimon](https://github.com/Duimon) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), published under a [Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License] |
| Megaduck | `megaduck-640x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| NeoGeo Pocket | `ngp-640x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| NeoGeo Pocket Color | `ngpc-640x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| Pico-8 | `pico8-640x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| PlayStation Portable | `psp-640x480` | Overlay by [chrizzo-hb](https://github.com/chrizzo-hb) |
| Pokemon Mini | `pokemini-640x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| Supervision | `supervision-640x480` | Overlay by [drkhrse](https://github.com/drkhrse/drkhrse_miyoo_bezels), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| Virtual Boy | `virtualboy-640x480` | Overlay by [antiKk](https://github.com/antiKk/muOS-Overlays), converted to Batocera format by [chrizzo-hb](https://github.com/chrizzo-hb) |
| WonderSwan | `wswan-640x480` | Overlay by [antiKk](https://github.com/antiKk/muOS-Overlays), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |
| WonderSwan Color | `wswanc-640x480` | Overlay by [antiKk](https://github.com/antiKk/muOS-Overlays), converted to Batocera format by [nvitaterna](https://github.com/nvitaterna/batocera_4_3_handheld_bezels) |

## 4:3 (1024x768) bezels

Same as 640x480. All bezels have been upscaled by [chrizzo-hb](https://github.com/chrizzo-hb) to 1024x768.

## 1:1 (720x720) bezels

| System | Filename | Source |
| ------ | -------- | ------ |
| Default (vertical) | `default-90-720x720`, `default-270-720x720` | by [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 720x720 scale for vertical aspect ratio |
| MAME | `fbneo-720x720` | by [gonejack](https://github.com/gonejack/rgb30) |
| FBNeo (vertical) | `fbneo-90-720x720`, `fbneo-270-720x720` | by [fabricecaruso](https://github.com/fabricecaruso) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 720x720 scale for vertical aspect ratio |
| MAME | `mame-720x720` | by [gonejack](https://github.com/gonejack/rgb30) |
| MAME (vertical) | `mame-90-720x720`, `mame-270-720x720` | by [fabricecaruso](https://github.com/fabricecaruso) for [Batocera Bezels](https://github.com/batocera-linux/batocera-bezel), adopted by [chrizzo-hb](https://github.com/chrizzo-hb) to 720x720 scale for vertical aspect ratio |
| Amiga | `amiga-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Amiga 500 | `amiga500-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Amiga 600 | `amiga-600-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Amiga 1200 | `amiga-1200-600-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Amiga CD32 | `amigacd32-1200-600-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Amiga CDTV | `amigacdtv-1200-600-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Atari 2600 | `atari2600-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Atari 5200 | `atari5200-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Atari 7800 | `atari7800-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Atari Lynx | `lynx-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Atari Lynx (vertical) | `lynx-90-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| C64 | `c64-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| DOS | `dos-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Dreamcast | `dreamcast-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Famicom Disk System | `fds-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Gameboy | `gb-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width |
| Gameboy Advance | `gba-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Gameboy Color | `gbc-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width |
| Game Gear | `gamegear-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width |
| Master System | `mastersystem-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) |
| Mega Drive | `megadrive-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| N64 | `n64-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| NeoGeo | `neogeo-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| NeoGeo Pocket | `ngp-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width |
| NeoGeo Pocket Color | `ngpc-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width |
| NES | `nes-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| PC Engine | `pcengine-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width and PC Engine |
| PC Engine CD | `pcenginecd-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) adopted by [chrizzo-hb](https://github.com/chrizzo-hb) for max width and PC Engine CD |
| PlayStation | `psx-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| PlayStation Portable | `psp-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb) |
| ScummVM | `scummvm-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb), based on DOSBox Overlay by [Ifan](https://forums.libretro.com/t/dosbox-overlay/19236) |
| Sega 32X | `sega32x-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Sega CD | `segacd-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| SG-1000 | `sg1000-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| SNES | `snes-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| SNES MSU-1 | `snes_msu-1-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| Virtualboy | `virtualboy-720x720` | Bezel by [chrizzo-hb](https://github.com/chrizzo-hb) |
| WonderSwan | `wswan-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| WonderSwan (vertical) | `wswan-90-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| WonderSwan Color | `wswan-90-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| WonderSwan Color (vertical) | `wswan-90-90-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
| X68000 | `x68000-720x720` | Boxart Bezel by [Vidnez](https://github.com/Vidnez/Boxart-Bezels-for-RGB30) |
