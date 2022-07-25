# st

## What is st?
st is a simple terminal emulator for X which sucks less (st is created by the good folks at https://suckless.org).  The Suckless team created st as an alternative to traditional terminal emulators like xterm and rxvt, which have tens of thousands of lines of code and are quite bloated in comparison to the rather slim st.

## Why to use this build
This is my personal build of st that is very heavily patched to add more functionality and more customization options.

### Patches
* st-alpha -- adds transparency to the background (must have a [compositor](https://wiki.archlinux.org/title/Xorg#Composite) for this to work)
* st-font2 -- adds the option to list multiple fonts; great for having a fallback font
* st-ligatures -- ligature support; requires harfbuzz
* st-scrollback -- adds scrollback with SHIFT+PageUp/PageDown
* st-scrollback-mouse -- adds the ability to scroll with SHIFT+MouseWheel
* st-scrollback-mouse-altscreen -- now you can scroll with just the MouseWhell (no SHIFT required)
* st-vertcenter -- better vertical alignment of lineszz
* st-workingdir -- adds option to open st at specific directory (ex: st -d /usr/bin)
* st-w3m -- support for w3m
# Install
```
git clone https://github.com/BishrGhalil/st.git
cd st
sudo make install
```
