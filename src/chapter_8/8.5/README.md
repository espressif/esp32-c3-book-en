# 🧐 Practice: Local Control in Smart Light Project

The local control component (`esp_local_ctrl`) of ESP-IDF enables you to
control Espressif chips via Wi-Fi+HTTPS or Bluetooth LE easily. With
this component, you can access application-defined properties, which can
be read from or written to through a set of configurable handlers. This
section mainly introduces the local control module based on Wi-Fi.
Taking the smart light as an example, the local control module can be
configured as follows:

-   Configure the local device to discover mDNS protocol.
-   Configure the local HTTPS server and certificate for data
    communication.
-   Configure the smart lights.

The previous sections have introduced the control of ESP32-C3 via
Bluetooth LE. When using Bluetooth LE, the TCP/IP protocol stack is not
involved, and local device discovery is not necessary. Bluetooth has its
own resource discovery service.
