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

