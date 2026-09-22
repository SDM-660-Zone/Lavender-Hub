# Device Changelog's
* Device changelogs related with Redmi Note 7 builds available by me;

## Redmi Note 7 - Lavender

### Device Tree - 18/09/2026

- device: Enable HWUI render-ahead;
- device: libperfmgr: Fix sysfs labels and permissions;
- device: sepolicy: Allow libperfmgr write to gpu/devfreq nodes;
- device: Properly arrange media codec configuration;
- device: Set ro.config.small_battery to true;
- device: Disable machine learning on product partition;
- device: Tune LMKD for improved memory management;
- device: Switch to lineage fork of displayservice HIDL;
- device: Drop HIDL Bluetooth Audio 2.1 implementation;
- device: Update blobs from LA.QSSI.17.0.r1-06700-qssi.0;

### Device Tree - 01/09/2026

- device: Tuned HWUI scaling for improved rendering performance;
- device: Updated Skia tracing properties for newer Android versions;
- device: Added SELinux permissions for system apps to read KGSL GPU information;
- device: Completed Lineage Health integration for battery charging control;
- device: Added torch strength control;
- device: Switched performance tuning from schedtune to UClamp;
- device: Updated the - kernel BPF version override to 5.10.239;
- device: Restored graphics acceleration by reverting ro.config.avoid_gfx_accel;
- device: Switched to the AIDL Camera HAL;
- device: Moved SPU NVM directory creation to an earlier boot stage;
- device: Fixed seccomp policy for the IMS RTP service;
- device: Replaced deprecated writepid cgroup migration with task profiles;
- device: Adjusted USB 2.0 UVC bandwidth for more reliable webcam output;
- device: Fixed DeviceAsWebcam color handling on Qualcomm hardware;
- device: Enabled USB UVC webcam support;
- device: Added MHI diagnostic pipe permissions;
- device: Updated proprietary blobs from Zebra/helios/helios:14/14-32-12.00-UG-U03-STD-HEL-04/21:user/release-keys and LA.QSSI.16.0.r1-06700-qssi.0;
- device: Tuned SurfaceFlinger timers, frame scheduling and HWUI memory behavior for smoother UI performance;
- device: Restored SurfaceFlinger client composition caching to reduce UI jank;
- device: Enabled ADPF CPU hints for improved UI responsiveness and frame pacing;
- device: Increased GPU minimum frequency during expensive rendering workloads;
- device: Tuned LMKD for improved memory management, multitasking and responsiveness;
- device: Tuned power hints and scheduler behavior;
- device: Improved expensive rendering handling by preventing interaction hints from reducing performance during blur and other heavy rendering workloads;
- device: Updated task profiles with newer Android process-group features;
- device: Restored normal statsd behavior;
- device: Updated Soong configuration variables to use boolean types where appropriate;
- device: Removed duplicated SELinux wakeup node definitions;
- device: Set the default pinned memory amount for the home application;
- device: Disabled high-performance transition mode;
- device: Reduced Bluetooth log spam;
- device: Fixed SELinux denials for the Qualcomm USB HAL;
- device: Fixed Qualcomm Wi-Fi Display media target variant property handling;
- device: Properly switched USB audio to the AOSP USB Audio HAL v2;
- device: Removed deprecated Bluetooth A2DP input audio configurations;
- device: Added the IPSEC_TUNNEL_MIGRATION feature using XFRM migration support;
- device: Enabled UFFD garbage collection support;


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

### Kernel - 01/09/2026

- kernel: Updated to SouthWest-NG as base from [here](https://github.com/pix106/android_kernel_xiaomi_sdm660_southwest-ng), credits go to [pix106](https://github.com/pix106)
- kernel: ...;
- kernel: Fixed NoMount compatibility with GNU89 - kernel build rules;
- kernel: Added NoMount v2.0.0 with hookless and lockless fast-path lookup support;
- kernel: Added SUSFS v2.2.0 support;
- kernel: Imported KernelSU v3.3.0 + 97;
- kernel: Improved Novatek touchscreen recovery from I2C errors to prevent system freezes and watchdog reboots;
- kernel: Improved alarmtimer handling to prevent userspace wakeup alarms from blocking suspend;
- kernel: Fixed ICNSS power management to prevent suspend failures and related log spam;
- kernel: Improved UART suspend handling to restore reliable deep sleep;
- kernel: Cleaned up FPC1020 fingerprint driver logging;
- kernel: Fixed fingerprint sensor wakeup and power management during deep sleep;
- kernel: Improved SDIO power management for better deep sleep;
- kernel: Improved filesystem performance by enabling NOATIME and NODIRATIME by default;
- kernel: Updated process tampering blacklist;
- kernel: Added Power HAL and IOP processes to the tampering blacklist;
- kernel: Added centralized protection against userspace processes tampering with - kernel-controlled performance nodes;
- kernel: Prevented Google Camera from consuming CPU and battery while running in the background;
- kernel: Tuned memory pressure handling for improved multitasking on 3/4 GB RAM devices;
- kernel: Removed unused camera focus and snapshot GPIO keys;
- kernel: Improved wakeup interrupt handling by replacing IRQF_NO_SUSPEND with proper IRQ wake support;
- kernel: Enabled the CPU-to-memory bandwidth governor for PowerHAL performance hints;
- kernel: Enabled IFB and IPv6 GRE networking support;
- kernel: Switched the - kernel timer frequency to 300 Hz;
- kernel: Enabled BBR, FQ_CODEL and FQ networking support;
- kernel: Added the missing SLIMbus audio flag required for proper Lavender DTBO boot;

### Kernel - 25/08/2025

- Merged EishinNull[Wake]-R1.1.106 release (4.19-st7 cip);
- Added more touchscreen drivers;
- Switched to qpnp wled driver for lcd-backlight;

### Kernel - 05/08/2025

- Backported SUSFS 1.5.9 (Thanks to [sidex15](https://github.com/sidex15)); 
- Updated - kernelSU-Next to 1.0.9;

### Kernel - 12/06/2025

- Updated to Radiethselunaris-r1.1.105-eol as base from [here](https://github.com/user-why-red/android_kernel_xiaomi_sdm660_419), credits go to [Santhosh](https://github.com/user-why-red)
- Line up/reverted some changes to match our priorities;
- Added back my personal modifications over it;
- Implemented - kernelSU-Next 1.0.6 + SUSFS 1.5.5;