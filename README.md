# ProjectK #
-------------------------------
> ProjectK is a kernel based on CAF 3.18 kernel source with linux-stable merged in comingout with bunch of features for MSM8953.

## Info ##
-------------------------------
* [Release Notes](https://github.com/khusika/projectk_kernel_xiaomi_msm8953/releases)
* [AnyKernel2](https://github.com/khusika/AnyKernel2/)

## How To Build ##
-------------------------------

    $ git clone https://github.com/khusika/projectk_kernel_xiaomi_msm8953 -b projectk
    $ cd ~/projectk_kernel_xiaomi_msm8953
    $ export CROSS_COMPILE=YOUR TOOLCHAIN(GCC/LINARO) && export ARCH=arm64 && make (SupportedDevice)_defconfig && make -j(# of cores)

## Supported Devices ##
-------------------------------

| DEVICE                         |      CONFIGS      |  DOWNLOAD LINK  |
| :----------------------------- | :---------------- | :-------------- |
| Mi A1 (Tissot)                 | tissot_defconfig  | [XDA-DEVELOPERS](https://forum.xda-developers.com/mi-a1/development/kernel-projectk-t3771691)  |
| Redmi 5 Plus (Vince)           | mido_defconfig    | COMINGSOON      |
| Redmi Note 4X (Mido)           | COMINGSOON        | COMINGSOON      |
| Redmi 4 Prime (Markw)          | COMINGSOON        | COMINGSOON      |

## Features ##
-------------------------------

* Linux version 3.18.106
* CAF Tag LA.UM.6.6.r1-08300-89xx.0
* CPU Governors: relaxed, chill, electron, impulse, zzmoove, alucard, darkness, nightmare, yankactive, intelliactive, blu_active, **_interactive_**, conservative, ondemand, powersave, performance, userspace
* CPU Hotplugs: autosmp, alucard_hotplug, thunderplug, blu_plug, msm_hotplug, intelli_plug, lazyplug
* I/O Schedulers: noop, deadline, cfq, zen, fiops, sio, maple, bfq
* Live Display Driver
* Native DT2W support
* WireGuard VPN support
* Double Tap to Wake (D2TW)
* Frandom
* KCAL colour control
* Sound Control
* Vibration Intensity Control
* Boeffla wakelock blocker
* exFAT & NTFS Support
* Better performance
* CRC & SHA256 crypto algorithms
* Blocked many wakelocks
* Removed safetynet flags (no need of magisk to bypass safteynet)
* Improved zRAM with lz4 compression
* Tweaked Westwood TCP Congestion set as default
* Fingerprint sensor boost driver
* Qnovo charging driver for maintaining temperature
* USB Fastcharge 2000mA
* Intellithermal v3.1 Driver
* Support PowerSuspend
* Adreno idler
* for more info check my [commits](https://github.com/khusika/projectk_kernel_xiaomi_msm8953/commits/projectk)
