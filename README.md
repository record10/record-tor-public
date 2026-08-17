<h1 align="center">
  <br>
  <img src="docs/logo.png" alt="RecordTor Logo" width="128">
  <br>
  RecordTor
  <br>
</h1>

<h4 align="center">Next-Gen Ultra-Fast BitTorrent Downloader & Wi-Fi Media Streaming Engine</h4>

<p align="center">
  <a href="https://github.com/Record10/record-tor-public/releases/latest">
    <img src="https://img.shields.io/github/v/release/Record10/record-tor-public?label=Download%20Latest&style=for-the-badge&color=6366f1" alt="Download Latest Release"/>
  </a>
  <a href="https://github.com/Record10/record-tor-public/issues">
    <img src="https://img.shields.io/github/issues/Record10/record-tor-public?style=for-the-badge&color=ec4899" alt="Report Issues"/>
  </a>
  <img src="https://img.shields.io/badge/Platform-macOS%20%7C%20Windows%20%7C%20Linux%20%7C%20Android-blue?style=for-the-badge" alt="Platforms"/>
  <img src="https://img.shields.io/badge/Rust-High%20Performance-orange?style=for-the-badge&logo=rust" alt="Rust Core"/>
</p>

<p align="center">
  <b>RecordTor</b> is a modern, high-performance BitTorrent client built with a <b>Rust engine (librqbit)</b> and a sleek Angular interface. Stream videos instantly while downloading, read PDFs & EPUBs and listen to audiobooks in-app, share media seamlessly over local Wi-Fi, and sync progress across all your devices using a unified SQLite backend.
</p>

---

## Key Highlights

- ⚡ **Stream While Downloading**: Instant video playback — start watching within seconds, even before the torrent finishes downloading.
- 📱 **Wi-Fi Media Sharing & QR Stream**: Stream your downloads directly to any phone, tablet, smart TV, or web browser on your local Wi-Fi using instant QR code pairing.
- 🔄 **Cross-Device Progress Sync**: Watch progress (timestamps, watched status, duration) synchronizes live across Desktop and Mobile Wi-Fi clients via central Rust SQLite (`recordtor.db`).
- 🎬 **Instant MKV Remuxing**: Real-time FFmpeg-powered audio/video remuxing for smooth in-browser playback of MKV, AVI, and MP4 formats.
- 📚 **Built-in PDF, EPUB & Audiobook Readers**: Read PDFs, EPUBs, and listen to audiobooks right inside the app — with search, zoom, typography controls, chapter navigation, and cross-device reading position sync.
- 🔍 **Legal Search Engine & Custom Indexers**: Built-in Internet Archive (`archive.org`) public domain search indexer + custom JSON API provider support.
- 🚀 **Ultra-Fast Rust Core**: Powered by `librqbit` in Rust with automatic file descriptor limit expansion (65,536 open files) for maximum multi-gigabit throughput.
- 🐛 **Direct Issue Reporting**: Integrated 1-click bug reporting directly to GitHub Issues.

---

## ⚡ Feature Overview

### 📥 Torrent Management
- **Magnet & File Support**: Open `magnet:` URLs or `.torrent` files instantly via protocol association.
- **Piece Visualizer**: Interactive visualizer showing real-time piece completion.
- **File Priority Control**: High, medium, low, or ignore priorities per file.
- **Seeding & Speed Limits**: Configurable upload/download caps (MB/s) and seeding ratios.
- **Network Controls**: Dynamic port selection, UPnP, NAT-PMP, DHT network, and Peer Exchange (PEX).
- **Hide / Unhide Torrents**: Tuck away torrents (individually or in bulk) to keep the list clean, with a dedicated view to bring them back.

### 📺 Built-in Media Player & Streaming
- **Picture-in-Picture (PiP)**: Keep watching in a floating mini-player while browsing.
- **Gesture Controls**: Touch & mouse gestures for brightness, volume, and seeking.
- **System Stay-Awake**: Optional sleep prevention to keep downloads active while streaming over Wi-Fi.

### 📚 Readers & Audiobooks
- **PDF Viewer**: In-app PDF reading with page navigation, zoom presets, full-text search, reading mode, and saved position.
- **EPUB Reader**: Chapter (TOC) navigation, typography panel with 10+ fonts (including OpenDyslexic), reading themes (Day, Sepia, Amber, Night), adjustable font size, and full-text search.
- **Audiobook Player**: Dedicated audiobook mode with chapter & track playlist, sleep timer, playback speed control, and ±15s skip — playback continues while the file is still downloading.
- **Cross-Device Reading Sync**: Reading position (page, chapter, timestamp) syncs across Desktop and Mobile Wi-Fi clients.

### 🎨 Modern UI & Tray Support
- **Glassmorphism Theme**: Vibrant dark/light theme switching with modern design system.
- **System Tray**: Minimize to system tray and download quietly in the background (Desktop).
- **Auto-Update**: Built-in updater notifications for seamless version upgrades.

---

## 🚀 Downloads

Download the latest installer for your platform from the [**Releases Page**](https://github.com/Record10/record-tor-public/releases/latest):

| Platform | Installer File | Architecture |
| :--- | :--- | :--- |
| 🍏 **macOS (Apple Silicon)** | `RecordTor-aarch64.dmg` | Apple Silicon (M1/M2/M3/M4) |
| 🍏 **macOS (Intel)** | `RecordTor-x86_64.dmg` | Intel 64-bit |
| 🪟 **Windows** | `RecordTor-x86_64-setup.exe` | Windows 10 / 11 (64-bit) |
| 🐧 **Linux (AppImage)** | `record-tor_amd64.AppImage` | Universal Linux |
| 🐧 **Linux (Debian/Ubuntu)** | `record-tor_amd64.deb` | Debian / Ubuntu |
| 🤖 **Android** | `RecordTor-arm64.apk` | Android 8.0+ (ARM64) |

---

## 🔧 Installation Instructions

### macOS
1. Download `RecordTor.dmg` from [Releases](https://github.com/Record10/record-tor-public/releases/latest).
2. Open the `.dmg` and drag **RecordTor** to your **Applications** folder.
3. If macOS displays an unsigned app warning on first launch, clear the Gatekeeper quarantine flag once in Terminal:
   ```bash
   xattr -cr /Applications/RecordTor.app
   ```

### Windows
1. Download `RecordTor_x64-setup.exe` from [Releases](https://github.com/Record10/record-tor-public/releases/latest).
2. Run the installer.
3. If Windows SmartScreen appears, click **"More info"** → **"Run anyway"**.

### Linux
- **AppImage**:
  ```bash
  chmod +x record-tor_amd64.AppImage
  ./record-tor_amd64.AppImage
  ```
- **Debian / Ubuntu**:
  ```bash
  sudo dpkg -i record-tor_amd64.deb
  ```

### Android
1. Download `RecordTor-arm64.apk` from [Releases](https://github.com/Record10/record-tor-public/releases/latest).
2. Allow installation from unknown sources if prompted by Android.

---

## 💬 Community & Bug Reporting

Found a bug, have a suggestion, or need help? 
Submit an issue on our public GitHub repository:

👉 [**File a Bug Report or Feature Request**](https://github.com/Record10/record-tor-public/issues)

---

## 📜 License

All rights reserved. Provided as-is for personal use.
