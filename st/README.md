# st - simple terminal
Just my personal build of [st](https://st.suckless.org/) version 0.8.1.

![screenshot](/st/screenshot.png)

## Changes
* Open latest url with shift + left click
* Colors ([sourcerer](https://github.com/xero/sourcerer))

Idea is to use st just for simple terminal emulation and let tmux handle all other stuff (like splitting/tabbing, scrollback, "keyboard-select", searching from buffer, advanced url opening etc.).

Added make option ```make binary``` compiles and installs only the binary itself to the ~/bin so its easy to for example write script and bind it to some keybinding to easily update configurations.

[xurls](/xurls) script that is used to url parsing must be in the $PATH.

## Patches used
* [st-externalpipe](https://st.suckless.org/patches/externalpipe/) for piping screen to url-parser
* [st-scrollback-mouse](https://st.suckless.org/patches/scrollback/) for mouse binding support(actual scrollback patch not used)
* [st-dracula](https://st.suckless.org/patches/dracula/) as a base for coloring
