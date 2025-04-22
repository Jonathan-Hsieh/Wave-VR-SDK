+   [Docs](https://hub.vive.com/storage/docs/en-us/index.html) » [Wave Native SDK](https://hub.vive.com/storage/docs/en-us/NativeSdk.html) » [SDK Overview](https://hub.vive.com/storage/docs/en-us/SdkOverview.html) » [WVR Init and Quit](https://hub.vive.com/storage/docs/en-us/Sdk_WvrInitAndQuit.html) » WVR\_Init

* * *

## WVR\_Init[¶](#wvr-init "Permalink to this headline")

`WVR_EXPORT WVR_InitError WVR_Init(WVR_AppType type = WVR_AppType_VRContent)`

Init the VR runtime.

**Return**

enum WVR\_InitError to know what error occurs

**Version**

API Level 1

**Parameters**

+   `type`: which indicate the application type for this rumtime initialization. **NOTE:** Now this param is ignored by system.

## How to use[¶](#how-to-use "Permalink to this headline")

Here is an example for the function:

```
#include <wvr/wvr.h>

// start to loading the WVR Runtime
WVR_InitError eError = WVR_InitError_None;
eError = WVR_Init(WVR_AppType_VRContent);
```