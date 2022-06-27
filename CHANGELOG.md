# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) as described in [The Cargo Book](https://doc.rust-lang.org/cargo/reference/manifest.html#the-version-field).

## [Unreleased]

### Fixed

- Add `toolchain: stable` in draft release

## [2.0.0] - 2022-06-27

### Added

- New input `build` for `draft-new-release.yml` to build the crate before add & commit the files, allows lockfile update
- New input `check_publish` for `draft-new-release.yml` to dry run the cargo publish before add & commit the files, allows to not open a PR on unpublishable state.

### Changed

- Update DPrint plugins
- Bump EndBug/add-and-commit from 7.4.0 to 9.0.0

## [1.1.0] - 2021-11-02

### Added

- Possibility to attach artifacts to releases with `artifact_name` and `files` inputs in create release workflow

### Changed

- Commit and release is done by the GitHub Actions bot identity

### Removed

- `name`, `email`, `with_lock` in draft new release workflow
- Identity secrets in draft new release and create new release workflows

## [1.0.0] - 2021-10-13

### Added

- `Crate release` shared workflow
- `Draft new release` shared workflow
- `Release to crates.io` shared workflow

[Unreleased]: https://github.com/monero-rs/workflows/compare/v2.0.0...HEAD
[2.0.0]: https://github.com/monero-rs/workflows/compare/v1.1.0...v2.0.0
[1.1.0]: https://github.com/monero-rs/workflows/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/monero-rs/workflows/compare/38f5205bf6af87a41fdbc6c80e101e13876fb915...v1.0.0
