# Device Changelog's
* Device changelogs related with Redmi Note 7 builds available by me;

## Redmi Note 7 - Lavender

### Device Tree - 25/08/2024

- device: Build libutils.vendor;
- device: Implemented a common section for all xiaomi parts;
- device: Update dolby atmos from Motorola Moto G52;
- device: Tune cpuset;
- device: audio: Update policy config;
- device: fstab: Add back f2fs optional support (We do not support inline f2fs encryption on our 4.4 baseline);
- device: fstab: Bring back 'quota' option;
- device: fstab: Properly set avb;
- device: dimens: Define start/end of status bar padding;

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
- device: Tweak surfaceflinger work durations;

### Device Tree - 16/04/2024

- gps: Don't include cutils/threads.h;
- device: Add BUILD_BROKEN_INCORRECT_PARTITION_IMAGES;
- device: Switch back to WiFi AIDL;
- parts: Migrate to CompoundButton.OnCheckedChangeListener;
- parts: Convert to SwitchPreferenceCompat;
- parts: Bring back Collapsingtoolbar again;
- power-libperfmgr: Sync with xiaomi aidl power;
- qcom-caf: audio: Resolve symbol duplication issues in the audio.primary.sdm660 module;
- device: Update Time Services, ANT+, Bluetooth, DRM (SEE, TUI, Widevine), Alarm blobs from Fairphone3;
- device: Update CNE, DPM, IMS, QMI, RIL blobs from LA.QSSI.14.0.r1-12000-qssi.0;
- device: Update CNE, DPM, IMS, QMI, RIL blobs and GPS blobs from Zebra TC57;
- libqti-perfd-client: Clean up;
- device: Improve zram init process;
- device: Enable ZRAM deduplication feature;
- device: Store TaskSnapshot in 16 bit pixel format to save memory;
- overlay: Improve pinner configuration;
- rootdir: Fix the battery drain due to statsd;
- device: Move some vendor props to system;

### Device Tree - 06/03/2024

- parts: Add Kcal support and refactor to our implementation
- overlay: Disable Now Playing Components;
- rootdir: Configure zram on fstab and switch to a fixed common size;
- device: Build Lineage Health Hal and adress it denials;
- overlay: Allow seamless Doze state transitions;
- device: Fixed sensor build and drop 32 bits version;
- device: Add AOSP audio policy engine configs to fixup some related denials;
- device: Switch CPU variant to Cortex-A73;
- audio: Set valid and supported channel mask for earpiece;
- audio: Offload 24 bits playback supports mp3/aac format;
- powerhint: Fix some denial's and reset some power hints only after boot it's complete;
- device: Optimized reserved space size on partitions;
- device: Build OMX HIDL HAL after deprecate 32-bit apps;
- device: Messed again with LMKD optimization;
- ...

### Device Tree - 01/01/2024

- Disable frame rate override feature;
- Sort out display props;
- parts: Target current sdk;
- parts: Get rid of HelpDialogFragment class;
- parts: Add an exported flag in manifest;

### Device Tree - 01/12/2023

- Disable backpressure;
- Don't cleanup resources due to rendering a prior frame;

### Device Tree - 24/11/2023

- Switch to two-stage init mounting;
- Releasetools: Include/flash DTBO image;
- Use logdump as metadata partition;
- Retrofit dynamic partitions;
- Reserve some space for partitions;

### Device Tree - 17/11/2023

- Import libnotifyaudiohal from lavender;
- Patched fingerprint blobs to workaround the removal of gBn/sConstructorMap;
- Patched camera blobs to fullify new aosp request's on linkerconfig;
- Decprecate SAR...
- Remove activity_recognition libs;
- Migrate to AIDL ClearKey DRM HAL;
- Move to QTI health AIDL service;
- Build android.hardware.bluetooth.audio-impl;
- Disable sound trigger support completly;
- Import deviceInfoServiceModule from Sweet;
- Set userspace lmk properties;
- Disable memcg kernel and socket accounting;
- Switch to legacy WiFi HIDL HAL;
- Build mlipay@1.0 interface;
- Follow qssi default behaviour and disable auto_latch_unsignaled property to keep latch-unsignaled working as intend;
- Improve SF durations;
- Force pre-5.10 devices to treat 170M as sRGB in SF;
- Satisfy EPPE enforcement;
- Remove duplicate SIP+VoIP permission;
- Update CarrierConfig from LA.UM.10.2.1.r1-04000-sdm660.0;
- Properly label /sys/kernel/qvr_external_sensor/fd;
- Update AIDL Pixel PowerHAL for Android 13/14;
- Suppress imsdatadaemon denials;
- Move init.recovery.qcom.rc out of root;
- Update mlipay from lavender V12.5.7.0.QFGCNXM;
- Build mtdservice interface lib from source;
- Drop useless thermal profile service;
- Drop hidl power stats mock;
- Use bluetooth.audio@2.1;
- Reorder and cleanup device tree makefiles;
- Switch to source-built mlipay interface;
- Update CNE, DPM, IMS, QMI, RIL blobs from LA.QSSI.13.0.r1-09700-qssi.0;
- Build android.hardware.bluetooth@1.0;
- Label goodix fingerprint interfaces;
- Label location SELinux find denial;
- Ship prebuilt libprotobuf-cpp from v29 VNDK;
- Explicitly disable AVB;
- Kang peripheral manager from caymanslm;
- Raise VINTF target level to 4;
- Replace isolated_app with isolated_app_all;
- Fix gps, display, media and audio hals build as needed by clang on Android 14;

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

