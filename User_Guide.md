# Insight Player v2.0 (Pro) — Comprehensive User Guide
**Official User Manual & Product Reference | INSIGHT TOOLS**

---

## 1. Introduction & Overview

**Insight Player v2.0** is a high-performance Windows multimedia player powered by **Qt 6** and the **LibVLC 3.0** engine. It is designed to deliver crystal-clear audio and video playback, a distraction-free dark interface, and powerful media manipulation tools.

### What's New in Version 2.0
* **Direct Explorer Double-Click Playback:** Click any audio or video file in Windows Explorer to play immediately.
* **Windows "Open with" Integration:** Full registry associations for all standard audio and video formats.
* **100% Arabic & Unicode Path Support:** Full fidelity for file names and folder paths containing Arabic characters or symbols without encoding errors.
* **Single Instance IPC:** Opening new media seamlessly routes the file to the active player window in milliseconds.
* **Native Dynamic Audio Waveform Visualizer:** High-performance, GPU-smooth dynamic waveform engine that displays the track title, format, and frequency pulse in real-time.
* **Media Converter & Toolkit (Pro):** Transcode media containers, trim segments with second precision, and extract or burn subtitles.
* **Real-Time Video Effects & 10-Band Equalizer:** Real-time color correction and graphic sound equalizer.
* **Floating Fullscreen HUD:** Auto-hiding control overlay during fullscreen playback.

---

## 2. Opening Media & Playback

### Ways to Open Media in Insight Player:
1. **Double-Click in Windows Explorer:**
   Simply double-click any media file (`.mp4`, `.mkv`, `.mp3`, `.wav`, etc.). Insight Player launches or brings itself to the front and starts playback immediately.
2. **Right-Click -> "Open with":**
   Choose **Insight Player** from the Windows context menu.
3. **Drag and Drop:**
   Drag any file or folder directly into the Insight Player window.
4. **Toolbar Buttons:**
   Click **Open File** (`Ctrl + O`) or **Open Folder** (`Ctrl + Shift + O`) at the top of the interface.
5. **Recent Files:**
   Access your 20 most recently played files from `File -> Recent Files`.

---

## 3. Playback Controls & Shortcuts

| Action | Mouse / UI | Shortcut | Description |
|:---|:---|:---|:---|
| **Play / Pause** | Center Play Button | `Space` | Toggle playback |
| **Seek Backward** | Skip Backward button | `Left Arrow` | Jump back 5 seconds |
| **Seek Forward** | Skip Forward button | `Right Arrow` | Jump forward 5 seconds |
| **Large Seek** | Seek slider | `Shift + Left/Right` | Jump 15 seconds |
| **Volume Control** | Volume slider / Wheel | `Up / Down Arrow` | Adjust volume by 5% |
| **Mute** | Speaker icon button | `M` | Mute or restore sound |
| **Fullscreen** | Fullscreen button | `F` or `Double-Click` | Enter/Exit fullscreen |
| **Exit Fullscreen** | Press key | `Esc` | Return to windowed mode |
| **Take Snapshot** | Camera icon button | `S` | Capture frame to Pictures |
| **Toggle Playlist** | Playlist icon button | `P` | Show/Hide playlist sidebar |
| **Video Effects** | Menu / Toolbar | `E` | Open Equalizer & Video Color |
| **Media Converter** | Menu `Tools` | `Ctrl + K` | Launch Converter & Toolkit |

---

## 4. Audio-Only Playback & Native Dynamic Visualizer

When playing an audio file (`.mp3`, `.flac`, `.wav`, `.aac`, `.ogg`, `.m4a`, etc.):
* **Dynamic Waveform Display:** Insight Player automatically activates the native `AudioVisualizerWidget`.
* **Track Metadata:** The visualizer displays the complete track name and file format dynamically.
* **Lightweight & High-Performance:** Renders dynamically at 60 FPS using Qt vector graphics with near-zero CPU footprint.
* **Toggle Visualizer:** You can toggle the visualizer on or off in `Preferences / Settings`.

---

## 5. Media Converter & Toolkit (Pro)

Accessible from `Tools -> Media Converter`:

### 1. Transcoder Tab
* Choose source video or audio file.
* Select target format: **MP4, MP3, MKV, AVI, WEBM, WAV, OGG**.
* Click **Start Conversion** to transcode.

### 2. Trim / Cut Tab
* Set **Start Time** and **End Time** in `HH:mm:ss`.
* Choose output path.
* Click **Trim Video/Audio** for lossless high-speed trimming.

### 3. Extract Subtitles Tab
* Select subtitle stream index (Stream 0, 1, 2...).
* Export embedded subtitles directly into a clean `.srt` file.

### 4. Burn Subtitles Tab
* Choose external subtitle file (`.srt`, `.ass`, `.vtt`).
* Select burning mode:
  * **Hardcode:** Permanently encodes subtitles onto the video frames.
  * **Softcode:** Fast stream muxing into an MKV container.

---

## 6. Video & Audio Effects (Equalizer & Color Grading)

Accessible from `Tools -> Effects` or pressing `E`:

### Audio Equalizer
* **10-Band Graphic Equalizer:** 60Hz, 170Hz, 310Hz, 600Hz, 1kHz, 3kHz, 6kHz, 12kHz, 14kHz, 16kHz.
* **Preamp slider:** Boost overall gain up to +12dB.
* **Built-in Presets:** Flat, Rock, Pop, Classical, Bass Boost, Vocal Boost.

### Video Color Grading
* **Brightness:** Fine-tune scene luminescence.
* **Contrast:** Enhance visual depth between dark and bright areas.
* **Saturation:** Control color vibrancy from monochrome to hyper-vivid.
* **Gamma:** Adjust mid-tone luminance without washing out shadows or highlights.
* **Hue:** Adjust color phase wheel.

---

## 7. Floating Fullscreen HUD

In fullscreen mode (`F` or `Double-Click` on the video area):
* The controls and title bar automatically hide to give an immersive cinematic experience.
* **Move your mouse** to immediately reveal the **Floating Fullscreen HUD** at the bottom of the screen.
* The HUD includes: Play/Pause, Previous/Next track, Seekbar with live timestamp, Volume slider, Mute, Snapshot, and Exit Fullscreen.
* Leaving the mouse still will automatically hide the HUD after 2 seconds.

---

## 8. Playlist Management & Search

* **Live Search Filter:** Type any text into the playlist search bar to filter thousands of tracks in real time.
* **Drag-and-Drop:** Drag external media files or folders directly into the playlist panel.
* **Shuffle & Repeat:** Toggle random playback (`Shuffle`) or loop current track/playlist (`Repeat`).
* **Clear & Options:** Right-click any playlist item to open properties, reveal in Explorer, or remove.

---

## 9. Subtitle Controls

* **Load External Subtitles:** `Subtitle -> Load Subtitle File` (`.srt`, `.ass`, `.vtt`).
* **Auto-Loading:** Place a subtitle file in the same folder with the same base name as the video (e.g., `movie.mp4` and `movie.srt`) and Insight Player loads it automatically.
* **Subtitle Track Selector:** Switch between multiple embedded audio/subtitle languages effortlessly from the `Subtitle -> Subtitle Tracks` menu.
* **Subtitle Settings:** Adjust font size, color, encoding, and delay alignment.

---

## 10. System Requirements & File Associations

* **Operating System:** Windows 10 or Windows 11 (64-bit).
* **Architecture:** x86_64.
* **File Associations:** Automatically configured during installation. Can be refreshed anytime by launching `InsightPlayer.exe`.
* **Hardware Acceleration:** Enabled automatically through Direct3D11 / LibVLC.

---

<div align="center">
  <sub>Insight Player v2.0 Pro | Developed by INSIGHT TOOLS | https://insight-ye.com</sub>
</div>
