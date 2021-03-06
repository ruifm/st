# st

This is my personal fork of the original [st suckless terminal](https://st.suckless.org/). I try to always backport upstream patches form st's master ASAP.

## Installation

If using arch or an arch based distro, you can manually install the
`st-ruifm-git` package provided in the `PKGBUILD`, using:

```bash
makepkg -si
```

Else, clone this repo, compile and install manually:

```bash
git clone https://github.com/ruifm/st.git
cd st
make
sudo make install
```

By default, it will be installed to your system's `/usr/local/` prefix. If, for
instance you prefer (or are only allowed) a local user installation:

```bash
mkdir -p ~/.local
make PREFIX=$HOME/.local install
```

## Features

Applied community patches:

* [application-sync](https://st.suckless.org/patches/sync/)
* [anysize](https://st.suckless.org/patches/anysize/)
* [blinking-cursor](https://st.suckless.org/patches/blinking_cursor/)
* [bold-is-not-bright](https://st.suckless.org/patches/bold-is-not-bright/)
* [boxdraw](https://st.suckless.org/patches/boxdraw/)
* [clipboard](https://st.suckless.org/patches/clipboard/)
* [copyurl](https://st.suckless.org/patches/copyurl/) with the highlight feature
* [font2](https://st.suckless.org/patches/font2/)
* [gruvbox](https://st.suckless.org/patches/gruvbox/)
* [hidecursor](https://st.suckless.org/patches/hidecursor/)
* [ligatures](https://st.suckless.org/patches/ligatures/)
* [scrollback](https://st.suckless.org/patches/scrollback/) without mouse support
* [spoiler](https://st.suckless.org/patches/spoiler/)
* [undercurl](https://st.suckless.org/patches/undercurl/)
* [vertcenter](https://st.suckless.org/patches/vertcenter/)
* [w3m](https://st.suckless.org/patches/w3m/)

Other popular patches suck as [alpha](https://st.suckless.org/patches/alpha/)
and [xresources](https://st.suckless.org/patches/xresources/) were not applied
since I personally do not use them and **I want to keep this st fork as minimal
as possible**.

## Shortcuts

Key combination | Action
--- | ---
alt + u | scroll-up
alt + d | scroll-down
alt + shift + u | big scroll-up
alt + shift + d | big scroll-down
alt + shift + k | increase font size
alt + shift + j | decrease font size
alt + o | font size reset
alt + shift + l | copy last printed url to clipboard
