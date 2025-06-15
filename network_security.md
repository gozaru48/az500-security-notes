# Network Security in Azure

This document summarizes key components and differences among major Azure network security features, including NSG, Azure Firewall, and Azure Bastion.

---

## Network Security Group (NSG)

- Operates at OSI Layer 3 and 4
- Controls inbound and outbound traffic using allow/deny rules
- Can be applied to subnets and individual NICs
- Stateless by design

---

## Azure Firewall

- Fully stateful, centralized network firewall service
- Supports both application rules (L7) and network rules (L3/L4)
- Integrates with Azure Monitor for logging and diagnostics
- Provides advanced capabilities such as deep packet inspection, DNAT, and SNAT
- Suitable for larger environments or centralized traffic control

---

## Azure Bastion

- Enables secure RDP/SSH access without exposing virtual machines to public IP addresses
- Removes the need to manage NSG rules for administrative access
- Works entirely through the Azure Portal
- Ideal for jump box–style secure access without agent installation

---

## Use Case Summary

| Feature         | Layer/State | Purpose                                      | Notes                                 |
|----------------|-------------|----------------------------------------------|---------------------------------------|
| NSG             | L3/L4, stateless | Basic traffic filtering at subnet/NIC level | Lightweight, low-cost                 |
| Azure Firewall  | L3–L7, stateful | Advanced traffic control and logging        | Centralized, more expensive           |
| Azure Bastion   | N/A         | Secure access to VMs via browser            | No public IP exposure, portal-based   |

---

All information is based on my preparation for the Microsoft AZ-500 certification and intended to support ACS documentation and real-world reference.
