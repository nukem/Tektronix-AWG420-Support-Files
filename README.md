# Tektronix-AWG420-Support-Files
Files to restore AWG420 boot drive and storage drive

## Boot Drive Setup
Any 44pin 5V IDE drive can be used as the boot drive.

Format the drive as FAT16 or FAT32 and make the primary partition active so it can be booted by the BIOS.

Use **VXSYS.EXE** to install a bootloader that can load bootrom.sys

Usage:
```
VXSYS.EXE <drive_letter>
```

VXSYS code can be found here: https://github.com/tpunix/vxworks-project/tree/master/vxsys
