<p align="center">
  <img src="https://raw.githubusercontent.com/GetHorizontal63/seneca/793e4d1/apps/icons/tamarack.png" width="84" alt="Tamarack logo">
</p>

<h1 align="center">Tamarack</h1>

<p align="center"><b>Your movies, TV shows and live TV, on Windows and Android.</b></p>

Tamarack is an app for **[Seneca](https://github.com/GetHorizontal63/seneca)**, a media server you run at home for your own movies, TV shows and music. It connects to your Seneca server the way the Jellyfin app connects to Jellyfin: enter the address, sign in, and your library is there. Everything you do (what you've watched, where you stopped, liked songs, playlists) is kept on the server, so you can carry on in the browser or on another device.

<p align="center">
  <a href="https://github.com/GetHorizontal63/tamarack/releases/latest/download/Tamarack-Setup.exe"><b>⬇ Windows</b></a> ·
  <a href="https://github.com/GetHorizontal63/tamarack/releases/latest/download/Tamarack.apk"><b>⬇ Android</b></a> ·
  <a href="https://github.com/GetHorizontal63/tamarack/releases">All releases</a> ·
  <a href="https://github.com/GetHorizontal63/seneca">Seneca (the server)</a>
</p>

| | |
|---|---|
| Latest version | **0.1.9** |
| Released | 2026-11-16 |
| Requires | Windows 10 or 11 (64-bit), or Android 7.0 or newer, and a Seneca server |
| Built from | Seneca [`793e4d1`](https://github.com/GetHorizontal63/seneca/commit/793e4d1) |

## Install

You need a Seneca server running on your network first. Its **[README](https://github.com/GetHorizontal63/seneca#quick-start)** covers TrueNAS, Docker and Windows.

**Windows**
1. Download **[Tamarack-Setup.exe](https://github.com/GetHorizontal63/tamarack/releases/latest/download/Tamarack-Setup.exe)** and run it.
2. Windows may say the publisher is unknown, because the app isn't signed with a paid certificate. Press **More info → Run anyway**.

**Android**
1. On your phone, open **[Tamarack.apk](https://github.com/GetHorizontal63/tamarack/releases/latest/download/Tamarack.apk)**.
2. Open the downloaded file. Android asks to **allow installing unknown apps** for your browser or file manager: allow it, go back, and press **Install**.
3. Newer versions install over older ones. You won't lose anything, because it all lives on the server.

**Then, on either:**
1. Type your server's address, for example **`http://192.168.1.50:8430`**: the IP of the machine running Seneca, with port **8430**. If the address opens in a browser on the same device, Tamarack will connect too.
2. Sign in with your Seneca username and password.

To use a different server later: **Settings → Server → Change server**.

## Updating

Download the latest version from the links above and install it over the one you have.

## Something wrong?

| Problem | What to do |
|---|---|
| "Failed to fetch" or "can't be reached" when connecting | Open the same address in a browser on that device. If it doesn't load there either, check the device is on your home network (not mobile data), use the server's IP address rather than a name like `truenas.local`, and check the port. |
| "It isn't a Seneca server" | Something answered, but not Seneca. Check the port: Seneca uses **8430** unless you changed it. |
| Android won't install an update | Uninstall Tamarack and install the new one. You only need to enter the address and sign in again. |

This repository holds only releases. The source is in **[Seneca](https://github.com/GetHorizontal63/seneca)**: the apps are built from its web client (`web/`) with the shells in `apps/`.
