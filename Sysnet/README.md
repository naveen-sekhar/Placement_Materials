# SYSNET Global Technologies — SOC L1 / Security Analyst L1 (₹3 LPA)

---

### 1.2 The six service lines — [CONFIRMED]

1. **Cloud Solutions**
2. **Security Solutions** ← your vertical
3. **Infrastructure Management Services**
4. **Field Services**
5. **Professional Services** (resource augmentation / staffing to client sites)
6. **Intelligent Automation** (AI/ML/NLP/RPA — 100,000 automated actions per month)

### 1.3 What SYSNET actually does in security — [CONFIRMED]

From the [Security Solutions page](https://sysnetglobal.com/security-solutions.php), the security umbrella covers:

- **Security Operations Centre (SOC)** — described by SYSNET as *"the correlation point for every event logged within the organization that is being monitored"*, covering prevention, detection, analysis and response
- **Security Incident and Event Management (SIEM)** — SYSNET explicitly lists the six SIEM attributes it works with: **retention, dashboards, correlation, alerting, aggregation, compliance**
- Threat Discovery, Assessment and Management (AI/ML-backed)
- Identity and Access Management (including third-party/vendor access)
- Risk, Compliance and Governance — GDPR, PIPEDA, CCPA, PDP
- Data Protection, Change Management, Configuration Management
- Service Level Management with **RCA → CAPA** (root cause analysis → corrective & preventive action)
- Logs and Analysis, Incident Response/Resolution/Automation
- Monitoring stack: Application Performance Monitoring, Transaction Monitoring, User Monitoring, Infrastructure Monitoring, Events & Analytics

**SYSNET's own security methodology — "ADAM" [CONFIRMED]:** a 24x7 continuous, automation-backed process of
**A**nticipation of risk → **D**iscoverability of risk → **A**ssessment of risk → **M**itigation of risk.

> 🔴 **Learn ADAM by name.** It is on SYSNET's public site, almost nobody in the interview room will have read it, and quoting it proves you researched the company. It also maps neatly onto the SOC lifecycle.

Security technology domains SYSNET says it implements: **Cloud security (CSPM/CPMS, CWPP, CASB, CNAPP), Network security (DLP, NAC, NGFW, NGAV), Endpoint security, Application security (Injection, Broken Authentication, Misconfiguration, XSS — i.e. OWASP-style threats).**

SYSNET also frames attacks in **generations**: Gen 1 virus → Gen 2 network → Gen 3 application vulnerabilities → Gen 4 payload/sandboxing & anti-bot → Gen 5/6 multi-vector mega attacks. (This is Check Point's well-known Gen I–VI model, reused in SYSNET's marketing.)

### 1.4 What a fresher will actually do in SYSNET's SOC — [INFERRED]

SYSNET is an **IT services / managed-services provider**, not a product company. Its Professional Services line explicitly outsources engineers to client environments. So expect:

- **24x7 rotational shifts**, including night shifts — SYSNET's site states the security process is "a 24x7 continuous process". This is non-negotiable for L1 and *will* be asked.
- **Monitoring a client's SIEM console**, not SYSNET's own — you may sit in a SYSNET NOC/SOC or be deployed at a client site (the Delivery Footprint page lists a **Network Operations Center**, Contact Center, Service Desk, Labs).
- **Alert triage against SOPs and playbooks**, ticket creation, escalation to L2, SLA adherence.
- **Multi-client / multi-tenant exposure** — MSSP analysts usually cover several customers, so process discipline and documentation matter more than deep tooling.
- Reporting into the **RCA/CAPA and Service Level Management** framework SYSNET markets to clients.
- Likely adjacency to **infrastructure and endpoint work** (AD, Intune, endpoint compliance, patching) because that is SYSNET's core DNA. One Glassdoor candidate was asked about **enrolling Windows devices in Intune** — endpoint management is genuinely part of this company's world.

---

### 2.2 Reconstructed SOC L1 JD — [INFERRED]

**Responsibilities you should expect:**
1. 24x7 monitoring of security alerts and events in the SIEM console
2. First-level triage, validation and classification of alerts using defined SOPs/playbooks
3. Review logs from firewalls, IDS/IPS, EDR, Active Directory, VPN, proxy, servers, applications
4. Identify **false positives** and close them with written justification
5. Escalate confirmed incidents to L2 / Incident Response within SLA
6. Raise and update tickets in the ITSM tool; document investigation steps and evidence
7. Basic phishing email analysis (headers, URLs, attachments)
8. Enrich alerts using threat intelligence (VirusTotal, AbuseIPDB, MITRE ATT&CK mapping)
9. Shift handover reports and daily/weekly monitoring reports for clients
10. Participate in post-incident review / RCA contribution

**Required skills (fresher level):**
- Networking fundamentals: OSI, TCP/IP, ports, protocols, subnetting, DNS, DHCP, NAT, VPN
- Cybersecurity fundamentals: CIA triad, AAA, threats/vulnerabilities/risk, attack types
- Windows and Linux basics, Active Directory concepts, log locations
- Understanding of SIEM concept and log flow (a named tool — Splunk / QRadar / Sentinel / Wazuh — is a strong differentiator)
- Incident response lifecycle, cyber kill chain, MITRE ATT&CK awareness
- Clear written English (ticket notes are the actual deliverable of an L1)
- Willingness for 24x7 rotational shifts and relocation

**Qualification:** B.E./B.Tech/BCA/MCA/B.Sc in CS/IT/Cyber Security or related. Certifications valued but rarely mandatory at ₹3 LPA: CEH, CompTIA Security+, CCNA, Microsoft SC-200, Google/IBM Cybersecurity Analyst (Coursera), Blue Team Level 1, TryHackMe SOC Level 1 path.

### 2.3 The five skills that decide this interview — [INFERRED, ranked]

1. **Networking fundamentals** — the #1 filter at every Indian SOC L1 interview. Non-negotiable.
2. **SOC alert triage thinking** — can you describe an investigation as a *sequence of steps*?
3. **Windows/AD + log literacy** — event IDs, where logs live, what a log line means.
4. **SIEM concept fluency** — you do not need years of Splunk, you need to explain log source → parsing → correlation rule → alert → triage.
5. **Communication + shift willingness** — SYSNET is a client-facing services company. Candidate reviews repeatedly stress communication skills.

---

## 5. QUESTION PATTERNS — ranked by likelihood

### 5.1 Tier ranking

| Tier | Meaning | Count |
|---|---|---|
| 🔥 **REPORTED** | Actually reported by SYSNET candidates (non-SOC roles) | 5 |
| ⭐ **HIGH PROBABILITY** | Strongly indicated by SYSNET's published security capabilities, MSSP business model, and the standard Indian SOC L1 interview pattern | ~40 |
| ○ **GENERAL** | Standard SOC L1 knowledge, worth knowing, lower per-question odds | rest |

### 5.2 Top 25 most likely questions, ranked

| Rank | Question | Tier | Why it ranks here |
|---|---|---|---|
| 1 | Tell me about yourself | 🔥/⭐ | Universal; SYSNET weights communication heavily |
| 2 | What are the layers of the OSI model? Give an example at each | ⭐ | Universal SOC L1 opener |
| 3 | TCP vs UDP — difference and when each is used | ⭐ | Universal |
| 4 | Explain the TCP three-way handshake | ⭐ | Universal |
| 5 | What is the CIA triad? | ⭐ | Universal |
| 6 | What is a SOC and what does an L1 analyst do? | ⭐ | Role-defining |
| 7 | Common port numbers (20/21, 22, 23, 25, 53, 80, 110, 143, 389, 443, 445, 3389) | ⭐ | Rapid-fire favourite |
| 8 | Are you comfortable with 24x7 rotational night shifts? | ⭐ | SYSNET states 24x7 security ops [CONFIRMED] |
| 9 | What is SIEM? How does it work? | ⭐ | SYSNET's site details SIEM's six attributes |
| 10 | Difference between IDS and IPS | ⭐ | SYSNET lists IDS/IPS in its stack |
| 11 | What is a firewall? Stateful vs stateless | ⭐ | Core |
| 12 | How would you investigate a phishing email? | ⭐ | #1 real L1 ticket type |
| 13 | Difference between a vulnerability, a threat, and a risk | ⭐ | Core |
| 14 | What is a false positive? How do you handle one? | ⭐ | Core L1 daily task |
| 15 | Why cybersecurity? Why SOC? | ⭐ | Universal HR |
| 16 | Why SYSNET? | ⭐ | Where ADAM/1,500 locations wins you points |
| 17 | Explain the incident response lifecycle | ⭐ | Core |
| 18 | What is an IOC? Give examples | ⭐ | Core |
| 19 | Symmetric vs asymmetric encryption; HTTP vs HTTPS | ⭐ | Core |
| 20 | Walk me through a brute-force alert investigation | ⭐ | Top-3 real alert type |
| 21 | What is MITRE ATT&CK? | ⭐ | Increasingly standard at L1 |
| 22 | Are you willing to relocate? | ⭐ | SYSNET has 100+ branches, 1,500+ locations |
| 23 | Explain your final-year project | ⭐ | Campus-specific certainty |
| 24 | Windows event IDs you know (4624/4625/4720/4672) | ⭐ | Differentiator |
| 25 | *"What do you know about troubleshooting?"* | 🔥 | Literally asked by SYSNET |

---

## 6. TECHNICAL PREPARATION — prioritised for this role

### 6.1 🔴 CRITICAL — Networking (expect 30–40% of the technical round)

| Topic | What to be able to say in 30 seconds |
|---|---|
| **OSI model** | All 7 layers in order + one protocol and one attack per layer |
| **TCP/IP model** | 4 layers and how they map to OSI |
| **TCP vs UDP** | Connection-oriented/reliable/ordered vs connectionless/fast; TCP = HTTP, SSH, SMTP; UDP = DNS, DHCP, SNMP, VoIP |
| **Three-way handshake** | SYN → SYN-ACK → ACK; and what a SYN flood does to it |
| **Ports** | 20/21 FTP, 22 SSH, 23 Telnet, 25 SMTP, 53 DNS, 67/68 DHCP, 80 HTTP, 110 POP3, 143 IMAP, 161 SNMP, 389 LDAP, 443 HTTPS, 445 SMB, 1433 MSSQL, 3306 MySQL, 3389 RDP |
| **DNS** | Recursive vs iterative; record types A/AAAA/MX/CNAME/TXT/NS/PTR; DNS tunnelling and DGA as attack signals |
| **DHCP** | DORA — Discover, Offer, Request, Acknowledge; rogue DHCP risk |
| **Subnetting** | CIDR /24 /25 /26 /27, usable hosts, private ranges 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16 |
| **NAT / PAT** | Why a SOC sees one public IP for many internal hosts (and why that complicates attribution) |
| **HTTP vs HTTPS** | TLS handshake at a high level; status codes 200/301/401/403/404/500 |
| **VPN** | Site-to-site vs remote access; IPsec vs SSL VPN; impossible-travel detection on VPN logs |
| **Firewall** | Packet filter vs stateful vs NGFW; ingress vs egress rules; why egress filtering catches C2 |
| **IDS vs IPS** | Detect-and-alert (out of band) vs detect-and-block (inline); signature vs anomaly based |
| **Proxy** | Forward vs reverse; why proxy logs are a SOC goldmine |

### 6.2 🔴 CRITICAL — Cybersecurity fundamentals

CIA triad (+ non-repudiation, authenticity) · AAA (Authentication, Authorization, Accounting) · Vulnerability vs Threat vs Risk vs Exploit · Zero-day · Defence in depth · Least privilege · Zero Trust · Symmetric vs asymmetric encryption · Hashing (MD5/SHA-256) vs encryption vs encoding (Base64) · Digital certificates and PKI · MFA · Common attacks: phishing, spear phishing, whaling, vishing, smishing, SQL injection, XSS, CSRF, MITM, DoS/DDoS, privilege escalation, social engineering.

> 💡 SYSNET's own site names **Injection, Broken Authentication, Misconfiguration and Cross-site Scripting** as the application threats it addresses [CONFIRMED]. Know these four cold — they are the highest-value OWASP items for this specific interview.

### 6.3 🔴 CRITICAL — SOC operations and alert triage

- SOC tiers: L1 (monitor/triage/escalate) → L2 (deep investigation/containment) → L3 (threat hunting/forensics/detection engineering)
- The triage loop: **Alert → Validate → Enrich → Classify (TP/FP/BTP) → Escalate or Close → Document**
- True positive / false positive / false negative / benign true positive
- SLA and MTTD/MTTR; why an L1 missing an SLA is the metric that gets reported to the client
- Shift handover discipline; ticket hygiene; playbooks and runbooks
- Severity classification (P1–P4) and what justifies escalation
- **Map this to SYSNET's ADAM model** (Anticipate → Discover → Assess → Mitigate) in your answer. [CONFIRMED company language]

### 6.4 🔴 CRITICAL — SIEM and log analysis

- What a SIEM does: **aggregation, normalisation/parsing, correlation, alerting, dashboards, retention, compliance** — this exact six-part list is on SYSNET's own site [CONFIRMED], so use their words
- Log source → forwarder/agent → parser → correlation rule → offence/alert → analyst queue
- Common log sources: firewall, proxy, AD/DC, DNS, VPN, EDR, email gateway, WAF, servers, cloud
- Know **at least one SIEM by name and be able to write one query.** Pick one:
  - **Splunk SPL:** `index=wineventlog EventCode=4625 | stats count by src_ip, user | where count > 10`
  - **Microsoft Sentinel KQL:** `SecurityEvent | where EventID == 4625 | summarize Attempts=count() by Account, IpAddress | where Attempts > 10`
  - **QRadar:** offences, log sources, building blocks, AQL basics
  - **Free hands-on:** Wazuh or ELK in a VM — sufficient to say "I built one"
- Log correlation: why 20 x 4625 followed by one 4624 is the whole story

### 6.5 🔴 CRITICAL — Windows security

| Event ID | Meaning | Why L1 cares |
|---|---|---|
| 4624 | Successful logon | Logon Type 3 = network, 10 = RDP |
| 4625 | Failed logon | Brute force detection |
| 4634 / 4647 | Logoff | Session timeline |
| 4648 | Logon with explicit credentials | Lateral movement signal |
| 4672 | Special privileges assigned | Admin logon |
| 4720 | User account created | Persistence |
| 4728 / 4732 | User added to a privileged group | Privilege escalation |
| 4688 | New process created | Command-line auditing, PowerShell |
| 1102 | Audit log cleared | Anti-forensics — always escalate |
| 7045 | New service installed | Persistence |

Also: Active Directory basics (domain, DC, OU, GPO, Kerberos vs NTLM), Event Viewer, Task Manager, `netstat -ano`, `tasklist`, `whoami /priv`, Sysmon (Event ID 1 process create, 3 network connect, 11 file create), Defender basics.

### 6.6 🟠 HIGH — Linux security

`/var/log/auth.log` (Debian/Ubuntu) and `/var/log/secure` (RHEL/CentOS) · `/var/log/syslog` · `/etc/passwd`, `/etc/shadow` · file permissions and chmod numbers · `ps`, `top`, `netstat`/`ss`, `lsof`, `crontab -l`, `last`, `history`, `who` · grep/awk for log hunting: `grep "Failed password" /var/log/auth.log | awk '{print $11}' | sort | uniq -c | sort -nr` · SSH hardening · cron jobs as persistence.

### 6.7 🟠 HIGH — Incident response, IOC/IOA, MITRE ATT&CK

- **NIST IR lifecycle:** Preparation → Detection & Analysis → Containment, Eradication & Recovery → Post-Incident Activity
- **SANS 6-step:** Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned
- **Cyber Kill Chain (Lockheed Martin):** Recon → Weaponization → Delivery → Exploitation → Installation → C2 → Actions on Objectives
- **MITRE ATT&CK:** 14 enterprise tactics; be able to name Initial Access, Execution, Persistence, Privilege Escalation, Defense Evasion, Credential Access, Discovery, Lateral Movement, Collection, C2, Exfiltration, Impact. Know 3 techniques by ID: **T1566 Phishing, T1059 Command and Scripting Interpreter, T1110 Brute Force**
- **IOC vs IOA:** IOC = evidence something already happened (hash, IP, domain, filename, registry key) — reactive. IOA = behaviour indicating an attack in progress (mass encryption, unusual parent-child process) — proactive.
- **Pyramid of Pain:** hashes trivial to change → TTPs hardest. Great answer to "why isn't blocking IOCs enough?"

### 6.8 🟠 HIGH — EDR/XDR and malware/phishing/ransomware

- EDR vs antivirus vs XDR: signature-based prevention vs behavioural detection + telemetry + response (isolate host, kill process, quarantine file) vs correlation across endpoint + network + email + cloud
- Products to be able to name: CrowdStrike Falcon, Microsoft Defender for Endpoint, SentinelOne, Trend Micro, Sophos
- Malware types: virus, worm, trojan, ransomware, spyware, rootkit, keylogger, botnet, fileless malware, LOLBins (`certutil`, `mshta`, `rundll32`, `wmic`)
- Phishing analysis: **headers** (SPF, DKIM, DMARC, Received chain, Return-Path vs From mismatch), **URLs** (defang, look-alike/homoglyph domains, redirect chains), **attachments** (hash → VirusTotal, macro-enabled .docm/.xlsm, double extensions), **sandbox** (Any.Run, Hybrid Analysis, Joe Sandbox)
- Ransomware chain: initial access → privilege escalation → discovery → lateral movement → shadow copy deletion (`vssadmin delete shadows`) → mass encryption → ransom note. Double extortion.
- Free tools you should name-drop: **VirusTotal, AbuseIPDB, URLScan.io, Any.Run, MXToolbox, Shodan, Whois, CyberChef, Wireshark, Nmap**

### 6.9 🟡 MEDIUM — Cloud security

Justified because SYSNET sells Cloud Solutions and names CPMS/CSPM, CWPP, CASB and CNAPP on its Security Solutions page [CONFIRMED]. Know the *expansions and one-line purposes* of those four acronyms, the shared responsibility model, and that Azure AD/Entra sign-in logs and AWS CloudTrail are log sources. Do not go deeper than that for L1.

### 6.10 🟡 MEDIUM — Scripting

Not a gate for SOC L1 at ₹3 LPA, but it differentiates:
- **Python:** read a log file, count failed logins, call the VirusTotal API
- **PowerShell:** `Get-WinEvent -FilterHashtable @{LogName='Security'; ID=4625}`; know that encoded commands (`-enc`), `-ExecutionPolicy Bypass` and `DownloadString` are red flags
- **Bash:** grep/awk/sort/uniq log pipeline (see 6.6)

### 6.11 🔵 LOW priority — deprioritise these

Pentesting/exploit development, reverse engineering, memory forensics, detection engineering, compliance frameworks in depth, DSA/coding rounds. **Do not spend time here.** A SOC L1 campus round will not go there, and SYSNET's reported interview difficulty is 2.7/5.

---

## 7. SCENARIO QUESTIONS — interview-ready answers

> **Universal answer framework — use this structure every single time:**
> **1. Validate** the alert → **2. Gather context** (who/what/when/where) → **3. Enrich** with threat intel → **4. Decide** TP or FP → **5. Contain/Escalate** per SOP → **6. Document** in the ticket.
> Saying "I would follow the SOP and escalate to L2 with my findings documented" is a *correct* L1 answer. Never claim you'd unilaterally block production traffic.

### 7.1 Phishing email reported by a user
"First I'd confirm whether other users received the same mail and whether anyone clicked. I'd analyse the headers — Return-Path versus From, SPF/DKIM/DMARC results, and the Received chain to see the true origin. I'd defang and check the URLs in URLScan or VirusTotal without clicking, and hash any attachment and check it in VirusTotal or detonate it in a sandbox. I'd check proxy and DNS logs for anyone who visited the URL and email gateway logs for the full campaign scope. If malicious, I'd escalate to L2, recommend blocking the sender domain and URL at the gateway and proxy, quarantine all copies of the mail, and force a password reset for anyone who submitted credentials. Then I'd document IOCs in the ticket." **ATT&CK: T1566.**

### 7.2 Brute force alert — 200 failed logins on one account
"I'd check Windows Event ID 4625 for the failure count, the source IP, and the failure reason code. The critical question is whether any 4624 success follows — that turns a failed brute force into a confirmed compromise. I'd check whether the source IP is internal or external, look it up in AbuseIPDB, check geolocation against the user's normal location, and see whether the same source is hitting multiple accounts — that's password spraying rather than brute force. If there was a success, I escalate immediately as a suspected account compromise and recommend disabling the account and resetting credentials. If no success, I'd still recommend blocking the source IP and check whether account lockout policy and MFA are enforced." **ATT&CK: T1110.**

### 7.3 Suspicious login — impossible travel
"An alert showing logins from Chennai and then Eastern Europe 20 minutes apart is a classic impossible-travel detection. I'd first rule out benign causes — a VPN, a corporate proxy, a cloud service acting on the user's behalf, or a mobile roaming IP. I'd check the sign-in logs for device, user agent, and whether MFA was satisfied, and look at what the account did after logging in — new mailbox rules, mass downloads, privilege changes. Legitimate VPN use makes it a benign true positive and I'd document why. Genuine impossible travel with MFA bypassed I escalate as account compromise."

### 7.4 EDR malware alert on an endpoint
"I'd check what the EDR actually did — quarantined, blocked, or only detected. Detected-but-not-blocked is the dangerous case. I'd get the file path, hash and the parent process. Parent-child matters enormously: winword.exe spawning powershell.exe is far more alarming than the file name itself. I'd look up the hash in VirusTotal, check whether the same hash appears on other endpoints, and review network connections from that host for C2 traffic. If it's a true positive, I'd escalate to L2 and recommend host isolation through the EDR, then document the IOCs so other hosts can be swept."

### 7.5 Suspicious IP or domain in outbound traffic
"I'd establish direction and volume — is it inbound or outbound, and how much data. Outbound to an unknown IP is usually the more serious. I'd check reputation in VirusTotal, AbuseIPDB and the threat intel feed, check Whois for a newly registered domain, and look at the beaconing pattern — regular intervals to the same destination strongly suggests C2. I'd identify which internal host and which process is generating it, check whether other hosts talk to the same destination, and escalate with a recommendation to block at firewall and proxy."

### 7.6 Ransomware indicators
"This is a P1. The priority is containment speed, not investigation depth. Signs I'd look for: mass file modifications in a short window, known ransomware extensions, ransom notes appearing, `vssadmin delete shadows` or `wbadmin delete catalog` execution, and spikes in SMB traffic suggesting lateral spread. I'd immediately escalate to L2 and the incident manager per the SOP, and recommend isolating affected hosts from the network while keeping them powered on to preserve memory evidence. I'd help scope which hosts are affected, whether backups are intact and reachable, and identify the initial access point. I would not attempt remediation myself at L1 — my job is to sound the alarm fast and accurately."

### 7.7 Suspicious PowerShell execution
"Red flags in the command line: `-enc` or `-EncodedCommand`, `-ExecutionPolicy Bypass`, `-WindowStyle Hidden`, `-NoProfile`, and `IEX (New-Object Net.WebClient).DownloadString(...)`. I'd pull Event ID 4688 or Sysmon Event 1 for the full command line and the parent process, decode the Base64 payload in CyberChef to see the real command, check any URL or IP it contacts, and check whether this is a one-off or repeating. A legitimate admin script from a known admin account during business hours is a false positive I'd document. An encoded downloader launched by Office is a true positive and I'd escalate." **ATT&CK: T1059.001.**

### 7.8 Data exfiltration alert
"I'd quantify it first — how much data, to where, over what protocol, and by which user and process. Common exfil channels are large HTTPS uploads to personal cloud storage, unusual outbound FTP or SMB, and DNS tunnelling where you see abnormally long subdomain queries at high volume. I'd compare against the user's baseline and their role — a developer pushing to a repo differs from someone in finance uploading 4 GB at 2 a.m. I'd check for preceding indicators like mass file access or archive creation. Confirmed exfil escalates immediately, and I'd flag it as a potential insider threat or data-breach notification issue." **ATT&CK: TA0010.**

### 7.9 Handling a false positive
"A false positive still requires work. I'd verify it genuinely is benign — confirm the source and activity are legitimate and expected, ideally with the asset owner. Then I'd close the alert with a written justification naming the evidence, not just 'FP'. If the same false positive recurs, I'd raise it for rule tuning so L2 or detection engineering can adjust the threshold or add an exclusion. High false positive rates cause alert fatigue, which is how real incidents get missed — so tuning is part of protecting detection quality, not a shortcut."

---

## 8. HR + PROJECT QUESTIONS

### 8.1 Tell me about yourself — [RECOMMENDED template]
> *"I'm [Name], a final-year [B.Tech CSE] student at [College] with a CGPA of [X]. I chose to specialise in cybersecurity because [one concrete trigger — a course, a CTF, an incident you read about]. I've built my fundamentals in networking and security through [certification/course], and applied them practically in [project] where I [specific action and result]. I've also spent time on hands-on platforms like TryHackMe on the SOC Level 1 path, working through SIEM and phishing analysis labs. I'm looking to start my career as a SOC L1 analyst because it's where you see real attacks daily, and SYSNET's 24x7 managed security operations across 1,500+ locations is exactly the kind of high-volume, multi-client environment where I'd learn fastest."*

Keep it to 60–90 seconds. End by connecting to SYSNET. Never recite your resume line by line.

### 8.2 Why cybersecurity / why SOC?
Give a **specific origin story**, not "it's a growing field." Then justify SOC specifically: it's the fastest real-world learning environment, you see live attacker behaviour rather than theory, and it builds the foundation for L2, incident response, or threat hunting later.

### 8.3 Why SYSNET? — the answer that wins points
> *"Three reasons. First, SYSNET has 25 years in IT infrastructure with a 1,500-location footprint across India, so the SOC covers genuinely diverse client environments — banking, government, insurance, healthcare — which means far broader exposure than a single-industry in-house SOC. Second, I read SYSNET's ADAM methodology on your Security Solutions page — Anticipation, Discoverability, Assessment and Mitigation of risk on a 24x7 basis — and that structured, process-led approach is how I want to learn the discipline rather than picking up habits ad hoc. Third, SYSNET partners with IBM, Kyndryl, TCS, DXC, Lenovo and Dell, and it's ISO 27001 and ISO 20000-1 certified, so I'd be learning inside a mature, audited process environment."*

**This is your differentiator.** Almost no candidate will have read the ADAM model.

### 8.4 Shift work — [answer with conviction]
SYSNET states its security process is 24x7 continuous [CONFIRMED]. Hesitation here loses offers.
> *"Yes, completely comfortable. A SOC only works because someone is watching at 3 a.m., and as an L1 that's a core part of the job, not an inconvenience. I understand rotational shifts including nights and weekends, and I'm prepared for it. I'd also want to be disciplined about handover notes, because a shift change is where context gets lost if the documentation is weak."*

### 8.5 Relocation
SYSNET has 100+ branches across the cities listed on its careers page (Delhi, Noida, Gurgaon, Mumbai, Bangalore, Chennai, Hyderabad, Pune, Kolkata and 45+ more). Answer **yes** if you can — it materially improves selection odds. If you have a genuine constraint, state it once, clearly and early, with your flexible options.

### 8.6 Projects — how to present them
Use **STAR**: Situation → Task → Action → Result. For each project be ready with: what problem it solved, your specific contribution (not the team's), the tools and why you chose them, what broke and how you fixed it, and what you'd do differently.

**If you have no security project, build one this week.** Any of these is enough to talk for five minutes:
- Wazuh or ELK SIEM in VirtualBox, ingesting Windows logs, with a custom rule for Event ID 4625
- A Python phishing-header analyser (parse SPF/DKIM/DMARC, extract and defang URLs)
- A home lab: Kali + Windows VM, generate failed logins, detect them in Splunk Free
- Documented write-ups of 5 TryHackMe SOC Level 1 rooms

### 8.7 Certifications
Be honest about status. In-progress counts — say *"I'm currently working through the Google Cybersecurity Certificate, about 70% complete."* Worth naming if you have them: **CEH, CompTIA Security+, CCNA, Microsoft SC-200, Google/IBM Cybersecurity Analyst (Coursera), TryHackMe SOC Level 1, Blue Team Level 1, Splunk Fundamentals 1 (free).**

### 8.8 Strengths and weaknesses
Strength: pick one that maps to SOC work — attention to detail, methodical documentation, calm under pressure — and back it with an example. Weakness: pick a real, non-fatal one with a stated fix. *"I used to over-investigate before escalating, because I wanted certainty. In lab exercises I learned that timely escalation with partial findings is more valuable than a late perfect answer, so I now set myself a time-box and escalate with what I have."* Never say "I'm a perfectionist" or "I work too hard."

### 8.9 Teamwork and communication
SYSNET candidates explicitly flag that **communication skills are required to work with client offices** [REPORTED, Glassdoor Chennai]. Have a real example of resolving a disagreement or handing off work cleanly. Emphasise that as an L1 your written output — the ticket — *is* the product.

### 8.10 Other HR questions to have ready
Where do you see yourself in 3 years? (L2 analyst / incident response — show a SOC career path, not "manager") · Why should we hire you? · Any bond or service agreement — are you okay with it? · What are your salary expectations? (for a campus drive: *"The ₹3 LPA package announced is acceptable; at this stage learning and exposure matter more to me"*) · Do you have any offers? · Do you have questions for us? (**always yes** — ask about the SIEM stack, L1→L2 progression timeline, shift rotation pattern, and the training period.)

---

## 9. FINAL PREPARATION

### 9.1 Top 20 MUST-PREPARE questions

1. Tell me about yourself
2. Why cybersecurity, and why a SOC role specifically?
3. Why SYSNET? (use ADAM + 1,500 locations + ISO 27001)
4. Explain the OSI model with an example at each layer
5. TCP vs UDP, and the three-way handshake
6. Name 15 common port numbers and their protocols
7. What is the CIA triad?
8. What does a SOC L1 analyst do in a typical shift?
9. What is a SIEM and how does log flow work end to end?
10. IDS vs IPS; stateful vs stateless firewall
11. Vulnerability vs threat vs risk
12. Walk me through investigating a phishing email
13. Walk me through a brute-force alert investigation
14. What is a false positive and how do you handle one?
15. Explain the incident response lifecycle
16. What is an IOC? IOC vs IOA
17. What is MITRE ATT&CK and name a few tactics
18. Which Windows event IDs matter for security monitoring?
19. Explain your project (STAR format)
20. Are you comfortable with 24x7 rotational shifts and relocation?

### 9.2 Top 20 MUST-PREPARE topics

1. OSI and TCP/IP models
2. TCP/UDP, handshake, common ports
3. Subnetting, CIDR, private IP ranges, NAT
4. DNS and DHCP (including DORA)
5. Firewalls, IDS/IPS, proxy, VPN
6. CIA triad, AAA, defence in depth, least privilege
7. Encryption vs hashing vs encoding; HTTPS/TLS/PKI
8. Common attacks: phishing, SQLi, XSS, MITM, DDoS, privilege escalation
9. SOC structure, tiers, SLA, MTTD/MTTR, playbooks
10. Alert triage workflow and TP/FP/BTP classification
11. SIEM architecture and at least one query language (SPL or KQL)
12. Windows security event IDs and Active Directory basics
13. Linux log files and grep/awk log analysis
14. Incident response lifecycle (NIST + SANS)
15. Cyber Kill Chain and MITRE ATT&CK
16. IOC/IOA and the Pyramid of Pain
17. Malware types, ransomware chain, LOLBins
18. Phishing email analysis (headers, URLs, attachments, SPF/DKIM/DMARC)
19. EDR/XDR concepts and named products
20. SYSNET company facts: ADAM, six service lines, SIEM's six attributes, ISO certifications, footprint, leadership

### 9.3 Skills ranked

| Priority | Skills |
|---|---|
| 🔴 **CRITICAL** | Networking fundamentals · Cybersecurity fundamentals · SOC triage methodology · SIEM concepts · Windows security & event logs · Clear spoken and written English · Willingness for 24x7 shifts + relocation · SYSNET company knowledge |
| 🟠 **HIGH** | Incident response lifecycle · Phishing analysis · MITRE ATT&CK / Kill Chain · IOC-IOA · Linux log analysis · EDR/XDR concepts · Threat intel tools (VirusTotal, AbuseIPDB, URLScan) · A demonstrable security project · Aptitude and logical reasoning |
| 🟡 **MEDIUM** | One hands-on SIEM (Splunk/Sentinel/Wazuh) · Python or PowerShell basics · Cloud security acronyms (CSPM/CWPP/CASB/CNAPP) · Active Directory depth · Wireshark/Nmap · Certifications |
| 🔵 **LOW / SKIP** | Pentesting, reverse engineering, memory forensics, detection engineering, DSA and coding rounds, deep compliance frameworks |

### 9.5 Final 24-hour revision checklist

**Knowledge — tick each only if you can say it out loud, unaided**
- [ ] OSI 7 layers in order, with a protocol per layer
- [ ] TCP vs UDP + three-way handshake
- [ ] 15 port numbers rapid-fire
- [ ] CIA triad; vulnerability vs threat vs risk
- [ ] Two private IP ranges and what /24 and /26 mean
- [ ] IDS vs IPS; stateful vs stateless firewall
- [ ] What a SIEM does (all six attributes)
- [ ] SOC L1 vs L2 vs L3 responsibilities
- [ ] The 6-step triage loop
- [ ] Windows event IDs 4624, 4625, 4672, 4688, 4720, 1102
- [ ] Two Linux log paths
- [ ] NIST IR lifecycle, 4 phases
- [ ] Cyber Kill Chain, 7 stages
- [ ] Five MITRE ATT&CK tactics
- [ ] IOC vs IOA with examples
- [ ] Phishing investigation, start to finish
- [ ] Brute force investigation, start to finish
- [ ] Ransomware response, start to finish
- [ ] How you handle and document a false positive
- [ ] Encryption vs hashing vs encoding

**Company**
- [ ] SYSNET = Indian IT infrastructure management, New Delhi, founded 1999 (**not** the Dublin PCI company, **not** the US federal one)
- [ ] ADAM: Anticipation → Discoverability → Assessment → Mitigation
- [ ] Six service lines
- [ ] ISO 27001:2013, ISO 20000-1:2011, ISO 9001
- [ ] 1,500+ service locations, 100+ branches, 3,500+ engineers
- [ ] Partners: IBM, Kyndryl, TCS, DXC, Lenovo, Dell, HP, Acer, Samsung, Hughes
- [ ] CEO Arush Sogani; COO Vinod Gaonkar
- [ ] Your 90-second "Why SYSNET" answer

**HR**
- [ ] 60–90 second "Tell me about yourself", rehearsed aloud
- [ ] "Why cybersecurity / why SOC" with a specific origin story
- [ ] Project in STAR form
- [ ] Unambiguous **yes** on shifts and relocation
- [ ] Strength + weakness, each with an example
- [ ] Three questions to ask the interviewer

**Logistics**
- [ ] 4 printed resume copies, ID, marksheets, passport photos
- [ ] Certificates and certification proofs in a folder
- [ ] Formal clothes ready; venue and reporting time confirmed
- [ ] Laptop/phone charged; OA platform tested if remote
- [ ] Sleep 7+ hours — this matters more than one more revision hour

---

### 10.2 Sources

**Official SYSNET — [CONFIRMED]**
- Home: https://sysnetglobal.com/
- Security Solutions (ADAM, SOC, SIEM attributes, security stack): https://sysnetglobal.com/security-solutions.php
- Careers (locations, role list, application form): https://sysnetglobal.com/careers.php
- Cloud Solutions: https://sysnetglobal.com/cloud-solutions.php
- Infrastructure Management Services: https://sysnetglobal.com/infrastructure-management-services.php
- LinkedIn: https://www.linkedin.com/company/sysnet-global-technologies-pvt-ltd/

**Candidate experiences — [REPORTED]**
- Glassdoor interviews (15 reports, updated 11 Jul 2024): https://www.glassdoor.co.in/Interview/Sysnet-Global-Technologies-Interview-Questions-E512463.htm
- Glassdoor reviews (166 reviews, 3.9/5): https://www.glassdoor.co.in/Reviews/Sysnet-Global-Technologies-Reviews-E512463.htm
- Indeed company page (117–122 reviews, ~150 interview respondents): https://in.indeed.com/cmp/Sysnet-Global-Technologies

**Company data — [CONFIRMED]**
- Tracxn (headcount 3,705 as of Mar 2025; revenue ₹100–500 Cr; founded 1999): https://tracxn.com/d/companies/sysnet-global-technologies/__-BfCCmyKcXxVxjWIV4ogrZIPC8AtZviq6RdxBgBfTlw
- ZoomInfo: https://www.zoominfo.com/c/sysnet-global-technologies-ltd/348454335
- IndiaMART listing (ISO certifications, partner list): https://www.indiamart.com/sysnet-glob/aboutus.html

**Disambiguation sources**
- Sysnet Global Solutions / SecureTrust acquisition, Oct 2021 (**different company**): https://www.businesswire.com/news/home/20211024005030/en
- SysNet Technologies Inc., Virginia USA (**different company**): https://sysnettech.com/

**Comparable SOC L1 JDs used for the [INFERRED] reconstruction in §2.2**
- Deloitte India SOC L1 (QRadar, 24x7 rotational shifts mandatory): https://southasiacareers.deloitte.com/job/Mumbai-T&T-Cyber-D&R-SIEM-Consultant-Mumbai/42517744
- Deloitte India SOC L1 (alert triage, false positive closure, log review across firewall/IDS/EDR/AD/VPN): https://southasiacareers.deloitte.com/job/Mumbai-I-Think-T&T-Cyber-D&R-SIEM-Deputy-Manager-Mumbai/51687744
- IBM SOC Analyst, Chennai (SOC entry channels, escalation model): https://www.themuse.com/jobs/ibm/soc-analyst-l2-adb4af
- NTT Data SOC Analyst L1 (24/7, 4-on-4-off shift pattern): https://findajob.dwp.gov.uk/details/16957834
- Assystem SOC L1, Gurugram: https://builtin.com/job/soc-l1-analyst/3200339

### 10.3 Research integrity statement

**No interview question has been invented and attributed to SYSNET.** The only questions marked 🔥 REPORTED are the five in §4.2, each traceable to a dated Glassdoor submission, and each from a non-security role. Everything marked ⭐ or ○ is explicitly a projection based on SYSNET's published capabilities and the standard Indian SOC L1 interview pattern.

**Known gaps in the public record:** no SYSNET SOC L1 job description, no SYSNET security-role interview experience, no SYSNET campus placement experience, and no confirmation of SYSNET's SIEM/EDR product stack. Your TPO's circulated JD overrides §2.2 wherever the two differ.

---

## 📌 The one-line answer

**Master networking fundamentals cold, be able to walk through a phishing and a brute-force investigation step by step, know Windows event IDs and what a SIEM does, be able to name SYSNET's ADAM model in your "Why SYSNET" answer, and say an unhesitating yes to 24x7 shifts.** SYSNET's reported interview difficulty is 2.7 out of 5 and its candidates consistently say communication matters as much as technical depth — so clarity beats cleverness. Explain simple things well.

**Good luck. 🛡️**
