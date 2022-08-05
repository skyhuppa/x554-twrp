# infinix_x544_device_tree

To clone tree automatically, then;
 `cd .repo && mkdir local_manifests`
 `cd local_manifests`

Add to `.repo/local_manifests/w4.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>

	<project path="device/tecno/w4" name="iykequame/android_device_infimix_x554" remote="github" revision="master" />

</manifest>
```

Then run `repo sync` or  `repo sync --force-sync`  to check it out.

or

`git clone https://github.com/iykequame/android_device_infimix_x554.git -b master  device/tecno/w4`


# How To Compile

```
 1. source build/envsetup.sh
 2. lunch
  and select your device from menu [select omni_x554-userdebug]
 3. mka -j5 recoveryimage
```
It will take time to compile your build/compile

 4. Find your compiled recovery - image in "$out/out/target/product/codename"


---------------
