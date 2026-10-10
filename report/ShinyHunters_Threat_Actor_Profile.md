ShinyHunters (G1057) — Threat Actor Profile

Classification: TLP WHITE
Author: [SALVO S]
Overall Confidence: Medium-High

***************

 1. Executive Summary

ShinyHunters is a financially motivated cybercriminal collective active
since at least 2019. The group operates under the ShinyCorp persona and
is associated with the broader collective known as The Com, alongside
Scattered Spider (G1015) and LAPSUS$ (G1004).

The group targets organizations across multiple industries and geographic
regions with the primary goal of stealing credentials and personally
identifiable information (PII) for resale or extortion. ShinyHunters
has been responsible for several high-profile data breaches affecting
millions of victims worldwide.


 2. Identification

Name: ShinyHunters
MITRE ATT&CK ID: G1057
Aliases: ShinyCorp, UNC6240, Bling Libra
First Seen: 2019
Status: Active
Malpedia References: 5
OTX Pulse Reports: 87
OTX Indicators: 40+ (IPs and domains)

**********

 3. Attribution

Motivation: Financial gain
Type: Cybercriminal collective (not nation-state)
Attribution confidence: Medium
Associated collective: The Com (also known as The Community)

Unlike nation-state APT groups, ShinyHunters is not attributed to any
government or intelligence agency. The group is driven purely by
financial incentives through credential resale on underground markets
and direct extortion of victims.

4. Victimology

ShinyHunters targets organizations globally with no specific geographic
focus. The group prioritizes targets based on the value of data held
rather than geopolitical interest.

Targeted sectors:

- Technology companies
- E-commerce platforms
- Financial services
- Healthcare
- Gaming and entertainment

Primary objective: Mass collection of credentials and PII for
resale on criminal marketplaces or use in extortion campaigns.

5. Tools and Software

Tor Network
Usage: Anonymization of infrastructure and operator identity.
MITRE reference: S0183

No custom malware families have been publicly attributed to
ShinyHunters. The group primarily relies on legitimate tools,
stolen credentials, and living-off-the-land techniques.

Mandiant and Google Threat Intelligence Group (GTIG) have identified an active compromise and extortion campaign attributed to UNC6240 (ShinyHunters) targeting Oracle PeopleSoft application infrastructure. The activity was observed between May 27, 2026, and June 9, 2026 and is consistent with the exploitation of CVE-2026-35273(https://nvd.nist.gov/vuln/detail/cve-2026-35273), a critical remote code execution vulnerability (CVSS 9.8) in the Environment Management component. The exploitation of this vulnerability directly aligns with the observed targeting of Environment Management Hub (PSEMHUB) endpoints. Because this activity predates Oracle's June 10, 2026 advisory, the vulnerability was exploited as a zero-day.



*******

 6. MITRE ATT&CK Tactics

The following tactics have been documented in public reporting.

TA0043 - Reconnaissance
Gathering information about target organizations and employees
before conducting attacks.

TA0042 - Resource Development
Acquiring infrastructure and tools to support operations,
including use of anonymization services such as Tor.

TA0002 - Execution
Running malicious code or commands on compromised systems.

TA0006 - Credential Access
Primary focus of operations. Stealing credentials through
various techniques to gain access to target environments.

TA0007 - Discovery
Identifying data stores, users and systems within compromised
environments to locate high-value information.

TA0009 - Collection
Aggregating stolen credentials and PII from compromised systems
and databases for exfiltration.

TA0040 - Impact
Extortion of victims using stolen data as leverage, threatening
public release if ransom demands are not met.

---

 7. Diamond Model

Adversary: ShinyHunters (ShinyCorp persona)
            Financially motivated criminal collective
            Associated with The Com

Capability: Credential theft techniques
            Data exfiltration tools
            Tor for anonymization
            Living-off-the-land methods

Infrastructure: Tor network
               Criminal marketplace infrastructure
               Underground forums for data resale

Victim: Organizations globally
        Any sector holding high-value credentials or PII
        Technology, finance, healthcare, e-commerce, gaming



 8. Defensive Recommendations

Priority High:
- Enforce MFA on all external-facing accounts and services
- Monitor for bulk credential validation attempts
- Implement data loss prevention controls on sensitive databases
- Alert on anomalous database query volumes

Priority Medium:
- Regular dark web monitoring for leaked credentials
- Employee awareness training on social engineering
- Network segmentation to limit lateral movement
- Monitor Tor exit node traffic at the perimeter


 9. References

1. MITRE ATT&CK Group G1057
   https://attack.mitre.org/groups/G1057
2. Malpedia - ShinyHunters actor page
   https://malpedia.caad.fkie.fraunhofer.de/actor/shinyhunters
3. AlienVault OTX - ShinyHunters pulse collection
   https://otx.alienvault.com
4. MITRE ATT&CK - Scattered Spider G1015
   https://attack.mitre.org/groups/G1015
5. MITRE ATT&CK - LAPSUS$ G1004
   https://attack.mitre.org/groups/G1004
6. https://www.ic3.gov/PSA/2026/PSA260515
---

TLP WHITE - This document may be distributed freely.