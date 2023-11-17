# Device Changelog's
* Device changelogs related with Redmi Note 7 builds available by me;

## Redmi Note 7 - Lavender

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


### Kernel - 17/11/2023

- We are now using Nexus Kernel as base from [here](https://github.com/projects-nexus/nexus_kernel_xiaomi_lavender), credits go to [Prashant](https://github.com/Prashant-1695)
- Implement KernelSU support;
- Merge A14 clang changes;
- Avoid problems around BPF properties;
- Switched to userspace LMK;

