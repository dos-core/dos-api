---
title: DOS Kernel
type: docs
prev: docs/
next: docs/kernel/errorcodes
sidebar:
  open: true
---
## DOS error codes:
* [error codes](errorcodes)

## DOS structures:
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


## DOS interrupts:
* [int 20h](int20h) - exit program
* [int 21h](int21h) - main interface
* [int 2Fh](int2Fh) - internal and multiplex interfaces
* [int 2Eh](int2Eh) - TSR/multiplex interface
* [int 25/26h](int2526h) - absolute read/write disk sectors

