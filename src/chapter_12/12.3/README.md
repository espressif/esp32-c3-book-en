# Power Management and Low-Power Debugging

Please note that the actual power consumption may exceed theoretical
values due to various factors, such as but not limited to:

-   Wi-Fi is receiving data or Bluetooth LE is receiving data.

-   The application acquires the power management lock for a long time
    and does not release it.

-   Process blocking (that is not related to calling operating system
    APIs) exists in the application.

-   The predefined interval to wake up the chip via a timer is too small
    or interrupts happen too often.

It's advised to identify the root cause and seek optimisation if the
power consumption exceeds theoretical values for a substantial amount of
time. Users can identify the root cause via log debugging and GPIO
debugging, or additionally use some network protocol analysers if the
high-power consumption may relate to Wi-Fi and Bluetooth LE. Note that
this process can iterate as many times as needed till the actual product
requirements are met.

The following sections describe the most commonly used methods to
optimise power consumption, namely log debugging and GPIO debugging, and
demonstrate how to put these methods into practice through real-world
examples and real-time power consumption data.
