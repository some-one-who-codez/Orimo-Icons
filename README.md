<div align="center">
  <center align="center">
      <img src="https://github.com/some-one-who-codez/Orimo-OS/blob/master/Orimo%20Os%20Logo.png" alt="Orimo OS" align="center" height=200 width=200 >
   </center>
  <br>
  <h1 align="center"><center>Orimo OS</center></h1>
  <br>
  <br>
</div>
 
## Disclaimer
This is not my source code. This code is originally from [here](https://github.com/elementary/os). I simply want to experiment and see what I can do. You are free to join. PS I have no experience so help is very welcome. I ultimately want the os to look like [this](https://www.youtube.com/watch?v=9zqN-f3wm-Y)

# elementary Icons

[![Bountysource](https://www.bountysource.com/badge/tracker?tracker_id=27377189)](https://www.bountysource.com/trackers/27377189-elementary-icons)

An original set of vector icons designed specifically for [elementary OS](http://elementary.io) and its desktop environment: Pantheon.

These icons are licensed openly under the terms of the [GNU General Public License](COPYING). Redistributing, forking, remixing, etc. are encouraged!

If you feel the desire to compensate the artists who maintain these icons for your usage, [please see this page](http://elementary.io/get-involved#funding) and thank you!

## Contributing Icons
It is recommended to use the free and open source [Inkscape](http://inkscape.org) vector editor to create elementary icons. Any and all icons must follow the elementary [Icon Design Guidelines](http://elementary.io/docs/human-interface-guidelines#iconography).

An [elementary color palette](data/elementary.gpl) ([rendered version](https://elementary.io/docs/human-interface-guidelines#color)) is provided; it is recommended to copy it into your Inkscape settings before you get started.

```bash
cp data/elementary.gpl ~/.config/inkscape/palettes/
```

To contribute to the elementary icon set, open a pull request to this repository with your icon(s).

It is strongly encouraged to vacuum all vectors with [Inkscape](http://inkscape.org). This keeps the repository lean, clean, and fast for everyone. For convenience, a git pre-commit hook is included. To install, run these commands from your local repository folder:
```bash
$ cp pre-commit .git/hooks/
$ chmod +x .git/hooks/pre-commit
```

## Installation
You need the [Meson](http://mesonbuild.com) build system to install it.
Once you've installed it, run these commands in the root of the icon set.
```bash
$ meson build --prefix=/usr
$ cd build
$ sudo ninja install
```

## Not a Universal Icon Set
Since this set is designed specifically for elementary OS, pull requests to add icons or symlinks that are specific to other desktop environments (such as `xfce-*` or `gnome-*` named icons) will be rejected.

Use of icon names in line with the [FreeDesktop.Org Icon Naming Specification](http://standards.freedesktop.org/icon-naming-spec/icon-naming-spec-latest.html) is encouraged.

## Third-Party Brand Preservation
elementary icons do not attempt to supply icons for third-party apps. Pull requests to add icons or symbolic links that would overwrite the branding of third-party apps will be rejected.

