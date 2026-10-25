# YT Downloader — downloads & updates

Portable Windows download manager for YouTube and 1,000+ sites. This repository only holds the
release files; it contains no source code.

## Download (always the latest version)

**[⬇ YTDownloader.zip](https://github.com/Hamza2136/YTDownloader-updates/releases/latest/download/YTDownloader.zip)**

`https://github.com/Hamza2136/YTDownloader-updates/releases/latest/download/YTDownloader.zip`

## Install
1. Right-click `YTDownloader.zip` → **Extract All** → choose a normal folder (Desktop, Documents, `D:\Apps`).
   Not `C:\Program Files`, because updates can't write there.
2. Open the `YTDownloader` folder and run **YTDownloader.exe**. If Windows says *"Windows protected your PC"*,
   click **More info → Run anyway** (only the first time; the app is not code-signed).
3. On first start the app asks to install its engines: click **Yes**, then in Engine Center click
   **Download Official GitHub Latest**. It downloads yt-dlp, FFmpeg and Deno (about 260 MB) from their
   official GitHub releases into the app's `engine` folder.

Requirements: Windows 10 or 11 (64-bit) and an internet connection.

## Updates
Nothing to do: the app checks this repository when it starts and offers new versions itself. Every package
is checked (size, SHA-256 checksum and version) before it is installed, and a failed install restores the
previous version. Settings, the download list and downloaded files are never touched by an update.

Each release contains:

| File | Purpose |
|------|---------|
| `YTDownloader.zip` | The app, for new installs (engines are downloaded on first start) |
| `YTDownloader_update_<version>.zip` | The same app files, used by the built-in updater |
| `version_manifest.json` | Version, changelog, download link and checksum the app reads |

## Third-party components
The app downloads these programs from their official sources on first start (they are not part of
the files in this repository):
- [yt-dlp](https://github.com/yt-dlp/yt-dlp) (Unlicense)
- [FFmpeg](https://ffmpeg.org) builds from [yt-dlp/FFmpeg-Builds](https://github.com/yt-dlp/FFmpeg-Builds) (GPL; source code available there)
- [Deno](https://github.com/denoland/deno) (MIT)

Please respect the terms of the sites you download from and copyright law.
