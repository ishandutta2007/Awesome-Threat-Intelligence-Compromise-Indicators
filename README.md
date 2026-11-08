# Awesome-Threat-Intelligence-Compromise-Indicators

# Awesome Threat Intelligence & Compromise Indicators

> A curated list of top Threat Intelligence and Compromise Indicator platforms — both SaaS/Hosted commercial solutions and open-source alternatives for collecting, enriching, and operationalizing indicators of compromise (IOCs) and adversary intelligence.  
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Recorded Future](#recorded-future)
  - [Mandiant Threat Intelligence](#mandiant-threat-intelligence)
  - [CrowdStrike Falcon X](#crowdstrike-falcon-x)
  - [Microsoft Threat Intelligence](#microsoft-threat-intelligence)
  - [Palo Alto Unit 42](#palo-alto-unit-42)
  - [Cisco Talos](#cisco-talos)
  - [Flashpoint](#flashpoint)
  - [ThreatConnect](#threatconnect)
  - [Anomali](#anomali)
  - [IntSights](#intsights)
- [Open-Source Software](#-open-source-software)
  - [MISP](#misp)
  - [OpenCTI](#opencti)
  - [TheHive & Cortex](#thehive--cortex)
  - [vamp-darkweb-intel](#vamp-darkweb-intel)
  - [AdversaryGraph](#adversarygraph)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Threat Intelligence and Compromise Indicator platforms. These are not open-source but are included as reference points for feature comparison.

### Recorded Future
**Type:** Real-time threat intelligence with AI-powered workflows  
Recorded Future provides real-time monitoring across open, technical, deep, and dark web sources, with over 200 network intelligence points. The platform identifies which adversaries are running targeted attacks, which campaigns are active, and which vulnerabilities are currently weaponized. Features include agent-based processing that turns vulnerability signals into actionable detection signatures in under 30 minutes, priority-based vulnerability patching using real-time exploitation data, malware analysis with MITRE ATT&CK mapping, and pre-written YARA, Snort, and Sigma rules. The platform emphasizes threat maps tailored to each organization and automated correlation of detections across the security stack [citation:4].

### Mandiant Threat Intelligence
**Type:** Frontline intelligence from incident response  
Mandiant provides threat intelligence derived from frontline incident response and breach intelligence. The platform offers alert prioritization and triage using up-to-the-minute actor, malware, and vulnerability tracking, with MITRE ATT&CK-based actor behavior insights. It includes access to open-source indicators with Mandiant confidence scoring, vulnerability views with exploit ratings, and finished intelligence reports covering cyber crime, espionage, and strategic analysis. The Security Operations subscription correlates SOC alerts with Mandiant and OSINT indicators, while the Fusion tier provides full unlimited access to ongoing, past, and predictive threat activity [citation:5].

### CrowdStrike Falcon X
**Type:** Adversary intelligence integrated with endpoint telemetry  
Falcon X provides detailed threat intelligence for adversaries and campaigns, with complete actor profiles including kill chain information, targets, CVEs in use, and indicators. Features include automatic analysis for quarantined files, IOC generation that can be downloaded and imported into existing TIPs or hunting toolkits, malware searches for related IOCs and YARA rules, and weekly threat intelligence reporting. APIs and SIEM integrations are available, with community feeds including Snort, Suricata, and YARA maintained by CrowdStrike analysts [citation:6].

### Microsoft Threat Intelligence
**Type:** Intelligence embedded across Microsoft security products  
Microsoft's threat intelligence is deeply integrated across its security ecosystem, with the Microsoft Threat Intelligence Center (MSTIC) analyzing over 65 trillion signals daily from Azure, Office 365, Windows, and other sources. MSTIC tracks nation-state actors, monitors the dark web, and collaborates with law enforcement and industry partners. Intelligence is directly integrated into Microsoft 365 security products, enabling rapid updates to block emerging campaigns across all tenants. Human expert analysis is combined with machine learning and AI for complex campaign discovery [citation:7].

### Palo Alto Unit 42
**Type:** Threat research and incident response intelligence  
Unit 42 is Palo Alto Networks' threat intelligence and incident response team, publishing research on APT groups, malware campaigns, and emerging threats. The 2026 Unit 42 Incident Response Report analyzed over 750 major incidents, finding that attackers are using AI across the attack lifecycle, with attack speed quadrupling in one year and initial compromise-to-data-theft time reduced to as fast as 72 minutes. Identity weaknesses were exploited in 89% of incidents, and 87% of attacks spanned multiple attack surfaces [citation:8].

### Cisco Talos
**Type:** Threat intelligence and research from Cisco  
Cisco Talos is one of the largest commercial threat intelligence teams, publishing research on APT groups including UAT-11985, UAT-7810, UAT-8302, UAT-4356, and others. Talos tracks sophisticated China-nexus and other APT actors targeting government entities, telecommunications infrastructure, and critical systems. Intelligence is integrated into Cisco security products and published through the Talos blog [citation:9].

### Flashpoint
**Type:** Primary-source threat intelligence with dark web focus  
Flashpoint provides primary-source intelligence from criminal communities, with 2026 capabilities including threat-informed External Attack Surface Management (EASM) that maps discovered assets to proprietary vulnerability intelligence, Business-Aligned Priority Intelligence Requirements (PIRs) that tie investigations to business risk, and a Managed Attribution Browser for safe underground research. The platform emphasizes operationalizing intelligence by connecting adversary activity to specific organizational assets [citation:10].

### ThreatConnect
**Type:** Threat and risk informed defense platform  
ThreatConnect contextualizes, prioritizes, and operationalizes threat intelligence through an integrated suite. TI Ops aggregates, enriches, and analyzes intelligence from 300+ OSINT, commercial, and internal sources, with AI-curated intelligence requirements and MITRE ATT&CK-driven detection rules mapped to each client's threat model. Polarity provides real-time data correlation, while Risk Quantifier analyzes and quantifies the financial impact of cyber risks. The platform serves more than 250 enterprises [citation:11].

### Anomali
**Type:** Intelligence-driven decisioning layer  
Anomali ThreatStream Next-Gen makes threat intelligence the active decisioning layer inside security workflows, validated at 300 times faster than traditional investigation workflows across 50 enterprise deployments. Features include Priority Intelligence Requirements automation, Command Center for prioritized threat views, Intelligence Search with AI-generated context, Case Management, and Reporting. Agentic AI capabilities include autonomous triage, scoring, and investigation steps, with autonomous response levels in development [citation:12].

### IntSights
**Type:** External threat protection (Rapid7)  
IntSights (acquired by Rapid7) provides external threat detection with deep and dark web monitoring, network traffic analysis, and exposure monitoring. Users praise its dark web search capabilities for tracking logins for sale and its ease of use, though some note quality has declined since the acquisition and customization options are limited for large organizations [citation:13].

---

## 🟩 Open-Source Software

Self-hosted, community-driven Threat Intelligence and Compromise Indicator tools. The open-source ecosystem is anchored by MISP and OpenCTI as the foundational platforms, with complementary tools for case management, enrichment, and specialized analysis.

### MISP
**Stack:** PHP / MySQL | **License:** AGPL-3.0  
MISP (Malware Information Sharing Platform) is the most widely deployed open-source threat intelligence platform, focused on **IOC correlation and sharing**. It stores indicators of compromise (IPs, domains, hashes, URLs), correlates them across events, and enables sharing between organizations and communities. MISP supports STIX and TAXII interoperability, with the platform serving as the backbone for many national and sector-specific threat sharing communities. It integrates with OpenCTI for bidirectional sync, with TheHive for case creation, and with SIEMs for real-time IOC push [citation:2].  
**Best for:** Organizations needing a proven, community-standard platform for IOC collection, correlation, and intelligence sharing with partners and sector communities.

### OpenCTI
**Stack:** Node.js / Python / Elasticsearch / Redis / RabbitMQ | **License:** Apache-2.0  
OpenCTI is the leading open-source **knowledge graph platform** for cyber threat intelligence, built on the STIX 2.1 data model. It structures intelligence around actors, campaigns, intrusion sets, malware, tools, vulnerabilities, and indicators, enabling analysts to explore relationships between entities. OpenCTI provides a web interface for analysis, connectors to ingest from MISP and other sources, and bidirectional sync with MISP. The platform is designed for analyst workflows, with dashboards, investigation views, and integration with TheHive for response actions [citation:2].  
**Best for:** CTI teams wanting a structured, STIX-native knowledge graph for threat actor and campaign analysis, paired with MISP for IOC management.

### TheHive & Cortex
**Stack:** Scala / Elasticsearch / Docker | **License:** AGPL-3.0  
TheHive is an open-source **security incident response platform** that integrates with MISP and OpenCTI for case management and response. Cortex provides automated **enrichment and analysis** of observables (IOCs) using analyzers for VirusTotal, Shodan, AbuseIPDB, and many others. Together, they complete the open-source TIP workflow: MISP/OpenCTI for intelligence collection and analysis, TheHive for case creation from high-confidence indicators, and Cortex for automated enrichment of case observables [citation:2].  
**Best for:** SOC and CSIRT teams wanting to operationalize threat intelligence with case management and automated IOC enrichment, completing the open-source TIP stack.

### vamp-darkweb-intel
**Stack:** Python (stdlib + rich) | **License:** Open Source  
vamp-darkweb-intel is a threat intelligence and dark web research CLI that queries a target (domain, IP, hash, or URL) across multiple public feeds in parallel. Sources include ThreatFox (IOC/C2), URLhaus (malware distribution), MalwareBazaar (samples), RansomLook and Ransomware.live (ransomware victims), GreyNoise Community (scanner context), Shodan InternetDB (ports/CVEs), AlienVault OTX, and Have I Been Pwned (with API key). The **correlation engine** escalates severity when two or more independent sources flag the same indicator. Works without API keys using free public feeds, with exports to JSON, HTML, Markdown, and CSV, and exit codes suited for CI/CD pipelines [citation:3].  
**Best for:** Analysts and security engineers wanting a zero-dependency CLI for rapid IOC investigation across multiple free feeds, without deploying a full TIP.

### AdversaryGraph
**Stack:** (Check repository) | **License:** Open Source  
AdversaryGraph is a self-hosted AI threat intelligence platform focused on **ATT&CK analysis and adversary profiling**. Version 2.5 adds local LLM support, DFIR examples indexing, OpenCTI STIX 2.1 export, and ATT&CK Group Library enhancements. Features include Navigator for browsing Enterprise, Mobile, and ICS ATT&CK plus MITRE ATLAS; manual TTP selection and ATT&CK Navigator layer import; group and campaign comparison using Jaccard overlap; report analysis with evidence review states (analyst decides what is defensible); and reference sync for keeping ATT&CK data current. The tool explicitly distinguishes TTP overlap from attribution — a high overlap means behavior shares characteristics, not that an actor definitely did it [citation:15].  
**Best for:** CTI analysts wanting AI-assisted ATT&CK mapping and adversary comparison with local LLM support and OpenCTI integration, accepting a younger project with evolving documentation.

---

## 📊 Comparison at a Glance

| Software | License | Type | IOC Focus | ATT&CK Mapping | Self-Hosted | Best For |
|----------|---------|------|-----------|----------------|-------------|----------|
| **Recorded Future** | Proprietary | Real-time intelligence | ✅ | ✅ | ❌ | Threat prioritization + automation |
| **Mandiant** | Proprietary | Frontline intelligence | ✅ | ✅ | ❌ | Incident response + actor tracking |
| **CrowdStrike Falcon X** | Proprietary | Adversary intelligence | ✅ | ✅ | ❌ | Falcon ecosystem + YARA/Snort |
| **Microsoft TI** | Proprietary | Integrated intelligence | ✅ | ✅ | ❌ | Microsoft 365 security estates |
| **Palo Alto Unit 42** | Proprietary | Research + IR | ✅ | ✅ | ❌ | Palo Alto ecosystem |
| **Cisco Talos** | Proprietary | Research intelligence | ✅ | ✅ | ❌ | Cisco security products |
| **Flashpoint** | Proprietary | Primary-source intel | ✅ | (Check) | ❌ | Dark web + EASM + PIRs |
| **ThreatConnect** | Proprietary | TIP + risk quantification | ✅ | ✅ | ❌ | TI Ops + financial risk |
| **Anomali** | Proprietary | Decisioning layer | ✅ | ✅ | ❌ | Agentic triage + speed |
| **MISP** | AGPL-3.0 | IOC sharing platform | ✅ Deep | ✅ | ✅ | Community-standard IOC sharing |
| **OpenCTI** | Apache-2.0 | STIX knowledge graph | ✅ | ✅ | ✅ | Threat actor/campaign analysis |
| **TheHive & Cortex** | AGPL-3.0 | Case mgmt + enrichment | ✅ (Enrichment) | (Via Cortex) | ✅ | Operationalizing IOCs |
| **vamp-darkweb-intel** | Open Source | CLI IOC correlation | ✅ | ❌ | ✅ (CLI) | Rapid multi-feed lookup |
| **AdversaryGraph** | Open Source | ATT&CK analysis + AI | (Check) | ✅ Deep | ✅ | Local LLM + ATT&CK mapping |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Threat Intelligence or Compromise Indicator tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source. Note that the open-source ecosystem is anchored by **MISP and OpenCTI** as the two foundational platforms — MISP for IOC correlation and sharing, OpenCTI for STIX-native knowledge graph analysis. They are designed to work together (bidirectional sync) rather than as competing alternatives, with TheHive and Cortex completing the operational workflow. Commercial platforms like Recorded Future, Mandiant, and CrowdStrike Falcon X remain differentiated by proprietary data sources, frontline incident response intelligence, and AI-driven automation that open-source tools cannot fully replicate.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
