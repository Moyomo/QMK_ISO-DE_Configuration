# ISO-DE Configuration for QMK
This is my personal configuration file for the DZ60 PCB. It's based on the standard 60% ISO-DE layout and has a few additional keybinds on the second layer.

To use this file you can either customize and compile it with the open-source [QMK Firmware](https://github.com/qmk/qmk_firmware) or simply import it on their configuration website at [config.qmk.fm](https://config.qmk.fm).

For more informations on how to customize and flash the keyboard visit their [website](https://docs.qmk.fm/).

---

Here's a visual representation of the different layers

**default layer**
```
┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───────┐
│Esc│ 1 │ 2 │ 3 │ 4 │ 5 │ 6 │ 7 │ 8 │ 9 │ 0 │ ß │ ´ │Backspc│
├───┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─────┤
│ TAB │ Q │ W │ E │ R │ T │ Z │ U │ I │ O │ P │ Ü │ + │Enter│
├─────┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┐    │
│ Caps │ A │ S │ D │ F │ G │ H │ J │ K │ L │ Ö │ Ä │ # │    │
├────┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴───┴────┤
│Shft│ < │ Y │ X │ C │ V │ B │ N │ M │ , │ . │ - │   Shift  │
├────┼───┴┬──┴─┬─┴───┴───┴───┴───┴───┴──┬┴───┼───┴┬────┬────┤
│Ctrl│Win │Alt │          Space         │AltG│Win │ Fn │Ctrl│
└────┴────┴────┴────────────────────────┴────┴────┴────┴────┘
```

**layer 2 (Fn + )**
```
┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───────┐
│   │F1 │F2 │F3 │F4 │F5 │F6 │F7 │F8 │F9 │F10│F11│F12│       │
├───┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─────┤
│     │RGB│RGB│RGB│   │   │   │   │   │   │F6 │Ins│         │
├─────┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┐    │
│      │RGB│RGB│RGB│   │   │   │   │   │Mut│Ply│F13│F14│    │
├────┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴───┴────┤
│    │   │   │   │   │   │   │   │   │   │Prv│Nxt│   Shift  │
├────┼───┴┬──┴─┬─┴───┴───┴───┴───┴───┴──┬┴───┼───┴┬────┬────┤
│    │    │    │                        │    │    │(Fn)│    │
└────┴────┴────┴────────────────────────┴────┴────┴────┴────┘
```
the 6 RGB keys are for controlling the PCB backlighting. Their functionality is arranged like the arrow keys (W,A,S,D)
From top left to bottom right:
-RGB toggle (On/Off)
-Increase brightness
-Toggle RGB mode
-Decrease effect speed
-Decrease brightness
-Decrease effect speed

**shift layer**
```
┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───────┐
│ ° │ ! │ " │ § │ $ │ % │ & │ / │ ( │ ) │ = │ ? │ ` │       │
├───┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─────┤
│     │   │   │   │   │   │   │   │   │   │   │   │ * │     │
├─────┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┐    │
│      │   │   │   │   │   │   │   │   │   │   │   │ ' │    │
├────┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴───┴────┤
│    │ > │   │   │   │   │   │   │   │ ; │ : │ _ │          │
├────┼───┴┬──┴─┬─┴───┴───┴───┴───┴───┴──┬┴───┼───┴┬────┬────┤
│    │    │    │                        │    │    │    │    │
└────┴────┴────┴────────────────────────┴────┴────┴────┴────┘
```

**AltGr layer**
```
┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───────┐
│   │   │ ² │ ³ │   │   │   │ { │ [ │ ] │ } │ \ │   │       │
├───┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─────┤
│     │ @ │   │ € │   │   │   │   │   │   │   │   │ ~ │     │
├─────┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┐    │
│      │   │   │   │   │   │   │   │   │   │   │   │   │    │
├────┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴───┴────┤
│    │ | │   │   │   │   │   │   │ µ │   │   │   │          │
├────┼───┴┬──┴─┬─┴───┴───┴───┴───┴───┴──┬┴───┼───┴┬────┬────┤
│    │    │    │                        │    │    │    │    │
└────┴────┴────┴────────────────────────┴────┴────┴────┴────┘
```
