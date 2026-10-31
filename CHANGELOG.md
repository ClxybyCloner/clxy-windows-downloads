# CLXY for Windows release history

All notable changes, newest first. Each version has a GitHub Release with its available Windows downloads and SHA-256 checksums.

| Version | App version | Date | Release notes |
|---|---|---|---|
| **1.0.7** | `1.0.7+121` | 2026-10-30 | [v1.0.7](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/tag/v1.0.7) |
| 1.0.6 | `1.0.6+120` | 2026-10-28 | [v1.0.6](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/tag/v1.0.6) |
| 1.0.5 | `1.0.5+119` | 2026-10-28 | [v1.0.5](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/tag/v1.0.5) |
| 1.0.4 | `1.0.4+118` | 2026-10-27 | [v1.0.4](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/tag/v1.0.4) |
| 1.0.3 | `1.0.3+117` | 2026-10-27 | [v1.0.3](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/tag/v1.0.3) |

---

## 1.0.7 (2026-10-30)

- The update notice now has a direct **Download** button. Installed copies download the installer; portable copies download the ZIP.
- CLXY checks for a newer release each time a VPN connection is confirmed, including after reconnecting. It does **not** install updates automatically.
- Flutter analysis and 150 Flutter tests passed; web log-sanitizer, Go, and Windows package checks passed. The installed app started its real core, reached its loopback endpoint, opened all four tabs, and uninstalled cleanly.
- All 37 installed third-party notice files matched the source copies byte-for-byte.

> The installer is unsigned. Update-feed tests used a fake response. Real account sign-in and live VPN/proxy traffic were not tested.

```text
5e07a95534ac0d81af882833496397363129eb42397a14c2522c38f20932b4d9  CLXY-1.0.7-Windows-Setup-x64.exe
c6d8053b9a2a7f63e1bd7adfc120f3119b7534ace75842ab86fb093ba215cedf  CLXY-1.0.7-Windows-x64.zip
```

## 1.0.6 (2026-10-28)

- Resizing the window keeps the desktop dashboard instead of switching to phone navigation. Compact layout tested at 930×860 and 805×560; <kbd>Ctrl</kbd>+<kbd>+</kbd> / <kbd>Ctrl</kbd>+<kbd>−</kbd> adjust zoom.
- Proxy and System Proxy, quota, the connection control, Download/Upload, Location, and Total Traffic stay on the desktop dashboard.
- All 133 Flutter tests passed, including updater checks. Windows package and legal-asset checks passed. Real install test confirmed a visible app window, a ready local core, and clean uninstallation. All 37 third-party notice files matched byte-for-byte.

> The installer is unsigned. Real account sign-in and live VPN/proxy traffic were not tested.

```text
5251a68c812924cda9f9e0613145aeb797e0b49ebd51f7555f33267990f9b790  CLXY-1.0.6-Windows-Setup-x64.exe
f3e4a3bb31e356fcbfc493a00caa50f59727d04ff5d5aefee0fa13cc1dedf290  CLXY-1.0.6-Windows-x64.zip
```

## 1.0.5 (2026-10-28)

- Proxy and System Proxy share one control. Usage and quota moved to the top; Location and Total Traffic sit below.
- Larger, centered connection circle with more breathing room; cards with faded, borderless edges.
- CLXY now checks this repository's latest stable release and shows a dismissible update notice. Downloading and installing stay the user's choice.
- First release with both the installer and the portable ZIP.
- Flutter analysis and 132 Flutter tests passed; web sanitizer and Go checks passed; Windows install, visible app window, real core readiness, legal payload checks, and uninstallation all passed.

> The installer is unsigned. Real account sign-in and live VPN/proxy traffic were not tested.

```text
66b34089208d1174abcebd0d75114884b751f99f0fe9a40f91fd11befbacee9b  CLXY-1.0.5-Windows-Setup-x64.exe
7c038177002da703458ffc9a921e40310d39ee4a4b3bb1ac2f7413870f9df51d  CLXY-1.0.5-Windows-x64.zip
```

## 1.0.4 (2026-10-27)

- Compact desktop dashboard tested at an 805×560 viewport (Surface Go 2 friendly); <kbd>Ctrl</kbd>+<kbd>+</kbd> / <kbd>Ctrl</kbd>+<kbd>−</kbd> adjust zoom. Disconnected → Connect button in the center; connected → globe and route.
- Logs view uses neutral wording ("upstream service"); raw logs and service behavior unchanged. Bundled Inter font with its SIL Open Font License notice.
- Validation passed: Flutter analysis, 123 Flutter tests, two web sanitizer tests, Go vet/tests, Windows x64 build/packaging checks, and the install → launch → local core → uninstall test. Legal assets and all 37 Go notice files matched byte-for-byte.

> The installer is unsigned. Real account sign-in and live VPN/proxy traffic were not tested.

```text
18837e6823424580f685762a6b88d7db50a64267eab7bea0d655d99896d72b12  CLXY-1.0.4-Windows-Setup-x64.exe
```

## 1.0.3 (2026-10-27)

- First verified Windows x64 installer release (18,040,769 bytes).
- Flutter static analysis and 122 automated tests passed. Real Windows install check confirmed the app window, bundled core startup, and a responding local HTTP endpoint; uninstall removed app, core, and shortcuts. All 37 Go notice files matched byte-for-byte.
- Sign-in/onboarding UI tests used fake APIs and synthetic data.

> **Unsigned installer:** Windows may show an unknown-publisher or SmartScreen warning.
> **Not validated:** real provider sign-in, token validity, live VPN/proxy traffic, tunnel establishment, external routing, or external DNS behavior.

```text
6c0a39b365101fd4d38ef5614cff464aadb0fb201366a9a11edf0e68ee2e3ef9  CLXY-1.0.3-Windows-Setup-x64.exe
```
