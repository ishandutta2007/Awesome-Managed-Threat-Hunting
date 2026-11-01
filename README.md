# Awesome-Managed-Threat-Hunting

## Top Managed Threat Hunting Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on 24/7 Human-Led Hunting, MDR Platforms & Self-Hosted Threat Hunting Tooling*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Managed Threat Hunting**. These services and tools enable organizations to proactively search for hidden adversaries that automated detection misses—combining human expertise with telemetry analysis to find threats before they cause damage.



**Examples** include CrowdStrike Falcon OverWatch, SentinelOne Vigilance, Mandiant Managed Defense, Red Canary MDR, Huntress, Sophos Managed Threat Response, Arctic Wolf, Rapid7 Managed Threat Complete, eSentire MDR, and Secureworks Taegis (the category leaders).



**Open-source emphasis**: Managed Threat Hunting is a domain where open-source tooling is **fundamentally different from the managed service it complements**. The commercial leaders provide **human threat hunters monitoring your environment 24/7**—a service that no open-source project can replicate. What open-source *can* provide is the **tooling and frameworks that threat hunters use**: **Velociraptor** is the standout open-source endpoint visibility and response platform for large-scale hunting and forensic collection (4k+ stars, Go-based, production-ready for serious pilots) , **Security Onion** provides a free platform for threat hunting, enterprise security monitoring, and log management , and **The ThreatHunter-Playbook** offers a structured playbook of hunting techniques mapped to MITRE ATT&CK, designed to help hunters develop hypotheses and reduce false positives . The critical caveat: **open-source gives you the tools a hunter uses, not the hunter**—managed threat hunting is a service, and organizations without dedicated security staff should evaluate MDR providers rather than attempting to self-hunt with open-source tools alone.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Managed Detection and Response (MDR) and Threat Hunting market is estimated at approximately $5.0B to $6.2B and is projected to expand at a CAGR of 18%–23% toward $15B–$25B over the next decade. The sector remains moderately fragmented: while platform leaders dominate telemetry ingestion, delivery of 24/7 human-led hunting and SOC operations is shared among cybersecurity giants, specialized pure-play MDR vendors, and regional MSSPs.

## SaaS/Hosted Platforms

| Platform | Valuation / Revenue | Starting Pricing | Free Tier / Free Trial Limits | Description |
|---|---|---|---|---|
| **[CrowdStrike Falcon OverWatch](https://www.crowdstrike.com/)** | ~$85B–$100B+ Market Cap | From $184.99/device/year ($19.99/device/month) for Falcon Enterprise (bundled with OverWatch hunting); MDR add-on from ~$42/endpoint/month | 15-day free trial (up to 50 endpoints with full Falcon platform functionality) | Proactive managed threat hunting across Falcon endpoint telemetry where human elite hunters hunt 24/7 and deliver actionable escalations. |
| **[SentinelOne Vigilance](https://www.sentinelone.com/)** | ~$8.5B Market Cap | Vigilance MDR add-on from ~$15–$50/endpoint/year (layered on Singularity Complete at ~$180/endpoint/year; combined ~$15–$20/endpoint/month) | 30-day proof-of-concept / evaluation trial (guided evaluation with full autonomous EDR & hunting access) | 24/7 managed threat hunting and triage add-on to Singularity XDR/EDR, responding and neutralizing threats on behalf of customers. |
| **[Mandiant Managed Defense](https://www.mandiant.com/)** | $5.4B (Acquired by Google) | Starting tier from ~$80,000–$90,000/year for enterprise baseline environments | No free trial for Managed Defense (human SOC service); 14-day trials available for standalone Mandiant Threat Intelligence & Attack Surface modules | Premier front-line MDR service backed by Mandiant incident responders and Google SecOps, integrating third-party EDR telemetry with proprietary adversary intel. |
| **[Arctic Wolf](https://arcticwolf.com/)** | $4.3B Valuation | From $44,000/year (MDR Basic for up to 100 users, ~$36.67/user/month); volume tiers at ~$190–$260/user/year | No self-service free trial; vendor-led technical scoping, architecture evaluation, and live customized SOC demo | Concierge Security Team delivery model providing 24/7 monitoring, managed threat hunting, log retention, and strategic risk guidance. |
| **[Sophos Managed Threat Response](https://www.sophos.com/)** | $3.9B (Acquired by Thoma Bravo; >$1B Rev) | From ~$240/endpoint/year (~$20/endpoint/month) for Sophos MDR Complete; MDR Essentials entry at ~$170/endpoint/year | 30-day free trial (full access to Sophos Central management, Intercept X Advanced with XDR) | 24/7 human-led threat hunting, investigation, and neutralization service natively integrated with Sophos endpoint, firewall, and identity products. |
| **[Huntress](https://www.huntress.com/)** | $1.55B Valuation | From $8.99/endpoint/month for Managed EDR (~$7.00–$7.99/endpoint/month at standard mid-tier volume) | 14-day free trial (full-featured unlimited endpoint deployment for Managed EDR/ITDR/SIEM; 21 days for SAT) | Human-led MDR designed for mid-market and MSPs, pairing lightweight agent detection with 24/7 human threat hunter investigation and remediation playbooks. |
| **[eSentire MDR](https://www.esentire.com/)** | $1.1B Valuation | From ~$60–$100/endpoint/year for smaller deployments (50–200 endpoints); drops to ~$40–$80/endpoint/year at scale | No self-service free trial; live proof-of-value (POV) and interactive threat investigation demo | 24/7 multi-signal Managed Detection and Response focusing on rapid human-led threat containment, ATLAS AI curation, and embedded DFIR capabilities. |
| **[Rapid7 Managed Threat Complete](https://www.rapid7.com/)** | ~$850M Market Cap (~$850M ARR) | From ~$15–$22/asset/month (typically structured around a 500-asset baseline minimum, starting ~$73,000–$90,000/year) | 30-day free trial (available for underlying InsightIDR SIEM/XDR and InsightVM platforms) | End-to-end MDR bundling InsightIDR cloud SIEM, unlimited InsightVM vulnerability management, and 24/7 SOC threat hunting. |
| **[Secureworks Taegis](https://www.secureworks.com/)** | $859M (Acquired by Sophos) | Managed XDR/MDR from ~$100–$130/endpoint/year (standalone Taegis XDR platform entry at ~$43,000/year for ~1,000 endpoints) | 14-day free trial (Taegis XDR evaluation tenant supporting limited host agents and cloud telemetry connectors) | Open XDR architecture with managed detection, adversary threat hunting, and comprehensive cross-vendor telemetry correlation. |
| **[Red Canary MDR](https://redcanary.com/)** | $675M (Acquired by Zscaler) | From $120/endpoint/year ($10/endpoint/month) base subscription; $10/unit overage; identity coverage at $100/account/year | No public self-service free trial; customized proof-of-value (POV) with environment telemetry mapping | Pioneer in detection engineering and human-led MDR, ingesting raw endpoint telemetry to conduct continuous 24/7 adversary hunting and threat neutralization. |

## Open-Source GitHub Projects



### Endpoint Visibility & Response Platforms (Velociraptor)



- **[Velociraptor](https://github.com/Velocidex/velociraptor)**  

  The **leading open-source endpoint visibility and response platform for threat hunting** (Go, 4k+ GitHub stars, 626 forks, active development through 2026) . Features: **VQL (Velociraptor Query Language)** for custom queries; **artifact-based collection** (version-controlled YAML+VQL); **live response actions** (kill process, isolate host, dump memory); **VFS (Virtual File System)** for interactive endpoint inspection; **hunts across thousands of hosts** with offline endpoint pickup; and **client-side tracing** for debugging hung collections. **Production readiness**: evaluated as "production-ready for a serious pilot" with strong community momentum and frequent updates . **Best for organizations with security staff** wanting to conduct their own hunting and forensic collection at scale—but it requires operational expertise and does not provide the 24/7 human monitoring of managed services.



### Threat Hunting Platforms & Playbooks



- **[Security Onion](https://github.com/Security-Onion-Solutions/securityonion)**  

  A free and open platform for **threat hunting, enterprise security monitoring, and log management** . Includes interfaces for alerting, dashboards, hunting, PCAP, detections, and case management, along with tools such as osquery, CyberChef, Elasticsearch, Logstash, Kibana, Suricata, and Zeek. **Best for organizations wanting an integrated open-source platform** for hunting and monitoring—but it is infrastructure you operate, not a managed hunting service.



- **[The ThreatHunter-Playbook](https://github.com/OTRF/ThreatHunter-Playbook)**  

  A **threat hunter's playbook** to aid the development of techniques and hypotheses for hunting campaigns (by Roberto Rodriguez @Cyb3rWard0g) . Provides specific chains of events at the host level (leveraging Sysmon and Windows Events logs) so hunters can develop queries or alerts in their preferred tool—Splunk, ELK, Sigma, GrayLog, etc. Follows the **MITRE ATT&CK framework** structure and includes hunting notes and references to back up each technique. **Best for threat hunters** wanting a structured starting point for hypothesis development—but it is a knowledge resource, not a platform or automated service.



### Additional Strong Open-Source Options



- **Wazuh** — Open-source SIEM/XDR platform (GPL-2.0) with log analysis, file integrity monitoring, vulnerability detection, and MITRE ATT&CK mapping; widely used as the foundation for SOC home labs and threat hunting exercises . **Best for teams wanting a self-hosted SIEM foundation** for hunting—but it is detection infrastructure, not a managed hunting service.

- **Matano** — Open-source **security data lake** for threat hunting, detection & response, and cybersecurity analytics at petabyte scale on AWS; supports custom detections in Python and log transformation via VRL . **Best for AWS-centric organizations** wanting a scalable data lake for hunting—but it is infrastructure requiring deployment and management.

- **Malwoverview** — First response tool for threat hunting across VirusTotal, Hybrid Analysis, URLHaus, Polyswarm, Malshare, Alien Vault, Malpedia, Malware Bazaar, ThreatFox, Triage, IPInfo, Shodan, AbuseIPDB, GreyNoise, URLScan.io, Whois/RDAP, NIST, and VulnCheck . **Best for individual hunters** wanting quick IOC enrichment—not a platform or service.



**Frameworks for building custom systems**: For **endpoint hunting and forensic collection at scale**, Velociraptor provides the most complete open-source platform . For an **integrated hunting and monitoring platform**, Security Onion . For **structured hunting hypotheses and techniques**, The ThreatHunter-Playbook . For **SIEM-based hunting foundations**, Wazuh . **No open-source project provides managed threat hunting**—that is a human service. Organizations requiring 24/7 hunting should evaluate commercial MDR providers (Huntress, Red Canary, CrowdStrike OverWatch) rather than attempting to self-hunt with open-source tools alone.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Managed threat hunting platforms handling security telemetry must comply with organizational security policies and privacy regulations; **self-hosted hunting tools require skilled operators**—Velociraptor and Security Onion are powerful but demand expertise to configure and interpret.

- **Open-source threat hunting is fundamentally different from managed threat hunting**—open-source provides the *tools* (Velociraptor, Security Onion, The ThreatHunter-Playbook) , but **managed threat hunting is a service** delivered by human analysts 24/7. Organizations without dedicated security staff should not assume that deploying open-source tools constitutes "managed" hunting—they should evaluate MDR providers like Huntress, Red Canary, or CrowdStrike OverWatch. Open-source is best suited for organizations with existing SOC teams who want to augment their capabilities.

- Verify license terms for commercial use; Velociraptor is open-source (check repository) , Security Onion is open-source , and The ThreatHunter-Playbook is a community resource .



---



**Made for SOC analysts, threat hunters, and organizations choosing their hunting and MDR strategy.**  

Let's make threat hunting more open at the tooling layer, but with clear eyes about the human expertise and 24/7 coverage that managed services provide.
