# Summary

This chapter first introduces two key aspects of IoT device security:
data storage and data transmission. These aspects have specific
requirements for data integrity, confidentiality, and legitimacy. Then,
the chapter proceeds to discuss several solutions that address these
security concerns, including:

-   **Data integrity verification algorithm** verifies the integrity of
    firmware data during the firmware loading process or OTA upgrades.

-   **Flash encryption** and **NVS encryption** safeguard the
    confidentiality of data stored in flash memory and prevent
    unauthorised access to key data. Encrypted data can only be loaded
    after decryption using a specific key. Enabling flash encryption
    ensures that even if the data is obtained from the flash, it cannot
    be copied to another device for loading, thereby protecting the
    intellectual property rights of software developers.

-   **Secure boot scheme** verifies the authenticity and legitimacy of
    firmware data, ensuring that only firmware from authenticated
    sources is allowed to run on the device.

Finally, the chapter provides a brief overview of how to enable flash
encryption and secure boot using the mass production download tools.
