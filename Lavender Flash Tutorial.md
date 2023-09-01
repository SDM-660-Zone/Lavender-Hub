# Lavender Flash Tutorial
* We are switching for a 4.19 baseline;
* Recovery internal data its encrypted and cannot be decrypted yet (Fbev2)
* Im not gonna provide any decrypted roms, don't even ask;

## Getting Started

### Clean flash

```
1. Wipe system, data, vendor, cache, dalvik, metadata;
2. Format data;
3. Install 4.19 recovery (provided on this repo);
4. Enter manage partitions on ofox configs, change Data & Cache partitions file system to F2FS;
5. Install rom;
5.1. Install your gapps package or other stuff if you are gonna need it later, remember recovery will not be decrypted, otherwise use a SDCard or USB OTG;
6. Reboot to system;
```

### Dirty flash 
```
1. Download rom update;
2. Reboot to recovery;
3. Enter on menu, connect your phone with pc and choose ADB & Sideload;
4. Execute adb sideload <rom package filename>.zip;
4.1. Or if you have a SD card, you can put the rom package into the SD card and flash it on recovery directly instead of using adb sideload;
5. Wipe cache and dalvik;
6. Reboot to system and voila!
```
