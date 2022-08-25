# Securing Azure: The Checklist
<br>
<br>

<h2>Strategy:</h2>

💡 Understand the shared responsibility model and the chosen cloud strategy - clear delineation between our responsibility and the customer's.

<h2>**Identities and Access Management:**</h2>

✔ Manage identities using Azure Active Directory. Enable SSO to alleviate potential issues revolving around weak passwords.

✔ Minimize the number of subscription owners. No more than three (two for managing and one backup account).

✔ Azure Key Vault should be used for cryptographic keys, secrets, and certificates.

<h2>**Security and Endpoint Protection:**</h2>

✔ Azure Security Center utilization is a must; understand alerts, the secure score, and follow suggestions where appropriate. If hybrid, use Azure Defender.

✔ Keep VMs updated. Azure Security Center should be the default method to automate security updates.

✔ Restrict remote access to your VMs and use VPNs where applicable. Just In Time access reduces brute force attack exposure.

✔ Enable OS vulnerabilties recommendations - this setting provides analysis of OS-level configurations to seek out issues that often make VMs vulnerable to attacks.

✔ Enabling endpoint protection allows Azure Security Center to push endpoint protection for provisioning of all Windows VMs and helps identify malicious software.

<h2>**Networks and Encryption:**</h2>

✔ Network access must have a layered approach:

  * Azure firewall or a 3rd party virtual network appliance
  
  *  Use Network Security Groups (NSGs) for traffic filtering to and from Azure virtual networks
  
  * Apply NSGs to VM NICs to regulate traffic to and from virtual machines
  
✔ Enable encryption for data in transit and at rest where authorized.



