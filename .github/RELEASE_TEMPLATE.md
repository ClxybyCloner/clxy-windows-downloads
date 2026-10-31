# CLXY Windows [VERSION]

[One sentence summarizing this release.]

**Build [BUILD]** · app version `[VERSION]+[BUILD]`

## ✨ What's new

- [Change 1]
- [Change 2]
- [Change 3]

## ✅ Release checks

- [ ] Flutter analysis and Flutter tests passed ([N] tests)
- [ ] Go checks passed
- [ ] Windows CI: built both x64 packages, installed the app, started the real local core, confirmed the local endpoint, uninstalled cleanly
- [ ] All 37 third-party notice files matched the source copies byte-for-byte

> [State whether the installer is signed. List important checks that were not performed, such as real account sign-in or live VPN/proxy traffic.]

## 📥 Windows downloads

- [Windows x64 installer](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/download/v[VERSION]/CLXY-[VERSION]-Windows-Setup-x64.exe)
- [Portable Windows ZIP](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/download/v[VERSION]/CLXY-[VERSION]-Windows-x64.zip)
- [SHA256SUMS.txt](https://github.com/ClxybyCloner/clxy-windows-downloads/releases/download/v[VERSION]/SHA256SUMS.txt)

SHA-256:

```text
[SHA]  CLXY-[VERSION]-Windows-Setup-x64.exe
[SHA]  CLXY-[VERSION]-Windows-x64.zip
```

---

### Publishing checklist (delete this section before publishing)

1. Tag: `v[VERSION]`, release title: `CLXY Windows [VERSION]`
2. Attach **three** files: the installer `.exe`, the portable `.zip`, and `SHA256SUMS.txt`
3. Fill in `[VERSION]`, `[BUILD]`, `[SHA]` values, and the download links above
4. Append the new hashes to the repo's `CHECKSUMS.txt` (keep the history)
5. After publishing, update the README: version line, both download links, sizes, the verify-hash example, and the specs table
