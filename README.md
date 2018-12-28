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

### Dependencies

On macOS you can use homebrew to get all necessary dependencies. This list might change and a more recent one can be
found at the [QMK Firmware repository](https://github.com/qmk/qmk_firmware/blob/master/docs/getting_started_build_tools.md).

```bash
brew tap osx-cross/avr
brew tap PX4/homebrew-px4
brew update
brew install avr-gcc@7
brew link --force avr-gcc@7
brew install dfu-programmer
brew install dfu-util
brew install gcc-arm-none-eabi
brew install avrdude
``` 

## Prerequisites

We have used the following tools to get our keyboards up and running. We use macOS, so this might be a bit different for
an other OS.

* [git](https://git-scm.com/)
* [homebrew](https://brew.sh/)
* [QMK Firmware](https://qmk.fm/)
* [QMK Toolbox](https://qmk.fm/toolbox/)
* [QMK Docs](https://docs.qmk.fm/#/)
