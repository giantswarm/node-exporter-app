# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project's packages adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.20.9] - 2025-11-25

### Changed

- Go: Update dependencies.

## [1.20.8] - 2025-11-01

### Changed

- Go: Update dependencies.

## [1.20.7] - 2025-10-09

### Changed

- Go: Update dependencies.

## [1.20.6] - 2025-10-02

### Changed

- Update Kyverno API to v2 for policy exceptions
- Go: Update dependencies.

## [1.20.5] - 2025-08-26

### Changed

- Go: Update dependencies.

## [1.20.4] - 2025-07-31

### Changed

- Go: Update to v1.24.5.

## [1.20.3] - 2025-06-03

### Changed

- Go: Update dependencies.

## [1.20.2] - 2025-03-18

### Changed

- Go: Update dependencies.

## [1.20.1] - 2025-02-17

### Changed

- Update Kyverno `PolicyExceptions` to `v2beta1`.
- Go: Update `go.mod`. ([#322](https://github.com/giantswarm/node-exporter-app/pull/322))

## [1.20.0] - 2024-08-22

### Changed

- Synced with upstream chart v4.38.0 (node-exporter 1.8.2).

## [1.19.0] - 2024-01-17

### Added

- Add VPA configuration to `node-exporter` app.

## [1.18.2] - 2023-12-20

### Changed

- Configure `gsoci.azurecr.io` as the default container image registry.

## [1.18.1] - 2023-10-23

### Changed

- Make PolicyException namespace configurable.

## [1.18.0] - 2023-10-18

### Changed

- Replace condition for PSP CR installation.

## [1.17.1] - 2023-08-01

### Changed

- fix apparmor annotation

## [1.17.0] - 2023-08-01

### Added

- Add relabelling for servicemonitor.

## [1.16.1] - 2023-06-02

### Changed

- Enable service monitor.

## [1.16.0] - 2023-05-04

### Changed

- Disable PSPs for k8s 1.25 and newer.

## [1.15.1] - 2023-04-24

### Changed

- Update icon.

## [1.15.0] - 2023-01-11

### Fixed

- Fix collector `systemd`
- Fix duplicate scrapping by GiantSwarm Prometheus

### Added

- Add values schema

## [1.14.1] - 2022-12-22

### Fixed

- Trim `-app` from names and labels

## [1.14.0] - 2022-12-22

- Enable `ethtool` collector.

## [1.13.0] - 2022-06-27

### Changed

- Disable boot partition from the `filesystem` exporter.

## [1.12.0] - 2022-05-30

### Changed

- Enabled `diskstats` collector.

## [1.11.0] - 2022-04-07

### Added

- Add options to be able to disable `nvme` and `conntrack` collectors.

## [1.10.0] - 2022-03-02

### Changed

- Disable the fibrechannel collector.
- Disable the tapestats collector.

## [1.9.0] - 2022-01-04

### Updated

- Updated node-exporter version to 1.3.1.

## [1.8.0] - 2021-08-12

### Changed

- Migrate to configuration management.
- Update `architect-orb` to v4.0.0.

## [1.7.2] - 2021-03-26

### Changed

- Set docker.io as the default registry

## [1.7.1] - 2020-12-11

### Changed

- Use the domain registry from installation values if it is present.

## [1.7.0] - 2020-11-26

### Changed

- Change the Kubernetes Daemonset name to include the app version.

## [1.6.0] - 2020-10-26

### Changed

- Disable the diskstats collector on azure.

## [1.5.0] - 2020-10-13

### Changed

- Enable the diskstats collector on azure.

## [1.4.2] - 2020-09-30

### Changed

- Disable `btrfs`,`softnet`,`rapl` and `thermal_zone` to reduce memory usage.
- Increase memory limit to `75Mi`.

## [1.4.1] - 2020-09-24

### Fixed

- Do not use priorityClass in KVM

## [1.4.0] - 2020-09-24

### Changed
- Updated helm chart to use resource helpers, more precise labels.
- Deploy `node-exporter-app` on installations as part of app collection.

## [1.3.0] - 2020-07-23

### Added

- Added workflows for automatic releases.

### Updated

- Updated node-exporter version to 1.0.1.
- Newly disabled collectors: powersupplyclass, schedstat, udp_queues.

## [1.2.0] 2020-01-08

### Changed

- Change Priority Class to `system-node-critical`

## [1.1.1] 2019-12-18

### Changed

- Updated dependencies to support Kubernetes 1.16.

## [1.1.0] 2019-11-20

Note: Version number 1.0.0 was skipped to align the version with other default apps.

### Changed

- Updated to node-exporter version 0.18.1.

## [0.6.0] 2019-10-02

### Changed

- Migrated to be deployed via an app CR not a chartconfig CR.

## [0.5.1] 2019-07-17

### Changed

- Tolerations changed to tolerate all taints.
- Change prioty class from to `giantswarm-critical`.
- Run node-exporter as root user to get proper permissions.
- Remove CPU limits, decrease CPU requests.

## [0.4.1] 2019-06-28

### Fixed

- Fix systemd collector D-Bus connection. https://github.com/giantswarm/kubernetes-node-exporter/pull/44

## [0.4.0] 2019-06-14

### Changed

- Disabled ipvs collector.

### Fixed

- Fix monitored file system mount points.

## [0.3.0] 2019-05-24

### Changed

- Upgrade to node-exporter 0.18.0.

## [0.2.0] 2019-05-17

### Added

- Separate pod security policy for node-exporter and node-exporter-migration workloads.
- Security context with non-root user (`nobody`) for running node-exporter inside container.

[Unreleased]: https://github.com/giantswarm/node-exporter-app/compare/v1.20.9...HEAD
[1.20.9]: https://github.com/giantswarm/node-exporter-app/compare/v1.20.8...v1.20.9
[1.20.8]: https://github.com/giantswarm/node-exporter-app/compare/v1.20.7...v1.20.8
[1.20.7]: https://github.com/giantswarm/node-exporter-app/compare/v1.20.6...v1.20.7
[1.20.6]: https://github.com/giantswarm/node-exporter-app/compare/v1.20.5...v1.20.6
[1.20.5]: https://github.com/giantswarm/node-exporter-app/compare/v1.20.4...v1.20.5
[1.20.4]: https://github.com/giantswarm/node-exporter-app/compare/v1.20.3...v1.20.4
[1.20.3]: https://github.com/giantswarm/node-exporter-app/compare/v1.20.2...v1.20.3
[1.20.2]: https://github.com/giantswarm/node-exporter-app/compare/v1.20.1...v1.20.2
[1.20.1]: https://github.com/giantswarm/node-exporter-app/compare/v1.20.0...v1.20.1
[1.20.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.19.0...v1.20.0
[1.19.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.18.2...v1.19.0
[1.18.2]: https://github.com/giantswarm/node-exporter-app/compare/v1.18.1...v1.18.2
[1.18.1]: https://github.com/giantswarm/node-exporter-app/compare/v1.18.0...v1.18.1
[1.18.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.17.1...v1.18.0
[1.17.1]: https://github.com/giantswarm/node-exporter-app/compare/v1.17.0...v1.17.1
[1.17.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.16.1...v1.17.0
[1.16.1]: https://github.com/giantswarm/node-exporter-app/compare/v1.16.0...v1.16.1
[1.16.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.15.1...v1.16.0
[1.15.1]: https://github.com/giantswarm/node-exporter-app/compare/v1.15.0...v1.15.1
[1.15.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.14.1...v1.15.0
[1.14.1]: https://github.com/giantswarm/node-exporter-app/compare/v1.14.0...v1.14.1
[1.14.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.13.0...v1.14.0
[1.13.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.12.0...v1.13.0
[1.12.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.11.0...v1.12.0
[1.11.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.10.0...v1.11.0
[1.10.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.9.0...v1.10.0
[1.9.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.8.0...v1.9.0
[1.8.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.7.2...v1.8.0
[1.7.2]: https://github.com/giantswarm/node-exporter-app/compare/v1.7.1...v1.7.2
[1.7.1]: https://github.com/giantswarm/node-exporter-app/compare/v1.7.0...v1.7.1
[1.7.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.6.0...v1.7.0
[1.6.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.5.0...v1.6.0
[1.5.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.4.2...v1.5.0
[1.4.2]: https://github.com/giantswarm/node-exporter-app/compare/v1.4.1...v1.4.2
[1.4.1]: https://github.com/giantswarm/node-exporter-app/compare/v1.4.0...v1.4.1
[1.4.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.3.0...v1.4.0
[1.3.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.2.0...v1.3.0
[1.2.0]: https://github.com/giantswarm/node-exporter-app/compare/v1.1.1...v1.2.0
[1.1.1]: https://github.com/giantswarm/node-exporter-app/compare/v1.1.0...v1.1.1
[1.1.0]: https://github.com/giantswarm/node-exporter-app/compare/v0.6.0...v1.1.0
[0.6.0]: https://github.com/giantswarm/node-exporter-app/releases/tag/v0.6.0
[0.5.1]: https://github.com/giantswarm/kubernetes-node-exporter/compare/v0.4.1...v0.5.1
[0.4.1]: https://github.com/giantswarm/kubernetes-node-exporter/compare/v0.4.0...v0.4.1
[0.4.0]: https://github.com/giantswarm/kubernetes-node-exporter/compare/v0.3.0...v0.4.0
[0.3.0]: https://github.com/giantswarm/kubernetes-node-exporter/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/giantswarm/kubernetes-node-exporter/releases/tag/v0.2.0
