---
id: cn-network-model
title: Computer Network Models
type: concept
tags:
  - cn-models
  - p2p
  - computer-network-models
  - cn
  - computer-network
last_updated: 2026-08-01
---
# Network Models

### Peer to Peer Network



- No centralized administration
- All peers are equal
- Simple sharing
- Not scalable


![Client Server Model](../assets/images/cn/peer_to_peer_model.png)


```mermaid
graph TD
    P1[Node A]
    P2[Node B]
    P3[Node C]

    P1 <--> P3
    P2 <--> P3



```


### Client Server Model



- Centralized administration
- Request-Response Model
- Scalable
- Server may be overloaded.
   

![Peer to Peer Network Model](../assets/images/cn/client_server_model.png)




```mermaid 
graph LR 
Server[Server] --> SW[Switch] 
SW <--> C1[Client A] 
SW <--> C2[Client B] 
SW <--> C3[Client C]

```
