# 🔐 Network Security in Azure

## 🔸 NSG (Network Security Group)

- Layer: OSI Layer 3 & 4
- Controls inbound/outbound traffic via allow/deny rules
- Applied to: Subnets and NICs
- Stateless

## 🔸 Azure Firewall

- Fully stateful, centralized network firewall
- Supports application rules and network rules
- Can log to Azure Monitor
- More advanced than NSG (deep inspection, DNAT/SNAT)

## 🔸 Azure Bastion

- Secure RDP/SSH without exposing public IP
- No need to manage NSG rules for remote desktop
- Works directly via Azure Portal
