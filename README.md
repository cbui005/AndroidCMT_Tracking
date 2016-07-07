# AndroidCMT_Tracking
Android mobile application designed to track user specified objects using OpenCV with TLD and CMT tracking algorithms.

## Dependencies

[OpenCV Android 3.1](http://opencv.org/downloads.html)

[Android Studio 2.1](https://developer.android.com/studio/index.html)


[Tracking Learning Detection (TLD)](http://www.gnebehay.com/tld/)

[Consensus-based Tracking and Matching of Keypoints for Object Tracking (CMT)](http://www.gnebehay.com/cmt/)

[Android NDK Bundle (allows application developers to build performance-critical portions of their apps by use of native (C/C++) code)](https://developer.android.com/ndk/downloads/index.html)

This setup is to support Android Marshmallow 6.0.1 (API 23) and testing is being done on Samsung Galaxy S7 edge.

## Configurations

In the app build.gradle, targetSdkVerison.apiLevel is set to 22 because with API 23, you need to request permissions to access and use the camera. Setting target API to 22 allows us to still use the camera without needing to explicitly request camera permission.
>targetSdkVersion.apiLevel = 22

Android NDK Settings
> Flags for c++ compiling. Settings are found in app's build.gradle under android.ndk
```
cppFlags += "-std=c++11"
cppFlags += "--debug"
cppFlags += "-frtti"
cppFlags += "-fexceptions"
```

## Todo
```
Finish implementing the different menu options
Make sure switching modes works smoothly
Possible methods for improving frame rate 
```


## License
[GNU License](https://github.com/gentlespoon/rshell/blob/exec/LICENSE)
