---
id: cn-protocols
title: Elements of Protocols CN
type: concept
tags:
  - protocol-elements
  - cn-protocols
  - protocol
  - cn
last_updated: 2026-08-01
---
# Protocols

### Definition

- It is a set of rules that govern data communication.

### Elements of Protocol

#### 1. Message Encoding

![Elements of Protocol: Message Encoding](../assets/images/cn/elements_of_protocol.png)

```mermaid
flowchart LR
    A["Message<br>(Source)"] --> B["Encoder<br>(Signal)"]
    B --> C["Transmitter"]
    C --> D["Transmission Medium"]
    D --> E["Receiver"]
    E --> F["Decoder<br>(Signal)"]
    F --> G["Message<br>(Destination)"]
```


#### 2.	Message Formatting and Encapsulation

- Agreed Format
- Encapsulate the information to identify the sender & receiver rightly.


#### 3.	Message Size

- Long messages must also be broken into smaller pieces to travel across a network.

#### 4. Message Timing

- Flow control
- Response Time out


#### 5.	Message Delivery Options

##### Unicast

- Unicast: one to one (1-1)

![Unicast](../assets/images/cn/unicast.png)

```mermaid 
%%Unicast Diagram%%
graph LR 
	S[Sender] <--> SW[Switch] 
	SW <--> R1[Node A] 
	SW <--> R2[Node B] 
	SW <--> R3[Receiver]

```



##### Multicast
- Multicast: One to many but not all.

![Multicast](../assets/images/cn/multicast.png)

```mermaid 
%%Multicast Diagram%%
graph LR 
S[Sender] <--> SW[Switch] 
SW <--> R1[Receiver] 
SW <--> R2[Node B] 
SW <--> R3[Receiver]
```


    

##### Broadcast

- Broadcast: One to all.
![Broadcast](../assets/images/cn/broadcast.png)

```mermaid 
%%Broadcast Diagram%%
graph LR 
S[Sender] <--> SW[switch] 
SW <--> R1[Receiver] 
SW <--> R2[Receiver] 
SW <--> R3[Receiver]
```
    
    
