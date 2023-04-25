This repository contains a number of commandline utilities for use
inside Flatpak sandboxes. They work by talking to portals.

Currently, there is flatpak-spawn for running commands in sandboxes
as well as `xdg-open` and `xdg-email`, which are compatible with the
well-known scripts of the same name.

Everything else in `xdg-utils` is not provided. That includes
`xdg-settings` and `xdg-mime` as they deal with settings that Flatpaks
do not have access or control to.

See http://flatpak.org/ for more information.

# Installation 

This repository uses meson to build. Just do
```
 meson [args] build
 ninja -Cbuild
 ninja -Cbuild install
```

The tools in flatpak-xdg-utils are only useful inside a Flatpak sandbox.
