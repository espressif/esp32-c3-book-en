# Summary

In this chapter, we introduced remote control and the MQTT protocol. It
is a commonly used protocol in remote control and connection of IoT
devices to the cloud. It is now adopted by many mainstream cloud
platforms, such as Amazon Cloud, Alibaba Cloud, Baidu Cloud, Tencent
Cloud, and ESP RainMaker introduced in this chapter. This simple and
lightweight protocol provides reliable network services for IoT devices
in low-bandwidth and unstable network environments.

Besides, we also covered how to build an MQTT broker locally to simulate
the cloud platform, and how to generate server and client certificates
for the TLS protocol handshake to ensure data security.

In the practice in this chapter, we took the development of a smart
light product as an example to complete the remote control of devices
using the ESP RainMaker platform over MQTT. Self Claiming is used to
obtain certificates. Multiple sets of MQTT topics are used for device
control, user-node mapping, and device status. The built-in basic
services can perform the scheduling operation and OTA upgrade. With the
completed cloud connection function of ESP RainMaker, smart lights can
quickly be given voice control capabilities.

ESP RainMaker's capabilities are not limited to this. Data collection
and analysis, device-to-device linkage, and third-party scene triggers
are all interesting functions yet not mentioned in this chapter. With
these cloud functions, we can roughly calculate power consumption by
counting the online/offline time and frequency of smart lights and found
out how they work together with other hardware. These functions can be
achieved using the open RESTful API. Chapter 10 will introduce the use
of the RESTful API and use them to develop a smartphone app.
