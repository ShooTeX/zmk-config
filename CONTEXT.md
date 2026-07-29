# ZMK Config

Keymap configuration for Corne, Corneish Zen, and Toucan keyboards, sharing a common base layer.

## Language

**Default layer (DEF)**:
The boot-time base layer for macOS keybinding conventions. Homerow modifiers place LGUI on the inner index-finger position, matching Cmd-based muscle memory.

**Linux layer (LIN)**:
An alternate base layer that swaps LGUI↔LALT and RGUI↔RALT to match Linux modifier conventions (Ctrl-based shortcuts). Mirror of DEF in all other respects.

**Platform toggle**:
A dedicated key on the FN layer that switches between DEF and LIN via `&tog`. The keyboard always boots to DEF; the toggle is transient.
