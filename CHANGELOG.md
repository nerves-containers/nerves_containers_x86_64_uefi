# Changelog

This project does NOT follow semantic versioning. The version increases as
follows:

1. Major version updates are breaking updates to the build infrastructure.
   These should be very rare.
2. Minor version updates are made for every major Buildroot release. This
   may also include Erlang/OTP and Linux kernel updates. These are made four
   times a year shortly after the Buildroot releases.
3. Patch version updates are made for Buildroot minor releases, Erlang/OTP
   releases, and Linux kernel updates. They're also made to fix bugs and add
   features to the build infrastructure.

## v1.31.3

This is an important security/bug fix that addresses Erlang CVEs for the ssh
module (see Erlang release notes).

* Package updates
  * [nerves_system_br v1.31.7](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.31.7). Also
    see [nerves_system_br v1.31.6](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.31.6)

* Important derived package updates
  * [Erlang/OTP 27.3.4.3](https://erlang.org/download/OTP-27.3.4.3.README.md)
  * [Buildroot 2025.02.6](https://lore.kernel.org/buildroot/b051d400-debc-4269-975a-b2992eed8d61@rnout.be/T/)

## v1.28.1

* Updated dependencies
  * [nerves_system_br: bump to v1.28.3](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.28.3)

## v1.12.2

This release updates to [Buildroot
2020.05.1](http://lists.busybox.net/pipermail/buildroot/2020-July/287824.html)
and OTP 23.0.3 which are both bug fix releases.

* Updated dependencies
  * [nerves_system_br: bump to v1.12.4](https://github.com/nerves-project/nerves_system_br/releases/tag/v1.12.4)
  * [Erlang/OTP 23.0.3](https://erlang.org/download/OTP-23.0.3.README)
  * [nerves_heart v0.3.0](https://github.com/nerves-project/nerves_heart/releases/tag/v0.3.0)

* New features
  * The `/data` directory now exists for storing application-specific data. It
    is currently a symlink to `/root`. Using `/data` will eventually be
    encouraged over `/root` even though currently there is no advantage. This
    change makes it possible to start migrating paths in applications and
    libraries.

* Fixes
  * Fixed old references to the `-Os` compiler flag. All C/C++ code will default
    to using `-O2` now.

## v1.11.0

* nerves_system_br v1.11.0
* linux: bump to 4.14.173 and include new patches
* bump to gcc 9.2
* nerves: support v1.6.0
* update deps

## v1.10.0

Initial release

This release corresponds to other Nerves releases with the same version number.
