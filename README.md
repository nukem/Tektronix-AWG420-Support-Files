# Tektronix-AWG420-Support-Files
Files to restore AWG420 boot drive and storage drive

## Boot Drive Setup
Any 44pin 5V IDE drive can be used as the boot drive.

Format the drive as FAT16 or FAT32 and make the primary partition active so it can be booted by the BIOS.

The following needs to be done on a DOS environment.  You can use FreeDOS to create a bootable HD or Floppy and use the AWG to do everything if you attach a keyboard on the internal keyboard socket.  The external keyboard connector will not work since it is connected to a serial port.

Use **VXSYS.EXE** to install a bootloader that can load bootrom.sys

Usage:
```
VXSYS.EXE <drive_letter>
```

VXSYS code can be found here: https://github.com/tpunix/vxworks-project/tree/master/vxsys

After installing the bootloader you can copy all the files from the **[boot_drive](https://github.com/nukem/Tektronix-AWG420-Support-Files/tree/main/boot_drive)** folder and the system will boot.
