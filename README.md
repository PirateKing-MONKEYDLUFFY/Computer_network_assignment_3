# Computer_network_assignment_3
### Assignment 3 – Computer Networks Lab

**Submitted by:** Vaibhav Kedia  
**Roll Number:** 2301730096  
**Program:** B.Tech CSE (AI/ML), Section B  
**Course:** Computer Networks Lab  

---

### 📌 Routing Tables

#### 1. Routing Information Protocol (RIP)

**🔗 Copper Straight-Through Connections**

| From | To | Interface Connection |
| :--- | :--- | :--- |
| PC0 | S1 | Fa0/1 |
| PC1 | S1 | Fa0/2 |
| S1 | R0 | Fa0/24 → Fa2/0 |
| PC2 | S2 | Fa0/1 |
| PC3 | S2 | Fa0/2 |
| S2 | R1 | Fa0/24 → Fa2/0 |
| PC4 | S3 | Fa0/1 |
| PC5 | S3 | Fa0/2 |
| S3 | R2 | Fa0/24 → Fa2/0 |

**🔌 Serial DTE Connections**

| From | To | Interface Connection |
| :--- | :--- | :--- |
| R0 | R1 | Se0/0 ↔ Se1/0 |
| R1 | R2 | Se0/0 ↔ Se1/0 |

---

### 🌐 Network Design

The network topology is created using **Cisco Packet Tracer** and includes:
*   **3 Routers** (R0, R1, R2)
*   **3 Switches** (S1, S2, S3)
*   **Multiple PCs** (end devices)

Each router connects to a switch, forming three separate LANs. The routers are interconnected using serial DTE links, allowing communication between different networks. IP addresses are assigned to all devices, and routing protocols (RIP and OSPF) are configured to enable network communication.

**✅ Design Highlights**
*   Proper network segmentation
*   Efficient inter-LAN communication
*   Scalable architecture for future expansion

---

### ⚖️ RIP vs OSPF (Simulation Comparison)

#### 1. ⏱️ Convergence Time
*   **RIP** converges slowly due to periodic updates.
*   **OSPF** converges faster using link-state updates.
*   👉 **Conclusion:** OSPF is faster than RIP.

#### 2. 📊 Routing Metric
*   **RIP** uses hop count.
*   **OSPF** uses cost (based on bandwidth).
*   👉 **Conclusion:** OSPF provides better path selection.

#### 3. ⚙️ Efficiency
*   **RIP** sends full routing tables periodically.
*   **OSPF** sends updates only when changes occur.
*   👉 **Conclusion:** OSPF is more efficient.

#### 4. 📈 Scalability
*   **RIP** is suitable for small networks (max 15 hops).
*   **OSPF** supports large and complex networks.
*   👉 **Conclusion:** OSPF is more scalable.

---

### 📎 Tools Used
*   Cisco Packet Tracer

---

### 📌 Summary
This assignment demonstrates the implementation of RIP and OSPF routing protocols and highlights their differences in terms of convergence speed, efficiency, and scalability through simulation.
