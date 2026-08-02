---
id: cn-reservation-protocol
title: Reservation Protocol
type: concept
tags:
  - reservation
  - multiple-access-protocol
  - dll
  - cn
  - computer-network
last_updated: 2026-08-01
---

# Reservation

- A station need to make a reservation before sending data.
- In each interval, a reservation frame precedes the data frame in that interval.
- If there are `N` systems, there are exactly `N` reservation.
- Each mini slot belongs to a station.
- When station needs to send data it makes reservation in its own mini slot.
- Those who made reservation can send their data frames.

![Reservation](../assets/images/cn/reservation.png)

