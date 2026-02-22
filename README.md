# ZT-Policy-Profile.md
This assignment shows how Zero Trust security protects sensitive HR data. It explains how the system checks the user, the device, and the network before allowing access. The goal is to make sure only authorized employees can see important information.
# ZTA Component Definitions

## Policy Engine (PE)
The Policy Engine is the decision-making component of a Zero Trust Architecture. It evaluates access requests by analyzing security signals such as user identity, device posture, and network context. Based on predefined policies, the Policy Engine decides whether access to a protected resource should be granted or denied.

## Policy Administrator (PA)
The Policy Administrator is responsible for executing the decision made by the Policy Engine. Once access is approved, the PA configures permissions, credentials, or session parameters and prepares the environment so that access can be established securely.

## Policy Enforcement Point (PEP)
The Policy Enforcement Point acts as the gatekeeper between the user and the protected resource. It enforces the access decision by allowing or blocking traffic based on instructions received from the Policy Administrator.

---

# Core Principle Application

## Chosen Principle: Verify Explicitly

The Zero Trust principle of Verify Explicitly requires that every access request be evaluated using multiple security signals before access is granted. At the Golden State Water Treatment Facility, the Policy Engine enforces this principle when an employee attempts to access the HR Employee PII Database.

For example, the Policy Engine verifies the user's authenticated identity, checks whether the device meets security compliance standards, and confirms that the request originates from an approved network location. Only if all conditions are satisfied does the Policy Engine approve access to the sensitive HR data.

---

# Simplified Policy Table

| Policy Requirement (Signal) | Condition to be Met by User | Action if Condition is Met |
|----------------------------|-----------------------------|----------------------------|
| User Identity | User is authenticated using multi-factor authentication (MFA) | Grant Access |
| Device Posture | Device is company-managed and fully patched | Grant Access |
| Network Context | Access request originates from the facility’s secure network or approved VPN | Grant Access |

---

# Git Repository Metadata

Project: Lab 6 - Zero Trust Policy  
Filename: ZT-Policy-Profile.md  
Commit Message: Initial commit of Zero Trust Policy Profile for HR PII database  
GitHub URL: [ZT-Policy-Profile Repository](https://github.com/N-alaiban/ZT-Policy-Profile](https://github.com/N-alaiban/ZT-Policy-Profile.md.git)
Due Date: March 2, 2026
