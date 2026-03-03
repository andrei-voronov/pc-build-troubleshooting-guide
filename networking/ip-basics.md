# IP Addressing Basics

## Definition
An IP address (Internet Protocol address) is a unique numerical identifier assigned to a device in a network. It allows devices to communicate and exchange data.

## IPv4 Structure
- IPv4 uses 32 bits.
- Written as 4 octets separated by dots.
- Example: 192.168.1.10
- Each octet ranges from 0 to 255.

## Public vs Private IP

### Private IP Ranges
- 10.0.0.0 – 10.255.255.255
- 172.16.0.0 – 172.31.255.255
- 192.168.0.0 – 192.168.255.255

Private IP addresses are used inside local networks and are not routable on the internet.

Public IP addresses are assigned by ISPs and are reachable over the internet.

## Subnet Mask
A subnet mask defines the network and host portion of an IP address.

Example:
- 255.255.255.0
- /24 notation

## Common Issues
- Incorrect IP configuration
- IP address conflict
- Wrong subnet mask
- Incorrect default gateway

## Troubleshooting
1. Use `ipconfig` (Windows) to check IP configuration.
2. Verify default gateway.
3. Test connectivity using `ping`.
4. Ensure DHCP is enabled if required.
