<div align="center">

<img src="./SetupIcon.ico" width="100" height="100" alt="Insight Player Logo" />

# Insight Player v2.0 (Pro)
### A Modern, Lightweight & Powerful Media Player for Windows
**High-Performance Multimedia Playback Engine Powered by Qt 6 & LibVLC**

[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-0078D6?logo=windows)](https://microsoft.com)
[![Version](https://img.shields.io/badge/Version-2.0.0%20Pro-10B981)](https://github.com)
[![Qt](https://img.shields.io/badge/Qt-6.11.1-41CD52?logo=qt)](https://www.qt.io)
[![C++](https://img.shields.io/badge/C%2B%2B-17-00599C?logo=c%2B%2B)](https://isocpp.org)
[![Engine](https://img.shields.io/badge/Engine-LibVLC%203.0-FF8800?logo=vlc-media-player)](https://www.videolan.org/vlc/libvlc.html)
[![License](https://img.shields.io/badge/License-Proprietary%20%2F%20LGPLv2.1-blue)](LICENSE)

<br/>

[English Description](#overview) • [الميزات بالعربية](#الميزات-الرئيسية-باللغة-العربية) • [Key Features](#key-features) • [Media Converter & Toolkit](#media-converter--toolkit-pro) • [Supported Formats](#supported-formats) • [Installation](#installation) • [Building from Source](#building-from-source)

<br/>

![Insight Player Screenshot](./Screenshot%202026-10-30%20072753.png)

</div>

---

## Overview

**Insight Player v2.0** is a next-generation Windows desktop media player crafted for users and professionals who demand pristine playback quality, an elegant distraction-free dark interface, and extensive media manipulation tools. 

Engineered with **C++17**, **Qt 6**, and the robust **LibVLC 3.0** decoding core, Insight Player plays virtually any audio, video, or disc format without the need for bloated external codec packs. Version 2.0 brings deep Windows Explorer integration with instantaneous **Double-Click** launch, seamless **"Open with"** registry associations, complete **Unicode & Arabic filename/path fidelity**, a standalone **Media Converter & Toolkit**, and a real-time **Dynamic Audio Waveform Visualizer**.

---

## الميزات الرئيسية (باللغة العربية)

* **تشغيل فوري عبر النقر المزدوج (Double-Click):** تشغيل أي ملف صوتي أو فيديو فوراً عند النقر المزدوج عليه في مستكشف Windows أو اختياره عبر قائمة **"فتح بواسطة" (Open With)**.
* **دعم كامل للغة العربية والمسارات المعقدة (Arabic & Unicode Paths):** دعم كامل بنسبة 100% للأسماء والمسارات باللغة العربية دون أي تلف في الترميز (UTF-8 / Unicode).
* **إدارة النسخة الواحدة (Single-Instance IPC):** عند فتح ملفات جديدة أثناء تشغيل البرنامج، يتم نقلها وتشغيلها فوراً داخل النافذة المفتوحة دون تكرار فتح البرنامج.
* **محرك المؤثرات البصرية التفاعلي (Native Audio Waveform):** مؤثر بصري حي مدمج برمجياً يرسم الترددات والموجات الصوتية مع اسم التراك بدقة متناهية (تم الاستغناء عن ملفات GIF لتقليل الحجم وتسريع الأداء).
* **أداة التحويل والمونتاج (Media Converter & Toolkit - Pro):** تحويل صيغ الفيديو والصوت، قص وتقطيع المقاطع بالثواني، واستخراج ودمج الترجمات.
* **معالجة الفيديو والألوان وتأثيرات الصوت (Effects & Equalizer):** معادل صوتي رسومي 10 حزم، والتحكم في السطوع والتباين والتشبع وألوان الفيديو في الوقت الفعلي.
* **شريط تحكم عائم في ملء الشاشة (Floating HUD):** وصول سهل وفوري لجميع أدوات التشغيل والصوت والالتقاط بمجرد تحريك الماوس في وضع ملء الشاشة.
* **التقاط صور الشاشة (Snapshot with Toast):** تصوير لقطات بدقة الفيديو الأصلية مع تأثير وميض بصري ومعاينة سريعة للقطة المحفوظة.
* **محرك الترجمات الاحترافي:** دعم كامل لملفات الترجمة (`.srt`, `.ass`, `.vtt`)، ضبط المزامنة والتوقيت، والتنسيق وتنزيل الترجمات.

---

## Key Features

### 🚀 Seamless Windows Explorer Integration
* **Instant Double-Click Playback:** Native Win32 argument processing using `CommandLineToArgvW` ensures zero character corruption and immediate playback.
* **Full File Type Association:** Automatic registry integration with HKCU/HKCR for all recognized audio & video extensions.
* **Single Instance IPC (LocalServer):** Queue or play files from anywhere in Windows directly into the running instance in under 3 milliseconds.

### 🎵 High-Fidelity Audio Engine
* **Dynamic Waveform Visualizer:** Native Qt `QPainter` drawing engine rendering smooth frequency pulses and track metadata without external GIF/video overhead.
* **10-Band Graphic Equalizer:** Custom presets (Rock, Pop, Classical, Vocal Boost, Bass Boost, Flat) with manual preamp and band tuning.
* **Audio Spatializer & Channels:** Instant stereo, left-channel, right-channel, and reverse stereo matrix switching.

### 🎬 Advanced Video Playback
* **Floating Fullscreen HUD:** Automatic autohide on fullscreen, exposing seekbar, time, volume, snapshot, and chapter controls.
* **Real-time Color Grading:** Hardware-accelerated adjustments for Contrast, Brightness, Saturation, Gamma, and Hue.
* **Aspect Ratio & Window Scaling:** 16:9, 4:3, 1:1, 2.35:1 (Cinemascope), 2.39:1, 5:4, and custom fit-to-window modes.
* **Picture-in-Picture (PiP):** Compact, frameless floating mode for multitasking.

### 🛠️ Media Converter & Toolkit (Pro)
* **Format Converter:** Transcode between popular container formats (MP4, MP3, MKV, AVI, WEBM, WAV, OGG).
* **High-Precision Trimmer / Cutter:** Trim audio/video losslessly with start and end time stamps (`HH:mm:ss`).
* **Subtitle Extractor:** Extract embedded subtitle streams into clean `.srt` text files.
* **Subtitle Hardcoding & Softcoding:** Burn subtitles permanently onto video frames or mux them into an MKV container.

### 📋 Intelligent Playlist & Media History
* **Live Search Filter:** Instant fuzzy search across playlists with thousands of files.
* **Drag-and-Drop:** Intuitive reordering, multi-file and entire folder dropping.
* **Smart History:** Recent files menu remembering up to 20 recently played items.

---

## Media Converter & Toolkit (Pro)

Insight Player includes a dedicated built-in conversion suite accessible from `Tools -> Media Converter`:

| Feature | Description | Modes |
|:---|:---|:---|
| **Transcoder** | Convert any media to target formats | MP4, MP3, MKV, AVI, WEBM, WAV, OGG |
| **Trimmer / Cutter** | Cut segments with millisecond precision | Stream Copy (Lossless) / Fast Cut |
| **Subtitle Extraction** | Extract stream track into standalone `.srt` | Automatic track index mapping |
| **Subtitle Burner** | Apply subtitles directly onto video | Hardcode (Permanent) / Softcode (Mux) |

---

## Supported Formats

| Category | File Extensions |
|:---|:---|
| **Video Containers** | `.mp4`, `.mkv`, `.avi`, `.mov`, `.wmv`, `.flv`, `.webm`, `.m4v`, `.mpg`, `.mpeg`, `.ts`, `.m2ts`, `.vob`, `.3gp` |
| **Audio Formats** | `.mp3`, `.wav`, `.aac`, `.flac`, `.ogg`, `.m4a`, `.wma`, `.opus`, `.alac`, `.aiff` |
| **Subtitles** | `.srt`, `.ass`, `.ssa`, `.vtt`, `.sub`, `.idx` |
| **Physical Media** | DVD-Video (ISO/Folder/Disc), Blu-ray (unprotected) |

---

## Keyboard Shortcuts

| Shortcut | Action |
|:---|:---|
| **Space** | Play / Pause toggle |
| **Left / Right Arrow** | Seek backward / forward 5 seconds |
| **Shift + Left / Right** | Seek backward / forward 15 seconds |
| **Up / Down Arrow** | Increase / Decrease volume by 5% |
| **M** | Mute / Unmute audio |
| **F** or **Double-Click** | Toggle Fullscreen mode |
| **Esc** | Exit Fullscreen |
| **Ctrl + O** | Open Media File |
| **Ctrl + Shift + O** | Open Media Folder |
| **S** | Take Video Snapshot |
| **P** | Toggle Playlist Panel |
| **E** | Open Video & Audio Effects |
| **Ctrl + K** | Open Media Converter & Toolkit |

---

## Installation

### Pre-Built Binary (Installer)
1. Download **[InsightPlayer_Setup_v2.0.exe](./InsightPlayer_Setup_v2.0.exe)**.
2. Run the setup wizard.
3. Select your preferred installation path and check **"Associate Media Files"** to enable double-click playback.
4. Launch Insight Player from your desktop or start menu.

---

## Building from Source

### Prerequisites
* **Windows 10 / 11** (64-bit)
* **CMake 3.20+**
* **MinGW-W64 GCC 13+** (or UCRT64 toolchain)
* **Qt 6.6+** (Widgets, Gui, Core, Network)
* **VLC SDK 3.0.x** (Included in `vlc_sdk/`)

### Build Steps

```powershell
# 1. Clone the repository
git clone https://github.com/insight-tools/insight-player.git
cd insight-player

# 2. Configure build environment
cmake -B build -G "MinGW Makefiles" -DCMAKE_BUILD_TYPE=Release

# 3. Compile the application
cmake --build build -j4

# 4. Package Inno Setup Installer (Optional)
& "C:\Program Files\Inno Setup 7\ISCC.exe" "InsightPlayer_Setup.iss"
```

The output executable will be placed at `bin/InsightPlayer.exe` alongside all required LibVLC runtimes and translations.

---

## Tech Stack & Architecture

```
Insight Player Architecture
┌────────────────────────────────────────────────────────┐
│               Qt 6 GUI Layer (Widgets)                 │
│  ┌───────────────────────┐   ┌──────────────────────┐  │
│  │ Floating Fullscreen   │   │  Audio Waveform      │  │
│  │ HUD & Controls        │   │  Visualizer (Native) │  │
│  └───────────────────────┘   └──────────────────────┘  │
│  ┌───────────────────────┐   ┌──────────────────────┐  │
│  │ Playlist & Search     │   │ Media Info & Status  │  │
│  └───────────────────────┘   └──────────────────────┘  │
├────────────────────────────────────────────────────────┤
│           Core Engine Integration Layer                │
│  ┌───────────────────────┐   ┌──────────────────────┐  │
│  │ VlcPlayer (LibVLC 3.0)│   │ Single-Instance IPC  │  │
│  └───────────────────────┘   └──────────────────────┘  │
│  ┌───────────────────────┐   ┌──────────────────────┐  │
│  │ Win32 Associations    │   │ Converter / Toolkit  │  │
│  └───────────────────────┘   └──────────────────────┘  │
├────────────────────────────────────────────────────────┤
│                     Operating System                   │
│             Windows 10 / 11 (64-bit NT Kernel)         │
└────────────────────────────────────────────────────────┘
```

---

## Support & Contact

* **Developer & Publisher:** INSIGHT TOOLS
* **Official Website:** [https://insight-ye.com](https://insight-ye.com)
* **Documentation:** Built-in PDF guide available via `Help -> User Guide`
* **Issue Tracker:** Submit bug reports and feature requests via GitHub Issues

---

<div align="center">
  <sub>Copyright © 2026 INSIGHT TOOLS. All rights reserved.</sub>
</div>
