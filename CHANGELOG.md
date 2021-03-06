# Change log

This document represents a high-level overview of changes made to this project.
It will not list every miniscule change, but will allow you to view - at a
glance - what to expact from upgrading to a new version.

## [unpublished]

### Added

### Changed

### Fixed

### Security

### Deprecated

### Removed


## [0.4.5] - 2018-09-09

### Fixed

- Handle ID 64s exceeding allowed range, by adding/subtracting multiples of
  range until fitting.


## [0.4.4] - 2018-03-25

### Fixed

- Handle vanity URLs which can't be part of a valid URI by throwing an
  exception instead of failing when creating an URL.


## [0.4.3] - 2017-11-30

### Fixed

- Handle non-ASCII vanity URLs by throwing an exception instead of failing when
  creating an URL.


## [0.4.2] - 2017-11-25

### Fixed

- Fix `SteamID::Parser#from_string` throwing an exception when resolving a
  vanity URL.


## [0.4.1] - 2017-11-19

### Fixed

- Missing functionality of `SteamID.from_string`.


## [0.4.0] - 2017-11-18

### Added

- `SteamID::SteamID` class representing a single Steam ID.
- `Parser` class allowing to parse various formats of Steam IDs into their
  respective account ID.
- `SteamID#from_string` convenience method.


## [0.3.0] - 2017-05-30

### Added

- Support for community URLs containing Steam ID3.


## [0.2.0] - 2017-03-07

### Added

- Support for brackets in SteamID 3 format, e.g. `[U:1:123456]`


## [0.1.2] - 2017-01-15

### Added

### Changed

### Fixed

- Fixed handling of account IDs starting with 765.


## [0.1.1] - 2017-01-02

### Fixed

- Implements missing SteamID::SteamID.from_string method.


## [0.1.0] - 2017-01-02

### Added

- Module to allow conversion of SteamIDs into account IDs suitable for e.g.
  Hive 2 API calls.

  Supported are:
  - Steam ID
  - Steam ID 3
  - Steam ID 64
  - Community URL
  - Profile URL
