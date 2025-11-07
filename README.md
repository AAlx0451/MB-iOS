## Minimal iOS 6

Chroot container with iOS 6 *really* clean enviroment. Just 9,7 MiB! (and 1.4 MiB zipped!)

## How to run it

Prereq: iOS 6 device with JB

1. cd MB-iOS
2. chroot .
3. enjoy!

You can install additional files from iOS 6.1 SDK. 

## What's included

1. dyld, libSystem, libc++abi, libobjc, libstdc++, some system libs, ~libgcc~
2. ~Debian `dash`~ Open Korn Shell

## example. just a joke 

```
/private/var/MB-iOS # chroot .
# ls
/bin/sh: 1: ls: not found
# whoami
/bin/sh: 2: whoami: not found
# exit
/private/var/MB-iOS #
```

## Changelog

Removed libgcc_s. Removed dash. Now we use oksh with only libSystem depend

Now you can run MBiOS with `make`. Just because I could add it. Why not?
