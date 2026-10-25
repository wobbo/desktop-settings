# Desktop Settings

*A personal hobby project for GNOME.*

I like GNOME, but I missed a few settings and found it annoying to jump between GNOME Settings, separate extensions and other tools just to get my desktop the way I wanted it.

<img height="300" alt="Screenshot From 2026-10-24 12-32-51" src="https://github.com/user-attachments/assets/b85dbcfc-1496-4c35-8964-1ef9249c3092" /> <img height="300" alt="Screenshot From 2026-10-24 12-32-59" src="https://github.com/user-attachments/assets/90eb7340-782e-452a-a492-ac3f34859382" />


That's why I started making **Desktop Settings** for myself. It's not meant to replace GNOME, just to bring useful options together and add a few things I felt were missing.

## What can you do?

- **Backgrounds:** make and edit your own wallpapers, use different images or solid colours for light and dark mode, and choose how they fit your screen.
- **Dock:** change its position, size, auto-hide, scrolling and other behaviour.
- **Desktop icons:** choose which icons appear and how they're arranged.
- **Windows:** adjust window behaviour and screen-edge options.
- **Startup apps:** manage applications that start when you log in.
- **Extensions:** find related GNOME extension settings in one place.

<img height="300" alt="Screenshot From 2026-10-24 12-35-12" src="https://github.com/user-attachments/assets/54fce70c-7012-4066-8828-0dbb8235fe58" /> <img height="300" alt="Screenshot From 2026-10-24 12-34-02" src="https://github.com/user-attachments/assets/18fe5d28-7150-4cae-b5a4-bab2d7e1d839" />


## Command-line options

Desktop Settings also has a command-line interface (CLI). These are the commands documented during development:

| Command | Purpose |
| --- | --- |
| `desktop-settings` | Open Desktop Settings. |
| `desktop-settings --help` | Show available command-line options. |
| `desktop-settings --page=desktop` | Open the Desktop page directly. |
| `desktop-settings --page=dock` | Open the Dock page directly. |
| `desktop-settings --page=background` | Open the Backgrounds page directly. |
| `desktop-settings defaults apply --profile=gnome --yes` | Apply the GNOME defaults profile. |
| `desktop-settings defaults apply --profile=ubuntu --yes` | Apply the Ubuntu defaults profile. |
| `sudo desktop-settings defaults install-system --profile=gnome` | Install the GNOME defaults at system level. |
| `sudo desktop-settings defaults install-system --profile=ubuntu` | Install the Ubuntu defaults at system level. |

**CLI status:** These commands are based on earlier development notes and have not yet all been verified against the current package. In one installed build, `desktop-settings --help` fails with `PermissionError: [Errno 13] Permission denied` when trying to start `/usr/lib/desktop-settings/desktop-settings-cli`. The executable permissions or packaging need to be checked before treating the CLI as working.

**Be careful:** `defaults apply` changes settings, and `defaults install-system` makes system-level changes. The commands above are for reference, not a suggested sequence to run.

## GNOME extensions and credits

I haven't made all of this from scratch. Desktop Settings uses existing **GNOME Shell extensions**, and I've adapted parts of some of them to make my own desktop work the way I want. The original extensions are the work of their respective developers.

Two important projects I've worked with and modified are:

- [Desktop Icons NG (DING)](https://gitlab.com/rastersoft/desktop-icons-ng) by **rastersoft**, for desktop icons.
- [Dash to Dock](https://github.com/micheleg/dash-to-dock) by **michele_g**, for the dock.

Other GNOME extensions used or referenced by this project include:

- [Add to Desktop](https://github.com/Tommimon/add-to-desktop), for creating desktop shortcuts.
- [App Hider](https://github.com/LynithDev/gnome-app-hider), for hiding apps in the application grid.
- [TopIconsFix](https://extensions.gnome.org/extension/1674/topiconsfix/), for legacy tray icons.
- [AppIndicator and KStatusNotifierItem Support](https://github.com/ubuntu/gnome-shell-extension-appindicator), for tray indicators.
- [Freon](https://github.com/UshakovVasilii/gnome-shell-extension-freon), for temperature sensors.

These links point to the **original projects**. Not every extension is necessarily included in the Desktop Settings package. Thanks to the developers who made them possible.

<img height="250" alt="Screenshot From 2026-10-24 12-33-28" src="https://github.com/user-attachments/assets/1406e9b8-a566-4036-8693-5c948fdf0f94" /> <img height="250" alt="Screenshot From 2026-10-24 12-35-17" src="https://github.com/user-attachments/assets/e357f106-2820-4e2d-b7d2-ad31ff834ef5" />


## Just a hobby

This is **my own personal hobby project**, originally made for my GNOME setup on Debian and Raspberry Pi OS. I keep changing and improving it as I use it.

It's not an official GNOME application. I'm sharing it because maybe someone else has missed the same things too.

<img height="300" alt="Screenshot From 2026-10-24 12-34-59" src="https://github.com/user-attachments/assets/b70fafcb-534d-4f53-8a2b-9458dfa6c678" /> <img height="300" alt="Screenshot From 2026-10-24 12-35-44" src="https://github.com/user-attachments/assets/93b6a635-1c5a-40d6-88e0-4ba3f52f52f2" />


