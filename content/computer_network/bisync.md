---
id: cn-bisync
title: BISYNC
type: concept
tags:
  - bisync
  - byte-oriented-framing-protocol
  - framing
  - dll
  - cn
  - computer-network
last_updated: 2026-08-02
---

# BISYNC

- Binary Synchronous Communication Protocol
- It is sentinel approach developed by IBM.

### Header Format

![BISYNC Header Format](../assets/images/cn/bisync_frame.png)

- Frames transmitted beginning with leftmost field.
- DLE: Data Link Escape (used in [byte stuffing](#byte-stuffing))

---

### Byte Stuffing

- Byte/char stuffing is the process of adding one extra byte whenever there is a flag or escape character in the text.



