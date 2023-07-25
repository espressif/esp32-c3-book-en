# Ensuring MQTT Data Security

Data transmitted using the MQTT protocol is in plain text, which means
it can be intercepted if not encrypted. In Chapter 8.4.1, the TLS
protocol is introduced as a means to ensure that data can only be
decrypted by the communicating parties, thereby safeguarding data
security and legitimacy.

Similarly, TLS can also be used for encryption in cloud communication
over MQTT. Since it has already been covered in Chapter 8.4.1, this
section only introduces what the certificates in the TLS handshake mean
and what functions they perform, how to generate certificates locally,
and how to set up a mutual authentication TLS environment based on the
local MQTT broker.
