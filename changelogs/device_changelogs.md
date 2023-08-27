# Device Changelog's
* Device changelogs related with Redmi Note 7 builds available by me;

## Redmi Note 7 - Lavender

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
