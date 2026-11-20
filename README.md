<p align="center">
  <img src="https://github.com/Prayag2/kde_modernclock/blob/main/assets/logo.jpg" width=100/>
  <h2 align="center">Modern Clock for KDE</h2>
  <p align="center">A modern looking clock widget!</center>
</p>

<p align="center">
<a href="https://github.com/prayag2/kde_modernclock/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/prayag2/kde_modernclock?color=%233DAEE9&style=for-the-badge"></a>
<a href="https://github.com/prayag2/kde_modernclock/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/prayag2/kde_modernclock?color=%233DAEE9&style=for-the-badge"></a>
<a href="https://github.com/prayag2/kde_modernclock/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/prayag2/kde_modernclock?color=%233DAEE9&style=for-the-badge"></a>
</p>

<p align="center">
  <img src="https://github.com/Prayag2/kde_modernclock/blob/main/assets/ss.png"/>
</p>

> [!NOTE]
> **This is a fork** of [Prayag2/kde_modernclock](https://github.com/Prayag2/kde_modernclock), which hasn't been updated since 2024.
> It adds a **Language** setting, proposed upstream in [#29](https://github.com/Prayag2/kde_modernclock/pull/29).

## What this fork adds

#### Language setting for day and month names
On recent Qt 6 / Plasma 6 versions, the original widget always shows day and month names in English, whatever your system language ([#11](https://github.com/Prayag2/kde_modernclock/issues/11), [#17](https://github.com/Prayag2/kde_modernclock/issues/17), [#19](https://github.com/Prayag2/kde_modernclock/issues/19)).
This fork formats them with your locale and adds a **Language** option in *Configure → Appearance → Date*:

- **System default** follows your system language (`VENDREDI · 20 NOVEMBRE` on a French system).
- Or pick a language to force it, e.g. **English (en_US)** for `FRIDAY · 20 NOVEMBER` on any system.

The option applies live, no restart needed.

## Installation
#### From this fork (with the Language setting)
1. Clone this repository  
`git clone https://github.com/3L0935/kde_modernclock && cd kde_modernclock/`  
2. Install it with kpackagetool (Plasma 6)  
`kpackagetool6 -t Plasma/Applet -i package`  
To update an existing install, use `-u package` instead of `-i package`.
3. Restart Plasma (`systemctl --user restart plasma-plasmashell`) or log out and back in.

#### KDE Store (original version, without the Language setting)
1. Right click on the desktop
2. Click on "Add Widgets"
3. Click on "Get New Widgets"
4. Click on "Download New Plasma Widgets"
5. Search for "Modern Clock"
6. Click on "Install" and you're done!

Installing from the Store replaces this fork's version with the original one.
