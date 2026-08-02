---
id: cn-topology
title: Network Topology CN
type: concept
tags:
  - cn-topology
  - bus-topology
  - ring-topology
  - dual-ring-topology
  - star-topology
  - extended-star-topology
  - mesh-topology
  - hybrid-topology
  - cn
  - computer-network
last_updated: 2026-08-01
---
# Network Topology

### Definition

- Arrangement of nodes of a computer network.
- Topology means layout

### Physical Topology
-  Placement of various nodes

### Logical Topology  
- Deals with data flow in the network

##### 1. Bus Topology

- Common transmission medium 
- Data will be received by all nodes in the network simultaneously.
- A signal containing the address of the intended receiving machine travel from a source in both direction to all nodes connected to the bus until it finds the intended recipient.

###### Advantages

1.	Less expensive
2.	Suited for temporary network
3.	Node failure does not affect others.

###### Disadvantages

1.	Not Fault tolerant
2.	Limited Cable Length
3.	No Security

![Bus Topology](../assets/images/cn/bus.png)


```mermaid
graph LR
    %% Main Backbone Cable
    Bus1[ ] --- Bus2[ ] --- Bus3[ ] --- Bus4[ ]
    
    %% Drop Lines to Nodes
    Bus1 --- A((Node 1))
    Bus2 --- B((Node 2))
    Bus3 --- C((Node 3))
    Bus4 --- D((Node 4))

    %% Formatting
    style Bus1 width:0px,height:0px;
    style Bus2 width:0px,height:0px;
    style Bus3 width:0px,height:0px;
    style Bus4 width:0px,height:0px;
    linkStyle 0,1,2 stroke:#2c3e50,stroke-width:6px;
    linkStyle 3,4,5,6 stroke:#7f8c8d,stroke-width:3px;

```

---

##### 2.	Ring Topology

- A ring topology is a bus topology in a closed loop.
- Peer to Peer Lan technology
- Two Connections: one to each of its nearest neighbors
- Unidirectional
- Sending and receiving data takes place with the help of a token.

###### Advantages

1.	Performance better than bus
2.	All nodes with equal access


###### Disdvantages

1.	Unidirectional
2.	Single point of failure will affect the network
3.	No Security
4.	Increment in load will cause poor performance.



![Ring Topology](../assets/images/cn/ring.png)

```mermaid
graph LR
    %% Nodes
    A((Node 1))
    B((Node 2))
    C((Node 3))
    D((Node 4))

    %% Main Backbone Ring (Clockwise)
    A --> B
    B --> D
    D --> C
    C --> A



```



###### Dual Ring Topology

![Dual Ring Topology](../assets/images/cn/dual_ring.png)


```mermaid
graph LR
    %% Nodes
    A((Node 1))
    B((Node 2))
    C((Node 3))
    D((Node 4))

    %% Primary Ring (Clockwise)
    A --- B
    B --- D
    D --- C
    C --- A

    %% Secondary Redundant Ring (Counter-Clockwise)
    A -.-> C
    C -.-> D
    D -.-> B
    B -.-> A





```



---

####  3.	Star Topology 

- Every node is connected to a central hub or switch.
- Centralized Management
- All traffic must pass through the hub/switch.


##### Advantages

1.	Easy to design & implement
2.	Centralized administration
3.	Scalable


##### Disadvantages

1.	Bottleneck due to overload switch/hub.
2.	Single point of failure will affect the network
3.	Increase cost due to switch/hub.

![Star Topology](../assets/images/cn/star.png)



```mermaid
graph TD
    Top[Node A]
    Left[Node B]
    SW[switch]
    Right[Node C]
    Bottom[Node D]

    SW <--> Top
    SW <--> Left
    SW <--> Right
    SW <--> Bottom


```

##### Extended Star Topology


![Extended Star Topology](../assets/images/cn/extended_star.png)


---

#### 4.	Mesh Topology

- Each node is directly connected to every other nodes in the network.
- Fault Tolerant and Scalable

##### Advantages

1.	Fault Tolerant
2.	Reliable

##### Disadvantages

1.	Issues with broadcasting messages
2.	Expensive and impractical for large networks.

![Mesh Topology](../assets/images/cn/mesh.png)



```mermaid
graph LR
    %% Nodes
    A((Node A))
    B((Node B))
    C((Node C))
    D((Node D))

    %% Full Mesh Interconnections
    A <==> B
    A <==> C
    A <==> D
    B <==> C
    B <==> D
    C <==> D



```

---

#### 5.	Hybrid Topology

![Hybrid Topology](../assets/images/cn/hybrid.png)


```mermaid
graph LR
    %% BUS TOPOLOGY SECTION
    subgraph Bus["Bus Segment"]
        direction LR
	    %% Main Backbone Cable
	    Bus1[ ] --- Bus2[ ] --- Bus3[ ] --- Bus4[ ]
	    
	    %% Drop Lines to Nodes
	    Bus1 --- B1((Node 1))
	    Bus2 --- B2((Node 2))
	    Bus3 --- B3((Node 3))
	    Bus4 --- B4((Node 4))
	
	    %% Formatting
	    style Bus1 width:0px,height:0px;
	    style Bus2 width:0px,height:0px;
	    style Bus3 width:0px,height:0px;
	    style Bus4 width:0px,height:0px;
	    linkStyle 0,1,2 stroke:#2c3e50,stroke-width:6px;
	    linkStyle 3,4,5,6 stroke:#7f8c8d,stroke-width:3px;
    end

    %% CENTRAL STAR TOPOLOGY SECTION
    SW[switch]
    subgraph Star["Star Segment"]
        direction LR 
	    SW --- SC1["Node A"]
	    SW --- SC2["Node B"]
	    SW --- SC3["Node C"]
	end

    %% Connect Bus to Star Switch
    B4 --- SW

    %% MESH TOPOLOGY SECTION
    subgraph Mesh["Mesh Segment"]
        direction LR
	    %% Nodes
	    A((Node A))
	    B((Node B))
	    C((Node C))
	    D((Node D))
	
	    %% Full Mesh Interconnections
	    A <==> B
	    A <==> C
	    A <==> D
	    B <==> C
	    B <==> D
	    C <==> D
	    
	end


    %% Connect Star Switch to Mesh Topology
    SW --- A



```
---

### Total Ports and Number of Cables

1. Star: Number of cables = n, Total ports = 2*n
2. Ring: Number of cables = n, Total ports = 2*n
3. Mesh: cables = n(n-1)/2, Total ports = n(n-1)







  
