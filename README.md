[![license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENCE)

# MHW MK. Armor

MK. Armor is a Monster Hunter World graphic program to customize the current armor equiped.

It is a C++ implementaion of the original [MHW Transmog](https://www.nexusmods.com/monsterhunterworld/mods/43) MOD based on a decompilation of it.

## State of Development
* Memory reading (working properly).
* Memory writing (working properly).
* GUI Basic Functions (50%).
* GUI Design and vanity (pending...)
* GUI Additional features (pending...)

## Depndencies

* CMake # [Download Link!](https://cmake.org/download/)
* QT5 (Select MinGW 7.30)# [Download Link!](https://www.qt.io/download)
* MinGW 64bits # Currently the only one that works is the one from Msys2, I apologize.
* Msys2 # [Download Link!](http://www.msys2.org/)

### Installation of MinGW using Msys2
* Install Msys2 (I recommend installing it on the root of C: drive)
* Open Msys Command Prompt
``` bash
pacman -Syu # When this update ends it will hang. Close the window, do not Ctrl+C to stop, it will corrupt the installation
pacman -S mingw-w64-x86_64-toolchain
```
* Be sure to add the installation directory which is (C:\msys64\mingw64\bin) to Path (Guide [Info](https://www.computerhope.com/issues/ch000549.htm)).

## Building Using MinGW

Build by making a build directory (i.e. `build/`), run `cmake` in that dir, and then use `mingw32-make` to build the desired target.

``` bash
$ mkdir build && cd build
$ cmake .. -DCMAKE_BUILD_TYPE=[Debug | Release] -G "MinGW Makefiles"
$ mingw32-make
```

## Building Using Visual Studio
Dunno, may be easier.
 




