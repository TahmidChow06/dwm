## Introduction
This is my fork of dwm.

## Patches
I have used **five** patches in this config.
They are described below:
* [gaps](https://dwm.suckless.org/patches/gaps) - Gaps between the window
* [actualfullscreen](https://dwm.suckless.org/patches/actualfullscreen) - super+f to fullscreen
* [alwayscenter](https://dwm.suckless.org/patches/alwayscenter/dwm-alwayscenter-20200625-f04cac6.diff) - It will open all floating window in center.
* [focusonclick](https://dwm.suckless.org/patches/focusonclick/) - It will disable the default sloppy focus.
* [barpadding](https://dwm.suckless.org/patches/barpadding/) - You can set padding in the bar.

## Installation
```
git clone https://github.com/TahmidChow06/neovim ~/.config/dwm
sudo make clean install
```

It will clone the config in ~/.config/dwm. and install dwm.


## Keybinding
Bindings that were changed are mentioned below:

|------------------|-------------------------------|
| Keybinding       | Description                   |
|------------------|-------------------------------|
| super+Enter      | To open St                    |
| super+shift+h    | Take current window to master |
| super+f          | full screen                   |
| super+ctrl+enter | to toggle floating layout     |
|------------------|-------------------------------|

And few bindings are also added. Like volume up, down and mute.
