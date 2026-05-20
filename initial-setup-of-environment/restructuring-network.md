---
description: >-
  I need to organize then implement the solutions for the problems I previously
  identified
---

# Restructuring network

I started by verifying that my vtnet0 interface is associated with WAN, an connected to the Vmbr0 bridge.

I did the same for vtnet1 and Vmbr1 ensuring they are associated with LAN.

Next I ensured my network actually reflects my logical topology on the home page. I changed all devices ports to connect to the LAN side of the firewall (except Kali Linux, which will remain on the outside).

Now that all devices are connected to the firewall LAN, I will begin implementing my new IP addressing scheme. So far the only IP in use is 10.0.0.1 on the firewall.

I will now add a static IP to the DC and configure DHCP

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

I'm using a /24 subnet mask for simplicity, however I'm only assigning out a block of 20 IP's.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

No exclusions are necessary, as the first 19 addresses will be reserved for servers.

I will assign 8 hours to the lease duration. This is a good middle ground between a long and lese secure lease, and a short lease that generates too much noise.

Configuration for the new scope will use DHCP options. All IP's within the scope will receive the following configurations.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
