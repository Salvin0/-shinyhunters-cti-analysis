# 🕵 ShinyHunters (G1057) — Cyber Threat Intelligence Analysis

CTI analysis of ShinyHunters conducted using free OSINT tools only.

## Overview
ShinyHunters (MITRE G1057) is a financially motivated cybercriminal collective
active since at least 2019, operating under the ShinyCorp persona. The group
targets multiple industries worldwide, stealing credentials and PII for resale
or victim extortion. ShinyHunters is associated with the broader collective
known as The Com, whose members also include Scattered Spider and LAPSUS$.

## Known Aliases
- ShinyCorp (MITRE ATT&CK)
- UNC6240 (Malpedia)
- Bling Libra (Malpedia)

## Associated Threat Actors
Part of the The Com collective, alongside Scattered Spider (G1015)
and LAPSUS$ (G1004).

## Repository Structure
- report — Full threat actor profile
- notebooks — Jupyter notebook with interactive analysis
- iocs — IOC dataset with 40+ indicators collected from OTX
- mitre — ATT&CK Navigator layer ready to import
- assets — Diagrams and visualizations

## Intelligence Sources
- MITRE ATT&CK G1057 — TTP mapping and software
- AlienVault OTX — 87 pulse reports, 40+ IOCs (IPs and domains)
- Malpedia — Aliases and group references
- VirusTotal — IOC enrichment
- AbuseIPDB — IP reputation scoring

## Methodology
This analysis follows the standard Intelligence Cycle.
Direction, Collection, Processing, Analysis, Dissemination, Feedback.
All sources used are free and publicly available.

## Disclaimer
All IOCs included are historical and publicly documented in vendor
security reports. Provided for educational and defensive purposes only.