# Summary

In this chapter, we first presented an overview of the framework model,
applicable conditions, and application scenarios of local control. We
also compared it to remote control, enabling you to assess the
suitability of local control functionality based on your unique project
requirements. Local discovery plays a pivotal role in local control as
it governs the ability of smartphones to search for devices within the
LAN. This allows smartphones to retrieve device characteristics and
facilitates subsequent control of the identified devices. Therefore, we
also delved into the operational mode of the local discovery protocols,
specifically in terms of the principle layer. We also conducted a
comparative analysis of the characteristics of the two modes: broadcast
and multicast, shedding light on their similarities and differences. The
most commonly used local discovery protocol is mDNS, which provides you
with the flexibility to implement local discovery functionality in your
IoT projects. You can also leverage the resource discovery technology
inherent in the Bluetooth protocol directly when utilising Bluetooth for
control purposes.

Then we introduced the most critical data communication protocols and
corresponding data encryption algorithms in local control. The
fundamental protocols for data communication in local control are TCP
and UDP . While you can directly utilise these protocols for local
control, it is generally not recommended due to certain limitations. TCP
and UDP are classified as transport layer protocols and do not
inherently carry application format data, in contrast to protocols like
HTTP and CoAP, which incorporate an application layer on top of the
transport layer. Furthermore, it's important to note that transport
layer protocols such as TCP and UDP do not support direct encryption of
data using protocols like TLS or DTLS. Therefore, relying solely on the
transport layer protocol for data transmission may not guarantee the
security of the transmitted data. Hence, it is recommended that you
utilise protocols such as HTTP with TLS or CoAP with DTLS for data
communication in local control scenarios.

Finally, we introduced how to implement the complete local control
function based on the `esp_local_ctrl` component in ESP-IDF.
`esp_local_ctrl` supports local control based on Wi-Fi and Bluetooth,
with data communication protocols that include HTTPS for Wi-Fi and
Bluetooth protocols for Bluetooth. You can get started with local
control development with `esp_local_ctrl` component. Additionally, the
`esp_local_ctrl` component does not support local network device
discovery functionality. You need to implement device discovery
functionality using the mDNS module. The `esp_local_ctrl` component is
widely used in ESP-IDF, and you can find provisioning and local
communication features in the `wifi_provisioning` component for network
configuration and local communication.

Of course, there are various protocols and implementation methods for
local control. If the `esp_local_ctrl` component does not meet your
requirements, you can follow the example codes in sections 8.2, 8.3, and
8.4 to build your own local control framework.
