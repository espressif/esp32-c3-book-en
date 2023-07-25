# Summary

This chapter introduces ESP Insights, which includes a firmware agent
(Insights agent) that runs on the user's device to capture the operating
status and abnormality of the device and report them to the ESP Insights
cloud. When verifying product functions and on-hook testing, users can
log in to the dashboard of the ESP RainMaker IoT cloud platform to view
the health status of each device and whether there is an abnormality.
Instead of capturing logs of device operation on every device run, logs
of device abnormality will be reported to the ESP Insights Cloud. Users
can view the reasons for device abnormality clearly through the ESP
Insights Cloud interface, making it considerably easier for debugging.

At present, the Insights agent sends data to the ESP RainMaker IoT cloud
platform by default. In the future, Espressif will release solutions to
support more cloud platforms to receive and process the device
information reported by the Insights agent. With these solutions, the
functional verification and debugging of the device will become much
easier, accelerating the release of user product firmware.
