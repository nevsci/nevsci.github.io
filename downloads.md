---
layout: page
title: Downloads
permalink: /downloads/
---

## The latest version of RYBA

**Windows (64-bit):**

- *Standard installer:* [**RYBA_1.34.0_x64-setup.exe**](../assets/projects/RYBA/Windows/RYBA_1.34.0_x64-setup.exe){: data-goatcounter-click="download-ryba-1.34.0-windows-setup" data-goatcounter-title="RYBA 1.34.0 Windows Installer" data-goatcounter-no-session="1" data-goatcounter-referrer="https://nevesely.science/downloads/" }
- *Portable executable, no installation:* [**RYBA_1.34.0_windows-x86_64_portable.exe**](../assets/projects/RYBA/Windows/RYBA_1.34.0_windows-x86_64_portable.exe){: data-goatcounter-click="download-ryba-1.34.0-windows-portable" data-goatcounter-title="RYBA 1.34.0 Windows Portable EXE" data-goatcounter-no-session="1" data-goatcounter-referrer="https://nevesely.science/downloads/" }

**Linux (Ubuntu 24.04 and compatible systems):**

- *Installer:* [**RYBA_1.34.0_amd64.deb**](../assets/projects/RYBA/Linux/RYBA_1.34.0_amd64.deb){: data-goatcounter-click="download-ryba-1.34.0-linux-deb" data-goatcounter-title="RYBA 1.34.0 Linux DEB" data-goatcounter-no-session="1" data-goatcounter-referrer="https://nevesely.science/downloads/" }
- *Self-contained package:* [**RYBA_1.34.0_amd64.AppImage**](../assets/projects/RYBA/Linux/RYBA_1.34.0_amd64.AppImage){: data-goatcounter-click="download-ryba-1.34.0-linux-appimage" data-goatcounter-title="RYBA 1.34.0 Linux AppImage" data-goatcounter-no-session="1" data-goatcounter-referrer="https://nevesely.science/downloads/" }

**macOS (macOS 13.0 and higher):**

- *Universal app (Intel and Apple Silicon):* [**RYBA_1.34.0_macos-universal.app.zip**](../assets/projects/RYBA/MacOS/RYBA_1.34.0_macos-universal.app.zip){: data-goatcounter-click="download-ryba-1.34.0-macos-universal" data-goatcounter-title="RYBA 1.34.0 macOS universal ZIP" data-goatcounter-no-session="1" data-goatcounter-referrer="https://nevesely.science/downloads/" }

### Windows SmartScreen notice

RYBA's Windows installer and portable executable are currently **unsigned**. Microsoft Defender SmartScreen may therefore display an *Unknown publisher* or *Windows protected your PC* warning when you first run them. This warning alone does not establish that RYBA is malicious, but it is not a security guarantee either. Download RYBA only from this official website and verify its SHA-256 checksum before running it. If you trust the verified download, Windows may offer **More info → Run anyway**. Do not disable SmartScreen globally.

### Verify your download (SHA-256)

[**Download RYBA 1.34.0 checksums**](../assets/projects/RYBA/RYBA_1.34.0_SHA256SUMS.txt) — contains the SHA-256 hash for each of the five packages.

On Windows, open PowerShell in the directory containing your download and run:

```powershell
Get-FileHash -Algorithm SHA256 .\RYBA_1.34.0_x64-setup.exe
```

Compare the resulting hash to the corresponding entry in the checksum file. On Linux or macOS, use `sha256sum <filename>` or `shasum -a 256 <filename>`, respectively. A matching hash confirms the file matches the published checksum; it does not independently establish that the program is safe.

## Older RYBA versions

Version numbers may skip intermediate builds because only tested releases are published.

**RYBA 1.26.0**

- Windows: [RYBA_1.26.0.exe](../assets/projects/RYBA/Windows/RYBA_1.26.0.exe){: data-goatcounter-click="download-ryba-1.26.0-windows-exe" data-goatcounter-title="RYBA 1.26.0 Windows EXE" data-goatcounter-no-session="1" }
- Linux: [RYBA_1.26.0_amd64.deb](../assets/projects/RYBA/Linux/RYBA_1.26.0_amd64.deb){: data-goatcounter-click="download-ryba-1.26.0-linux-deb" data-goatcounter-title="RYBA 1.26.0 Linux DEB" data-goatcounter-no-session="1" } · [RYBA_1.26.0_amd64.AppImage](../assets/projects/RYBA/Linux/RYBA_1.26.0_amd64.AppImage){: data-goatcounter-click="download-ryba-1.26.0-linux-appimage" data-goatcounter-title="RYBA 1.26.0 Linux AppImage" data-goatcounter-no-session="1" }
- macOS: [RYBA_1.26.0_macos-universal.app.zip](../assets/projects/RYBA/MacOS/RYBA_1.26.0_macos-universal.app.zip){: data-goatcounter-click="download-ryba-1.26.0-macos-universal" data-goatcounter-title="RYBA 1.26.0 macOS universal ZIP" data-goatcounter-no-session="1" }
