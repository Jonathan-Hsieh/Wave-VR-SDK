+   [Docs](https://hub.vive.com/storage/docs/en-us/index.html) » [Wave Native SDK](https://hub.vive.com/storage/docs/en-us/NativeSdk.html) » [SDK Overview](https://hub.vive.com/storage/docs/en-us/SdkOverview.html) » [WVR Init and Quit](https://hub.vive.com/storage/docs/en-us/Sdk_WvrInitAndQuit.html) » WVR\_GetInitErrorString

* * *

## WVR\_GetInitErrorString[¶](#wvr-getiniterrorstring "Permalink to this headline")

`WVR_EXPORT const char* WVR_GetInitErrorString(WVR_InitError error)`

Get the error description for the WVR\_InitError.

**Return**

const char\*, refer the string description to know what error occurs

**Version**

API Level 1

**Parameters**

+   `error`: which indicate WVR\_InitError type.

## How to use[¶](#how-to-use "Permalink to this headline")

Here is an example for the function:

```
#include <wvr/wvr.h>

// Loading the WVR Runtime
WVR_InitError eError = WVR_InitError_None;
eError = WVR_Init(WVR_AppType_VRContent);

//Get the error description
if (eError != WVR_InitError_None) {
    LOGE("Unable to init VR runtime: %s", WVR_GetInitErrorString(eError));
    return false;
}
```

WVR\_InitError includes the following below:

*enum* `WVR_InitError`[¶](#_CPPv213WVR_InitError "Permalink to this definition")  

returned error of initialize VR runtime

Describes what kind of error is being returned by the WVR\_Init function

*Values:*

`WVR_InitError_None` = 0[¶](#_CPPv218WVR_InitError_None "Permalink to this definition")  

Init successed

`WVR_InitError_Unknown` = 1[¶](#_CPPv221WVR_InitError_Unknown "Permalink to this definition")  

Unknown error

`WVR_InitError_NotInitialized` = 2[¶](#_CPPv228WVR_InitError_NotInitialized "Permalink to this definition")  

Init failed