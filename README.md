# evans-moonlander-keyboard-config
This repository contains the custom keyboard layout and configurations I use with my [ZSA Moonlander keyboard](https://www.zsa.io/moonlander). It's pretty awesome (both the keyboard and the layout) and I use it every day for both work and gaming.

If you're interested in using this layout (or just want to view its layout/mappings/etc.), check it out on [Oryx](https://configure.zsa.io/moonlander/layouts/wwgZ3/latest/0) -- Oryx is the primary source of truth, has a lovely GUI editor, and you can flash your keyboard directly from your Chromium-based browser (or the [Keymapp native desktop app](https://www.zsa.io/flash)). This GitHub repo is more of a failsafe.

# Boilerplate guidance from the folks at ZSA (not me)

- Use the documentation at [https://docs.qmk.fm/](https://docs.qmk.fm/) to set up your environment for building your firmware.
- Build your layout against [https://github.com/zsa/qmk_firmware/](https://github.com/zsa/qmk_firmware/) which is our QMK fork (instead of qmk/qmk_firmware). This is what Oryx (the graphical configurator) uses, so it's guaranteed to work.
- Create a folder with a simple name (no spaces!) for your layout inside the qmk_firmware/keyboards/moonlander/keymaps/ folder.
- Copy the contents of the \*\_source folder (in the .zip you downloaded from Oryx) into this folder.
- Make sure you've set up your environment per the [QMK docs](https://docs.qmk.fm/#/newbs_getting_started?id=set-up-your-environment) so compilation would actually work.
- From your shell, make sure your working directory is qmk*firmware, then enter the command `make moonlander:_layout_`, substituting the name of the folder you created for "_layout_".
