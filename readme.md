# Magisk Boot Image Patcher

Forked from [topjohnwu/Magisk:/scripts](https://github.com/topjohnwu/Magisk/tree/v26.1/scripts), Magisk v26.1


## Usage
Run it in `adb shell`, and *root* isn't needed.
```shell
boot_patch.sh <bootimage>
```

## Environment variables
- KEEPVERITY
- KEEPFORCEENCRYPT
- PATCHVBMETAFLAG
- RECOVERYMODE
- SYSTEM_ROOT


## This script should be placed in a directory with the following files

| File name         | Type   | Description                                                                                                                |
| ----------------- | ------ | -------------------------------------------------------------------------------------------------------------------------- |
| boot_patch.sh     | script | A script to patch boot image for Magisk. The script will use files in its same directory to complete the patching process. |
| util_functions.sh | script | A script which hosts all functions required for this script to work properly.                                              |
| magiskinit        | binary | The binary to replace /init.                                                                                               |
| magisk(32/64)     | binary | The magisk binaries.                                                                                                       |
| magiskboot        | binary | A tool to manipulate boot images.                                                                                          |
| stub.apk          | binary | The stub Magisk app to embed into ramdisk.                                                                                 |
| chromeos          | folder | This folder includes the utility and keys to sign chromeos boot images. Only used for Pixel C.                             |
