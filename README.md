# ProjectK #
---
ProjectK is a kernel based on CAF 3.18 kernel source with linux-stable merged in comingout with bunch of a features for MSM893.
---

## Release Notes ##
-------------------------------
* [RELEASE NOTES PROJECTK] (https://github.com/khusika/projectk_kernel_xiaomi_msm8953/releases)

## How To Build ##
-------------------------------

For Tissot:

    export CROSS_COMPILE=YOUR TOOLCHAIN && export ARCH=arm64 && make tissot_defconfig && make -j(# of cores)

For Mido:

    export CROSS_COMPILE=YOUR TOOLCHAIN && export ARCH=arm64 && make mido_defconfig && make -j(# of cores)

## Supported Devices
-------------------------------

| DEVICE                         |
| :----------------------------- |
| Mi A1 (Tissot)                 |
| Redmi Note 4 Snapdragon (Mido) |

## Features ##
-------------------------------

* Linux version 3.18.105
* CAF Tag LA.UM.6.6.r1-07200-89xx.0
* CPU Governors: relaxed, chill, electron, impulse, zzmoove, alucard, darkness, nightmare, yankactive, intelliactive, blu_active, interactive, conservative, ondemand, powersave, performance, userspace
* CPU Hotplugs: autosmp, alucard_hotplug, thunderplug, blu_plug, msm_hotplug, intelli_plug, lazyplug
* I/O Schedulers: noop, deadline, cfq, zen, fiops, sio, maple, bfq
* Live Display Driver
* Native DT2W support
* WireGuard VPN support
* Frandom
* KCAL colour control
* Sound Control
* Vibration Intensity Control
* Boeffla wakelock blocker
* exFAT & NTFS Support
* Better performance
* CRC & SHA256 crypto algorithms
* Blocked many wakelocks
* HZ 300
* Removed safetynet flags (no need of magisk to bypass safteynet)
* Improved zRAM with lz4 compression
* Tweaked Westwood TCP Congestion set as default
* Fingerprint sensor boost driver
* Qnovo charging driver for maintaining temperature
* USB Fastcharge 2000mA
* Intellithermal v3.1 Driver
* Support PowerSuspend
* Adreno idler
* for more info check my [commits] (https://github.com/khusika/projectk_kernel_xiaomi_msm8953/commits/projectk)
