# hello-cordova

## REQUISITES

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
