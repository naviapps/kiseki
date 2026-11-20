# Kiseki

Kiseki is a macOS gesture app for running app and system actions with a mouse or trackpad.
Hold a secondary click, draw, and release to run shortcuts or arrange windows from
wherever your pointer is.

This public repository hosts Kiseki releases and support. The app source is
maintained separately and is not required to install Kiseki.

## Download

Download Kiseki for macOS 26 and later from:

[Download Kiseki](https://kisekiapp.com)

Versioned downloads are also available on the
[Kiseki releases page](https://github.com/naviapps/kiseki/releases).

### Verify a direct download

Download `Kiseki.dmg` and `SHA256SUMS` from the same release. Save both files in
the same folder. Run this command from that folder in Terminal.

```sh
grep -E '^[[:xdigit:]]{64}  Kiseki\.dmg$' SHA256SUMS | shasum -a 256 -c
```

The expected result is `Kiseki.dmg: OK`. If the check fails, download both files
again from the same release. macOS checks the app's signature and notarization
when you open the downloaded app.

## Homebrew

Install from the official [Navi Apps Tap](https://github.com/naviapps/homebrew-tap):

```sh
brew install --cask naviapps/tap/kiseki
```

The Tap uses the same signed and notarized DMG as the direct download, with support
for Apple silicon and Intel Macs. Open Kiseki from Applications and follow its
Accessibility guide. See the Tap README for updates, uninstalling, and switching
from a manual installation.

## Guides

- [Getting started](https://kisekiapp.com/getting-started): permissions, your first gesture, and troubleshooting.
- [Official presets](https://kisekiapp.com/presets): ready-made app settings and import instructions.
- [Plans and activation](https://kisekiapp.com/billing): Free and Pro, license activation, and purchase help.
- [Release notes](https://github.com/naviapps/kiseki/releases): published versions and downloads.

## Support

Use [GitHub Issues](https://github.com/naviapps/kiseki/issues) for public bug reports,
feature requests, and support questions. Include the app version, macOS version,
reproduction steps, and expected and observed behavior. Email [Kiseki support](mailto:support@kisekiapp.com)
for billing, activation, refunds, or private account details. Follow the
[security policy](SECURITY.md) to report vulnerabilities privately. Keep license
keys, tokens, payment details, and personal data out of public reports.

## Checking this repository

To validate changes to the public documentation or workflows, install [mise](https://mise.jdx.dev/).
Review `mise.toml` in your clone, then run:

```sh
mise trust mise.toml
mise install
mise run check
```

`mise.toml` supplies the tool versions for both local checks and GitHub Actions.
Run `mise run format` to apply the repository's text formatting.
