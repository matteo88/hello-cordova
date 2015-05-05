# hello-cordova

## REQUISITES

[Java >= 1.7](http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html) or Openjdk 7 (see your linux distribution package)

[Android-sdk >= API 19](http://developer.android.com/sdk/installing/index.html)

[Node](https://nodejs.org/)

[Apache Cordova](http://cordova.apache.org)

Then:

```
npm isntall [-g] phonegap
```

## BUILD

Set path for android sdk (Android and tools: API 19 nedeed)

```
PATH=$PATH:~/android-sdk/android-sdk-linux/platform-tools:~/android-sdk/android-sdk-linux/tools
```
```
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
