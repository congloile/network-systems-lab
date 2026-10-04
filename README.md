# Network Systems Lab

Hands-on networking and Linux systems lab using Raspberry Pi, SSH, router configuration, MQTT and technical troubleshooting.

This repository documents selected practical exercises involving network configuration, Linux administration, remote access, MQTT communication and systematic troubleshooting.

## Technologies and Topics

- Raspberry Pi OS / Linux
- SSH and SSH key authentication
- TCP/IP networking
- DHCP and static IP configuration
- Router configuration
- DNS and connectivity testing
- DDNS and port forwarding
- MQTT messaging with Mosquitto
- Raspberry Pi Pico W
- Command-line tools
- Message logging
- Technical troubleshooting and documentation

## Practical Work

During the practical exercises, I:

- Configured and accessed a Raspberry Pi remotely using SSH
- Generated and configured SSH keys for passwordless authentication
- Hardened SSH by disabling password and root login
- Configured and tested local network connectivity
- Worked with static IP addressing and DHCP
- Configured router settings, DDNS and port forwarding
- Installed and tested Mosquitto MQTT
- Published and subscribed to MQTT messages
- Connected a Raspberry Pi Pico W to an MQTT broker
- Logged MQTT messages to a timestamped text file
- Investigated connectivity and configuration issues
- Documented configurations, test results and troubleshooting steps

## Project Documentation

- [Network addressing](docs/network-addressing.md)
- [SSH setup and security](docs/ssh-setup-and-security.md)
- [MQTT testing](docs/mqtt-testing.md)
- [Troubleshooting example](docs/troubleshooting.md)

## Example Troubleshooting

### SSH connectivity

When an SSH connection did not work as expected, I checked:

1. Device IP address
2. Local network connectivity
3. SSH configuration
4. Authentication and authorized keys
5. Router and network settings

This helped isolate whether the issue was related to the device, authentication or network configuration.

### DDNS and remote connectivity

In one test, the DDNS hostname resolved correctly and SSH worked from the local network, while a connection from an external network timed out.

I verified DNS resolution, router configuration, port forwarding and local SSH connectivity to narrow the issue down to external connectivity rather than the Raspberry Pi itself.

More details are available in the [troubleshooting notes](docs/troubleshooting.md).

### MQTT messaging

I configured Mosquitto and tested message delivery between MQTT publishers and subscribers.

Example:

```bash
mosquitto_sub -h <broker-address> -t <topic>
```

I also tested MQTT communication with a Raspberry Pi Pico W and verified that received messages could be written to a timestamped log file.
## Selected Evidence
- [SSH key authentication](screenshots/ssh-key-authentication.png)
- [Passwordless SSH login](screenshots/ssh-passwordless-login.png)
- [SSH security configuration](screenshots/ssh-security-config.png)
- [Port forwarding configuration](screenshots/port-forwarding.png)
- [DDNS lookup](screenshots/ddns-nslookup.png)
- [Raspberry Pi Pico W MQTT publish](screenshots/mqtt-pico-publish.png)
- [MQTT messages received in MQTTX](screenshots/mqttx-received-messages.png)
- [MQTT message logging](screenshots/mqtt-message-logging.png)
## What I Learned
This work helped me develop a more systematic approach to technical troubleshooting:

identify the problem → test connectivity → isolate the cause → verify the solution → document the result

It also gave me practical experience working with Linux systems, networking tools, MQTT and connected devices in a small network environment.
