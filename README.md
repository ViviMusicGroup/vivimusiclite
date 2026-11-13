<div align="center">
    <img src="./app/src/main/ic_launcher-playstore.png" width="120" height="120" style="display: block; margin: 0 auto" alt="ViviMusic Lite Logo"/>
    <h1>ViviMusic Lite</h1>
    <p><strong>A beautiful, fast, and lightweight YouTube Music streaming client for Android.</strong></p>
    <p>Ad-free • Background Playback • Word-Synced Lyrics • Material 3 Expressive • Account Sync</p>

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](./LICENSE)
[![Android](https://img.shields.io/badge/Android-7.0%2B-green.svg)](https://developer.android.com)
[![Kotlin](https://img.shields.io/badge/Kotlin-2.1-purple.svg)](https://kotlinlang.org)
[![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose-4285F4.svg)](https://developer.android.com/jetpack/compose)
[![Media3](https://img.shields.io/badge/Audio-AndroidX%20Media3-red.svg)](https://developer.android.com/media/media3)

[**Download Latest APK**](https://github.com/ViviMusicGroup/vivimusiclite/releases/latest) • [**Report an Issue**](https://github.com/ViviMusicGroup/vivimusiclite/issues)
</div>

---

## 🌟 Highlights

- 🚫 **100% Free & No Ads**: Seamless uninterrupted music streaming without audio or video advertisements.
- ⚡ **Lightweight & Battery Efficient**: Ultra-lean native Android app built with Jetpack Compose and ExoPlayer.
- 🔐 **YouTube Music Account Sync**: Optional Google sign-in to sync Liked Songs, Playlists, Subscribed Artists, and listening history.
- 🎤 **Live Synchronized Lyrics**: Word-by-word feathered karaoke sweep, duet vocals, and instrumental interlude indicators.
- 🎨 **Material 3 Expressive Design**: Fluid animations, dynamic Material You color theming, AMOLED Pure Black, and real-time artwork blur.
- 🔁 **Smart Autoplay (Infinity Queue)**: Seamlessly discovers and queues similar songs when your playlist ends.
- 💾 **Full Library & Account Backup**: Export and restore your complete database, favorites, and login session across devices.

---

## ✨ Features

### 🎧 Seamless Playback & Smart Queue
- **Background Playback**: Keep listening with the screen off or while multitasking in other apps.
- **Offline Caching**: Automatically caches streamed tracks for fast replays and offline enjoyment.
- **Infinity Queue**: Automatically fetches YouTube Radio tracks so the music never stops.
- **Persistent State**: Remembers your active queue and position even after closing or restarting the app.
- **Queue Controls**: Drag-to-reorder tracks, queue lock/unlock, shuffle, repeat (all / single), and sleep timer.
- **Audio Output Switcher**: Live indicator showing connected Bluetooth devices, wired headphones, or phone speakers.
- **Stream Recovery**: Real-time error diagnostics with one-tap **Copy Error** and **Retry** to immediately resume playback.

### 🎨 Modern Visuals & Player Experience
- **Custom Player Backgrounds**: Choose between **Blur** (crossfading artwork blur engine) or clean **Material** styling.
- **Apple Music Motion Artwork**: Optional looping animated video album covers (HLS stream via `:motionart`).
- **Interactive Seekbars**: Apple-style linear expanding progress pill or classic squiggly waveform.
- **Audio Quality Details**: Detailed bitrates, audio codecs, and format tiers via the *Details & Credits* menu.
- **Adaptive Layouts**: Full landscape and tablet optimization with dual-pane queue and lyrics view.

### 🎤 Word-by-Word Synchronized Lyrics
- **Multi-Source Engine**: Powered by LRCLIB, KuGou, and Apple Music TTML with automatic fallback.
- **Animated Karaoke Glow**: Feathered word-level highlighting with sustained vocal tracking.
- **Duet Vocal Separation**: Automatic left/right vocal lane separation for duets and backup vocals.
- **Instrumental Indicators**: Rhythm-synced interlude cookies that count down until vocals resume.

### 📚 Discovery & Library Management
- **Personalized Home Feed**: Dynamic carousels directly from YouTube Music (*Quick picks, Mixed for you, Listen again, New releases*).
- **Search Everything**: Instant search across tracks, albums, artists, music videos, and community playlists.
- **Local Playlists & Favorites**: Organize custom playlists, mark favorites with quick ❤️, and import/export playlists.
- **Android Auto**: Full support for dashboard controls and car displays.

---

## 📥 Download & Installation

1. Grab the latest `.apk` from [**GitHub Releases**](https://github.com/ViviMusicGroup/vivimusiclite/releases/latest).
2. If prompted, allow installation from unknown sources in Android Settings.
3. Open **ViviMusic Lite** and start listening!

> **Tip:** You can check for updates directly inside the app under **Settings → About**.

---

## 🛠️ Building from Source

```bash
git clone https://github.com/ViviMusicGroup/vivimusiclite.git
cd vivimusiclite
./gradlew assembleDebug
```

### Prerequisites
- **JDK 17**
- **Android SDK Platform 35**
- Gradle 8.7+

---

## 🧩 Project Architecture

| Module | Description |
|---|---|
| `:app` | Primary Android application, Compose UI, Player service, and Room SQLite database |
| `:innertube` | YouTube Music API client, extractor, and response deserializers |
| `:lyricsprovider` | Unified synchronized and plain lyrics resolver (LRCLIB & KuGou) |
| `:motionart` | HLS video motion artwork extractor |
| `:ktor-client-brotli` | Brotli decompression compression engine for Ktor |
| `:compose-routing` | Navigation and screen routing |
| `:compose-reordering` | Smooth drag-and-drop reordering utilities |
| `:compose-persist` | State persistence across screen navigations |

---

## ⚖️ Disclaimer

This project is not affiliated with, authorized, or endorsed by Google LLC, YouTube, Apple Inc., or any of their affiliates. All trademarks, service marks, and company names belong to their respective owners.

Distributed under the [**GNU General Public License v3.0**](./LICENSE).
