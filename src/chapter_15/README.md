# ESP Insights: Remote Monitoring Platform

The previous chapters introduced the ESP RainMaker IoT cloud platform, a
device-to-cloud solution provided by Espressif. Using the components of
the ESP RainMaker IoT cloud platform, users can easily connect to ESP
RainMaker, realizing remote control of devices. With the help of the ESP
RainMaker IoT cloud platform, users can develop the ESP32-C3 smart LED
products with ease. But we all know that from project approval to mass
production, a product needs to go through main processes including
functional evaluation, implementation, and verification.

Based on the introduction about the functions of smart LED products and
how these functions are realized from the previous chapters, you may
wonder after realizing the functions of the smart LED, how to carry out
systematic functional verification and on-hook verification.

After developing the function code of a project, functional verification
is required. At this time, you can set the log level to Debug mode, and
monitor the log on the serial port to get the debugging done. This is a
necessary verification before releasing the software. Upon completing
the basic functional verification, functions such as log output and
command line debugging should often be disabled. Then, it's time to
release the Release version. Thereafter, even if the software behaves
abnormally during the Quality Assurance (QA) test or during usage, it
will be difficult for developers to quickly locate and fix the issues by
obtaining device logs. Sometimes, developers may even need to
disassemble the device for the logs to analyze the cause of the
abnormality. To solve this problem, Espressif Systems has developed ESP
Insights, which supports developers to check the running status and logs
of firmware remotely, so as to detect and solve firmware problems in
time, speeding up the software development process.
