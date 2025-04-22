+   [Docs](https://hub.vive.com/storage/docs/en-us/index.html) » [Wave Native SDK](https://hub.vive.com/storage/docs/en-us/NativeSdk.html) » [SDK Overview](https://hub.vive.com/storage/docs/en-us/SdkOverview.html) » [WVR Init and Quit](https://hub.vive.com/storage/docs/en-us/Sdk_WvrInitAndQuit.html) » WVR\_Quit

* * *

## WVR\_Quit[¶](#wvr-quit "Permalink to this headline")

`WVR_EXPORT void WVR_Quit()`

Quit the VR runtime.

Close and release all the resource allocated form VR runtime.

**Version**

API Level 1

## How to use[¶](#how-to-use "Permalink to this headline")

Here is an example for the function:

```
#include <wvr/wvr.h>

//work is done, call WVR_Quit to release all resource.
WVR_Quit();
```