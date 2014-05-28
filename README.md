BasicOS
=======

Simple C kernel with a bootloader.
Allows you to press keys and get them echoed back to screen.

# Prerequisites
You'll need at least ``gcc`` and ``nasm`` to compile and an emulator like ``qemu`` or ``bochs``.
As a debian user, you can just run ``setup.sh`` to install all required packages:

```shell
    cd /path/to/repository
    chmod +x setup.sh
    ./setup.sh
```

# Compiling

```shell
    cd /path/to/repository
    make
```
which will generate a ``kernel.img`` that contains your bootable kernel image, 
along with ``bootloader.bin`` that is the generic bootloader image and ``kernel.bin`` that contains the actual kernel binary.

# Running
The provided ``bochsrc`` file makes Bochs the easiest way to run the kernel:

```shell
    cd /path/to/repository
    bochs
```
You should see something like this:

![](https://lh4.googleusercontent.com/wvP40Viuk1ptT1LuRQGu3_nid-PjlCUFoYIIgA_dx0XkzijOsvGd35Y0NGbk9m3fGLuUWb9szRM_ManFPG-EqdTp35sqTKkFsAdktbT5lDE32du4x1lECzAZ2xToVV-vsLg4)
