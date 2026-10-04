# Network Addressing

The lab network used the subnet `192.168.2.0/24`.

| Device | Addressing | IP address |
|---|---|---|
| Router | Static | 192.168.2.254 |
| Raspberry Pi | Static | 192.168.2.253 |
| Raspberry Pi Pico W | DHCP | Dynamic |

The router acted as the default gateway. The Raspberry Pi used a static address so that services such as SSH and MQTT could be reached consistently.

The remaining client devices received addresses through DHCP.

## Address range

- Network address: `192.168.2.0`
- Subnet mask: `255.255.255.0`
- Default gateway: `192.168.2.254`
- Available DHCP range: `192.168.2.1 – 192.168.2.252`
