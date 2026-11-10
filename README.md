# Kiseki

Kiseki is a macOS gesture app for running app and system actions with a mouse or trackpad.
Hold a secondary click, draw, and release to run shortcuts or arrange windows from
wherever your pointer is.

This public repository hosts Kiseki releases and support. The app source is
maintained separately and is not required to install Kiseki.

## Download

Download Kiseki for macOS 26 and later from:

https://kisekiapp.com

## Homebrew

Install from the official [Navi Apps Tap](https://github.com/naviapps/homebrew-tap):

```sh
brew install --cask naviapps/tap/kiseki
```

Kiseki supports macOS 26 and later on Apple silicon and Intel Macs. The Tap uses
the same signed and notarized DMG as the direct download. Open Kiseki from
Applications and follow its Accessibility guide. See the Tap README for updates,
uninstalling, and switching from a manual installation.

## Support

Use [GitHub Issues](https://github.com/naviapps/kiseki/issues) for public bug reports,
feature requests, and support questions. Email [Kiseki support](mailto:support@kisekiapp.com)
for billing, activation, refunds, or private account details. Follow the
[security policy](SECURITY.md) to report vulnerabilities privately.

## Checking this repository

To validate changes to the public documentation or workflows, install [mise](https://mise.jdx.dev/).
Review `mise.toml` in your clone, then run:

```sh
mise trust
mise install
mise run check
```

`mise.toml` supplies the tool versions for both local checks and GitHub Actions.
Run `mise run format` to apply the repository's text formatting.
