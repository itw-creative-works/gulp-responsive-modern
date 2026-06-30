# CHANGELOG

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## Changelog Categories

- `BREAKING` for breaking changes.
- `Added` for new features.
- `Changed` for changes in existing functionality.
- `Deprecated` for soon-to-be removed features.
- `Removed` for now removed features.
- `Fixed` for any bug fixes.
- `Security` in case of vulnerabilities.

---
## [1.0.1] - 2025-06-30
### Fixed
- `format.js`: Case-insensitive extension matching — `.JPG`, `.PNG`, etc. now resolve correctly instead of returning `unsupported`
- `sharp.js`: Prefer `file.contents` buffer over `file.path` when available, fixing failures on case-sensitive filesystems where upstream transforms rename the Vinyl path

## [0.0.1] - 2025-02-01
### Changed
- `package.json`
  - Changed `sharp` to `0.33.5`
- `sharp.js`
  - Changedv `const image = sharp(file.contents)` to `const image = sharp(file.path)`
