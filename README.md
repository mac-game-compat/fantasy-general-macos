# Fantasy General macOS

A compatibility and playability project for running a legally owned copy of
Fantasy General on modern macOS. Intended future home:
https://github.com/mac-game-compat/fantasy-general-macos

This repository documents reproducible setup, compatibility observations, and
troubleshooting. It is not a game rebalance, replacement engine, or general-purpose
modding framework. No macOS or emulator combination has been validated yet.

## Getting started

Read [installation](docs/installation.md), the
[compatibility record](docs/compatibility.md), and
[troubleshooting](docs/troubleshooting.md). The
[DOSBox example](config/dosbox.conf.example) is a starting point, not a verified
game profile.

## Asset boundaries

Supply your own legally owned game and appropriately licensed emulator separately.
Do not commit game executables, data, artwork, music, manuals, disc images,
installers, commercial DOSBox bundles, saves, credentials, or experimental dumps.
The project does not grant rights to any third-party material or bypass access
controls. The MIT license covers only project-authored material.

`local/` is entirely ignored and holds private working material:

- `local/game/`: a working copy of legally owned game files, only after explicit approval.
- `local/dosbox/`: private emulator configuration and separately supplied runtime files.
- `local/saves/`: private save backups.
- `local/scratch/`: logs and experiments.

Existing game installations must not be inspected, moved, or modified without
explicit approval. Keep backups outside this repository as well: Git does not
protect ignored files. Ignore rules are a guardrail, not an asset scanner; inspect
all staged paths and diffs before committing, and never force-add private files.

## Possible future work

Optional tools could validate configuration, collect sanitized compatibility
reports, or back up saves without interpreting or modifying their contents.
No tools are implemented yet. Any future tool should be opt-in, narrowly scoped,
and preserve original files. Save editors and game modifications are outside the
initial scope.

## Contributing

Keep changes small and evidence-based. Record macOS, CPU architecture, game
edition, emulator version, reproduction steps, and observed results. Share only
original documentation/configuration and sanitized diagnostics, never assets or
personal paths. Review `git diff --cached` and the complete staged-file list
before committing.
