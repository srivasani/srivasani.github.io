---
id: cn-channelization-protocol
title: Channelization Protocol
type: concept
tags:
  - fdma
  - tdma
  - cdma
  - channelization-protocol
  - maca
  - dll
  - cn
  - computer-network
last_updated: 2026-08-01
---

# Channelization Protocol

- The available bandwidth of a link is shared in time, frequency or through code between different stations.

### Types of Channelization Protocol

#### FDMA
- Frequency Division Multiple Access 
- The available bandwidth of common channel is divided into bands that are separated by guard bands.
- Available bandwidth is shared by all stations.
- FDMA is a `dll` protocol that uses Frequency Division [Multiplexing](../computer_network/multiplexing.md) physical layer.

![Frequency Divison Multiple Access](../assets/images/cn/fdma_1.png)

![FDMA](../assets/images/cn/fdma_2.png)

---

#### TDMA

- Time Division Multiple Access
- The bandwidth is just one channel that is time shared between different stations.
- Stations share the capacity of the channel in time.

![Time Division Multiple Access](../assets/images/cn/tdma.png)


---

#### CDMA

- Code Division Multiple Access
- One channel carries all information simultaneously.
- CDMA differs from FDMA because only one channel occupies the entire bandwidth of the link.
- CDMA differs from TDMA because all stations can send data simultaneously, there is no time sharing.

##### Code Properties

- If we multiply each code by another we get = 0.
- If we multiply each code by itself we get = no of nodes.

![Code Division Multiple Access](../assets/images/cn/cdma.png)

