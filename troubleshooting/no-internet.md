# No Internet Connection Troubleshooting

## Step 1: Check Physical Connection

- Ensure Ethernet cable is connected
- Check Wi-Fi is enabled
- Verify router lights (LEDs)

---

## Step 2: Check IP Address

Run:

ipconfig

Check:
- IP address assigned?
- Is it 169.254.x.x (APIPA)?

---

## Step 3: Check Default Gateway

Example:
192.168.1.1

Test:
ping 192.168.1.1

If no reply → problem with router or local network

---

## Step 4: Test Internet Connectivity

ping 8.8.8.8

If works:
→ Internet is OK
→ Problem is DNS

---

## Step 5: Test DNS

nslookup google.com

If fails:
→ DNS issue

---

## Step 6: Renew IP

ipconfig /release  
ipconfig /renew  

---

## Step 7: Restart Devices

- Restart PC
- Restart router

---

## Common Causes

- DHCP failure
- DNS misconfiguration
- Router offline
- ISP outage
