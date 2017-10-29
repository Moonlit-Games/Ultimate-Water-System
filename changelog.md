# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [unreleased] - 2.0.0b3


### Added
- [#16](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/16) - WaveEmitters from PW2.0b13

### Changed
 - merged fixes from _PlayWay Water v2.0b13_
 - _Water.GetHeightAt_ and other data sampling methods now compensate horizontal displacements by default.
 For the old behaviour, use _Water.GetHaightAtUncompensated_
- _Toggle SceneView Rendering_ is now saved in _Water Project Settings_

### Fixed
- [#12](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/12) - searching for the UWS folder causing errors when trying to create new _WaterQualitySettings_ asset
- [#12](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/12) - lack of _WaterQualitySettings_ synchronization with Unity profiles after creating new WQS asset
- [#12](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/12) - issue with _WaterQualitySettings_ not creating after entering playmode (when it was deleted earlier)
- [#9](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/9) - removed black line caused by not cleared _WaterlessDepth_ texture
- [#9](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/9) - fixed EdgeBlendFactor equation in _Deferred Module_
- [#18](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/18) - "disco" effect with _Planar Reflections_ on AMD cards
- [#19](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/19) - Image Effect Deferred problems with depth precision flicker
- errors in _CollectLight_ caused by unused shader variations
- .NET 4.6 compatibility issues caused by different path separators
- issue with growing dynamic wave amplitudes when timeScale == 0
- gizmo showing currently selected _Custom mesh_ in _Water component_ is now multiplied by _water gameObject_ transform matrix

## [2.0.0] - Ultimate Water System release
## [1.X.X] - Reserved for Playway Water
