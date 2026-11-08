# 4diac-ide-release-history-rc

Archive of [Eclipse 4diac](https://eclipse.dev/4diac/) IDE downloads – channel **`rc`**.

4diac IDE release candidates.

Every build is published as its own GitHub Release with all platform packages attached
under their **original file names**, plus a `SHA256SUMS.txt`. Releases are created by
the 4diac download job; existing releases are never deleted or overwritten.

## Channels

| Channel | Repository |
|---------|------------|
| latest    | [4diac-ide-release-history-latest](https://github.com/Meisterschulen-am-Ostbahnhof-Munchen/4diac-ide-release-history-latest) |
| rc        | [4diac-ide-release-history-rc](https://github.com/Meisterschulen-am-Ostbahnhof-Munchen/4diac-ide-release-history-rc) |
| milestone | [4diac-ide-release-history-milestone](https://github.com/Meisterschulen-am-Ostbahnhof-Munchen/4diac-ide-release-history-milestone) |
| nightly   | [4diac-ide-release-history-nightly](https://github.com/Meisterschulen-am-Ostbahnhof-Munchen/4diac-ide-release-history-nightly) |

## Naming

- **Tag:** the file name without platform and extension, e.g. `4diac-ide_<version>_rc_<YYYY-MM-DD>_<HHMM>`
- **Assets:** unchanged original file names, one per platform
  (`win32.win32.x86_64` .zip, `linux.gtk.x86_64` .tar.gz,
  `macosx.cocoa.aarch64` / `macosx.cocoa.x86_64` .dmg and .tar.gz)
- **Pre-release flag:** yes – every release is marked as pre-release

## Download

Stable download URL:

```
https://github.com/Meisterschulen-am-Ostbahnhof-Munchen/4diac-ide-release-history-rc/releases/download/<tag>/<file name>
```

Verify the download against `SHA256SUMS.txt` from the same release:

```powershell
(Get-FileHash .\<file name> -Algorithm SHA256).Hash   # Windows
```

```sh
sha256sum -c SHA256SUMS.txt --ignore-missing          # Linux / macOS: shasum -a 256 -c
```

## License

Eclipse 4diac is licensed under the [Eclipse Public License 2.0](LICENSE).
The packages are redistributed unmodified; the license files are included in each package.
This repository is an unofficial mirror and not affiliated with the Eclipse Foundation.
