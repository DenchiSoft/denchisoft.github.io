When VTube Studio detects a new Live2D Cubism model file (_<model>.model3.json_) in its Live2DModels-Folder, it will automatically create a VTube Studio Model file with the name <model>.vtube.json.

This file will hold all the model meta-information and the model parameter setup (mapping between face tracking and Live2D parameters).

The structure is mostly self-explanatory. The first part holds the file structure version, the model name abd file references. The second part is an array of all VTS parameters. Each VTS parameter is a mapping of an input parameter (face-tracking) to an output parameter (Live2D).

```json
{
    "Version": 1,
    "Name": "My Model Name",
    "FileReferences": {
        "Icon": "icon_name.jpg",
        "Model": "my_live2d_model.model3.json",
        "IdleAnimation": "my_idle_animation.motion3.json"
    },
    "ParameterSettings":
    [
        {
            "Name": "Face Left/Right Rotation",
            "Input": "FaceAngleX",
            "InputRangeLower": -30.0,
            "InputRangeUpper": 30.0,
            "OutputRangeLower": -30.0,
            "OutputRangeUpper": 30.0,
            "ClampInput": false,
            "ClampOutput": false,
            "UseBlinking": false,
            "OutputLive2D": "PARAM_ANGLE_X",
            "Smoothing": 15
        }
    ]
}
```


