
![Logo](https://github.com/koengu/XposedFrameworkOffline/assets/40539111/8e6a281e-3f77-4bde-bb7d-9ab4aab1eb6f)


Xposed Installer and Framework for offline use contains Android 5.0 to 8.0 support.


## Installation - Genymotion
1. Install [**Xposed_Installer.apk**](https://github.com/6f090441-b1ae-4a94-bf8d-0deb1854aafa) via Drag and Drop.
2. Download **Xposed Framework** and drag and drop it. For Genymotion use the x86 versions of Framework.

## Installation - nonGenymotion
1. Install [**Xposed_Installer.apk**](https://github.com/6f090441-b1ae-4a94-bf8d-0deb1854aafa), you can use ADB:
```bash
adb install Xposed_Installer.apk

```
2. Download **Xposed Framework** and extract it, then install it via ADB:
```bash
adb connect [DeviceIpAddress]
adb push system /sdcard
adb push META-INF\com\google\android\* \sdcard
adb shell
cd /sdcard
su
sh flash-script.sh
reboot
```
If you get error on *adb push META-INF\com\google\android\* \sdcard* command, you can push all files individualy.

 
