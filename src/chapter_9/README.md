# Cloud Control

After reading the local control introduced in Chapter 8, you should know
how to design the local control function for your IoT projects. However,
this function is far from enough, because a complete IoT project aims to
connect all things and local control has a geographical limitation: the
smartphone must be in the same local area network (LAN) as the
controlled device. If you want to remotely control the IoT devices at
home through your smartphone, you will need the remote control function.

This chapter mainly introduces how to remotely control devices based on
ESP32-C3. The purpose is to help you understand what remote control and
its process are, what protocol is involved, how to build an MQTT server
locally to simulate the cloud server, and how to build a product model
through ESP RainMaker for remote control of a device.
