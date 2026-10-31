<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,4f8cff,7c5cff&height=210&section=header&text=CLXY&fontSize=95&fontColor=ffffff&animation=fadeIn&fontAlignY=40&desc=Cloner%20Xray%20for%20Windows&descSize=22&descAlignY=66" alt="CLXY" width="100%"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=24&duration=2800&pause=900&color=7C5CFF&center=true&vCenter=true&width=640&lines=Fast.+Private.+Yours.;One+click+to+connect.;Windows+x64+%E2%80%94+ready+to+run." alt="Fast. Private. Yours." />
</p>

<p align="center">
  <a href="https://github.com/ClxybyCloner/clxy-windows-downloads/releases/latest"><img src="https://img.shields.io/github/v/release/ClxybyCloner/clxy-windows-downloads?label=latest&color=7c5cff" alt="Latest release"></a>
  <a href="https://github.com/ClxybyCloner/clxy-windows-downloads/releases"><img src="https://img.shields.io/github/downloads/ClxybyCloner/clxy-windows-downloads/total?label=downloads" alt="Total downloads"></a>
  <img src="https://img.shields.io/badge/Windows-10%2F11-0078D4?logo=windows&logoColor=white" alt="Windows 10/11">
  <img src="https://img.shields.io/badge/arch-x64-4f8cff" alt="x64">
</p>

<p align="center"><b>The Windows download and update channel for the CLXY desktop app.</b><br/>
<sub>Installer, portable ZIP, checksums, and release notes.</sub></p>

<p align="center">
  <a href="https://github.com/ClxybyCloner/clxy-windows-downloads/releases/download/v1.0.7/CLXY-1.0.7-Windows-Setup-x64.exe">⬇️ <b>Download installer: CLXY 1.0.7 (x64)</b></a><br/>
  <a href="https://github.com/ClxybyCloner/clxy-windows-downloads/releases/download/v1.0.7/CLXY-1.0.7-Windows-x64.zip">📦 Portable ZIP (no install)</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/ClxybyCloner/clxy-windows-downloads/releases/tag/v1.0.7">Release details</a>
  &nbsp;·&nbsp;
  <a href="#-verify-your-download">Verify your download</a>
</p>

> ⚠️ **Unsigned installer:** this build carries no publisher signature, so Windows may show an
> unknown-publisher / SmartScreen warning. Windows CI verified installation, app launch, and local
> core startup. Real account sign-in and live VPN/proxy traffic were **not** tested.

<p align="center">
  <img src="windows-preview.png" alt="CLXY running on Windows, showing its dark first-run sign-in screen" width="820">
</p>
<p align="center"><sub>CLXY on Windows during a launch check. The screenshot shows the sign-in screen. It does not demonstrate a working VPN connection.</sub></p>

---

## 📥 Download

| | |
|---|---|
| Release | **1.0.7** (app version `1.0.7+121`) |
| Platform | Windows 10 / 11, **x64** |
| 🖥️ Installer | [`CLXY-1.0.7-Windows-Setup-x64.exe`](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/download/v1.0.7/CLXY-1.0.7-Windows-Setup-x64.exe) · 20,147,441 bytes |
| 📦 Portable | [`CLXY-1.0.7-Windows-x64.zip`](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/download/v1.0.7/CLXY-1.0.7-Windows-x64.zip) · 24,153,118 bytes |
| Code signing | Unsigned, no Authenticode certificate |
| Checksums | [`SHA256SUMS.txt`](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/download/v1.0.7/SHA256SUMS.txt) · [checksum history](CHECKSUMS.txt) |

> 🗂️ This repository provides binary downloads and documentation. Installers live as
> [Release assets](https://github.com/ClxybyCloner/clxy-windows-downloads/releases), not in git history.
> GitHub's **Code → Download ZIP** and the auto-generated *Source code* archives contain only this
> repo's docs. Download the `.exe` or portable `.zip` above. Do not use a source archive.

---

## ⚡ Install on Windows

1. **Download** the [installer](#-download) above.
2. **Verify its SHA-256** ([how-to below](#-verify-your-download)) before running it.
3. **Open it** and follow the prompts (per-user install). If SmartScreen appears, see [the security notes](#-windows-security-warnings) first.
4. **Launch CLXY** from the installer or the Start menu.
5. Read [what CLXY is](#-what-clxy-is) before signing in or connecting.

The app installs to `%LOCALAPPDATA%\Programs\CLXY` and keeps its private account data,
settings, and logs in a `user-data` folder beside it. Treat that folder as private.

### 📦 Portable copy

Prefer no installer? Download the [portable ZIP](#-download), verify its hash, extract the
`CLXY` folder, and run `clxy.exe`. Keep the folder writable. The app stores its private
`user-data` right beside the executable.

---

## ✅ Verify your download

In PowerShell, from your download folder:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath .\CLXY-1.0.7-Windows-Setup-x64.exe
```

The result must match the hash published in the
[release notes](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/tag/v1.0.7)
and in [`CHECKSUMS.txt`](CHECKSUMS.txt):

```text
5e07a95534ac0d81af882833496397363129eb42397a14c2522c38f20932b4d9  CLXY-1.0.7-Windows-Setup-x64.exe
c6d8053b9a2a7f63e1bd7adfc120f3119b7534ace75842ab86fb093ba215cedf  CLXY-1.0.7-Windows-x64.zip
```

A matching hash proves the file is exactly what we published. It is *not* a security audit
or a publisher signature.

---

## 🛡️ Windows security warnings

- The installer is **unsigned**. A successful install test does not establish SmartScreen reputation or publisher identity.
- Only proceed if you trust this repository **and** the checksum matches.
- **Never** disable Defender, antivirus, or your organization's security policy to install it. If you're unsure about a warning, stop.

---

## 🔄 How updates work

CLXY checks this repository's latest stable release **after each successful VPN connection**
(including reconnects). When a newer build is found, the app shows a notice with a
**Download** button. Installed copies fetch the installer. Portable copies fetch the ZIP.
Downloading and installing always stay *your* choice: **CLXY never auto-installs updates.**

---

## 🧭 What CLXY is

CLXY is an independent, unofficial Windows desktop client. It uses a Flutter interface with a
bundled Go core that starts locally and talks to the app over loopback. The package includes
the sign-in/onboarding UI, desktop integration, and the required legal notices
([`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md), [`LICENSE`](LICENSE)).

CLXY is an independent third-party client; account and upstream-service access are external
dependencies. Publishing this installer does **not** provide an account or guarantee service
access. The upstream proxy is TCP-only on web ports **80, 443, 8080, and 8443**. UDP-dependent
apps and other ports may not work. Don't assume every app's traffic is protected just because
the desktop app is open.

---

## ❓ FAQ

**Is the source code here?**
This repository contains only binary downloads and documentation. The app source is not published.

**Installer or portable?**
Installer for a normal setup (Start-menu entry, per-user install). Portable if you want a
folder you can carry around or run without installing.

**Where are my settings?**
In the `user-data` folder next to the app (installed or portable). Back it up if it matters to you.

**Windows 7 / 8 / ARM?**
Not supported. The target is **Windows 10/11 on x64**. This release has no ARM64 or 32-bit package.

**The dashboard looks cramped in a small window.**
It keeps the desktop layout when resized. Press <kbd>Ctrl</kbd>+<kbd>+</kbd> /
<kbd>Ctrl</kbd>+<kbd>−</kbd> to zoom.

**Older versions?**
They stay on the [Releases page](https://github.com/ClxybyCloner/clxy-windows-downloads/releases),
with their checksums in [`CHECKSUMS.txt`](CHECKSUMS.txt).

---

## 📜 Release history

Full notes for every build live in [`CHANGELOG.md`](CHANGELOG.md), newest first.

## 💬 Support

- 🌐 [clonerr.ir](https://clonerr.ir)
- ✈️ Telegram: [@cloner42](https://t.me/cloner42)

## 📄 Terms

© CLXY. All rights reserved. The builds published here are free to download and use.
Please don't re-upload them elsewhere. Link people here so they can get
the genuine, verified build. Third-party components are listed in
[`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md).

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,7c5cff,4f8cff&height=130&section=footer&animation=fadeIn" alt="" width="100%"/>
</p>
<p align="center"><sub>Made with 💙 for the CLXY community</sub></p>
