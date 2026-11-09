<p align="center">
  <img src="media/logo.svg" width="96" alt="MoonBeam_IG logo">
</p>

<h1 align="center">MoonBeam_IG</h1>

<p align="center">
  Your Instagram DMs in a tiny desktop panel. None of the feed.
</p>

<p align="center">
  <a href="https://github.com/zuhuHix/moonbeam-ig-releases/releases/latest"><b>Download</b></a> ·
  <a href="media/showcase.mp4">Video</a> ·
  <a href="#themes">Themes</a> ·
  <a href="#features">Features</a>
</p>

<p align="center">
  <a href="media/showcase.mp4">
    <img src="media/showcase-teaser.gif" width="720" alt="MoonBeam_IG teaser: a popup pill expands into a chat">
  </a>
  <br>
  <a href="media/showcase.mp4">▶ Watch the 35 s video (with sound)</a>
</p>


https://github.com/user-attachments/assets/3c6588c2-62fe-4b74-b3ad-2eace2541f6d



## Why

- DMs without the feed and reels.
- Lives in your tray.
- Pops up only when someone writes.

## Themes

<p align="center">
  <img src="media/themes.webp" width="100%" alt="The five MoonBeam_IG themes: MoonBeam, Cyberpunk 2077, Fallout Pip-Boy, Minecraft, Undertale">
  <br>
  MoonBeam · Cyberpunk 2077 · Fallout Pip-Boy · Minecraft · Undertale — <i>the popup pill follows the theme</i>
</p>

<table align="center">
  <tr>
    <td align="center"><img src="media/pill-moonbeam.webp" width="300" alt="MoonBeam popup pill"><br><sub>MoonBeam</sub></td>
    <td align="center"><img src="media/pill-cyberpunk.webp" width="300" alt="Cyberpunk 2077 popup pill"><br><sub>Cyberpunk 2077</sub></td>
    <td align="center"><img src="media/pill-fallout.webp" width="300" alt="Fallout Pip-Boy popup pill"><br><sub>Fallout Pip-Boy</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="media/pill-minecraft.webp" width="300" alt="Minecraft popup pill"><br><sub>Minecraft</sub></td>
    <td align="center"><img src="media/pill-undertale.webp" width="300" alt="Undertale popup pill"><br><sub>Undertale</sub></td>
    <td align="center"><img src="media/pill-entrance.webp" width="300" alt="Popup pill entrance animation"><br><sub>Drops in as a circle, opens from the middle</sub></td>
  </tr>
</table>

## Features

<table align="center">
  <tr>
    <td align="center" valign="top"><img src="media/feature-tabs.webp" width="260" alt="Tabs: one per friend with unread badges"><br><b>Tab per friend</b><br>Up to 8 chats, unread badges, Ctrl+Tab.</td>
    <td align="center" valign="top"><img src="media/pill-entrance.webp" width="260" alt="Island popup pill"><br><b>Island popups</b><br>No focus steal, hover to keep it, click opens that chat; DND from the tray.</td>
    <td align="center" valign="top"><img src="media/feature-typing.webp" width="260" alt="Typing indicator above the message box"><br><b>Typing indicator</b><br>"Mia is typing" over the box, via the realtime socket.</td>
  </tr>
  <tr>
    <td align="center" valign="top"><img src="media/feature-quick-replies.webp" width="260" alt="Quick replies: chips above the composer"><br><b>Quick replies</b><br>⚡, <code>/</code> in an empty box, or the chips above the composer; Shift+Enter sends.</td>
    <td align="center" valign="top"><img src="media/feature-stickers.webp" width="260" alt="My stickers sent as photos"><br><b>My stickers</b><br>Your own PNG/WebP/GIF, sent as photos on a light or dark square.</td>
    <td align="center" valign="top"><img src="media/feature-viewer.webp" width="260" alt="Full-size photo viewer with zoom"><br><b>Photo viewer</b><br>Full size, zoom, ←/→ through the chat's photos, Save.</td>
  </tr>
  <tr>
    <td align="center" valign="top"><img src="media/feature-drafts.webp" width="260" alt="Drafts kept per chat across tabs"><br><b>Drafts per chat</b><br>Kept across tabs and restarts; the tab gets a marker.</td>
    <td align="center" valign="top"><img src="media/feature-settings.webp" width="260" alt="Settings panel with themes and updates"><br><b>Settings &amp; updates</b><br>Themes, popup position/duration, start on login, auto-updates that never interrupt unsent work.</td>
  </tr>
</table>

Also: outline bubbles (cyan for yours) · reactions · Esc → tray · start on login · instant notifications.

## Install (Windows)

1. Download `MoonBeam_IG_<version>_x64-setup.exe` from the [latest release](https://github.com/zuhuHix/moonbeam-ig-releases/releases/latest) and install it once.
2. Log in once. Instagram's own login page opens in a private window; only session cookies are kept, encrypted.
3. Add your people from your inbox.

From then on it updates itself. Windows 10/11 (WebView2).

## Install (Linux)

x86_64, tested on Linux Mint 22 Cinnamon (X11). Download one of these from the [latest release](https://github.com/zuhuHix/moonbeam-ig-releases/releases/latest):

- **.deb** (Debian, Ubuntu, Mint): `MoonBeam_IG_<version>_amd64.deb`. Install it with apt, which pulls in the libraries it needs:
  ```sh
  sudo apt install ./MoonBeam_IG_<version>_amd64.deb
  ```
  Then start MoonBeam_IG from your app menu.
- **AppImage** (any distro): `MoonBeam_IG_<version>_amd64.AppImage`. Keep it somewhere you can write to (e.g. `~/Applications`), make it executable and run it:
  ```sh
  chmod +x MoonBeam_IG_*_amd64.AppImage
  ./MoonBeam_IG_*_amd64.AppImage
  ```
  On Ubuntu 22.04+ / Mint 21+ it needs FUSE 2: `sudo apt install libfuse2t64` (Ubuntu 24.04, Mint 22) or `libfuse2` (Ubuntu 22.04, Mint 21). It also needs webkit2gtk 4.1, GTK 3 and libayatana-appindicator3.

Then log in once and add your people, as on Windows. Both versions update themselves (the .deb asks for your password to install an update).

- **Keyring:** your login is kept encrypted with a key in your desktop's keyring, so a keyring must be running. GNOME, Cinnamon, MATE and XFCE ship gnome-keyring; on a minimal system run `sudo apt install gnome-keyring`.
- **Tray:** Cinnamon, KDE, XFCE and MATE show the tray icon out of the box. On stock GNOME, enable the "AppIndicator and KStatusNotifierItem Support" extension (Ubuntu has it on by default).
- **Uninstall:** `sudo apt remove moon-beam-ig` for the .deb, or delete the AppImage. Your data is in `~/.config/MoonBeam_IG`.

> **Note:** Uses Instagram's unofficial web endpoints, which is against Instagram's ToS. Personal use only, at your own account risk.
>
> <sub>Not affiliated with Instagram or Meta. Instagram is a trademark of Meta Platforms, Inc.</sub>

Full video: [media/showcase.mp4](media/showcase.mp4)

