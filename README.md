# PicoPlay — Official Unified Portal 🎮📱

[![GitHub Pages Deployment](https://github.com/birth1mark/picoplay/actions/workflows/deploy.yml/badge.svg)](https://birth1mark.github.io/picoplay/)
[![PS4 Release](https://img.shields.io/github/v/release/birth1mark/picoplay-ps4?label=PS4%20PKG&color=0070d1)](https://github.com/birth1mark/picoplay-ps4/releases/latest)
[![Android Release](https://img.shields.io/github/v/release/birth1mark/picoplay-android?label=Android%20APK&color=00e436)](https://github.com/birth1mark/picoplay-android/releases/latest)
[![itch.io](https://img.shields.io/badge/itch.io-birth1mark.itch.io%2Fpicoplay-fa5c5c)](https://birth1mark.itch.io/picoplay)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> **Official Live Website**: [https://birth1mark.github.io/picoplay/](https://birth1mark.github.io/picoplay/)

**PicoPlay** is an authentic, high-performance C++ player and arcade emulator for 8-bit fantasy console cartridges (PICO-8 compatible). It is engineered natively for both jailbroken **PlayStation 4** consoles and **Android** mobile devices/gaming handhelds.

---

## 🚀 Platforms

### 🎮 [PlayStation 4 (`picoplay-ps4`)](https://github.com/birth1mark/picoplay-ps4)
- **Engine**: C++17 with OpenOrbis Toolchain & SDL2 software framebuffer blitter.
- **Performance**: Rock-solid 60 FPS with hardware VSYNC synchronization (`sceVideoOutSubmitFlip` + `sceKernelWaitEqueue`) and custom `-O2` scanline integer scaler (< 0.3 ms per frame).
- **Control Innovations**: Direct DualShock 4 touchpad & right stick mouse cursor emulation (`stat(32)`, `stat(33)`, `stat(34)`) for mouse-driven games like *Slipways*.
- **Deployment**: Single Fake PKG (`picoplay-ps4.pkg`) installable via GoldHEN Package Installer.

### 📱 [Android (`picoplay-android`)](https://github.com/birth1mark/picoplay-android)
- **Engine**: Native NDK C++ core with SDL2 Android backend.
- **Modern Compatibility**: Full **16 KB page-size memory alignment** compliant with Android 15 & 16 requirements.
- **Controls**: Pocket Touch Gamepad with haptic feedback, customizable layout, plus USB/Bluetooth controller support (Retroid Pocket, AYN Odin, 8BitDo).
- **Deployment**: Standalone APK and Google Play bundle (AAB).

---

## 🛒 Features
- **In-App BBS Arcade Store**: Browse, search, and download thousands of public domain and indie cartridges directly from Lexaloffle BBS inside the player.
- **Chiptune Audio Synthesizer**: 4-channel authentic sound chip with real-time waveform synthesis.
- **Built-in Starter Pack**: Pre-loaded with classics like *Slipways*, *Celeste*, *Pullfrog*, and *Mistigri*.
- **Save State & Cart Data**: Full support for `cartdata()`, `dget()`, and `dset()` persistent game saves.

---

## 🛠️ DevOps & Web Portal Structure

```text
picoplay/
├── .github/
│   └── workflows/
│       └── deploy.yml       # Automated GitHub Pages CI/CD deployment
├── assets/
│   ├── hero-banner.png      # 1024x500 OpenGraph & Twitter banner
│   ├── icon-512.png         # High-resolution vector/pixel icon
│   ├── icon-ps4.png         # PlayStation 4 icon0.png
│   ├── favicon-32.png       # 32x32 Favicon
│   ├── icon-192.png         # 192x192 PWA icon
│   ├── screenshot-ps4.png   # 1280x720 PS4 arcade capture
│   └── screenshot-android.png # High-res Android gameplay
├── index.html               # Semantic HTML5, WCAG accessible, SEO optimized
├── manifest.webmanifest     # PWA manifest
├── robots.txt               # Crawler directives
├── sitemap.xml              # XML Sitemap with image extensions
└── README.md
```

---

## 📄 License & Disclaimer

Maintained by **[birth1mark](https://github.com/birth1mark)**.

*Disclaimer: PICO-8 is a registered trademark of Lexaloffle Games. PicoPlay is an independent open-source recreation and is not affiliated with or endorsed by Lexaloffle Games.*
