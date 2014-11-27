# Keymap
## Power key doesn't work
Use `KC_PWR` instead of `KC_POWER` or vice versa.
- `KC_PWR` works with Windows and Linux, not with OSX.
- `KC_POWER` works with OSX and Linux, not with Windows.

http://geekhack.org/index.php?topic=14290.msg1327264#msg1327264

## Oneshot modifier
Solves my personal 'the' problem. I often got 'the' or 'THe' wrongly instead of 'The'.  Oneshot Shift mitgates this for me.
https://github.com/tmk/tmk_keyboard/issues/67

## Modifier/Layer stuck
Modifier keys or layers can be stuck unless layer switching is configured properly.
For Modifier keys and layer actions you have to place `KC_TRANS` on same position of destination layer to  unregister the modifier key or return to previous layer on release event.

https://github.com/tmk/tmk_keyboard/blob/master/doc/keymap.md#31-momentary-switching
http://geekhack.org/index.php?topic=57008.msg1492604#msg1492604


## Mechanical Lock Switch Support
https://github.com/tmk/tmk_keyboard#mechanical-locking-support

This feature is for *mechanical lock switch* like this Alps one.
http://deskthority.net/wiki/Alps_SKCL_Lock

Using enabling this feature and using keycodes `LCAP`, `LNUM` or `LSCR` in keymap you can use physical locking CapsLock, NumLock or ScrollLock keys as you expected.

Old vintage mechanical keyboards occasionally have lock switches but modern ones don't have. ***You don't need this feature in most case and just use keycodes `CAPS`, `NLCK` and `SLCK`.***