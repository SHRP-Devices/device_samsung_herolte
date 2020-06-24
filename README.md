# SHRP Device Tree For Samsung Galaxy S7 aka Herolte

Add to .repo/local_manifests/herolte.xml:

```xml
 <?xml version="1.0" encoding="UTF-8"?>
 <manifest>
  <project name="SHRP-Devices/device_samsung_herolte" path="device/samsung/herolte" remote="github" revision="android-9.0" />
 </manifest>
```

Then run repo sync to check it out.

To build:

```sh
export ALLOW_MISSING_DEPENDENCIES=true
. build/envsetup.sh
lunch omni_herolte-eng
mka recoveryimage
```

Kernel sources are available at: https://github.com/morogoku/android_kernel_samsung_universal8890
