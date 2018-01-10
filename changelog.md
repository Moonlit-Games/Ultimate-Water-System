# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [2.1.0] - 2018-01-01

### Added
- [#16](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/16) - WaveEmitters from PW2.0b13
- [#30](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/30) - the _WaterVolumeBase_ takes collider.center into account
- [#26](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/26) - _WaterProfileBlendSimple_ for easier integration
- [#23](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/23) - customizable submersion detection
- very basic demo scene showing ShipBowWaves

### Changed
 - merged fixes from _PlayWay Water v2.0b13_
 - _Water.GetHeightAt_ and other data sampling methods now compensate horizontal displacements by default.
 For the old behaviour, use _Water.GetHaightAtUncompensated_
- _Toggle SceneView Rendering_ is now saved in _Water Project Settings_
- all demo scenes now include reflection probes
- renamed part of the API variables to new naming conventions
- changed _WaterForceData_ to _WaterForce.Data_
- GetAndResetFast now take _out_ instead of _ref_ parameters
- changed _WaterGlobals_ to _WaterSystem_
- moved _FindWater_ methods from _Water_ script to _WaterSystem_

### Fixed
- [#12](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/12) - searching for the UWS folder causing errors when trying to create new _WaterQualitySettings_ asset
- [#12](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/12) - lack of _WaterQualitySettings_ synchronization with Unity profiles after creating new WQS asset
- [#12](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/12) - issue with _WaterQualitySettings_ not creating after entering playmode (when it was deleted earlier)
- [#9](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/9) - removed black line caused by not cleared _WaterlessDepth_ texture
- [#9](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/9) - fixed EdgeBlendFactor equation in _Deferred Module_
- [#18](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/18) - "disco" effect with _Planar Reflections_ on AMD cards
- [#19](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/19) - Image Effect Deferred problems with depth precision flicker
- [#7](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/7) - hardcoded 1000 units clipping
- [#1](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/1) - invisible water
- [#28](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/28) - removed _Camera.Main_ check in _DynamicWater
- [#28](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/28) - allocations in _VersionCompatibility_ check
- [#25](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/25) - _RadialGrid_ matrix calculations when camera's facing down
- [#5](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/5) - vertical dark lines with _deferred_ 
- [#5](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/4) - transparency bug
- [#15](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/15) - shader compilation error on Collect Light shader
- [#16](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/35) - NRE in _WaterSample_ when we change scene from one that contains water to one that does not
- [#38](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/38) - shader compiler error caused by lack of _static_ keyword on _WaterData_ variable definition
- [#23](https://github.com/Moonlit-Games/Ultimate-Water-System/issues/23) - submersion state not behaving correctly

- errors in _CollectLight_ caused by unused shader variations
- .NET 4.6 compatibility issues caused by different path separators
- issue with growing dynamic wave amplitudes when timeScale == 0
- gizmo showing currently selected _Custom mesh_ in _Water component_ is now multiplied by _water gameObject_ transform matrix
- removed unnecessary _Graphics.Blit_ calls in _WaterSimulationArea_
- removed linq foreach iteration in _Water_ to prevent memory allocations
- removed unnecessary _string memcpy_ in _WaterParticleDislplacement_
- mimap info in _WaterProjectSettings_ is now cached
- exploding _WaterSimulationArea_
- OpenGl: "Graphics.CopyTexture called on textures of different sizes" error in _WaterRaindropsIME_
- OpenGl: inverted Raindrops texture in the _Final_ shader
- render textures not being cleared between scene switches

## [2.0.0] - Ultimate Water System release
## [1.X.X] - Reserved for Playway Water
