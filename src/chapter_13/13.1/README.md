# Overview of IoT Device Data Security

The previous chapters introduced how to ensure the security of data
during data transmission, that is to use HTTPS protocol. Although the
data is secured during transmission, it can still face varying threats
on the device side.

We want security for the data on our devices, but what exactly does
"security" mean? As we will explore in this chapter, security is a
multifaceted concept that encompasses many different aspects. At a
minimum, data security should include the following key components:

## Confidentiality

Only authorised developers can access the real content of the data. In a
smart lighting system, data such as the Wi-Fi password, user login
information, and device ID need to be protected from unauthorised access
or disclosure.

## Integrity

Data can be maliciously tampered with during transmission and storage
stages, and code errors may occur accidentally. Therefore, device must
have the capability to verify the completeness of the data to ensure its
integrity. In a smart lighting system, data such as new firmware and
stored network certificates obtained during over-the-air (OTA) upgrades
must be verified for completeness before loading and usage. This
verification is necessary to prevent loading and using data that has
been tampered with or contains errors.

## Legitimacy

It is important that devices receiving data have the ability to
authenticate the sender and accept data only from legitimate sources. In
the context of a smart lighting system, control commands and firmware
updates should only originate from authorised devices. Just imagine, if
anyone can control the lights in your bedroom using their smartphones,
will you sleep well?

<br></br>
So, what types of data must be protected on the device?

## Firmware data

Firmware is an executable binary file running on the device, which is
responsible for coordinating system resources and enabling data exchange
between the device and the external system. Firmware security is just as
critical as operating system security on a PC. If the security of
firmware is compromised, the device's normal functions may be seriously
impacted. Therefore, it is imperative to ensure firmware data security.
In the case of ESP32-C3 based smart lighting devices, firmware usually
includes bootloader and app firmware stored in the flash memory.

## Key data to be used by the device

Such as the key to connect to the cloud, and the key to log in to the
device, etc.
