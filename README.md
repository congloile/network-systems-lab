# network-systems-lab
Hands-on networking and Linux lab using Raspberry Pi, SSH, router configuration, MQTT and troubleshooting.
This repository documents practical exercises in networking and Linux system administration using Raspberry Pi, SSH, router configuration, MQTT messaging and troubleshooting.

## Technologies and Topics

Raspberry Pi OS / Linux
SSH and SSH key authentication
TCP/IP networking
DHCP and local IP configuration
Router configuration
DNS and connectivity testing
MQTT messaging with Mosquitto
Command-line tools
Message logging
Technical troubleshooting and documentation

## Practical Work

During the practical exercises, I:

- Configured and accessed a Raspberry Pi remotely using SSH
- Generated and configured SSH keys for passwordless authentication
- Configured and tested local network connectivity
- Worked with router settings and network addressing
- Installed and tested Mosquitto MQTT
- Published and subscribed to MQTT messages
- Logged MQTT messages to a text file
- Investigated connection and configuration issues
- Documented configurations, test results and troubleshooting steps

## Example Troubleshooting

### SSH connectivity

When an SSH connection did not work as expected, I checked:

1. Device IP address
2. Local network connectivity
3. SSH configuration
4. Authentication and authorized keys
5. Router and network settings

This helped isolate whether the issue was related to the device, authentication or network configuration.

### MQTT messaging

I configured Mosquitto and tested message delivery between MQTT publishers and subscribers.

Example:

```bash
mosquitto_sub -h <broker-address> -t <topic>
```
I also tested message logging and verified that received messages were written correctly to a file.
## What I Learned
This project helped me develop a more systematic approach to technical troubleshooting:
**identify the problem → test connectivity → isolate the cause → verify the solution → document the result**
It also gave me practical experience working with Linux, networking tools and services in a real system environment.
