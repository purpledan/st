# Dan's build of st - simple terminal

st is a simple terminal emulator for X which sucks less.

## Current Defaults
The default font for this fork is Intel One Mono
Install using pkg on FreeBSD:

    pkg install intel-one-mono

Default colourscheme is Elementary from [Gogh](https://github.com/Gogh-co/Gogh).

## Applied Patches
- [Boxdraw](https://st.suckless.org/patches/boxdraw)
- [Ligatures](https://st.suckless.org/patches/ligatures)
- [Font2](https://st.suckless.org/patches/font2)

## Requirements
In order to build st you need the Xlib header files.


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

## Credits
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

