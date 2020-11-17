# Changelog

[\[Back to main page\]](https://denchisoft.github.io/)

## Version 1.4.1

_Released November 17 2020_

#### New features
 - Selection list for backgrounds.
 - Support for [Newtek NDI](https://en.wikipedia.org/wiki/Network_Device_Interface) (transparent streaming to OBS without showing VTube Studio UI)
 - Update-reminder popup when new version is available on itch.io

#### Improvements & Bugfixes
 - Updated all AR related libraries to newest version.
 - Fixed bugs in tracking setup that resulted in tracking glitches/lag/jumps.
 - Slightly improved tracking performance/stability and various crashes.
 - Fixed model texture import so models on Windows/MacOS can now be resized without looking pixelated.

## Version 1.4.0

_Released September 23 2020_

#### New features
 - Hotkeys can now set model position.
 - Models can now be moved when config is open.
 - Search bar for parameter lists.
 - Full support for iOS 14.

#### Improvements & Bugfixes
 - Fixed bug in expressions: Expression values are now additive. Multiply mode not yet supported.
 - Fixed bug where missing Live2D parameters prevented successful model loading.
 - Increased scrolling speed (mouse wheel).
 - Added scrollbar for model config tab.

## Version 1.3.2

_Released August 29th 2020_

#### New features
 - Added mouse tracking as input parameter.
 - Added mouse click (left/right/mid) as hotkey, on MacOS only within window.
 - Streaming Mode: Automatically choose optimal settings to ensure phone won’t get too hot while streaming to PC.
 - Added FPS options: 60 FPS, 30 FPS and VSync (match screen refresh rate).
 - Smooth resize/rotate for Live2D model on Windows and MacOS.
 - More face tracking parameters on iOS: FaceAngry, CheekPuff, BrowLeftY, BrowRightY
 - Model physics: Boost settings.
 - Model physics: Wind settings.
 - Pressing back button on Android will now close config if it’s open. Otherwise app is closed.
 
#### Improvements & Bugfixes
 - Fixed face rotation glitch and calibration drift.
 - Set CubismGlobalMaskTexture to 4096/2084 depending on platform for better mask quality.
 - Fixed accidental clicks (breath/blink button, etc.) when scrolling through UI.
 - Removed black overlay in config on Win/Mac so model isn’t transparent in OBS anymore.
 - Removed bear.
 - Updated ARCore/ARKit SDK to latest version.
 - Replaced Live2D animation system with own implementation.
 - Fixed looping for idle animations including Live2D “repeat parameters”.
 - Removing model selection bar when closing UI.
 - Improved texture quality on Windows and MacOS.
 - Fixed auto-breath and auto-blink when no input/output parameter is selected.
 - Fixed bug where Auto-Blink wouldn’t work sometimes.
 - Slightly improved blink detection on iPhone.

## Version 1.2.2

_Released July 27th 2020_

#### New features
 - Trigger hotkeys. Background hotkeys (window not in focus) supported only on windows. You can also set hotkey combinations.
 - Screen button hotkeys: Use smartphone as a remote to activate hotkeys in the Windows/Mac app.
 - Settings are now saved between app restarts.
 - Option to "save scene setup": last background and model are saved/loaded when restarting the app.
 - Virtual webcam to stream directly into other apps (Windows only)
 - Automatically scan for and find server from within app.
 - Windows/Mac app now shows list of all IPs instead of just the first one.
 - Live2D rendering performance improvements. 

#### Bugfixes
 - Fixed smaller networking issues.
 - Fixed audio quality issues when recording on Android.
 - Fixed screen rotation bug.

## Version 1.0.2
_Released June 27th 2020_

#### New features
 - Japanese translation / 日本語版
 - In-App recording/sharing on Android and iOS
 - Support for phone-rotation: portrait and portrait-upside-down
 - "None" can be selected for icon and idle animation
 - Auto-breathing can now be set for parameters
 - Model movement: automatically move model right/left, up/down, close/far depending on your head position
 - Basic Anti-Aliasing (FXAA)
 
#### Bugfixes
 - Fixed bug where parameter breaks when parameter input max is set to the same value as parameter input min
 - Fixed wrong camera aspect ratio
 - Better error handling: app now warns you when broken model is imported instead of just freezing

## Version 1.0.1
_Released June 1st 2020_

 - Initial version
 - Basic face tracking functionality
