---
id: cn-data-link-layer
title: Dala Link Layer
type: concept
tags:
  - dll
  - data-link-layer
  - layering
  - osi-model
  - cn
  - computer-network
last_updated: 2026-08-01
---

# Data Link Layer 

- It is responsible for moving frames from node to node. It has two sublayers:-

### LLC/DLC Sublayer (Logical/Data Link Control)
- Handles communication between upper and lower layers.
- Adds control information to help deliver the packet to the destination. [Flow Control](../computer_network/flow_control.md)
- [Error Control](../computer_network/error_control.md)

### MAC Sublayer (Media Access Control)

- Implemented by hardware NIC
- Responsible for placement and removal of frames on/from the media
- Communicates directly with physical layer.

#### Responsibilities

- **Data Encapsulation**: This sublayer add header & trailer to the packet
- [Media Access Control](../computer_network/multiple_access_protocols.md) 
- [Framing](../computer_network/framing.md)
- [Physical Addressing](../computer_network/physical_addressing.md)

#### Data Link Layer Protocols

1. [Ethernet](../computer_network/ethernet.md)
2. [PPP](../computer_network/ppp.md) (SLIP replaced by PPP)
3. [HDLC](../computer_network/hdlc.md)
4. Frame Relay
 - connection-oriented, Virtual Circuit Packet Switching approach
 - Variable-Length Framing
 - flexible payload allocation
 - non-real-time (bursty) data like LAN-to-LAN traffic

5. ATM
 - connection-oriented, Virtual Circuit Packet Switching
 -  Fixed-Size Framing (Cell Relay) where every single unit is strictly 53 bytes long
 - each cell into a precise allocation of a 5-byte header and a 48-byte payload
 - real-time data like voice and video conferencing

6. Token Ring
 - Developed by IBM LAN protocol
 - Deterministic access
 - speed 4 mbps to 16 mbps
