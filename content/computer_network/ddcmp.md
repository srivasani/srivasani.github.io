---
id: cn-ddcmp
title: ddcmp
type: concept
tags:
  - ddcmp
  - byte-oriented-framing-protocol
  - framing
  - dll
  - cn
  - computer-network
last_updated: 2026-08-01
---

# DDCMP

- Designed by Digital Equipment Protocol.
- Byte-counting approach 
- Count: bytes are contained in the frame body

### Frame Format

![DDCMP Frame Format](../assets/images/cn/ddcmp_frame.png)

#### Drawback of count
- If transmission error corrupted the count field then end of frame will not be detected correctly by the receiver.


