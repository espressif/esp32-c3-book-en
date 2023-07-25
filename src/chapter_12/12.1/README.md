# ESP32-C3 Power Management

Power management algorithm included in ESP-IDF can adjust the advanced
peripheral bus (APB) frequency, CPU frequency, and put the chip into
Light-sleep mode to run an application at smallest possible power
consumption, given the requirements of application components.
Additionally, the chip automatically enters Light-sleep mode when idle,
reducing the power consumption during application runs. The ESP32-C3's
various low-power modes are discussed in detail in Section 12.2.
Enabling power management features comes at the cost of increased
interrupt latency. Extra latency depends on several factors, such as the
CPU frequency, single/dual core mode, whether frequency switch is
required.

Applications can acquire/release locks to control the power management
algorithm. When an application acquires a lock, the operation of power
management algorithm is restricted. When the lock is released, such
restrictions are removed. Power management locks have acquire/release
counters. If the lock has been acquired a number of times, it needs to
be released the same number of times to remove associated restrictions.

ESP32-C3 supports three types of locks described in Table 12.1.

<p align="center"><i>Table 12.1. Power management locks</i></p>

|Power management lock|Description|
|---------------------|-----------|
|`SP_PM_CPU_FREQ_MAX`|Requests CPU frequency to be at the maximum value set with `esp_pm_configure()`. For ESP32-C3, this value can be set to 80 MHz, 160 MHz, or 240 MHz.|
|`ESP_PM_APB_FREQ_MAX`|Requests the APB frequency to be at the maximum supported value. For ESP32-C3, this is 80 MHz.|
|`ESP_PM_NO_LIGHT_SLEEP`|Disable automatic switching to Light-sleep mode|

Applications can acquire or release power management locks in a way that
can accommodate scenarios where power management is not required. For
example, driver for a peripheral clocked from APB can request the APB
frequency to be set to 80 MHz while the peripheral is used; RTOS can
request the CPU to run at the highest configured frequency while there
are tasks ready to run; A peripheral driver may need interrupts to be
enabled, which means it will have to request disabling Light-sleep mode.

Since requesting higher APB or CPU frequencies or disabling Light-sleep
mode causes higher current consumption, please keep the usage of power
management locks by components to a minimum.
