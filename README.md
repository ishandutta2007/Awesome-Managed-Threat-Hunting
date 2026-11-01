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

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[CrowdStrike Falcon OverWatch](https://www.crowdstrike.com/)**  

  Managed threat hunting service that proactively searches for adversary activity across the Falcon platform's telemetry; human hunters investigate and escalate confirmed threats with full context.



- **[SentinelOne Vigilance](https://www.sentinelone.com/)**  

  Managed threat hunting add-on to SentinelOne's autonomous EDR; human analysts hunt for threats and respond on the customer's behalf.



- **[Mandiant Managed Defense](https://www.mandiant.com/)**  

  Managed detection and response from Mandiant's incident response teams; combines front-line threat intelligence with continuous monitoring and hunting.



- **[Red Canary MDR](https://redcanary.com/)**  

  Managed detection and response platform with a focus on detection engineering and threat hunting; provides 24/7 SOC coverage.



- **[Huntress](https://www.huntress.com/)**  

  Managed detection and response built for small businesses and MSPs; combines endpoint detection with a **human threat hunting team** that investigates and responds to incidents.



- **[Sophos Managed Threat Response](https://www.sophos.com/)**  

  Managed threat hunting, detection, and response service integrated with Sophos endpoint protection.



- **[Arctic Wolf](https://arcticwolf.com/)**  

  Managed detection and response with 24/7 SOC coverage and threat hunting.



- **[Rapid7 Managed Threat Complete](https://www.rapid7.com/)**  

  Managed detection and response combining InsightIDR with Rapid7's SOC team.



- **[eSentire MDR](https://www.esentire.com/)**  

  Managed detection and response service with 24/7 threat hunting.



- **[Secureworks Taegis](https://www.secureworks.com/)**  

  Cloud-native XDR platform with managed detection and response services.



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
