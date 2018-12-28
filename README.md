# mech

> Support project for mechanical keyboards

## Compile

Please follow the instructions on the [QMK Firmware](https://qmk.fm/) website. If you have everything installed and
configured correctly, you should be able to run this command.

```bash
# dz60 is the 'keyboard' and neele_1 the 'keymap'
./scripts/build dz60:neele_1
``` 

Please exchange `neele_1` with whatever keymap you wanna build. If the build was successful, you can grab the firmware
file from the `./build` dir. We use the [QMK Toolbox](https://qmk.fm/toolbox/) to flash.

## Setup

You can use `./build/setup` to grab the lastest QMK Firmware. It will setup all folders for the *build* step. You can
also add new keymaps to `./keyboards/<keyboard>/keymaps/<your-keymap>`.

## Prerequisites

* [git](https://git-scm.com/)
