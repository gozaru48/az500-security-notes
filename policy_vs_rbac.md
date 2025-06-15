# Azure Policy vs RBAC: Key Differences and Use Cases

## Overview

Azure provides two major tools for managing resource governance and access control: **Azure Policy** and **Role-Based Access Control (RBAC)**. Understanding their differences and applications is essential for ensuring security and compliance in cloud environments.

---

## Azure Policy

- Enforces organizational rules and compliance.
- Prevents non-compliant resource creation or updates.
- Example: Prohibit creation of public IP addresses in a specific subscription.

### Common Scenarios
- Enforcing tags on resources
- Restricting VM SKUs
- Denying resource deployments in non-approved regions

---

## RBAC (Role-Based Access Control)

- Manages *who* has *what* access to *which* Azure resources.
- Assigns roles at different scopes (subscription, resource group, resource).

### Common Scenarios
- Reader role for audit teams
- Contributor role for DevOps engineers
- Custom roles for granular access

---

## Key Differences

| Feature        | Azure Policy                          | RBAC                                |
|----------------|----------------------------------------|-------------------------------------|
| Purpose        | Enforce compliance and governance      | Assign access permissions           |
| Scope          | Organization-wide or specific scopes   | Resource-specific                   |
| Action         | Allow/Deny resource operations         | Grant/Restrict access               |
| Enforcement    | Preventative (pre-deployment)          | Access control (post-deployment)    |

---

## When to Use

- Use **Azure Policy** to control the *what* and *how* of resources.
- Use **RBAC** to control *who* can do *what*.

---

## Notes

Combining both tools provides layered security and effective resource management.
