---
id: cn-token-passing
title: Token Passing Protocol
type: concept
tags:
  - token-passing
  - multiple-access-protocol
  - formula
  - dlc
  - cn
  - computer-network
last_updated: 2026-08-01
---

# Token Passing

- A station is authorized to send data when it receives a special frame called a token.
- No master node.
- `A small, special purpose frame = token` is exchanged in fixed order.
- If a node receives a token, it holds only if have to send something otherwise it passes the token to the next node.
- Decentralized/Highly Effective.

### Drawback
- one node can crash, a node accidentally neglects to release the token.

> If $\text{N} = \text{ No of Nodes, S } = \text{ Throughtput }$ and $\text{a} = \frac{\text{T}_\text{p}}{\text{T}_\text{t}}$, then


$$
\text{Performance S } = \Bigg(\frac{1}{1+\frac{\text{a}}{\text{N}}} \Bigg) \text{, a} \le 1 \text{ or } \Bigg(\frac{1}{\text{a}\times\big(1+\frac{1}{\text{N}}\big)}\Bigg) \text{, a} \ge 1
$$
