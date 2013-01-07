BIOS Boot Partition
===================

This is the BBO bootcode that get's loaded by MBR.

File list
---------

* boot.asm - main BBP entry code
* kmain.c - C entry point that get's called by boot.asm
* main.asm - Assembly routines for kmain.c (here we'll put all the stuff that's not possible in C)
* bbp.ld - BBP linker script
* makefile - Make build script
* buildimg.bat - Bach script to merge MBR and BBP code into Bochs disk image file using DiskUtils
* bbp.vcxproj - Visual Studio 2010 project file


Requirements
------------

* MinGW Cross-compiler that's capable of building ELF files. See how to build one here: http://gusc.lv/2012/12/myos-mingw-cross-compiler/
* Netwide Assembler from: http://www.nasm.us/
* DiskUtils from: https://github.com/gusc/diskutils
* Microsoft Visual Studio Express 2010