# modly.desktop

Public release artifacts for [Modly Desktop](https://modly.one).

This repository hosts signed release binaries and the Tauri updater manifest
consumed by installed Modly Desktop clients. **Source code lives in a private
repository** (`codeparticle/modly.web`, under `apps/desktop`). This repo only
receives:

- GitHub Releases tagged `desktop-v*.*.*` containing:
  - macOS `.dmg` (Apple Silicon + Intel) + `.app.tar.gz` + `.sig`
  - Linux `.AppImage` + `.sig`
- `latest.json` — Tauri updater manifest pointing at the current release.
- `CHANGELOG.md` — auto-generated from Conventional Commits.

## Verifying a release

Every artifact is signed with an Ed25519 key held in AWS KMS. The public key is
embedded in the app binary itself (`plugins.updater.pubkey` in Tauri config);
the updater verifies each download before applying it, so there is nothing a
user needs to check manually.

If you want to verify by hand, the pubkey is reproducible from
[`apps/desktop/src-tauri/tauri.conf.json`](https://github.com/codeparticle/modly.web/blob/main/apps/desktop/src-tauri/tauri.conf.json)
in the source repo.

## Auto-updates

Installed clients check `https://releases.modly.one/` (a thin proxy for this
repo's latest release) on launch. The release manifest is cached; downloads
are fetched from this repo's GitHub Release assets directly.

## Reporting issues

Please file bugs at <https://github.com/codeparticle/modly.web/issues> — this
repo does not accept issues or pull requests.
