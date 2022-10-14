# keyboard tour

## overview

![crkbz-main](tsoim-crkbz-20221013.png)

### highlights

* [Corne-ish Zen keyboard](https://github.com/LOWPROKB/zmk-config-Corne-ish-Zen) with ZMK firmware
* 4 layers - base, navigation/numbers, symbols, and functions
* base layer is a customized version of dvorak that suits my fingers better
* navigation/numbers and symbols layers are reachable by holding down thumb keys,
    with the "core" functionality for each layer on the opposite hand
* functions/shortcuts layer to be used with one-shot tap on left thumb key

---

## base layer

![crkbz-base](tsoim-crkbz-20211030-dvorak.png)

### layout

tldr; a modified dvorak layout with `U`/`I` swapped and `C`/`L`/`Z` rotated

* when I started on my ortho-split journey, I figured I might as well try a completely new layout
    so that I retain the muscle memory for qwerty on a traditional keyboard
* for some reason I kept mistyping `U` and `I` - I figured I would only really type dvorak on my own keebs
    so it doesn't matter that I'm using a non-standard dvorak, so I swapped the keys
* `L` and `C` were swapped originally because I needed `ls` to be comfortable considering how often I use it
* `C` and `Z` were then swapped because top right pinky was much harder for me to reach
* unfortunately, even though `Z` is used infrequently in the English language, I had forgotten
    that I use it extensively in vim commands. but `C` was overall more used so for now I just deal with it

### layers

* thumb keys are used to manipulate layers
* navnum and symbol layers are reachable by holding down thumb keys
* function layer is to be triggered via one-shot tap on left thumb key

---

## navigation/numbers layer

![crkbz-navnum](tsoim-crkbz-20211030-navnum.png)

tldr; access via hold on right thumb key for numpad and arrows

### navigation

* arrow keys live in qwerty `HJKL` positions
    * better alternative than trying to actually use `HJKL` in dvorak positions or to remap vim commands
    * bonus - there's now vim-like navigation everywhere!
* threw in volume and brightness controls

### numbers

* numpad layout with `x` for hex codes
* arithmetic symbols on right for when this layer is locked to be used as a calculator mode

---

## symbols layer

![crkbz-symbol](tsoim-crkbz-20211030-symbol.png)

tldr; access via hold on left thumb key for any symbol not accessible on base layer

### shift-num symbols

* symbols normally accessible by pressing shift + number are placed in corresponding spots of numpad layer
* may not be most ergonomic but less mental gymnastics
* arithmetic symbols are also placed in same spots as in navnum layer

### other symbols

* `()`, `{}`, and `[]` are placed as pairs surrounding home positions
* the rest were just kind of filled in to wherever made sense to me tbh


---

## functions/shortcuts layer

![crkbz-function](tsoim-crkbz-20211030-functn.png)

tldr; access via one-shot tap on left thumb key for shortcuts and function keys

### shortcuts

* the shortcuts were designed to be accessible with left hand only while mousing
* to make sure symbols layers take precedence over function keys when typing quickly
    (mainly `-` for command line flags), the `hold-preferred` flavor was selected for `behavior-hold-tap`

* top row: desktop navigation - desktop switching + mission control
* home row: editing - undo, cut, copy, paste, and paste and match destination format
* bottom row: text formatting + screenshotting

### layer toggle on

* right thumb keys are used to turn on base, navnum, or symbol layers
    * these keys don't have a corresponding function in symbol layer, see `hold-preferred` comment above
* function layer needs to be turned on in symbols layer
    * `TO` doesn't seem to take effect when selected via sticky layer.
        my guess is the sticky layer is just released after term expires

### misc

* zmk bluetooth keys to cycle to prev or next connection, or to clear a connection
* personally don't really use function keys so left them on this layer in a numpad-ish fashion

---

## some thoughts

* at some point an internet stranger said that the layout should adapt to the person, not vise versa
* so as I tested new layouts, if I kept mistyping something, I just altered the layout to what my fingers were actually pressing

---

## notes

* [keyboard layout editor](http://www.keyboard-layout-editor.com/#/gists/052b74409d9075edf47ff1b15d0820e1)
