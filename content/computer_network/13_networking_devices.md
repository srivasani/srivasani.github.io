---
id: cn-devices
title: Networking Devices
type: concept
tags:
  - hub
  - switch
  - multi-layer-switch
  - router
  - repeater
  - bridge
  - transparent-bridge
  - source-routing-bridge
  - modem
  - firewall
  - networking-devices
  - cn
  - computer-network
last_updated: 2026-08-01
---
# Networking Devices

### Hub

- Physical Layer
- Used to setup LAN
- Multiport Device, Star Topology
- Working
    - When a packet arrives at any port, it is copied on all ports except the port on which packet arrived
    - NOT Intelligent

- Issues with Broadcasting
- No memory
- Half Duplex
- High Security Risk
- Less Efficient


---

### Switch


- Data Link Layer
- Used to setup LAN
- Multiport Device, Star Topology
- Intelligent forwarding
- Can do unicast, multicast, broadcast.
- Has memory stores MAC Address Table
- Full Duplex
- Low Security Risk
- High Efficient



#### Multi-layer Switches
- Layer-3 switch
- router + switch = multi-layer switch


---

### Router

- It forwards data packets between computer networks
- It is connected to at least two networks (two LANs or two WANs or LAN to it’s ISP)
- Layer-3 Device
- Stores Routing Tables
- Full Duplex


---


### Repeater

- The data signal generally become two weak or corrupted if they tend travel a long distance.
- Repeater regenerates (not amplify) the signal over the same network.
- It is a two-port device.
- Layer-1 Device

---

### Bridge

- Bridge = Repeater + Functionality of reading MAC addresses
- Layer-2 Device
- Two-port Device
- It is used for interconnecting two LANs with the same protocol.
- Same protocols includes frame formats, access methods, mac address scheme, ethernet LAN etc.

#### Types of Bridge

##### 1. Transparent Bridges

- Stations are completely unaware of the bridge’s existence.
- Reconfiguration is not necessary when bridge is added or removed.


##### 2. Source Routing Bridges

- In these bridges routing operation is performed by source station and the frame specifies which route to follow.


---

### Modem 
- Modulation (Digital to Analog)


### Firewall 

- Security Devices


