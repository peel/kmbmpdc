# Change Log

## [Unreleased]

## [1.2.0] - 2017-03-01
### Added
- Client reconnects automatically to the server after getting disconnected.
- Playlists can be loaded and played from the playlists submenu.

### Changed
- MediaKeyTap switched a forked version to manually update kmbmpdc as the active listener application.

### Fixed
- Pressing any of the menubar buttons now properly sets kmbmpdc as the active listener.

## [1.1.0] - 2017-01-29
### Added
- Playback can be stopped after the current track finishes with the "Stop after current" menu item.
- Server password can be specified in preferences.

### Changed
- Clicking the menubar buttons now sends `NSWorkspaceDidActivateApplication` notifications to ensure [MediaKeyTap](https://github.com/nhurden/MediaKeyTap) switches kmbmpdc to most recently active application.
- ID3v2 cover art parsing changed to use [imeji](https://github.com/arttuperala/imeji).
- Notifications are displayed even if kmbmpdc is considered to be the active application.
- Track change notification is presented when playback is restarted after a stop.
- Track change notifications are executed in main thread instead of the idle thread.

### Fixed
- Application won't crash on start when libmpdclient is not installed locally.
- Application won't crash if client has insufficient permissions due to incorrect server password.

[Unreleased]: https://github.com/arttuperala/kmbmpdc/compare/v1.2.0...HEAD
[1.2.0]: https://github.com/arttuperala/kmbmpdc/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/arttuperala/kmbmpdc/compare/v1.0.0...v1.1.0
