# ITT633-Network-Automation-using-Ansible

# Project Title: Automating Multiaccess OSPFv2 Using Ansible

## 📌 Project Overview
This project demonstrates how **Ansible** can be used to automate the deployment, verification, and management of **OSPFv2** in a **broadcast multiaccess network**. The automation replaces manual router configuration and helps ensure consistency, reliability, and faster network operations.

The network topology consists of multiple Cisco routers connected to the same LAN segment, where OSPF elects a **Designated Router (DR)** and a **Backup Designated Router (BDR)**.

---

## 🎯 Objectives
- Automate OSPFv2 configuration using Ansible
- Verify OSPF neighbor adjacency and routing
- Demonstrate DR/BDR election in a multiaccess network
- Perform controlled OSPF changes using automation
- Save verification outputs for auditing and reporting

---

## 🧱 Network Topology
- 4 Cisco IOS routers
- Broadcast multiaccess LAN (10.10.10.0/24)
- OSPF Area 0 (Backbone)
- Loopback interfaces used as Router-ID

---

## ⚙️ Automation Approach
- Tool: **Ansible**
- Connection: SSH (`network_cli`)
- Modules used:
  - `cisco.ios.ios_config`
  - `cisco.ios.ios_command`

Automation tasks are divided into:
1. OSPF Deployment
2. OSPF Verification
3. Change Control (DR/BDR manipulation)

---

## ✅ Expected Outcome
- All routers form FULL OSPF adjacency
- DR and BDR are elected correctly
- OSPF routes are exchanged successfully
- Network changes are applied consistently using automation

---

## 🚀 Future Improvements
- Add rollback mechanism
- Multi-area OSPF support
- Structured output parsing
- CI/CD integration
