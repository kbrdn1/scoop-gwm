# scoop-gwm

[Scoop](https://scoop.sh) bucket for [**gwm**](https://github.com/kbrdn1/gwm-cli) — a git worktree manager (TUI + CLI, native libgit2, per-repo bootstrap) for Windows.

## install

```powershell
scoop bucket add gwm https://github.com/kbrdn1/scoop-gwm
scoop install gwm
```

Then run `gwm` from any repo.

## update

```powershell
scoop update gwm
```

## how this bucket stays current

`bucket/gwm.json` is regenerated automatically on every **stable** release of
`gwm-cli` by the `scoop-bucket-update` job in
[`release.yml`](https://github.com/kbrdn1/gwm-cli/blob/main/.github/workflows/release.yml),
from the canonical template
[`packaging/scoop/gwm.json.template`](https://github.com/kbrdn1/gwm-cli/blob/main/packaging/scoop/gwm.json.template).
Pre-release tags (`-rc.N`, `-alpha.N`, `-beta.N`) are filtered out, so
`scoop install gwm` always tracks the latest stable. Don't edit `bucket/gwm.json`
by hand — changes belong in the template upstream.

## links

- Source & issues: <https://github.com/kbrdn1/gwm-cli>
- Install matrix (crates.io, Homebrew, Nix, prebuilt): <https://github.com/kbrdn1/gwm-cli#install>

MIT © Kylian Bardini
