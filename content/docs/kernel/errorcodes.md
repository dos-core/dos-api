---
title: DOS error codes
type: docs
prev: docs/kernel/
next: docs/kernel/mbr
---
| hex | dec | minver   | description
|----:|----:|:---------|:-----------
| 00h |   0 |          | success (no error)
| 01h |   1 |          | function number invalid
| 02h |   2 |          | file not found
...
| 12h |  18 |          | no more files
|     |     | --- DOS 3+ ---
| 13h |  19 | DOS 3+   | disk write protected
| 14h |  20 | DOS 3+   | unknown unit
...
| 24h |  36 | DOS 3+   | sharing buffer overflow
| 25h |  37 | DOS 4+   | code page mismatch
| 26h |  38 | DOS 4+   | unable to complete file operation (no input)
| 27h |  39 | DOS 4+   | insufficient disk space
| 28h |     |          | reserved
| 29h |     |          | reserved
| 2Ah |     |          | reserved
| 2Bh |     |          | reserved
| 2Ch |     |          | reserved
| 2Dh |     |          | reserved
| 2Eh |     |          | reserved
| 2Fh |     |          | reserved
| 30h |     |          | reserved
| 31h |     |          | reserved
| 32h |  50 | DOS 3+   | network request not supported
...
| 4Fh |  79 |          | reserved
| 50h |  80 | DOS 3+   | file exists
| 51h |  81 |          | reserved
| 52h |  82 | DOS 3+   | cannot make directory
| 53h |  83 | DOS 3+   | fail on Int 24h
| 54h |  84 | DOS 3.3+ | too many redirections
...
| 59h |  89 | DOS 4+   | function not supported on network
| 5Ah |  90 | DOS 4+   | required component not installed

64h (100) starts MSCDEX error codes
