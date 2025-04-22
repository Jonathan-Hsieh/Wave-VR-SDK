[Wave VR](https://hub.vive.com/storage/docs/en-us/index.html)

+   [Docs](https://hub.vive.com/storage/docs/en-us/index.html) » [Wave Native SDK](https://hub.vive.com/storage/docs/en-us/NativeSdk.html) » [SDK Overview](https://hub.vive.com/storage/docs/en-us/SdkOverview.html) » [WVR Init and Quit](https://hub.vive.com/storage/docs/en-us/Sdk_WvrInitAndQuit.html) » WVR Supported Features

* * *

## WVR Supported Features[¶](#wvr-supported-features "Permalink to this headline")

Check if the following features are supported in your device before using the related APIs.

+   [PassthroughOverlay](https://hub.vive.com/storage/docs/en-us/WVR_ShowPassthroughOverlay.html#wvr-showpassthroughoverlay)
+   [hand tracking](https://hub.vive.com/storage/docs/en-us/Sdk_WvrHand.html#sdk-wvrhand)
+   [Eye tracking/expression](https://hub.vive.com/storage/docs/en-us/Sdk_WvrEye.html#sdk-wvreye)
+   [Lip expression](https://hub.vive.com/storage/docs/en-us/Sdk_LipExpression.html#sdk-lipexpression)
+   [Tracker](https://hub.vive.com/storage/docs/en-us/Sdk_WvrTracker.html#sdk-wvrtracker)
+   [Marker](https://hub.vive.com/storage/docs/en-us/Sdk_WvrMarker.html#sdk-wvrmarker)

`WVR_EXPORT uint64_t WVR_GetSupportedFeatures()`

Function to get if a feature is supportted.

This API can work before or after invoking WVR\_Init

**Return**

The bitmask of all the supported features

**Version**

API Level 5

## How to use[¶](#how-to-use "Permalink to this headline")

Here is an example for WVR\_GetSupportedFeatures:

```
#include <wvr/wvr.h>
#include <wvr/wvr_arena.h>
#include <wvr/wvr_hand.h>
#include <wvr/wvr_eyetracking.h>
#include <wvr/wvr_eyeexp.h>
#include <wvr/wvr_lip.h>
#include <wvr/wvr_tracker.h>

uint64_t supported = WVR_GetSupportedFeatures();

if (supported & WVR_SupportedFeature_PassthroughOverlay) {
    // This device supports passthrough overlay feature
    WVR_ShowPassThroughOverlay(true)
}

if (supported & WVR_SupportedFeature_HandTracking) {
    // This device supports hand tracking feature
    // WVR_StartHandTracking
}

if (supported & WVR_SupportedFeature_HandGesture) {
    // This device supports hand gesture feature
    // WVR_StartHandGesture
}

if (supported & WVR_SupportedFeature_EyeTracking) {
    // This device supports eye tracking feature
    WVR_StartEyeTracking();
}

if (supported & WVR_SupportedFeature_EyeExp) {
    // This device supports eye expression feature
    WVR_StartEyeExp();
}

if (supported & WVR_SupportedFeature_LipExp) {
    // This device supports lip expression feature
    WVR_StartLipExp();
}

if (supported & WVR_SupportedFeature_Tracker) {
    // This device supports tracker feature
    WVR_StartTracker();
}
```

The enum type **WVR\_SupportedFeature** is defined in header wvr.h (as below) for being uesed to check the return value of function WVR\_GetSupportedFeatures.

```
typedef enum {
    WVR_SupportedFeature_PassthroughImage   = 1<<0,    /**< Passthrough image feature type */
    WVR_SupportedFeature_PassthroughOverlay = 1<<1,    /**< Passthrough overlay feature type */

    WVR_SupportedFeature_HandTracking       = 1<<4,    /**< Hand tracking feature type */
    WVR_SupportedFeature_HandGesture        = 1<<5,    /**< Hand gesture feature type */
    WVR_SupportedFeature_ElectronicHand     = 1<<6,    /**< Electronic hand feature type */
    WVR_SupportedFeature_ColorGamutsRGB     = 1<<7,    /**< Color gamut sRGB */
    WVR_SupportedFeature_ColorGamutP3       = 1<<8,    /**< Color gamut P3 */
    WVR_SupportedFeature_EyeTracking        = 1<<9,    /**< Tracking of Eye */
    WVR_SupportedFeature_EyeExp             = 1<<10,   /**< Expression of Eye; Wide, Squeeze, Frown*/
    WVR_SupportedFeature_LipExp             = 1<<11,   /**< Expression of Lip; Jaw, Mouth, Cheek, Tongue*/
    WVR_SupportedFeature_Tracker            = 1<<16,   /**< Tracker feature type */
    WVR_SupportedFeature_ScenePerception    = 1<<17,   /**< Scene Perception feature type */
    WVR_SupportedFeature_Marker             = 1<<18,   /**< Marker feature type */
} WVR_SupportedFeature;
```