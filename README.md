# adb-fastboot

Overview
========

This repository contains patches that can be used to build "adb" and "fastboot"
binaries without needing the full Android build environment.

This is useful when needing up-to-date binaries for Linux versions that are not
supported by the official Android SDK.

As building the binaries can be tricky, this repository contains pre-build
binaries for Linux i386, x86-64 (also known as amd64) and for ARM. These files
might be useful to anybody trying to run "adb" and "fastboot" from within
"crouton".

N.B. these binaries are linked dynamically against Ubuntu (14.04, Trusty) system
libaries. They should work on any system that looks like a normal Linux
distribution. But while they can talk to Android phones, the binaries probably
won't run on Android phones. Unfortunately, there are technical issues that
make it impossible to link these programs statically.

The binaries were built in 03-15-2016 from a snapshot of the Android source
repository. To the best of my knowledge, this is equivalent to version 1.0.35+
