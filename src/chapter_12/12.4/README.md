# 🧐 Practice: Power Management in Smart Light Project

After understanding ESP32-C3's power management feature and different
low-power modes, users can implement different power management schemes
to reduce power consumption during the development of their actual IoT
projects. This section introduces how to optimise the power consumption
of the Smart Light project, which is also used as an example in other
sections of this book, by implementing ESP32-C3's power management
scheme and using different low-power modes.

To save energy in general or obtain certification for energy
consumption, it is necessary to reduce the power consumption of ESP32-C3
during operation as much as possible in the Smart Light project. As
explained in Sections 12.1 and 12.2, when ESP32-C3 is operating in
Deep-sleep mode, its LEDC function does not work properly, and its Wi-Fi
and BLE connections cannot be maintained. As a result, ESP32-C3 can not
receive control commands from the user. Therefore, a power management
scheme that utilises Wi-Fi Modem-sleep mode, Bluetooth Low Energy
Modem-sleep mode, power management, and automatic Light-sleep mode is
commonly employed to minimise power consumption in smart light projects.
After implementing this scheme:

-   When the light is on, the power management lock is acquireed to
    ensure that the LEDC works normally, while Wi-Fi and Bluetooth LE
    remain connected to receive the user's control commands. By using
    the Modem-sleep mode of Wi-Fi and the Modem-sleep mode of Bluetooth
    LE, the working time of the RF circuit can be reduced to reduce
    power consumption.

-   When the light is off, the power management lock is released so CPU
    can enter Light-sleep mode when it is idle to further reduce power
    consumption.

Implementing this scheme in the Smart Light project involves two steps:

1.  Configure ESP32-C3's power management feature, enable Automatic
    Light-sleep mode, turn on Wi-Fi Modem-sleep mode and Bluetooth LE
    Modem-sleep mode.

2.  Complete the operation of the power management lock in the
    application so the driver for LEDC dimming works properly.

To learn how to optimise for lower power consumption for your existing
projects, please visit [`book-esp32c3-iot-projects/device_firmware/6_project_optimize`](https://github.com/espressif/book-esp32c3-iot-projects/tree/main/device_firmware/6_project_optimize).
