# License and third-party notices

CLXY's original project copyright and MIT permission notice are retained verbatim in [`LICENSE`](LICENSE). The download repository does not replace that license or the terms of bundled components.

[`THIRD-PARTY-LICENSES.txt`](THIRD-PARTY-LICENSES.txt) collects complete legal texts from the release's Go runtime/module notice bundle and the bundled fonts, flags, and globe artwork. Section labels retain component/version identifiers and a SHA-256 of each original notice. The surrounding index is not a substitute for the license text itself.

| Component | Notice |
| --- | --- |
| Original application project | MIT notice in `LICENSE` |
| Go runtime and declared module/tool dependencies | Respective complete copyright, license, patent, and author notices in `THIRD-PARTY-LICENSES.txt` |
| flag-icons country flags | MIT notice, including the original copyright |
| Inter and Vazirmatn fonts | SIL Open Font License 1.1 |
| Natural Earth globe geography | Public-domain data notice and source attribution |
| Flutter/Dart and bundled dependencies | Generated notices bundled with the installed app |

The Go notice bundle conservatively includes declared module and tool dependencies. Its contents do not mean that every listed dependency is linked into the Windows app or that a particular protocol or feature is available.

## Notices inside the Windows package

The v1.0.4 installer is the exact Windows build artifact verified by CI. It includes the project's `LICENSE`, a `licenses` directory for Go component notices, and the Flutter asset notices for dependencies, fonts, flags, and artwork. Flutter's generated dependency notices are supplied in its compressed `NOTICES.Z` asset.

The Windows installation check compared all 37 files in the installed Go notice directory with the release source byte-for-byte. This is a packaging check, not a legal opinion or an endorsement by any dependency author.

Keep the relevant copyright, permission, patent, and attribution notices with any redistributed application copy. CLXY is an independent, unofficial client. The use of upstream software, names, data, or fonts does not imply affiliation with or endorsement by their authors.
