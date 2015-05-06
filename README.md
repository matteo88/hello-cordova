# Quickstart

## Prerequisites

On Debian/Ubuntu, install OpenJDK 7 and NPM:

```
$ sudo apt-get install openjdk-7-jdk npm
```

Create a symlink to the node executable:

```
$ sudo ln -s /usr/bin/nodejs /usr/bin/node
```

Download Android [SDK tools](http://developer.android.com/sdk/index.html#Other) (not *Android Studio Packages*) 

Extract into your home:

```
$ cd ~
$ tar xzf android-sdk_r24.2-linux.tgz
```

Then do:

```
$ cd android-sdk-linux
$ ./tools/android
```

The android sdk manager will open. From it, install:

  * (at least) Android API 19
  * android sdk tools
  * andrid sdk build-tools 19.1
  * android sdk build-tools 20


Install phonegap:

```
$ sudo npm install -g phonegap
```

## Build

Set path for android sdk

```
$ PATH=$PATH:~/android-sdk-linux/platform-tools:~/android-sdk-linux/tools

$ phonegap -V build android
```

## Install

Intall on device:

Makes use of `adb` to detect plugged devices. If only one device is plugged:

```
$ phonegap run android
```

otherwise:

```
$ phonegap run android --device=<device-code-here>
```
           
