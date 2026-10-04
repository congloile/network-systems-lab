# Troubleshooting Example

## Remote SSH through DDNS

### Problem

The DDNS hostname resolved correctly and SSH worked from the local network, but a connection from a separate remote network timed out.

### Checks performed

- Verified that the DDNS hostname resolved correctly
- Verified the router WAN address
- Checked the port forwarding rules
- Confirmed that SSH worked locally
- Compared local and remote connectivity results

### Result

The Raspberry Pi and local SSH configuration were working correctly.

Because the hostname resolved correctly and local SSH access worked, the issue was isolated to external connectivity rather than the Raspberry Pi itself.

This exercise helped me practice troubleshooting by checking each layer separately instead of changing multiple settings at once.
