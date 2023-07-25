# LED Dimming Driver Development

After understanding the basics of LED drivers, we can start developing a dimming driver based on the ESP32-C3 chip. This mainly includes the development of functional APIs for controlling the switch, brightness, color, and color temperature. In daily life, it is usually expected to maintain the color, brightness, and color temperature of a light consistent with its previous status when turning it on. This requires preserving the light's status when it is turned off. To achieve this, we can use the non-volatile storage (NVS) feature provided by ESP-IDF.

So before writing the driver code, it is also necessary to learn about the LED PWM controller of ESP32-C3, its programming procedures, and non-volatile storage.