# Device Changelog's
* Device changelogs related with Redmi Note 7 builds available by me;

## Redmi Note 7 - Lavender

### Device Tree - 25/08/2025

- device: More and more;
- device: Tune cpuset configs;
- device: Tune powerhint performace;
- device: Decrease GPU default min freq;
- device: Improved task_profiles performance;
- device: Improved phase offset sf durations;

### Device Tree - 05/08/2025

- device: Switch to sm8150 display hals (Thanks to [wHoEMi](https://github.com/wHo-EM-i));
- device: Partially update display blobs from Nabu;
- device: Add support for FIXED_PERFORMANCE power hints;

### Device Tree - 12/07/2025

- device: More and more;
- device: Dropped IPictureAdjustment from livedisplay (Buggy since we switch to aosp colors managment);
- device: Improved display performance;
- device: Fixed LMOFreeform related problems;
- device: Properly enable charging control configuration;
- device: Drop legacy ANT remnants;
- device: Cgroups_v2 and task_profiles improvements;

### Device Tree - 12/06/2025

- device: More and more;
- device: Reorganize device specific flags (I'm not gonna support another devices anyway...);
- device: Stop copying libhidlbase-v32;
- device: Build com.fingerprints.extension@2.0 lib from source;
- device: Set vendor init lib via soong config;
- device: Comunize cnss-daemon, libmmcamera_dbg;
- device: Migrate away from TARGET_RECOVERY_DEVICE_MODULES;
- device: Switch to FBE v2;
- device: Build keymaster 4.1 HAL;
- device: Switch to sony dolby implementation;
- device: sepolicy: Remove duplicate /dev/lirc0 label;
- device: Update Gps stack from LA.UM.12.2.1.r1-04300-sdm660.0;
- device: Switch to QTI Memtrack AIDL HAL;
- device: Patch soname of required libraries;
- device: Set TARGET_ENFORCES_QSSI (We now use last available display/audio/media sdm660 tags);
- device: Update all blobs including some device speficic from Zebra/helios/helios:14/14-23-05.00-UG-U05-STD-HEL-04/5:user/release-keys and LA.QSSI.15.0.r1-14500-qssi.0;
- device: Don't explicitly build qcom.fmradio;
- device: Kill all BUILD_BROKEN_* flags;
- device: Drop BOARD_VNDK_VERSION;
- device: Implement ELF checks & swap to python extract;
- device: Libraries are now automatically added to PRODUCT_PACKAGES;
- device: Migrate mount point creation out of Android.mk;
- device: Update boot-image-profile.txt path for A15 QPR2;
- device: tetheroffload: Version 1.1;
- device: sepolicy: Fix mlipayd file context;
- device: Cleanup dead targets;
- device: Disable UFFD GC via OVERRIDE_ENABLE_UFFD_GC;
- device: Cleanup init.qcom.post_boot;
- device: Disable SF backpressure;
- device: Enable slow-cpu media_codecs;
- device: Enable HWUI with PerformanceHintManager;
- device: Boost TASchedtuneBoost interaction hint;
- device: Disable async MTE for specific apps;
- device: Set threshold for filtering unused apps via dexopt;
- device: Set logging tags to suppress verbose logs;
- device: Disable GPU acceleration in system_server;
- device: Enable socket disable and compactvdex;
- device: Disable Idle timeout;
- device: Configure EGL multi-file cache;
- device: Disable debug.sf.recomputecrop;
- device: Disable surfaceflinger prime shader cache;
- device: Set debug.sf.layer_caching_active_layer_timeout_ms to 1000;
- device: Optimize dex2oat configuration for performance;
- device: ...

### Kernel - 25/08/2025

- Merged EishinNull[Wake]-R1.1.106 release (4.19-st7 cip);
- Added more touchscreen drivers;
- Switched to qpnp wled driver for lcd-backlight;

### Kernel - 05/08/2025

- Backported SUSFS 1.5.9 (Thanks to [sidex15](https://github.com/sidex15)); 
- Updated KernelSU-Next to 1.0.9;

### Kernel - 12/06/2025

- Updated to Radiethselunaris-r1.1.105-eol as base from [here](https://github.com/user-why-red/android_kernel_xiaomi_sdm660_419), credits go to [Santhosh](https://github.com/user-why-red)
- Line up/reverted some changes to match our priorities;
- Added back my personal modifications over it;
- Implemented KernelSU-Next 1.0.6 + SUSFS 1.5.5;