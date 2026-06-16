# mocarram/homebrew-tap

Homebrew tap for [Mocarram Hossain](https://github.com/mocarram)'s macOS apps.

## Usage

```bash
brew tap mocarram/tap
brew install --cask <app>
```

The builds are currently **unsigned** (no Apple Developer account yet). Homebrew
no longer offers `--no-quarantine`, so clear Gatekeeper once after installing
(each cask prints the exact command):

```bash
xattr -dr com.apple.quarantine "/Applications/<App>.app"
```

`brew upgrade` keeps every installed app up to date.

## Apps

| App | Cask | Install |
| --- | --- | --- |
| [Lekha](https://github.com/mocarram/Lekha) - clean, distraction-free Markdown editor | `lekha` | `brew install --cask lekha` |
| [Tora](https://github.com/mocarram/Tora) - privacy-first clipboard manager | `tora` | `brew install --cask tora` |

## Notes

- Each app's `.dmg` is published to that app's own repo releases; this tap only
  holds the cask definitions.
- Unsigned builds are quarantined by macOS on first launch. Clear it with the
  `xattr` command above, or right-click the app and choose Open. Once an app is
  signed + notarized, that step goes away.
