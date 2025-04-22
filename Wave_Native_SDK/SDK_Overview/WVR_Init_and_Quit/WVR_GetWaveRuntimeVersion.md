+   [Docs](https://hub.vive.com/storage/docs/en-us/index.html) » [Wave Native SDK](https://hub.vive.com/storage/docs/en-us/NativeSdk.html) » [SDK Overview](https://hub.vive.com/storage/docs/en-us/SdkOverview.html) » [WVR Init and Quit](https://hub.vive.com/storage/docs/en-us/Sdk_WvrInitAndQuit.html) » WVR\_GetWaveRuntimeVersion

* * *

## WVR\_GetWaveRuntimeVersion[¶](#wvr-getwaveruntimeversion "Permalink to this headline")

`WVR_EXPORT uint32_t WVR_GetWaveRuntimeVersion()`

Get the runtime version.

**Return**

Retrieves the runtime version. It is considered an error if the returned value is 0.

**Version**

API Level 1

## How to use[¶](#how-to-use "Permalink to this headline")

Here is an example for the function:

```
#include <wvr/wvr.h>

uint32_t version;
version = WVR_GetWaveRuntimeVersion();
```