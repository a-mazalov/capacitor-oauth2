# Changelog

## [Unreleased]

### Breaking
* Core: Capacitor 2.x is new minimum peer dependency. closes #80
* Additional method argument for `OAuth2CustomHandler#logout`. closes #58
  * iOS: `viewController` as 1st argument
  * Android: `activity` as 1st argument

### Added
* If the user touches "done" in safari without entering the credentials 
the USER_CANCELLED error is sent. closes #71

### Fixed

* XCode 11.4 crash on app start. closes #73. thx [@macdja38](https://github.com/macdja38)
  
### Docs

* CustomHandler Facebook example logout fixed. closes #79. thx [@REPTILEHAUS](https://github.com/REPTILEHAUS)
* Facebook force authentication with FB App. closes #69. thx [@mrbatista](https://github.com/mrbatista)

## [1.1.0] - 2020-01-22
### Changed
- Docs for Facebook if using iOS 13 and Facebook pod 5.x #56
- Align Android behavior to iOS where the additional parameters are not overwritten #57 (thx @maggix)
- Upgrade dev dependencies to Capacitor 1.4.0

### Added
- Refresh token feature for iOS and Android #64 (thx @dennisameling)
- Detect when user cancels authentication on web (implicit flow) #25 (thx @michaeltintiuc)

## [1.0.1] - 2019-09-19
### Added
- Add OpenID not supported to README
- Add CHANGELOG file to project

### Fixed
- web/pwa: `pkceCodeChallenge` was always `undefined` because promise was not awaited properly #53 (thx @nicksteenstra)

## [1.0.0] - 2019-06-26

### Added
- Add minimum cap version to installation notice

### Changed
- Upgrade to Capacitor 1.0.0 #43,#39

### Fixed
- Android: Fix plugin does not send resource url response to app after specific steps #28
- Android: Fix Java compiler error #36 (thx @Anthbs)
- Fix github security error by updating Jest lib


[Unreleased]: https://github.com/moberwasserlechner/capacitor-oauth2/compare/1.1.0...master
[2.0.0]: https://github.com/moberwasserlechner/capacitor-oauth2/compare/1.1.0...2.0.0
[1.1.0]: https://github.com/moberwasserlechner/capacitor-oauth2/compare/1.0.1...1.1.0
[1.0.1]: https://github.com/moberwasserlechner/capacitor-oauth2/compare/1.0.0...1.0.1
[1.0.0]: https://github.com/moberwasserlechner/capacitor-oauth2/releases/tag/1.0.0