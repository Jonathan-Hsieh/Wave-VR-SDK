+   [Docs](https://hub.vive.com/storage/docs/en-us/index.html) » [Wave Native SDK](https://hub.vive.com/storage/docs/en-us/NativeSdk.html) » [SDK Overview](https://hub.vive.com/storage/docs/en-us/SdkOverview.html) » WVR Init and Quit

* * *

## WVR Init and Quit[¶](#wvr-init-and-quit "Permalink to this headline")

Wave VR does not automatically start or end a VR instance for an app. The app must invoke WVR\_Init to start the VR operation and invoke WVR\_Quit to release resources used by the app.

```
#include <wvr/wvr.h>
```

+   [WVR\_Init](https://hub.vive.com/storage/docs/en-us/WVR_Init.html)
+   [WVR\_Quit](https://hub.vive.com/storage/docs/en-us/WVR_Quit.html)
+   [WVR\_GetInitErrorString](https://hub.vive.com/storage/docs/en-us/WVR_GetInitErrorString.html)
+   [WVR\_RegisterMain](https://hub.vive.com/storage/docs/en-us/WVR_RegisterMain.html)
+   [WVR\_GetWaveRuntimeVersion](https://hub.vive.com/storage/docs/en-us/WVR_GetWaveRuntimeVersion.html)
+   [WVR\_GetWaveSDKVersion](https://hub.vive.com/storage/docs/en-us/WVR_GetWaveSDKVersion.html)
+   [WVR Supported Features](https://hub.vive.com/storage/docs/en-us/WVR_GetSupportedFeatures.html)