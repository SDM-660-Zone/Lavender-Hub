# Device Changelog's
* Device changelogs related with Redmi Note 7 builds available by me;

## Redmi Note 7 - Lavender

### Device Tree - 15/07/2024

- device: Use common libqti-perfd-client and power-libperfmgr;
- device: qcom-caf: media: mm-video-v4l2: Disable OMX_BUFFERFLAG_DECODEONLY support;
- device: Disable the usage of ConfigStore;
- device: Set manifest target-level to 5;
- device: Inherit from QTI and common Xiaomi FCMs;
- device: Include lineage FCM; 
- device: Build missing libraries for 14 QPR3;
- device: Reverted "Set block_binder_thread_on_incoming_calls in product.prop";
- device: Move to new RFS install_symlink targets;
- device: Unset BUILD_BROKEN_INCORRECT_PARTITION_IMAGES;
- device: Declare IMS and EGL libs as symlinks during extraction;
- device: Convert WiFi firmware symlinks to install_symlink targets;
- device: Don't chown DT2W node;
- device: rootdir: Tune LMK;
- device: Enable the backward-compatible memory reduction option;
- device: Import device_framework_matrix from lineage;
- device: media: Remove software omx codec references;
- device: media: Use AOSP default Codec2/OMX ranks;
- device: media: Set higher priority to c2 than OMX;
- device: media: Remove software OMX blobs;
- device: media: Remove media_codecs_google_c2*;
- device: rro_overlays: Drop explicit 'sdk_version' declaration;
- device: Remove vendor RenderScript implementation;
- device: rootdir: Tune our cpuset setup;
- device: Rename property to disable MTE in system_server;
- device: powerhint: Tune powerhint (again!);
- device: powerhint: Add DT2W;
- device: Bring back renderer properties;
- device: Tweak surfaceflinger work durations;
- device: qcom-caf: audio: Fix compilation due to compiler changes;

### Device Tree - 28/05/2024

- device: Adressed a lot of sepolicy denial's;
- bluetooth: Build android.hardware.bluetooth.audio-impl;
- device: Move to QTI health AIDL service;
- device: Migrate to AIDL ClearKey DRM HAL;
- parts: Add an exported flag in manifest;
- parts: Get rid of HelpDialogFragment class;
- parts: Target current sdk;
- parts: Add Kcal support;
- parts: Refactor KCAL Implementation;
- rootdir: Configure zram on fstab;
- device: Build Lineage Health HAL;
- device: Enabled level 1(core) Multi-Gen LRU;
- device: Update CNE, DPM, IMS, QMI, RIL blobs from Zebra/helios/helios:13/13-22-18.00-TG-U02-STD-HEL-04/84:user/release-keys;
- device: libqti-perfd-client: Clean up;
- device: Improve zram init process;
- device: Build Codec2 Packages on vendor;
- configs: Import keylayout and reconfigure it (hopefully screenshots issue may be fixed now);
- properties: Prefer 'cache' backing storage;
- device: Import thermal configs from lavender dt and adapt to 4.19;
- device: Import thermal from Hon660;
- device: Switch to xiaomi common libperfmgr;
- fstab: Add formattable flag for userdata ext4 entry;
- fstab: Prefer ext4 for /cache and /data (f2fs proved to be even slower than ext4 in RW operations);
- fstab: Disable encryption for now (users will annoy me if it isn't);
- device: Retune powerhint;
- device: Sign builds with private releasekeys (Google it's going harder on integrity restrictions);
- A lot more things that I would prefer not to write here (I'm watching!);

### Device Tree - 18/10/2023

- Switch to Wifi service AIDL;
- Fix gps, display, media and audio hals build as needed by clang on Android 14;

### Device Tree - 13/10/2023

- Follow qssi default behaviour and disable auto_latch_unsignaled property to keep latch-unsignaled working as intend;
- Force triple frame buffers;
- Improve SF Phase Offsets;
- Disable HD Logo

### Device Tree - 09/10/2023

- Switch back to schedtune boost
- Drop conflicting wakeup nodes
- Bring back zram in QCOM's init post boot script
- Drop userspace lmk

### Device Tree - 26/09/2023

- Properly label /sys/kernel/qvr_external_sensor/fd
- Fix adm buffering size
- Update CarrierConfig from LA.UM.10.2.1.r1-04000-sdm660.0
- Import QTI datastatusnotification from FP3
- Remove duplicate SIP+VoIP permission
- Decrease battery charging thresholds
- Set userspace lmkd properties
- Satisfy EPPE enforcement
- Force pre-5.10 devices to treat 170M as sRGB in SF
- Extend buffer size to 256kb for offload playback
- Add DPM props
- Compact cached app heaps in the background
- Remove activity_recognition libs

### Device Tree - 30/08/2023

- Set swappiness from kernel side
- Remove zram cold page writeback file
- Write 0 for zs_handle and zspage when configuring zram
- Enable ZRAM deduplication feature
- Decreased zram to a fixed-size of 2gb

### Device Tree - 23/08/2023

- Switched to Pixel Powerhal from android-13.0.0_r3
- Adapted Pixel Powerhal for sdm660 usage
- Updated our powerhint
- Enabled MGLRU configs

### Device Tree - 20/08/2023

- Fixed USB-C Dac
- Fixed adsprpcd logspam
- Fixed some wakelocks
- Suppress imsdatadaemon denials 

### Device Tree - 18/08/2023

- Bring up changes for kernel 4.19
- Adress denial's needed on 4.19
- Switch to source-built mlipay interface
- Move back to Xiaomi power AIDL HAL
- Reorder makefiles respecting alphabetical order
- Move to common IFAAService
- Move to common Xiaomi fingerprint HIDL
- Label FPC/4.19 nodes recursively
- Labeled missing wakeup nodes
- rootdir: Update qcom.post-boot from S62Pro
- Adapt light HAL for k4.19
- Updated media and audio qcom-caf hals from sdm660 tags
- Support new ANT stack
- Set PRODUCT_SET_DEBUGFS_RESTRICTIONS
- Adapt sdm660 powerhint to k4.19
- Adjust msm_irqbalance prio
- Add glink lpass irq to ignored list
- Don't configure zram in QCOM's init post boot script
- Switch to QTI USB 1.3 HAL and fix some vendor/product id
- Switch to FBEv2 emmc optimised encryption
- Update most blobs from Honeywell/hon660 and qssi;
- Update Gps stack from LA.UM.11.2.1.r1-02500-sdm660.0
- Build mtdservice interface lib from source
- Update mlipay from lavender V12.5.7.0.QFGCNXM
- Import HotwordEnrollment from blueline-user 12
- Update rootdir from LA.UM.9.2.1.r1-08000-sdm660.0
- Update most configs from Honeywell/hon660
- Properly disable phantom process killing
- manifest: Add FCM to satisfy vintf check
- Create dummy libldacBT_bco
- Comunize cnss-daemon and thermal
- Switch to two-stage init mounting
- Use emulated storage
- Use logdump as metadata partition
- Include/flash DTBO image
- Much and much more...


### Kernel - 15/07/2024

- Updated to S0NiX-R1.1 as base from [here](https://github.com/ImSpiDy/sonix_kernel_lavender), credits go to [ImSpiDy](https://github.com/ImSpiDy)
- Line up/reverted some changes to match our priorities;
- Added back my personal modifications over it;

### Kernel - 28/05/2024

- Updated to S0NiX-R1 as base from [here](https://github.com/ImSpiDy/sonix_kernel_lavender), credits go to [ImSpiDy](https://github.com/ImSpiDy)

### Kernel - 09/10/2023

- Switched to S0NiX-v3.0-LA.UM.11.2.1.r1-04200 as base from [here](https://github.com/ImSpiDy/kernel_xiaomi_lavender-4.19), credits go to [ImSpiDy](https://github.com/ImSpiDy)

### Kernel - 26/09/2023

- vmscan: Go back to default swapiness level´s
- ion: Limit concurrency of workqueues freeing buffers asynchronously
- defconfig: Enable powersave and userspace cpufreq governor
- defcongif: Disable slmk and enable userspace lmk
- Revert "block: remove legacy IO schedulers"
- defconfig: Enable CFQ Group Scheduling support

### Kernel - 30/08/2023

- ksu: Update ksu version
- Fixed a typo on "Support capture for tas2557 amp"
- vmscan: Reduce swapping aggressiveness to 10

### Kernel - 23/08/2023

- Uclamp task is back
- multi-gen LRU: log when min_ttl is unsatisfied
- multi-gen LRU: export min_ttl unsatisfied counter to sysfs
- multi-gen LRU: set min_ttl to 5000ms by default
- configs: Drop ARMv8.1/v8.2 architectural features
- configs: disable PROCESS_RECLAIM
- configs: Support UAS of usb storage
- configs: Disable media usb bus support
- configs: Disable THERMAL_STATISTICS
- configs: Disable support for ARM64 SVE
- kgsl: Zap performance counters across context switches

### Kernel - 20/08/2023

- We are now using SouthWest Kernel as base from [here](https://github.com/pix106/android_kernel_xiaomi_southwest-4.19), credits go to [Pix106](https://github.com/pix106)
- Enabled Multi-Gen LRU
- Add missing slim_aud flag
- Fix adoptable storage
- Implement KernelSU support
- Merged F2FS upstream
- Switch to CONFIG_SCHED_TUNE
