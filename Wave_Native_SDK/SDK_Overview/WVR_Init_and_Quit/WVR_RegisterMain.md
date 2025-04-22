## WVR\_RegisterMain[¶](#wvr-registermain "Permalink to this headline")

`typedef int (* WVR_Main_t)(int argc, char *argv[])`

It is the entry function pointer of the native application.

The pointer of the entry function is set to associate with the runtime library.

`WVR_EXPORT void WVR_RegisterMain(WVR_Main_t main)`

Interface to register the main function.

When VM needs to load native library and call JNI\_Onload, runtime expect the entry function of native application registed here via this API.

**Version**

API Level 1

**Parameters**

+   `WVR_Main_t`: the entry function pointer of native application.

## How to use[¶](#how-to-use "Permalink to this headline")

Here is an example for the function:

```
// Example in MainActivity.java
public class MainActivity extends VRActivity {

    @Override
    protected void onCreate(Bundle icicle) {
        init();
        super.onCreate(icicle);
    }

    // Pass this acitivty instance to native
    @SuppressWarnings("unused")
    public native void init();
}
```

```
// Example in jni.cpp
#include <wvr/wvr.h>

int main(int argc, char *argv[]) {
    return 0;
}

JNIEXPORT void JNICALL Java_com_htc_vr_samples_wvr_1hellovr_MainActivity_init(JNIEnv * env, jobject obj) {
    LOGI("register WVR main here.");
    WVR_RegisterMain(main);
}
```