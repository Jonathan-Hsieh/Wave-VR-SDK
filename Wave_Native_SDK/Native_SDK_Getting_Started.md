+   [Docs](https://hub.vive.com/storage/docs/en-us/index.html) »
+   [Wave Native SDK](https://hub.vive.com/storage/docs/en-us/NativeSdk.html) »
+   Native SDK Getting Started

* * *

## Native SDK Getting Started[¶](#native-sdk-getting-started "Permalink to this headline")

In this section, you will learn how to build your first application: “HelloVR”.

<table class="docutils"><colgroup><col width="100%"></colgroup><tbody><tr class="row-odd"><td><p class="first"><strong>Contents</strong></p><ul class="last simple"><li><a class="reference internal" href="#set-up-your-development-environment">Set up your development environment</a></li><li><a class="reference internal" href="#download-wave-sdk">Download Wave SDK</a></li><li><a class="reference internal" href="#build-wave-app">Build Wave App</a></li></ul></td></tr></tbody></table>

## Set up your development environment[¶](#set-up-your-development-environment "Permalink to this headline")

The first step is to set up the development environment on your PC.

+   Download, install and launch your Android™ Studio: [https://developer.android.com/studio](https://developer.android.com/studio)
+   In Android Studio, go to **Configure** > **Project Defaults** > **Project Structure** to set up your **SDK location**, **JDK location** and **NDK location** in Android™ Studio.

![_images/AndroidStudio_Project_Structure.PNG](https://hub.vive.com/storage/docs/en-us/_images/AndroidStudio_Project_Structure.PNG)

![_images/AndroidStudio_SDK_Location.PNG](https://hub.vive.com/storage/docs/en-us/_images/AndroidStudio_SDK_Location.PNG)

## Download Wave SDK[¶](#download-wave-sdk "Permalink to this headline")

You can download the Wave SDK from [here](https://developer.vive.com/resources/vive-wave/download/latest/).

**SDK Folder Layout:**

> +   **repo:** SDK repository.
> +   **samples:** native sample source.
> +   **tools:** SDK tool APK.

For more information, refer to **SDK/README.md**

## Build Wave App[¶](#build-wave-app "Permalink to this headline")

1.  Use Android Studio to open the sample project `SDK/samples/wvr_native_hellovr`.
2.  Modify `app/build.gradle` to comply with the Android™ SDK and build tool version of your Android Studio and then click **File** > **Sync Project with Gradle Files**.

Note

+   Please check your Wave VR version and android targetSdkVersion on [Wave VR Version List](https://hub.vive.com/storage/docs/en-us/SDKVersion.html)

![_images/AndroidStudio_build_gradle.PNG](https://hub.vive.com/storage/docs/en-us/_images/AndroidStudio_build_gradle.PNG)

3.  Make project: **Build** > **Make Project**.
4.  Build apk: **Build** > **Build APK(s)**.
5.  After a successful build, you will see Event Log **“APK(s) generated successfully”**. Click **locate** to get the sample APK.

![_images/AndroidStudio_build_apk.PNG](https://hub.vive.com/storage/docs/en-us/_images/AndroidStudio_build_apk.PNG)