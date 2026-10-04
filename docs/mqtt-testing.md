# MQTT Testing

MQTT was tested using a Raspberry Pi as the broker and a Raspberry Pi Pico W as a client.

## Pico W publishing

The Pico W connected to the WLAN and received an IP address through DHCP.

It then connected to the MQTT broker running on the Raspberry Pi and published messages to the topic:

`pico/test`

MQTTX was used to subscribe to the same topic and verify that the messages were received successfully.

## Message logging

MQTT messages were also redirected to a text file with timestamps.

Five test messages were sent and the contents of the log file were checked to confirm that the messages were stored correctly.
