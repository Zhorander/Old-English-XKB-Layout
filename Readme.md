# Old English Layout for Linux

This project defines two layouts for typing in old english:

- 1) A layout with minimal intrusion to the standard US layout.
- 2) A layout with (to me) maximal ergonomics for typing old english.

They both feature additional diacritics and characters, but are by far not
comprehensive in additional diacritics.

_note_: This only works with Wayland

## Layout 1

### Diacritics

The grave key (\`) has four functions:

- unmodified it applies a macron (for e.g. ō)
- shift + \` applies an overdot (for e.g. ġ)
- alt mod + \` applies a diaeresis (for e.g ä)
- alt mod + shift + \` applies an acute (for e.g. é)

### Special Symbols

The special characters are slightly inconveniant to use as they all require
the use of the alternate mod key (see below). The reason for this is to maintain
as much compatability with the default us layout as possible.

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
* alt mod + o -> œ
* alt mod + shift + o -> Œ

## Layout 2

This layout contains many remappings to the standard US layout. The way I will
present them is in a four-stage mapping of [unmodified, with shift, with alternate mod, with shift + alternate mod].
Since the remappings are on top of the standard US layout I will only present those
that have been altered.

| Original | New         | with Shift     | with Alt Mod | with Shift + Alt Mod |
|----------|-------------|----------------|--------------|----------------------|
| ~        | dead acute  | dead diaeresis | \`           | ~                    |
| 3        | 3           | ~              |              |                      |
| 4        | 4           | \`             |              |                      |
| \-       | dead macron | dead abovedot  | \-           | _                    |
| q        | ƿ           | Ƿ              | q            | Q                    |
| o        | o           | O              | œ            | Œ                    |
| [        | ð           | Ð              | [            | {                    |
| ]	       | ȝ           | Ȝ              | ]            | }                    |
| s        | s           | S              | ſ            | ß                    |
| j        | þ           | Þ              | ꝥ            | Ꝥ                    |
| k        | æ           | Æ              | k            | K                    |

_note_: A dead diactricit decorates the next typed character. For example, dead macron + o = ō.

## The Alternate Mod Key

The Gnome desktop environment defaults to right alt, but I had to set it to
right ctl for compatability reasons. You may also have to do this if right mod
conflicts with built-in functionality of your desktop environment/window manager.

You can check this in Gnome by going to settings -> Keyboard

It will be the option _Alternate Characters Key_ under _Special Character Entry_

## How to Install

Clone or copy this repository, then copy it into $XDG_CONFIG_HOME if it's set, else into $HOME/.config, then rename it to `xkb`

Once you've done that, go ahead and log out and back in again. You should see it under Settings -> Keyboard -> Input Sources

The two layouts are named:

- Layout 1 : English (Old English Compat)
- Layout 2 : English (Old English Re-map)
