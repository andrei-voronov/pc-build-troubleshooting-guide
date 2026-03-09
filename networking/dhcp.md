# DHCP – Dynamic Host Configuration Protocol

## What is DHCP?

DHCP is a network protocol that automatically assigns IP configuration to devices on a network.

It provides:
- IP address
- Subnet mask
- Default gateway
- DNS server

Without DHCP, devices must be configured manually (static IP).

---

## DHCP Process (DORA)

DHCP uses a 4-step process called DORA:

1. Discover  
   The client broadcasts a request to find a DHCP server.

2. Offer  
   The DHCP server responds with an available IP address.

3. Request  
   The client requests the offered IP address.

4. Acknowledge  
   The server confirms and assigns the IP configuration.

---

## DHCP Lease

- IP addresses are assigned temporarily.
- This is called a lease.
- When the lease expires, the client must renew it.

---

## DHCP Ports

- UDP 67 → Server
- UDP 68 → Client

(Important for exams.)

---

## Common DHCP Issues

- Client receives 169.254.x.x (APIPA address)
- DHCP server not reachable
- Incorrect subnet configuration
- IP conflict

---

## APIPA

If a device cannot reach a DHCP server, it assigns itself an IP address in the range:

169.254.0.0 – 169.254.255.255

This allows limited local communication.

---

## Troubleshooting DHCP

1. Check physical connection
2. Run ipconfig /all
3. Release and renew IP:
   ipconfig /release
   ipconfig /renew
4. Ping default gateway
5. Restart router / DHCP service
