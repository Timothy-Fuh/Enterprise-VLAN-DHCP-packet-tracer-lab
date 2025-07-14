# Enterprise-VLAN-DHCP-packet-tracer-lab
## 📘 Overview

This project simulates a corporate office network environment using **Cisco Packet Tracer**. The design features **three departmental VLANs** — Sales, Marketing, and HR — each segmented for security and scalability. It demonstrates **inter-VLAN routing**, **dynamic IP assignment via DHCP**, and the integration of a statically addressed **data server**. The goal is to mirror a realistic small- to medium-sized business LAN infrastructure.

---

## 🧱 Network Topology

- 🔹 **3 VLANs**: 
  - VLAN 10 – Sales  
  - VLAN 20 – Marketing  
  - VLAN 30 – HR

- 🔹 **Multilayer Switch (MLS)**:
  - Acts as default gateway for all VLANs via SVIs
  - Performs inter-VLAN routing
  - Functions as DHCP server for all VLANs

- 🔹 **Access Layer**:
  - 3 access switches (one per VLAN)
  - Access ports for user workstations
  - Trunk ports connected to the MLS

- 🔹 **Server**:
  - Connected to the MLS via access port
  - Statically assigned IP (outside DHCP pool)
  - Used for testing and future service hosting

---

## ⚙️ Features Demonstrated

- ✅ VLAN segmentation for department isolation
- ✅ Trunking between access switches and MLS
- ✅ Inter-VLAN routing using Switch Virtual Interfaces (SVIs)
- ✅ DHCP pools for each VLAN with IP exclusions
- ✅ Static IP configuration for critical devices
- ✅ Simulation Mode used to visualize PDU movement

---

## 🧪 Technologies Used

- Cisco Packet Tracer (version XX)
- Cisco IOS CLI (Catalyst 3560 syntax)
- Networking concepts: VLANs, DHCP, Trunking, Inter-VLAN Routing

---

## 🚀 How to Run the Simulation

1. Open the `.pkt` file in Cisco Packet Tracer.
2. Switch to **Simulation Mode**.
3. Use the **"Add Simple PDU"** tool to test connectivity between VLANs.
4. Open **Command Prompt** on PCs to test:
   - IP configuration
   - DHCP assignment
   - Ping across VLANs and to server

---


## 📚 What I Learned

- How to properly segment traffic using VLANs
- Setting up and troubleshooting inter-VLAN routing on a multilayer switch
- Assigning static vs dynamic IPs in a managed enterprise network
- Identifying and resolving common errors like:
  - Native VLAN mismatches
  - Trunk encapsulation issues
  - Inactive SVIs

---

## 🧩 Future Improvements

- Add ACLs to restrict access between departments
- Introduce a guest VLAN with wireless access
- Move DHCP service to a dedicated server
- Simulate remote branch with static or dynamic routing
