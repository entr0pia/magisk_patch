# Magisk Boot Image Patcher

Forked from [topjohnwu/Magisk:/scripts](https://github.com/topjohnwu/Magisk/tree/v25.2/scripts), Magisk v25.2


## Usage
```shell
boot_patch.sh <bootimage>
```

## Environment variables
- KEEPVERITY
- KEEPFORCEENCRYPT
- RECOVERYMODE


## This script should be placed in a directory with the following files

| File name         | Type   | Description                                                                  |
| ----------------- | ------ | ---------------------------------------------------------------------------- |
| boot_patch.sh     | script | A script to patch boot image for Magisk                                      |
| util_functions.sh | script | A script which hosts all functions required for this script to work properly |
| magiskinit        | binary | The binary to replace /init                                                  |
| magisk(32/64)     | binary | The magisk binaries                                                          |
| magiskboot        | binary | A tool to manipulate boot images                                             |
| chromeos          | folder | This folder includes the utility and keys to sign                            |
