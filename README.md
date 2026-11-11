# F.O.R.G.E

An early Starsector mod metadata scaffold.

**Status:** experimental scaffold, version `0.0.1`. This repository currently
contains example metadata and version-checker configuration. It does not yet
contain the source code, compiled JAR, or build instructions needed to run a mod.

## Repository guide

The original files remain at their existing paths:

| File | Purpose |
| --- | --- |
| [mod_info.json](.github/workflows/mod_info.json) | Draft mod identity, target game version, dependencies, and plugin entry point |
| [Forge.version](.github/workflows/Forge.version) | Draft version-checker and download metadata |
| [version_files.csv](.github/workflows/data/config/version/version_files.csv) | Version-checker file registration |
| [Original readme](.github/workflows/readme.md) | Initial repository placeholder, retained for context |

These files are stored under `.github/workflows/`, but they are mod metadata,
not GitHub Actions workflows. Their paths are retained until the intended mod
layout and any consumers have been confirmed.

## What needs to be completed

The metadata currently targets Starsector `0.98a-RC8` and lists LazyLib and
LunaLib as dependencies. Those declarations have not been validated against a
runnable implementation.

Before preparing an installable release:

- Add the mod source and a reproducible build process.
- Replace the placeholder JAR and plugin values in `mod_info.json`.
- Confirm the author, description, supported game version, and dependencies.
- Complete the version-checker URLs, thread identifier, and release metadata.
- Validate the finished metadata and installation layout against the intended
  Starsector version.

The version file still contains example values and incomplete JSON-style syntax;
it should be treated as a template, not a production update feed.

## Development and history

Use `main` as the current repository entry point. The older `test` branch is
retained as historical context; its existing commits are included in `main`.

Review [the commit history](https://github.com/Victorp1811/F.O.R.G.E/commits/main)
before moving or replacing the scaffold. Submit future layout changes through
a dedicated branch and pull request, including any references that need updating.
