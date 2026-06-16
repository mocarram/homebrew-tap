# mocarram/homebrew-tap

Homebrew tap for [Mocarram Hossain](https://github.com/mocarram)'s macOS apps.

## Usage

```bash
brew tap mocarram/tap
```

Then install any app below. The builds are currently **unsigned** (no Apple
Developer account yet), so pass `--no-quarantine` on first install or macOS
Gatekeeper will block launch:

```bash
brew install --cask --no-quarantine <app>
```

`brew upgrade` keeps every installed app up to date.

## Apps

| App | Cask | Install |
| --- | --- | --- |
| [Lekha](https://github.com/mocarram/Lekha) — clean, distraction-free Markdown editor | `lekha` | `brew install --cask --no-quarantine lekha` |
| [Tora](https://github.com/mocarram/Tora) — privacy-first clipboard manager | `tora` | `brew install --cask --no-quarantine tora` |

> **Tora** is wired up here but its first public release is pending — the cask
> goes live the moment `v0.1.1` is published to
> [mocarram/Tora/releases](https://github.com/mocarram/Tora/releases).

## Notes

- Each app's `.dmg` is published to that app's own repo releases; this tap only
  holds the cask definitions.
- Unsigned builds need `--no-quarantine` (or right-click → Open on first launch).
  Once an app is signed + notarized, that requirement goes away.
