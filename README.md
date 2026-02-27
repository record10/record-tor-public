<h1 align="center">RecordTor</h1>

<p align="center">
  A modern, lightweight desktop torrent client with built-in video streaming.
</p>

<p align="center">
  <a href="https://github.com/Record10/record-tor-public/releases/latest">
    <img src="https://img.shields.io/github/v/release/Record10/record-tor-public?label=Download&style=for-the-badge" alt="Download Latest Release"/>
  </a>
</p>

---

## Features

- **Torrent Downloads** — Add torrents via magnet links or `.torrent` files
- **Stream While Downloading** — Watch video content as it downloads, no need to wait
- **Create Torrents** — Create `.torrent` files from your local directories
- **File Priority Control** — Choose which files to download and set per-file priority (high/medium/low)
- **Video Player** — Built-in video player with playback progress tracking
- **Seeding Controls** — Configure seed ratio and automatic seeding behavior
- **Dark / Light Theme** — Switch between dark and light mode
- **Deep Linking** — Open magnet links directly from your browser via `torrent://` protocol
- **System Tray** — Minimize to tray and keep downloading in the background
- **Start on Boot** — Optionally launch RecordTor when your system starts
- **Cross-Platform** — Available for macOS, Windows, and Linux

---

## Download

Head to the [**Releases**](https://github.com/Record10/record-tor-public/releases/latest) page and download the installer for your operating system:

| Platform             | File                        |
| -------------------- | --------------------------- |
| **macOS**            | `RecordTor_x64.dmg`         |
| **Windows**          | `RecordTor_x64-setup.exe`   |
| **Linux (AppImage)** | `record-tor_amd64.AppImage` |
| **Linux (Debian)**   | `record-tor_amd64.deb`      |

---

## Installation

### macOS

1. Download `RecordTor_x64.dmg` from the [Releases](https://github.com/Record10/record-tor-public/releases/latest) page.
2. Open the `.dmg` file and drag **RecordTor** into your **Applications** folder.
3. **Important — the app is unsigned.** macOS will block it on first launch. To allow it, run the following command in Terminal **once** after installation:

   ```bash
   xattr -cr /Applications/RecordTor.app
   ```

4. Now you can open RecordTor normally from Applications.

### Windows

1. Download `RecordTor_x64-setup.exe` from the [Releases](https://github.com/Record10/record-tor-public/releases/latest) page.
2. Run the installer and follow the on-screen instructions.
3. **The app is unsigned**, so Windows SmartScreen may show a warning. Click **"More info"** and then **"Run anyway"** to proceed with the installation.

### Linux

#### AppImage

1. Download `record-tor_amd64.AppImage` from the [Releases](https://github.com/Record10/record-tor-public/releases/latest) page.
2. Make it executable and run:

   ```bash
   chmod +x record-tor_amd64.AppImage
   ./record-tor_amd64.AppImage
   ```

#### Debian / Ubuntu (.deb)

1. Download `record-tor_amd64.deb` from the [Releases](https://github.com/Record10/record-tor-public/releases/latest) page.
2. Install it:

   ```bash
   sudo dpkg -i record-tor_amd64.deb
   ```

---

## Troubleshooting

### macOS — "App is damaged and can't be opened"

This happens because the app is not signed with an Apple Developer certificate. Run the following command to remove the quarantine flag:

```bash
xattr -cr /Applications/RecordTor.app
```

### Windows — SmartScreen warning

Click **"More info"** → **"Run anyway"**. This warning appears because the app is not signed with a Windows code-signing certificate.

### Linux — AppImage won't launch

Make sure the file is executable:

```bash
chmod +x record-tor_amd64.AppImage
```

---

## License

All rights reserved. This software is provided as-is for personal use.
