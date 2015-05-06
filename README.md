# QUICKSTART

## PREREQUISITES

Install Openjdk 7:
```
 # apt-get install openjdk-7-jdk
```
Install Android sdk and tools:

  * Download [Android-sdk](http://developer.android.com/sdk/index.html#Other)

Extract into your home, then:

```
cd ~/android-sdk-linux
./tools/android
```
The android sdk manager will open.
From the mangaer, install:

  * (at least) Android API 19
  * android sdk tools
  * android sdk build-tools 19.1
  * android sdk build-tools 20

Install node:

```
# npm isntall -g phonegap
```
## BUILD

Set path for android sdk

```
PATH=$PATH:~/android-sdk-linux/platform-tools:~/android-sdk-linux/tools

phonegap -V build android
```

## INSTALL

Intall on device:

Makes use of `adb` to detect plugged devices. If only one device is plugged:

```
phonegap run android
```

otherwise:

```
phonegap run android --device=<device-code-here>
```
           
