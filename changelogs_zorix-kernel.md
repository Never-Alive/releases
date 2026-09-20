# Changelogs

## v2.0 - 20/9/2026

> **Since 2.0 is full rebase many changes of v1.0 are missing**

* Rebased kernel on CLO tag `LA.UM.9.14.1.r1-21100-QCM6490.QISI15.0`
* Import qcacld-3.0 from CLO tag `LA.UM.9.14.1.r1-21100-QCM6490.QISI15.0`
* Import fw-api from CLO tag `LA.UM.9.14.1.r1-21100-QCM6490.QISI15.0`
* Import qca-wifi-host-cmn from CLO tag `LA.UM.9.14.1.r1-21100-QCM6490.QISI15.0`
* Import datarmnet from CLO tag `LA.UM.9.14.1.r1-21100-QCM6490.QISI15.0`
* Import dataipa from CLO tag `LA.UM.9.14.1.r1-21100-QCM6490.QISI15.0`
* Import display-drivers from CLO tag `LA.UM.9.14.1.r1-21100-QCM6490.QISI15.0`
* Import camera-kernel from CLO tag `LA.UM.9.14.1.r1-21100-QCM6490.QISI15.0`
* Import audio-kernel from CLO tag `LA.UM.9.14.1.r1-21100-QCM6490.QISI15.0`
* Import video-driver from CLO tag `LA.UM.9.14.1.r1-21100-QCM6490.QISI15.0`
* Import OEM changes for THERMAL from `haydn-r-oss`
* Import OEM changes for USB, IR, POWER from `venus-r-oss`
* Import OEM changes for techpack/audio from `redwood-s-oss`
* Import TOUCHSCREEN driver and OEM changes for haptics from `zijin-s-oss`
* Import FPC FP driver from `psyche-r-oss`
* Remove display ramdump memory region
* Disable coresight and DCC driver
* Supress verbose output during boot
* Step down reglulator for GPU freq `<379mhz>` && `<315mhz>` by 1
* Add GPU `<150mhz>` step with regulator `RPMH_REGULATOR_LEVEL_MIN_SVS` for better idle drain
* Optimise Energy Model
* Disable debugging for QCACLD even more and optimised for size
* Use 100hz for ticking
* Backported ZSTD algorithm `v1.5.6` and make it default algo
* Apply optimizations from Samsung to ZSTD
* Switched to `<KernelSU>` Updated ksu to `v32663`
* Disable useless driver and debloat defconfig
* Disable AUDIT, Tracing
* Debloated FP driver by removing unnecessary stuff and reducing wakelock hold to 400ms
* Mount Firmware correctly
* Stop I/O Stats and compile out debugging
* Fix memory leaks in camera
* Use `-O3` globally
* Disabled watchdog, gki stuff
* Disable unwanted Security stuff for performance imporvement
* Upstream dtc to `v1.7.0-93`
* Build only reequired dts for haydn
* Disable YUPIK/SHIMA/SUNXI/HISI arch(s)
* Merge `5.10-bpfs` into kernel
* Backport `FUSE` into kernel
* Optimise POWER supply to improve charging speed
* Compile out debugging for POWER
* Implemented SMLK again with some chnages
* Cleanup ION
* Set idle state correcly
* Swiched to Neutron Clang 24

---

## v1.0 - 5/5/2026

* Merge clo tag `LA.UM.9.14.r1-26700-LAHAINA.QSSI16.0` into audio.
* Merge clo tag `LA.UM.9.14.r1-26700-LAHAINA.QSSI16.0` into dataipa.
* Merge clo tag `LA.UM.9.14.r1-26700-LAHAINA.QSSI16.0` into camera.
* Merge clo tag `LA.UM.9.14.r1-26700-LAHAINA.QSSI16.0` into video.
* Merge clo tag `LA.UM.9.14.r1-26700-LAHAINA.QSSI16.0` into qcacld-3.0.
* Merge clo tag `LA.UM.9.14.r1-26700-LAHAINA.QSSI16.0` into qca-wifi-host-cmn.
* Merge clo tag `LA.UM.9.14.r1-26700-LAHAINA.QSSI16.0` into fw-api.
* Debloat WiFi drivers.
* Debloat defconfig and disable unnecessary stuff.
* Hardened the kernel.
* Introduced `SBalance` and make it poll every 20sec.
* Debloat techpack.
* Set correct idle node for our `CMD` display.
* Use O3 optimization level for Clang and perf.
* Optimise small cluster `cortex-55` by clang.
* Wake GPU upon receiving ioctl.
* Fix frequency calculation for high refresh rate.
* Set `GPU idle timeout` to 58ms.
* Remove `legacy low power states` for gpu.
* Enable power efficient workloads.
* Hardcoded the zRam to `4GB`.
* Hardcoded swappiness to `80%`.
* Reduce polling interval for devfreq.
* Reduce ntp wakeups.
* Diable `CONFIG_DEBUG_KERNEL`.
* Guard debug code with `CONFIG_DEBUG_KERNEL` condition.
* Disable STATS for `I/O` completely.
* Disable STATS for `THERMALS`.
* Fix some warnings.
* Enable polyhedral loops.
* Enable LD_DEAD_CODE_DATA_ELIMINATION.
* Hardcode for `a660 & a624L`.
* Disable `CORESIGHT` `SNAPSHOT` `TRACING` for adreno.
* Disable TRACING in defconfig.
* Remove TRACING for {f2fs and ext4}.
* Silence `no longer affine to cpu` logspam for {irq,sched}.
* Stop `libperfmgr` spamming by spoofing.
* Enter wfi state instead of polling during active migration.
* Disable `IPC_LOGGING`.
* Fix stuff for `unity-based` games.
