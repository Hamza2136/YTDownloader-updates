# YT Downloader — updates

This repository only holds **update packages** for YT Downloader. It contains no source code.

You don't need to download anything here by hand: YT Downloader checks this repository at start-up
(or when you click **Updates**) and offers new versions itself. Every package is checked (size,
SHA-256 checksum and version) before it is installed, and a failed install restores the previous
version. Your settings, download list and downloaded files are never touched by an update.

Each release contains two files:

| File | Purpose |
|------|---------|
| `YTDownloader_update_<version>.zip` | The app files of that version |
| `version_manifest.json` | Version, changelog, download link and checksum the app reads |

Got YT Downloader from a friend and it never offers updates? Your copy is older than the update
system — ask them for a fresh copy once.
