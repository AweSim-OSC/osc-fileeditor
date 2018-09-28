# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Changed
- Entire app converted from Rails to Sinatra.
  [#77](https://github.com/OSC/ood-fileeditor/issues/77)
- Updated to Ace Editor 1.3.3.
- Modified error pages.
- Improved navbar for different screen widths.

### Added
- Ability to change tab spacing.
  [#79](https://github.com/OSC/ood-fileeditor/issues/79)

### Fixed
- Issuing :w in Vim mode doesn't save the file
  [#78](https://github.com/OSC/ood-fileeditor/issues/78)
  Though not officially supported by Ace, this implementation works
- Low-hanging letters get cut off in toolbar
  [#75](https://github.com/OSC/ood-fileeditor/issues/75)
- Long file path names hide the toolbar controls
  [#44](https://github.com/OSC/ood-fileeditor/issues/44)
  Smaller screens will see a blue info button to toggle the file path
  Very long paths on even large screens will instead expand the toolbar, no longer hiding the controls

## [1.3.3] - 2018-01-03
### Changed
- Modified `CHANGELOG.md` formatting.
  [#72](https://github.com/OSC/ood-fileeditor/issues/72)
- Updated date in `LICENSE.txt`.

### Fixed
- Set cursor focus in editor on load.
  [#15](https://github.com/OSC/ood-fileeditor/issues/15)

## [1.3.2] - 2017-11-27
### Changed
- Update to Rails 4.2.10 to better support Ruby 2.4.
  [#71](https://github.com/OSC/ood-fileeditor/issues/71)
- Update `ood_support` gem to 0.0.3 to better support Ruby 2.4.

## [1.3.1] - 2017-06-05
### Changed
- Save user preferences to local storage instead of cookies.

## [1.3.0] - 2017-05-26
### Changed
- Updated to Ace Editor 1.2.6.
- Updated gem dependencies.
- Updated to Rails 4.2.7.1.

## [1.2.5] - 2017-04-20
### Added
- Added `bin/setup` script for easier deployment.

## [1.2.4] - 2017-04-17
### Changed
- Uses the ace modelist extension to automatically select the appropriate
  syntax highlighting.
- Updated `ood_appkit` gem version.

### Fixed
- Fixed deprecation warnings when precompiling assets.
- Patched mime type check to allow broader range of files.

## [1.2.3] - 2017-03-07
### Fixed
- Ensure we treat all files we open as plain text and avoid executing any files
  as scripts.
- Updated `ood_appkit` dependency so editor can work without valid cluster
  config.

## [1.2.2] - 2017-01-24
### Fixed
- Fix bundler issue.

## [1.2.1] - 2017-01-05
### Fixed
- Fix AJAX 404 response when selecting default keybinding.

## [1.2.0] - 2016-11-21
### Changed
- Updated to Rails 4.2.7.1.
- Documentation improvements.
- Some bugfixes.

## [1.1.1] - 2016-11-15
### Fixed
- Fixed `.env.production` by setting `OOD_DATAROOT`.

## [1.1.0] - 2016-10-28
### Added
- Updated `README.md` documentation with screenshot.
- Added extra font size options.

### Changed
- Made more responsive by hiding some controls when the browser width is
  shrinked.

## 1.0.0 - 2016-06-15
### Added
- Initial release!

[Unreleased]: https://github.com/OSC/ood-fileeditor/compare/v1.3.3...HEAD
[1.3.3]: https://github.com/OSC/ood-fileeditor/compare/v1.3.2...v1.3.3
[1.3.2]: https://github.com/OSC/ood-fileeditor/compare/v1.3.1...v1.3.2
[1.3.1]: https://github.com/OSC/ood-fileeditor/compare/v1.3.0...v1.3.1
[1.3.0]: https://github.com/OSC/ood-fileeditor/compare/v1.2.5...v1.3.0
[1.2.5]: https://github.com/OSC/ood-fileeditor/compare/v1.2.4...v1.2.5
[1.2.4]: https://github.com/OSC/ood-fileeditor/compare/v1.2.3...v1.2.4
[1.2.3]: https://github.com/OSC/ood-fileeditor/compare/v1.2.2...v1.2.3
[1.2.2]: https://github.com/OSC/ood-fileeditor/compare/v1.2.1...v1.2.2
[1.2.1]: https://github.com/OSC/ood-fileeditor/compare/v1.2.0...v1.2.1
[1.2.0]: https://github.com/OSC/ood-fileeditor/compare/v1.1.1...v1.2.0
[1.1.1]: https://github.com/OSC/ood-fileeditor/compare/v1.1.0...v1.1.1
[1.1.0]: https://github.com/OSC/ood-fileeditor/compare/v1.0.0...v1.1.0
