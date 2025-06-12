# Device Changelog's
* Device changelogs related with Redmi Note 7 builds available by me;

## Redmi Note 7 - Lavender

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


### Kernel - 12/06/2025

- Updated to Radiethselunaris-r1.1.105-eol as base from [here](https://github.com/user-why-red/android_kernel_xiaomi_sdm660_419), credits go to [Santhosh](https://github.com/user-why-red)
- Line up/reverted some changes to match our priorities;
- Added back my personal modifications over it;
- Implemented KernelSU-Next 1.0.6 + SUSFS 1.5.5;