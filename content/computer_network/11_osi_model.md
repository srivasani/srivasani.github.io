---
id: cn-osi
title: OSI Model
type: concept
tags:
  - osi-model
  - application-layer
  - presentation-layer
  - session-layer
  - transport-layer
  - network-layer
  - data-link-layer
  - physical-layer
  - osi-working
  - cn-models
  - computer-network-models
  - cn
  - computer-network
last_updated: 2026-08-01
---
# OSI Model

- Open Systems Interconnection
- A model for understanding and designing a network architecture that is flexible, robust and interoperable.
- Developed by ISO(International Standard Organization).
- It’s not a protocol, it is only a guideline and hence it is referred as OSI reference model. It is never fully implemented.

---

![OSI Reference Model](../assets/images/cn/osi_ref_model.png)

---

### Purpose: 

- Showing how to facilitate communication between different systems without requiring changes to the logic of underlying hardware and software. 


### Working of OSI Model

![Working of OSI Model](../assets/images/cn/working_of_osi.png)


![Working of OSI](../assets/images/cn/working_osi.png)

---

### 1.	Application Layer

- It enables the use to access the network resources.

- Services
    1. File Transfer & Access Management (FTAM)
    2. Mail Services
    3. Directory Services

### 2.	Presentation Layer

- It is concerned with the syntax & semantics of the information exchanged between two systems.

- Services
    1. Translation
    2. Encryption
    3. Compression

### 3. Session Layer

- It establishes, maintains and synchronizes the information among communicating devices.

- Services

    1. Dialog Control
    2. Synchronization

### 4.	Transport Layer

- It is responsible for process-to-process delivery of the entire message.

- Services

    1. Port Addressing
    2. Segmentation & Reassembly
    3. Connection Control
    4. End-End Flow Control
    5. Error Control

### 5.	Network Layer

- It is responsible for delivery of data from the original source to destination network.

- Services

    1. Logical Addressing
    2. Routing

### 6.	Data Link Layer

- It is responsible for moving frames from one node to another node.

- Services
    1. Framing
    2. Physical Addressing
    3. Flow Control
    4. Error Control
    5. Access Control

### 7.	Physical Layer

- It is responsible for transmitting bits over a medium. It also provides electrical & mechanical specifications.

- Services

    1. Physical Characteristics of the media
    2. Representation of bits
    3. Data Rate
    4. Synchronization of bits
    5. Line Configuration
    6. Physical Topology
    7. Transmission Mode

