# ESP-IDF Overview
ESP-IDF (Espressif IoT Development Framework) is a one-stop IoT
development framework provided by Espressif Technology. It uses C/C++ as
the main development language and supports cross-compilation under
mainstream operating systems such as Linux, Mac, and Windows. The
example programs included in this book are developed using ESP-IDF,
which offers the following features:

-   **SoC system-level drivers**. ESP-IDF includes drivers for ESP32,
    ESP32-S2, ESP32-C3, and other chips. These drivers encompass
    peripheral low level (LL) library, hardware abstraction layer (HAL)
    library, RTOS support and upper-layer driver software, etc.

-   **Essential components**. ESP-IDF incorporates fundamental
    components required for IoT development. This includes multiple
    network protocol stacks such as HTTP and MQTT, a power management
    framework with dynamic frequency modulation, and features like Flash
    Encryption and Secure Boot, etc.

-   **Development and production tools**. ESP-IDF provides commonly used
    tools for building, flash, and debugging during development and mass
    production (see Figure 4.1), such as the building system based on
    CMake, the cross-compilation tool chain based on GCC, and the JTAG
    debugging tool based on OpenOCD, etc.

<!-- ![Building, flashing, and debugging tools for development and mass
production](Pics/D4Z/4-1.png) -->
<figure align="center">
    <img src="../../Pics/D4Z/4-1.png" width="80%">
    <figcaption>Figure 4.1. Building, flashing, and debugging tools for development and mass
production</figcaption>
</figure>

It is worth noting that the ESP-IDF code primarily adheres to the the
Apache 2.0 open-source license. Users can develop personal or commercial
software without restrictions while complying with the terms of the
open-source license. Additionally, users are granted permanent patent
licenses free of charge, without the obligation to open-source any
modifications made to the source code.