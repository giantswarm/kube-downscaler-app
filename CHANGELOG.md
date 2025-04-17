# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.6.2] - 2025-04-17

- Fix home URL in chart metadata

## [0.6.1] - 2025-03-17

### Changed

- Fix ciliumnetpol's endpointSelector.

## [0.6.0] - 2025-03-12

### Changed

- Update chart's image.

## [0.5.0] - 2025-03-06

### Changed

- Updated Helm chart to use the `caas-team/py-kube-downscaler` upstream one as dependency.
- Updated application.giantswarm.io/team label from Team Horizon to Team Planeteers.

## [0.4.0] - 2024-12-09

### Added

- Add cilium network policy template.

## [0.3.0] - 2024-07-17

### Changed

- Push `kube-downscaler` app to all collections.

## [0.2.0] - 2024-07-15

### Changed

- Added `enabled` field in values to disable whole chart if needed.

## [0.1.0] - 2024-04-05

### Added

- First chart version running.

### Changed

- changed: `app.giantswarm.io` label group was changed to `application.giantswarm.io`

[Unreleased]: https://github.com/giantswarm/kube-downscaler-app/compare/v0.6.2...HEAD
[0.6.2]: https://github.com/giantswarm/kube-downscaler-app/compare/v0.6.1...v0.6.2
[0.6.1]: https://github.com/giantswarm/kube-downscaler-app/compare/v0.6.0...v0.6.1
[0.6.0]: https://github.com/giantswarm/kube-downscaler-app/compare/v0.5.0...v0.6.0
[0.5.0]: https://github.com/giantswarm/kube-downscaler-app/compare/v0.4.0...v0.5.0
[0.4.0]: https://github.com/giantswarm/kube-downscaler-app/compare/v0.3.0...v0.4.0
[0.3.0]: https://github.com/giantswarm/kube-downscaler-app/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/giantswarm/kube-downscaler-app/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/giantswarm/kube-downscaler-app/releases/tag/v0.1.0
