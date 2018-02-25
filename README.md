# My macOS Whitefox keyboard configuration

This is my configuration for the  [Whitefox keyboard](https://input.club/whitefox/) (True Fox layout)

![macOS compatible configuration for the Whitefox keyboard](https://raw.githubusercontent.com/crosbyhayton/whitefox/master/assets/kiibohd-config.png)

## Key Features

* Modifier keys are set according to Apple’s standard.
* Includes functions keys for media, volume/mute, eject
* F16 & F17 keys — I use F16 as a cough button for calls with [Shush](http://mizage.com/shush/), and F17 for a [Keyboard Maestro](https://www.keyboardmaestro.com/main/) palette.
* [Hyper key](http://brettterpstra.com/2012/12/08/a-useful-caps-lock-key/)— My layout uses some custom KLL via the [kiibohd configurator](https://github.com/kiibohd/configurator)  to remap the Caps Lock key to Command+Control+Option+Shift, which is useful for mapping systemwide keyboard shortcuts with Keyboard Maestro, inspired by [Brett Terpstra’s post](http://brettterpstra.com/2012/12/08/a-useful-caps-lock-key/).
* 6/N-KRO switch in case media keys stop working in Windows 10, based on [this layout](https://github.com/boyvanamstel/Whitefox-keyboard-macOS-configuration).

## Hyper key custom KLL
The KLL to remap Caps Lock to Hyper is:

`U"CAPSLOCK" : U"LCTRL" + U"LSHIFT" + U"LALT" + U"LGUI";`

Here is what it looks like inserted into the base layer in kiibohd configurator:

![Custom kll for macOS hyperkey](https://raw.githubusercontent.com/crosbyhayton/whitefox/master/assets/kiibohd-custom-kll.png)

Holding Caps Lock now functions as holding all modifier keys, and caps lock functionality is still available on the f1 layer.

## Installation
1. [Download a copy of the configuration file.](https://github.com/crosbyhayton/whitefox/archive/master.zip)
2. [Follow the Input Club guide to install the customized firmware.](https://input.club/configurator-setup/)

## Modifying
If you would like to modify this layout, I’d recommend you import WhiteFox-TrueFoxBlank.json into the [kiibohd configurator](https://github.com/kiibohd/configurator). I have not tested the firmware with the Input Club online configurator.
