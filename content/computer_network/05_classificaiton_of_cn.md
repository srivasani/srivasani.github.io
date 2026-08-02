---
id: cn-classification
title: Classification of CN
type: concept
tags:
  - cn-type
  - lan
  - man
  - wan
  - cn
  - computer-network
last_updated: 2026-08-01
---
# Classification of CN

### 1.	LAN

- A local area network is a computer network that interacts computers within a limited area such as a residence, school etc.

#### LAN Devices

-  Wired LAN
	- Hub 
	- Switches

 - Wireless LAN
	 - Wi-Fi 

![LAN](../assets/images/cn/lan.png)

```mermaid 
graph LR 
Server[Node S] <--> SW[Switch] 
SW <--> C1[Node A] 
SW <--> C2[Node B] 
SW <--> C3[Node C]

```


---


### 2. MAN

- A metropolitan area network is a computer network that interconnects users with computer resources in a geographic region of the size of metropolitan area(city).

#### MAN Devices

- Hub , Switches
- Routers, Bridges

![MAN](../assets/images/cn/man.png)


```mermaid
graph TD
    LAN1["LAN 1"]
    LAN2_L["LAN 2"]
    MAN(("MAN"))
    LAN2_R["LAN 2"]
    LAN3["LAN 3"]

    LAN1 <--> MAN
    LAN2_L <--> MAN
    MAN <--> LAN2_R
    MAN <--> LAN3

```

---

### 3. WAN

- A wide area network is a telecommunications network that extends over a large geographical area for the primary purpose of computer networking.

#### WAN Devices
- End Devices
- Intermediary Devices

![WAN](../assets/images/cn/wan.png)

```mermaid
graph TD
    %% Nodes

    
    WAN <--> SW1[Switch A]
    SW1 <--> C1[Node A]
    SW1 <--> C2[Node B]
    SW1 <--> C3[Node C]

    WAN <--> SW2[Switch B]
    SW2 <--> C4[Node D]
    SW2 <--> C5[Node E]
    SW2 <--> C6[Node F]

```
