---
title: Documentation
next: first-page
---
## Overview:

Microsoft Disk Operating System (MS-DOS/PC-DOS) API was designed for use by assembly programs but is often wrapped for usage with a compatible C/C++ compiler.  DOS API is invoked from an 8086+ compatible processer in 'real' mode (a 16 bit mode where memory is identity mapped and accessed by 64KB segments and offsets).  The DOS API is versioned based on the release of Microsoft MS-DOS (or IBM PC-DOS) a given API was added or updated.  Unless otherwise indicated this site documents latest version of API, roughly DOS 6.x/7.x interfaces with differences between FAT32 enabled versions and other advanced functionality (e.g. long file names LFNs) annotated.  Most DOS API functionality was implemented by MS/PC DOS 3.x line.  Corresponding core files provided may have varying levels of support.  Thanks to its Open Source release by Microsoft, MS/PC DOS 4 is the minimal supported version available.  For more advanced support, the FreeDOS kernel, RxDOS kernel, and EDR-DOS (Enhanced DR-DOS) kernels are available.  4DOS is provided as the primary command shell, though FreeCOM and other COMMAND.COM shells may be provided along with their associated API extensions.  Additional APIs provided by core* drivers such as SHARE, SETVER/CALLVER, etc. are also documented (* i.e. tightly bound to specific kernel, generally any modules within FreeDOS kernel repository). 

## Structures:
### MBR/GPT partition table - Master Boot Record / Guid Partition Table
Note: GPT is generally not supported by DOSes
### BPB/boot sector - BIOS Parameter Block
This is also referred to a Volume Boot Record (VBR), see MBR for primary boot sector and sharing/spliting hard drive storage.
### DPB - Disk Parameter Block
### CDS - Current Directory Structure
### LOL/... - List of Lists / ...
### MCB - Memory Control Blocks
### FAT - File Allocation Table
See corresponding specifications - FAT12/FAT16/FAT32/exFAT
### SFN/LFN dirent - short and long filename directory entries

## DOS Interrupts 
### int 20h - exit program
### int 21h - main interface
### int 2Fh - internal and multiplex interfaces
### int 2Eh - TSR/multiplex interface
### int 25/26h - absolute read/write disk sectors

## BIOS/Other Common Interrupts
### int 10h - video
### int 15h - BIOS extensions
### ...

## Example DOS program - Hello, World!

```c {filename="main.c"}
#include<stdlib.h>
#include<stdio.h>

int main(void) {
    printf("Hello, World!");
    return 0;
}
```
