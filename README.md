# YordiLorenzo/homebrew-tap

Homebrew formulae for [hbkit](https://github.com/YordiLorenzo/hbkit).

## Install

```sh
brew install YordiLorenzo/tap/hbkit
```

That gives you two commands:

```sh
hbk /Volumes/Backup doctor      # can this archive be recovered?
hbk-tui                         # full-screen browser
```

## Formulae

| Formula | Description |
| ------- | ----------- |
| `hbkit` | Recover files from Synology Hyper Backup (`.hbk`) archives without Synology software |

## Notes

`cryptography` comes from its own Homebrew formula rather than being built here, so
installing does not need a Rust toolchain. PyNaCl links against the `libsodium` formula
instead of compiling the copy vendored in its sdist.

To mount an archive kept in S3 or Cloudflare R2, also install rclone:

```sh
brew install rclone
```

## License

Formulae in this tap are MIT-licensed, as is hbkit itself.
