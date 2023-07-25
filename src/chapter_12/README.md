# Power Management and Low-Power Optimisation

With the wide application of IoT products, people can see more and more
IoT products in daily life, such as smart watches, smart sockets, smart
light bulbs, smart speakers, etc. Many of these IoT products are under
pressure to reduce their power consumption because they are powered by
battery or require certification for energy consumption. For example,
the CEC Tile 20 specification mandates that smart bulbs must not exceed
a standby power consumption of 0.2W to obtain energy consumption
certification in California, USA. Battery-powered smartwatches also aim
to extend their working hours. Developers of such IoT products must
prioritise power consumption as a crucial consideration during product
development. They must have a comprehensive understanding of the power
consumption characteristics of the chips they use, and be skilled in
utilising the relevant chips in practical IoT projects. To achieve this,
they should prioritise using low-power wireless communication
technologies, such as Bluetooth LE, and employ low-power circuit design
in their implementations. This ensures that power consumption is
minimised throughout the development process.

In low-power scenarios, the lifetime of a battery-powered device and its
ability to pass energy certification are often determined by its average
current. This average current is influenced by several factors,
including the current in different low-power modes, the operating
current in active states, the duration of low-power mode activation or
deactivation, and the processing power of the CPU. ESP32-C3 provides
chip-level support for low-power scenarios. It employs advanced power
management technology to switch between different power modes and
features intelligent low-power peripherals that help reduce CPU wakeup
times, resulting in further reduction of overall power consumption.
