# My Notes — Okeke Marycynthia

## Key Concepts I Learned

Azure Key Vaults & Defense-in-Depth
Secure Secret Management: Storing sensitive credentials, connection strings, and keys in Azure Key Vault is a fundamental requirement for defense-in-depth, preventing single-point-of-compromise scenarios where one exposed secret escalates into a full workload breach.

Proactive Security: Implementing automated key rotation, centralized secret versioning, and anomaly monitoring via Microsoft Defender for Cloud significantly reduces the attack surface.
Certificate Integration: Integrated Key Vault certificates can be provisioned through partnered Certificate Authorities (specifically DigiCert and GlobalSign), which requires maintaining external accounts alongside Microsoft resources.

Authorization Methods: Azure RBAC vs. Legacy Access Policies
Azure RBAC (Recommended): Utilizes a unified, modern authorization model across the Azure ecosystem. RBAC role assignments are highly granular, fully auditable, restricted to specific scopes, and integrate seamlessly with Azure Managed Identities.
Legacy Access Policies: Uses a segregated, vault-specific permission model. This approach is highly prone to configuration drift over time and lack of uniformity, though it remains visible in legacy environments.

Core Key Vault Assets
Key Vault manages three distinct secure asset types:
1. Secrets: Plaintext configuration strings, database connection strings, passwords, and API keys.
2. Keys: Cryptographic keys utilized directly for encryption, decryption, and digital signing operations.
3. Certificates: X.509 certificates alongside automated lifecycle management and renewal tools.

Managed Identities in Azure
Azure utilizes managed identities to eliminate the need for hardcoded credentials, categorized into two types:
1. System-Assigned: Automatically created and tightly coupled to a single, specific Azure resource. It is deleted automatically when the resource is destroyed.
2. User-Assigned: Created as a standalone, reusable Azure resource that can be assigned to multiple independent services simultaneously.

Data Protection & Network Security Controls
To safeguard Key Vault data from both unauthorized exfiltration and accidental deletion, three primary layers of defense are enforced:
1. Firewalls & Network Access Control: Restricting public endpoints to specific virtual networks (VNets) or utilizing private endpoints to isolate traffic.
2. Soft-Delete & Purge Protection: Safeguarding against accidental or malicious deletions. Soft-delete retains deleted vaults for a specified window, while purge protection prevents permanent deletion of those vaults during that period.
3. Operational Guardrails: Applying administrative locks and governance policies to prevent unauthorized configuration changes.
-
-
-

---

## Lab / Hands-On Work

<!-- Describe what you did in the lab. Include steps, commands, or screenshots descriptions -->

### What I did


### What happened / Result


### Challenges I faced


---

## My Takeaways

<!-- What was most valuable to you personally from this session? -->


---

## Questions I Still Have

<!-- Anything you want to follow up on or ask the mentor -->

-
-

---

## Resources I Found Useful

<!-- Any links, docs, or Microsoft Learn modules you found helpful -->

-

---

*Submitted by: Marycynthia Okeke · Nechy_Okeke*
