# Release history

## 1.0.4 (app version 1.0.4+118)

The dashboard was tested in an 805×560 logical viewport for Surface Go 2. Press Ctrl+plus or Ctrl-minus to change zoom. While disconnected, the center shows Connect. After a successful connection, it shows the globe and route.

- Location, Total Traffic, and Data used show the app's existing values.
- The local Logs view replaces the known upstream product name with “upstream service” in displayed messages. Raw logs and service behavior are unchanged.
- The installer includes the Inter font and its SIL Open Font License notice.
- Flutter analysis and 123 Flutter tests passed. The two web sanitizer tests and Go checks passed. The Windows x64 build, install, launch, local core readiness, legal-asset, and uninstall checks passed.

The installer is unsigned. Real account sign-in and live VPN/proxy traffic were not tested.

SHA-256:

```text
18837e6823424580f685762a6b88d7db50a64267eab7bea0d655d99896d72b12
```

## 1.0.3 (app version 1.0.3+117)

First public Windows x64 binary publication in this download repository.

- Windows installer: `CLXY-1.0.3-Windows-Setup-x64.exe`.
- Includes the desktop app, bundled local core, and required legal notices.
- The published installer is the unchanged verified release candidate.
- Flutter analysis and 122 automated tests passed.
- A real Windows installation check confirmed app/core startup, a visible app window, a responding local core endpoint, and successful uninstall.
- The installer is unsigned and may trigger Windows SmartScreen or unknown-publisher warnings.
- Real account sign-in, live VPN/proxy traffic, tunnel establishment, external routing, and external DNS behavior were not validated.

SHA-256:

```text
6c0a39b365101fd4d38ef5614cff464aadb0fb201366a9a11edf0e68ee2e3ef9
```

See the [installation and verification guide](README.md) and [third-party notices](THIRD-PARTY-NOTICES.md) before using or redistributing the package.
