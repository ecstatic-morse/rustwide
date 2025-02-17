# Changelog

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Unreleased

### Added

- New method `Toolchain::uninstall` to remove a previously installed toolchain.
- New method `Workspace::installed_toolchains` to get a list of all the
  toolchains in the workspace.

### Changed

- **BREAKING:** The `cmd::Binary` enum is not exaustive anymore.
- **BREAKING:** The `cmd::MountKind` enum is not exaustive anymore.
- **BREAKING:** The `cmd::Toolchain` enum is not exaustive anymore.
- The base path of mounts inside the sandbox is now `/opt/rustwide` on Linux
  and `C:\rustwide` on Windows.

### Fixed

- Issue with cloning repos on Windows caused by the credential manager.

## [0.1.0] - 2019-08-22

### Added

- Initial version of Rustwide, extracted from Crater.

[0.1.0]: https://github.com/rust-lang/rustwide/releases/tag/0.1.0
