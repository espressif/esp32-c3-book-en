# How to use this book?

The code of the projects in this book has been open sourced. You can download it from our GitHub repository and share your thoughts and questions on our official forum.

> GitHub: <https://github.com/espressif/book-esp32c3-iot-projects>  
> Forum: <https://www.esp32.com/bookc3>

Throughout the book, there will be parts highlighted as shown below.

> 📝 **Source code**
>
> In this book, we emphasise the combination of theory and practice, and thus set a **Practice** section about the Smart Light project in almost every chapter. Corresponding steps and source page will be provided in blockquotes beginning with the tag 📝 **Source code**.

> 📌 **Tip**
>
> This is where you may find some critical information and reminding for successfully debugging your program. They will be marked in blockquotes beginning with the tag 📌 **Tip**.

> 📚 **Further Reading**
>
> Here is the expanded reading section, which will facilitate a deeper understanding for you of the related technical points. They will be marked in blockquotes beginning with the tag 📚 **Further Reading**.

Most of the commands in this book are executed under Linux, prompted by the character “`$`”. If the command requires superuser privileges to execute, the prompt will be replaced by “`#`”. The command prompt on Mac systems is “`%`”, as used in Section 4.2.3 Installing ESP-IDF on Mac.

Commands or texts that need to be input by the user, and commands that can be entered by pressing the “Enter” key will be printed in **`bold`**.

## Example:

Second, use `esp-idf/components/nvs_flash/nvs_partition_generator/nvs_
partition_gen.py` to generate the NVS partition binary file on the development host with the following command:

<pre><code>$ <b>python $IDF_PATH/components/nvs_flash/nvs_partition_generator/nvs_partition_gen.py --input mass_prod.csv --output mass_prod.bin --size NVS_PARTITION_SIZE</b></code></pre>

## Book Structure

This book takes an engineer-centered perspective and expounds the necessary knowledge for IoT project development step by step. It is composed of four parts, as follows:

- **Preparation** (Chapter 1-4): This part introduces the architecture of IoT, typical IoT project framework, the ESP RainMaker&reg; cloud platform, and the development environment ESP-IDF, so as to lay a solid foundation for IoT project development.

- **Hardware and Driver Development** (Chapter 5-6): Based on the ESP32-C3 chipset, this part elaborates on the minimum hardware system and driver development, and implements the control of dimming, colour grading, and wireless communication.

- **Wireless Communication and Control** (Chapter 7-11): This part explains the intelligent Wi-Fi configuration scheme based on ESP32-C3 chip, local & cloud control protocols, and local & remote control of devices. It also provides schemes for developing smartphone apps, firmware upgrade, and version management.

- **Optimisation and Mass Production** (Chapter 12-15): This part is intended for advanced IoT applications, focusing on optimisation of products in power management, low-power optimisation, and enhanced security. It also introduces firmware burning and testing in mass production, and how to diagnose the running status and logs of device firmware through the remote monitoring platform ESP Insights.

## About the Source Code

Readers can run the example programmes in this book, either by entering the code manually or by using the source code that accompanies the book. We emphasise the combination of theory and practice, and thus set a *Practice* section based on the Smart Light project in almost every chapter. All the codes are open-sourced. Readers are welcome to download the source code and discuss it in the sections related to this book on [GitHub](https://github.com/espressif/book-esp32c3-iot-projects) and our official forum [esp32.com](https://www.esp32.com/bookc3). The open-sourced code of this book is subject to the terms of Apache License 2.0.