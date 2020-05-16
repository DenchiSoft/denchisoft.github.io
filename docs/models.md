# How to load your own Live2D Models

[\[Back to main page\]](https://denchisoft.github.io/)

Loading your own Live2D models to use them in VTube Studio is super easy! First, find the __"Live2DModels"-Folder__ in the app. Depending on the platform, you'll find it here:

- **iPhone:** Open VTube Studio app data folder on your iPhone in iTunes (Windows or macOS) or Finder (on macOS Catalina). You'll find a Live2DModels-Folder.
- **Android:** \<Your Phone\>/Android/data/com.denchi.vtubestudio/files/Live2DModels
- **Mac:** VtubeStudio.app/Contents/Resources/Data/StreamingAssets/Live2DModels
- **Windows:** \<VTubeStudio.exe-Path\>/Vtube Studio_Data/StreamingAssets/Live2DModels

Create a folder for your model in the Live2DModels-Folder. In that folder, put the following files:
- All your Live2D model files, as you have exported it from Live2D ("export for runtime"). This includes the .model3.json file, the .moc3 file, the folder for the texture(s) and the physics3.json file.
- __\[optional\]__ A .PNG or .JPG to use as icon for the model in the model picker.
- __\[optional\]__ An animation to use as default idle animation for the model.

The model will now be available in the VTube Studio app and you can load it. You can then use Auto-Setup to set up the face tracking using VTS parameters or create them automatically. For more information, see the [VTube Studio Interface Documentation](https://denchisoft.github.io/docs/interface.html) or watch the following video.

<iframe width="360" height="252" src="//www.youtube.com/embed/pg6A4srAXyA" frameborder="0" allowfullscreen="allowfullscreen">&nbsp;</iframe>

<br />
