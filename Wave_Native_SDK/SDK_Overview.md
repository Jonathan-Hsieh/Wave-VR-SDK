+   [Docs](https://hub.vive.com/storage/docs/en-us/index.html) » [Wave Native SDK](https://hub.vive.com/storage/docs/en-us/NativeSdk.html) » SDK Overview

* * *

## SDK Overview[¶](#id1 "Permalink to this headline")

VIVE Wave™ SDK provides a suite of Virtual Reality APIs to introduce VR content applications on mobile device to independently work with VR accessories. VR content developers have no need to pick up the specific VR hardware knowledge and can concentrate on the content core design.

VIVE Wave™ SDK adopts the client-server architecture. The content application in client side works with server via IPC connection and the IPC interface is backward compatible. The client content application does not need to re-compile for the further server upgrade. They are totally transparent for the maintenance of version forward in the future.

<table class="docutils"><colgroup><col width="100%"></colgroup><tbody><tr class="row-odd"><td><p class="first"><strong>Contents</strong></p><ul class="last simple"><li><a class="reference internal" href="#init-and-quit">Init and Quit</a></li><li><a class="reference internal" href="#interfaces">Interfaces</a></li><li><a class="reference internal" href="#others">Others</a></li></ul></td></tr></tbody></table>

## Init and Quit[¶](#init-and-quit "Permalink to this headline")

Consider that content applications access VR stack flexibly in the suitable time of content lifecycle. VIVE Wave™ does not automatically initiate or destroy VR instance for content app. The content app must invoke WVR\_Init function prior to any VR operations and invoke WVR\_Quit to release the VR resource finally.

+   [WVR Init and Quit](https://hub.vive.com/storage/docs/en-us/Sdk_WvrInitAndQuit.html)

## Interfaces[¶](#interfaces "Permalink to this headline")

VIVE Wave™ API includes the following interfaces:

+   [WVR Device](https://hub.vive.com/storage/docs/en-us/Sdk_WvrDevice.html) : Main interface for the device state, tracking pose, and user input of tracked device.
+   [WVR Event](https://hub.vive.com/storage/docs/en-us/Sdk_WvrEvent.html) : Common Event Access
+   [WVR Arena](https://hub.vive.com/storage/docs/en-us/Sdk_WvrArena.html) : Interfaces to access the settings of Arena.
+   [WVR Display](https://hub.vive.com/storage/docs/en-us/Sdk_WvrProjection.html) : Interfaces about the model view transform and projection.
+   [WVR Render](https://hub.vive.com/storage/docs/en-us/Sdk_WvrRender.html) : Interfaces about controlling render thread and updating render target to display.
+   [WVR System](https://hub.vive.com/storage/docs/en-us/Sdk_WvrSystem.html) : Interfaces to get the system status of VR runtime.
+   [WVR Overlay](https://hub.vive.com/storage/docs/en-us/Sdk_WvrOverlay.html) : Interface to draw 2D images over 3D scenes.
+   [WVR Vulkan](https://hub.vive.com/storage/docs/en-us/Sdk_WvrVulkan.html) : Interface to integrate with Vulkan application.
+   [WVR Controller Model](https://hub.vive.com/storage/docs/en-us/Sdk_WvrControllerModel.html) : Interface to get controller model or emitter information of current connected controller.
+   [WVR Hand](https://hub.vive.com/storage/docs/en-us/Sdk_WvrHand.html) : Interface to get hand tracking data of VR runtime.
+   [WVR Hand Model](https://hub.vive.com/storage/docs/en-us/Sdk_WvrHandModel.html) : Interface to get hand model data of VR runtime.
+   [WVR Tracker](https://hub.vive.com/storage/docs/en-us/Sdk_WvrTracker.html) : Interface to get tracker data of VR runtime.
+   [WVR Eye](https://hub.vive.com/storage/docs/en-us/Sdk_WvrEye.html) : Interfaces to get eye tracking pose and expresion data.
+   [WVR Lip](https://hub.vive.com/storage/docs/en-us/Sdk_LipExpression.html) : Interfaces to get lip expression data.
+   [WVR Notify DeviceInfo](https://hub.vive.com/storage/docs/en-us/Sdk_NotifyDeviceInfo.html) : Interfaces Let AP notify DS information.
+   [WVR Scene](https://hub.vive.com/storage/docs/en-us/Sdk_WvrScene.html) : Interfaces Let AP access scene DS to manage the system resource of the scene perception and anchors.
+   [WVR Marker](https://hub.vive.com/storage/docs/en-us/Sdk_WvrMarker.html) : Interfaces Let AP access marker DS to manage the system resource of the marker detection and trackable markers.

## Others[¶](#others "Permalink to this headline")

+   [WVR Version Check](https://hub.vive.com/storage/docs/en-us/Sdk_WvrVersionCheck.html) : About runtime, sdk Version.
+   [WVR Supported Features](https://hub.vive.com/storage/docs/en-us/WVR_GetSupportedFeatures.html) : Get device supported features。
+   [WaveVR Time Warp Stabilization](https://hub.vive.com/storage/docs/en-us/Sdk_WvrTimeWarpStabilization.html) : Introduce Time Warp Stabilized mode.