# Old English Layout for Linux

This is a custom layout to have old english (and some middle english) characters on linux.

_note_: This only works with Wayland

## Layout

### Diacritics

The grave key (\`) has four functions:

- unmodified it applies a macron (for e.g. ō)
- shift + \` applies an overdot (for e.g. ġ)
- alt mod + \` applies a diaresis (for e.e ä)
- alt mod + shift + \` applies an acute (for e.g. é)

### Special Symbols

The special characters are slightly inconveniant to use as they all require
the use of the alternate mod key (see below).

They are:

* alt mod + a -> æ
* alt mod + shift + a -> Æ
* alt mod + s -> ſ
* alt mod + shift + s -> ß
* alt mod + z -> ȝ
* alt mod + shift + z -> Ȝ
* alt mod + t -> þ
* alt mod + shift + t -> Þ
* alt mod + d -> ð
* alt mod + shift + d -> Ð
* alt mod + y -> ꝥ
* alt mod + shift + y -> Ꝥ

## The Alternate Mod Key

The Gnome desktop environment defaults to right alt, but I had to set it to
right ctl for compatability reasons.

You can check this in Gnome by going to settings -> Keyboard

It will be the option _Alternate Characters Key_ under _Special Character Entry_

## How to Install

Clone or copy this repository, then copy it into $XDG_CONFIG_HOME if it's set, else into $HOME/.config, then rename it to `xkb`

Once you've done that, go ahead and log out and back in again. You should see it under Settings -> Keyboard -> Input Sources
