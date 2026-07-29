# Layer toggle for Linux modifier swap

The keyboard firmwares in this repo share a single base layer (DEF) with homerow mods arranged for macOS (LGUI on inner index). When the same keyboard connects to a Linux desktop, LGUI becomes Super instead of Cmd, breaking muscle memory. Rather than OS-level remapping (which requires per-machine config), we added a second base layer (LIN, index 1) toggled by a dedicated FN-layer key. The LIN layer swaps LGUI↔LALT and RGUI↔RALT on homerow mods. The keyboard always boots into DEF; the toggle is transient.

**Rejected alternative**: OS-level remapping with tools like `hidutil` (macOS) or `setxkbmap`/Interception Tools (Linux) — abandoned because it requires configuring every host machine and doesn't work on locked-down machines.
