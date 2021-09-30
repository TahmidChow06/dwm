## Introduction
This is my fork of [dwm](https://dwm.suckless.org).

## Patches
I have used **five** patches in this config.
They are described below:
* [gaps](https://dwm.suckless.org/patches/gaps) - Gaps between the window
* [actualfullscreen](https://dwm.suckless.org/patches/actualfullscreen) - super+f to fullscreen
* [alwayscenter](https://dwm.suckless.org/patches/alwayscenter) - It will open all floating window in center.
* [focusonclick](https://dwm.suckless.org/patches/focusonclick/) - It will disable the default sloppy focus.
* [barpadding](https://dwm.suckless.org/patches/barpadding/) - You can set padding in the bar.

## ScreenShot
By default value of gaps and barpadding are set to 0. Change the
following value if you want your dwm look like below:

```
static const unsigned int gappx     = 5;        /* gaps between windows */
static const int vertpad            = 10;       /* vertical padding of bar */
static const int sidepad            = 10;       /* horizontal padding of bar */
```

![DWM Image](screenshot/dwm.png)

The above bar is [slstatus](https://tools.suckless.org/slstatus). If you want to get my slstatus get it from [here](https://github.com/TahmidChow06/slstatus).

## Installation
```
git clone https://github.com/TahmidChow06/neovim ~/.config/dwm
sudo make install
```

It will clone the config in ~/.config/dwm. and install dwm.


## Keybinding
Bindings that were changed are mentioned below:

| Keybinding       | Description                   |
|------------------|-------------------------------|
| super+Enter      | To open St                    |
| super+shift+h    | Take current window to master |
| super+f          | full screen                   |
| super+ctrl+enter | to toggle floating layout     |

And few bindings are also added. Like volume up, down and mute.

## Pywal
This fork of dwm by default uses pywal by default.  Make sure to change the `tahmid` with your username.
If you don't have pywal or want to use the exact colorscheme I have then, add the following to your config:

```
static const char norm_fg[] = "#b7b6ba";
static const char norm_bg[] = "#101010";
static const char norm_border[] = "#807f82";

static const char sel_fg[] = "#101010";
static const char sel_bg[] = "#595C63";
static const char sel_border[] = "#b7b6ba";

static const char *colors[][3]      = {
    /*               fg           bg         border                         */
    [SchemeNorm] = { norm_fg,     norm_bg,   norm_border }, // unfocused wins
    [SchemeSel]  = { sel_fg,      sel_bg,    sel_border },  // the focused win
};

```

also remove or comment out this line.
```
#include "/home/tahmid/.cache/wal/colors-wal-dwm.h"
```
