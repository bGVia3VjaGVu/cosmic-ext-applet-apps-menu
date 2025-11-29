Archived - 30 Nov 2025


I have decided not to further develop COSMIC applets.

COSMIC is a great step forward, but it is not ready yet. Therefore, I am not actively using it and am not gaining anything from developing these applets.

COSMIC still lacks basic features, such as proper drag-and-drop support and Nightlight.

The COSMIC toolkit is also not ready and requires a lot of boilerplate code for simple features.


The applets are still perfectly usable because, unlike GNOME, COSMIC does not frequently break applets.

They don't statically link to the latest LIBCOSMIC version, so they won't receive new features, but they work fine otherwise.


Best regards,


bGVia3VjaGVu


Thank you!

# Install 
```sh
git clone https://github.com/lbGVia3VjaGVu/cosmic-ext-applet-apps-menu 
cd cosmic-ext-applet-apps-menu 
cargo b -r
sudo just install
```

# Config

The configuration directory is `.config/cosmic/dev.dominiccgeh.CosmicAppletAppsMenu/`.

Each configuration option coresponds to a filename, e.g. you can set `skip_empty_categories` with `true > .config/cosmic/dev.dominiccgeh.CosmicAppletAppsMenu/skip_empty_categories`.

These are the default options:

```
skip_empty_categories: true,
categories: [
    "Favorites",
    "Audio",
    "AudioVideo",
    "COSMIC",
    "Education",
    "Game",
    "Graphics",
    "Network",
    "Office",
    "Science",
    "Settings",
    "System",
    "Utility",
    "Other",
],
sort_categories: true,
```

Note that Favorites` and `Other` are not
acutally categories in your desktop files.

# Dependencies
(some may not be required)
```
Build-Depends:
  debhelper (>= 11),
  debhelper-compat (= 11),
  rustc ,
  cargo,
  libdbus-1-dev,
  libegl-dev,
  libpulse-dev,
  libudev-dev,
  libxkbcommon-dev,
  libwayland-dev,
  libinput-dev,
  just,
  pkg-config,
```
