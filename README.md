# st - simple terminal

st is a simple terminal emulator for X which sucks less.

## Basic keybindings
- `Ctrl+Print`: Toggles print screen (for recording to `iofile`).
- `Shift+Print`: Prints the full screen to `iofile`.
- `CapsLock+Print`: Prints selection to `iofile`.
- `Ctrl+Shift+C`: Clipboard copy
- `Ctrl+Shift+V`: Clipboard paste
- `Ctrl+Shift+Y`: Paste selection
- `Ctrl+Shift++`: Zoom in
- `Ctrl+Shift+-`: Zoom out
- `Ctrl+Shift+0`: Zoom reset
- `Shift+PageUp` or `Shift+MouseScrollUp`: Scroll up
- `Shift+PageDown` or `Shift+MouseScrollDown`: Scroll down

## Requirements

In order to build st you need the Xlib header files.

*IMPORTANT*: Make sure you have the latest code for `dmenu` or
some parts won't work. The best option is to clone the repo and
`make install`.


## Installation

Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

# Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code and
the guys at Suckless :D

