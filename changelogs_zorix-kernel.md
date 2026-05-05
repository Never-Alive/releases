## Changelogs
**v1.0 - 5/5/2026**
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
