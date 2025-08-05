# Device Changelog's
* Device changelogs related with Redmi Note 7 builds available by me;

## Redmi Note 7 - Lavender

### Device Tree - 05/08/2025

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
- device: Migrate away from TARGET_RECOVERY_DEVICE_MODULES;
- device: Switch to sony dolby implementation;
- device: sepolicy: Remove duplicate /dev/lirc0 label;
- device: Update Gps stack from LA.UM.12.2.1.r1-04300-sdm660.0;
- device: Switch to QTI Memtrack AIDL HAL;
- device: Patch unresolved symbols of vulkan.sdm660;
- device: Patch soname of required libraries;
- device: Updated DRM, SSE, TUI from Fairphone/FP3/FP3:13/6.A.023.1/gms-497e9bef:user/release-keys
- device: Updated CNE, DPM, IMS, QMI, RIL, ANT, Charger, GPS, FM, Peripheral, Alarm, Soter, TimeServices, Bluetooth from Zebra/helios/helios:14/14-23-05.00-UG-U05-STD-HEL-04/5:user/release-keys and LA.QSSI.15.0.r1-14500-qssi.0;
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

### Kernel - 05/08/205

- More bpf backport's;
- Updated KernelSU-Next to 1.0.9;
- Qcom power adjustments;

### Kernel - 27/12/2024

- More bpf backport's;
- Switch to KernelSU-Next;
- Misc improvements under scheduler;

### Kernel - 01/01/2024

- Merge some changes/backports from msm8998;

### Kernel - 24/11/2023

- Adapt for retrofit dynamic partitions;

### Kernel - 17/11/2023

- We are now using Nexus Kernel as base from [here](https://github.com/projects-nexus/nexus_kernel_xiaomi_lavender), credits go to [Prashant](https://github.com/Prashant-1695)
- Implement KernelSU support;
- Merge A14 clang changes;
- Avoid problems around BPF properties;
- Switched to userspace LMK;

