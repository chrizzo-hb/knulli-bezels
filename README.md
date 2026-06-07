# KNULLI Bezels

This repository holds bezel sets for [KNULLI](https://knulli.org).

KNULLI is an open-source custom firmware (CFW) for **handheld** retro gaming devices. It is a fork of [Batocera](https://batocera.org).

These bezel sets are maintained as **multi-resolution bezel sets** to be used with KNULLI. Since **KNULLI Firefly**, the CFW allows to use sets of bezels for multiple different resolutions ([read more here](https://github.com/knulli-cfw/distribution/pull/131)). Multi-resolution bezel sets allow the users to **choose a single bezel set** which will **work just as well** on the **built-in screen** of the handheld device as it does on a **16:9 TV set** when the device is plugged via HDMI.

> [!IMPORTANT]
> The bezel sets you will find in this repository are **compatible with KNULLI versions above Gladiator**. They are **not** compatible with **Gladiator and below** versions of KNULLI. You find a bezel pack for **older KNULLI versions** in the [**legacy branch** of this repository](https://github.com/chrizzo-hb/knulli-bezels/tree/legacy-resolution-based-pattern/).

## Bezel Sets

In this repository you will find several KNULLI-compatible bezel sets:

### Default sets

The default sets are curated by [chrizzo-hb](https://github.com/chrizzo-hb). You will find detailed credits in the [documentation here](default-knulli.md).

* **default-knulli** is the default bezel set that comes with KNULLI and is enabled by default.
* **default-knulli-sp** should be used **only** for the Gameboy Advance (GBA) system. It contains alternate versions of the GBA bezel which say "Gameboy Advance SP" rather than just "Gameboy Advance". This set is popular with clamshell device users.

### Generic sets

A simple generic multi-purpose bezel decoration (e.g. for Ports), created by [chrizzo-hb](https://github.com/chrizzo-hb) and based on the background image by [angel77lopez](https://forums.pimoroni.com/t/new-artwork-for-picade-cabinet/2618/495). It is intended to match with the [Knulli Bootlogo by chrizzo-hb](https://github.com/chrizzo-hb/knulli-bootlogo).

* **generic-4-by-3** should be used on 4:3 content (e.g., if you play a 4:3 game on a 16:9 or 1:1 screen).
* **generic-16-by-9** should be used on 16:9 content (e.g., if you play a 16:9 game on a 4:3 or 1:1 screen).

### mugwomp93 sets

These sets are contributed by [mugwomp93](https://github.com/mugwomp93). You will find detailed credits in the [documentation here](mugwomp93.md).

> [!IMPORTANT]
> Mind that mugwomp93 integer scaling bezels are **best used** with the corresponding mugwomp93-grids shader!

* **mugwomp93-integer-grids** a set of bezels which implicitly do **integer scaling** and come with **grids**.
* **mugwomp93-integer-grids-gb-noshader** an alternate set of Gameboy (GB) bezels which implicitly do integer scaling and come with grids. This version should **not** to be used with the mugwomp93-grids shader.
* **mugwomp93-integer-nogrids** a set of bezels which implicitly do **integer scaling** but do **not** come with grids.
* **mugwomp93-noninteger-grids** a set of bezels which do **not** do any integer scaling (so they max out on your screen while maintaining aspect ratio) but come with **grids**.
* **mugwomp93-noninteger-grids-sp** an alternate set of Gameboy Advance (GBA) bezels which do **not** do any integer scaling (so they max out on your screen while maintaining aspect ratio) but come with **grids**. It contains alternate versions of the GBA bezel which say "Gameboy Advance SP" rather than just "Gameboy Advance". This set is popular with clamshell device users.
* **mugwomp93-noninteger-nogrids** a set of bezels which **neither** do integer scaling **nor** come with any grids. The bezels in this set are also used in the **default-knulli** set.

## Installation

Some of the bezel sets, e.g., the `default-knulli` set, comes **pre-installed** with KNULLI ever since the **Firefly** version. However, if the pre-installed version of the bezel set is outdated or if you wish to modify it to your liking, you can manually install it on your KNULLI device:

* **[Download](https://github.com/chrizzo-hb/knulli-bezels/archive/refs/heads/main.zip)** the bezel pack from this GitHub repository
* **unpack** the bezel pack (e.g., with [7Zip](https://www.7-zip.org/))
* **enable** the bezel pack on your KNULLI device by
    * **copying** the **entire folder** `default-knulli` to your KNULLI device into the `decorations` folder
    * **selecting** *DEFAULT-KNULLI* in the *Decorations* subsection of the *Game Settings*
    * (If you need any help with setting up the bezel set, do not worry, the KNULLI website has a [section on Bezel decorations](https://knulli.org/configure/customization/bezel-decorations/))

### Customization

> [!IMPORTANT]
> Since the release of **KNULLI Gladiator**, the **naming pattern has changed** from a **resolution-based** pattern to an **aspect-ratio-based pattern**. Hence, the instructions below are only compatible with KNULLI versions **above** Gladiator!
>
> You will find the instructions for **KNULLI Gladiator and below** in the [**legacy branch** of this repository](https://github.com/chrizzo-hb/knulli-bezels/tree/legacy-resolution-based-pattern?tab=readme-ov-file#customization).

Let's say, for arguments sake, that you like the pre-installed version of  `default-knulli` on your KNULLI device but you would like to customize a little bit by replacing specific bezels. In this case, try the following:

* On your KNULLI device, select *DEFAULT-KNULLI* in the *Decorations* subsection of the *Game Settings*
* Create a new folder `default-knulli` inside your `decorations` folder
* Create a new folder `systems` inside the `default-knulli` folder
* Create a new folder `games` inside the `default-knulli` folder
* Put your preferred system- or game-specific bezel `png` files into the respective folder
* Mind the naming pattern:
    * `<system>-<aspect ratio>.png` for bezels with a specific **aspect ratio**, e.g. `mame-4_3.png` for a 4:3 aspect ratio screen
	* `<system>-<resolution>.png` for bezels with a specific **resolution**, e.g. `mame-1024x768.png` for a 1024x768 screen
    * `<system>-<rotation>-<aspect ratio>.png` **or** `<system>-<rotation>-<resolution>.png` for bezels for rotated games with a device-specific aspect ratio or resolution, e.g. `mame-90-4_3.png` for running games which are rotated by 90° on a 4:3 aspect ratio screen
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

> [!IMPORTANT]
> Since the release of **KNULLI Gladiator**, the **naming pattern has changed** from a **resolution-based** pattern to an **aspect-ratio-based pattern**. Hence, the instructions below are only compatible with KNULLI versions **above** Gladiator!
>
> You will find the instructions for **KNULLI Gladiator and below** in the [**legacy branch** of this repository](https://github.com/chrizzo-hb/knulli-bezels/tree/legacy-resolution-based-pattern?tab=readme-ov-file#example-replacing-the-gba-bezel-decoration-with-a-gba-sp-variant).

> [!TIP]
> You can simply enable the SP-specific GBA bezel decoration via EmulationStation: Go to the Gameboy Advance system and press *Select* to bring up the system menu, then go to *Advanced System Options*. Find *Decorations* and set *Decoration Set* to *DEFAULT-KNULLI-SP*. (The set does **only** contain 4:3 and 16:9 bezel decorations for GBA!)
>
> However, for the purpose of learning  from an example how to override bezel decorations manually, you might also follow the steps below.

While the default GBA bezel works fine for most devices, users of clamshell devices, e.g., the Anbernic RG35XX SP, obviously prefer a GBA SP variant for their handhelds. Consequently, `default-knulli` comes with an SP variant for 4:3 displays.

You can use the customization options as explained above to **override** the default GBA bezel with a GBA SP bezel:

* On your KNULLI device, select *DEFAULT-KNULLI* in the *Decorations* subsection of the *Game Settings*
* Create a new folder `default-knulli` inside your `decorations` folder
* Create a new folder `systems` inside the `default-knulli` folder
* download the [gba-4_3.png](https://github.com/chrizzo-hb/knulli-bezels/blob/main/default-knulli-sp/systems/gba-4_3.png) bezel image from this repository
* download the [gba-4_3.info](https://github.com/chrizzo-hb/knulli-bezels/blob/main/default-knulli-sp/systems/gba-4_3.info) bezel info file from this repository
* Copy both files to your new `decorations/default-knulli/systems` folder

Now launch a GBA game and be amazed that your original GBA bezel has been replaced by the SP variant!

## Contribution

If you want to propose additions or changes to this bezel library, feel free to hand in a pull request anytime! If you hand in a pull-request, make sure to add licensing information and links to the sources of the proposed bezels if they aren't your own creation!

## License

All works in this repository are published under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/), unless they are covered by a different license. You will find links to the original sources, authors, and licenses in the credits pages:

* [**default-knulli** credits](default-knulli.md)
* **generic** created by [chrizzo-hb](https://github.com/chrizzo-hb), based on a background image by [angel77lopez]
* [**mugwomp93** credits](mugwomp93.md)
