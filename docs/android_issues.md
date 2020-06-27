# Android Issues

[\[Back to main page\]](https://denchisoft.github.io/)

Android uses ARCore for face tracking. Compared to Apple's ARKit, Google ARCore is relatively slow and also doesn't quite compare in terms of tracking quality.

Unlike ARKit, ARCore also doesn't directly give the developer face parameters such as "smile" and "mouth open/close", but you have to calculate them yourself. To get high-quality zero-latency face tracking, I recommend using the iPhone version of VTube Studio.

The current version of Google ARCore also has a bug on many devices, effectively causing a delay of half a second in the tracking (see [here](https://github.com/google-ar/arcore-unity-sdk/issues/706) and [here](https://github.com/google-ar/arcore-unity-sdk/issues/711)).

### Downgrading ARCore for faster tracking
Instead of using the newest version of ARCore from the Google Play Store (versions 1.16.xxx and 1.17.xxx), you can try using an older version (1.15.200121046) which seems to not have this issue. However, this version will not work on some devices and just show a black screen in the preview window.

To downgrade to that version, uninstall ARCore in the Google Play Store (app name is **Google Play Services for AR**), then install the [older APK from APKMirror](https://www.apkmirror.com/apk/google-inc/arcore/arcore-1-15-20012104-release/google-play-services-for-ar-1-15-200121046-android-apk-download/). If you don't know how to install APKs on your Android device, there are [many guides on the internet](https://www.google.com/search?hl=en&q=how+to+install+apk+android&oq=how+to+install+apk+android).
