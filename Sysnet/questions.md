# SOC L1 Analyst — Interview Question Bank

Legend: ⭐ = asked in almost every L1 interview. Prepare these first.

---

## 1. Cybersecurity Fundamentals

### 1.1 Basic

1. ⭐ What is the CIA triad (Confidentiality, Integrity, Availability)? Give one attack example against each.
2. ⭐ What is the difference between a threat, a vulnerability, and a risk?
3. What is the difference between a vulnerability, an exploit, and a payload?
4. What is AAA (Authentication, Authorization, Accounting)?
5. ⭐ Authentication vs authorization — what is the difference?
6. What is MFA (multi-factor authentication)? What are the factor types? Why is SMS OTP (one-time password) considered weak?
7. ⭐ Encryption vs hashing vs encoding — what is the difference, and when do you use each?
8. ⭐ Symmetric vs asymmetric encryption — differences, with algorithm examples of each.
9. What is salting? Why do we salt password hashes?
10. What is a digital signature? What is a digital certificate? How does PKI (public key infrastructure) work?
11. ⭐ Name the types of malware and explain each: virus, worm, trojan, ransomware, rootkit, spyware, keylogger, fileless malware.
12. ⭐ Virus vs worm vs trojan — what is the key difference?
13. ⭐ What is phishing? Explain spear phishing, whaling, vishing, and smishing.
14. What is social engineering? Give three examples.
15. ⭐ IDS (intrusion detection system) vs IPS (intrusion prevention system) — difference, and where each is placed.
16. ⭐ What is a firewall? Stateless vs stateful vs NGFW (next-generation firewall) vs WAF (web application firewall).
17. What is defence in depth? What is the principle of least privilege? What is zero trust?
18. Vulnerability assessment vs penetration testing — difference?
19. Red team vs blue team vs purple team — who does what?
20. What is a false sense of security from antivirus alone? Signature-based vs behaviour-based detection.

### 1.2 Intermediate

21. ⭐ What is a DoS (denial of service) vs DDoS (distributed denial of service) attack? Explain a SYN flood.
22. ⭐ What is a MITM (man-in-the-middle) attack? How does ARP (Address Resolution Protocol) spoofing enable it?
23. ⭐ Explain SQL injection, XSS (cross-site scripting), and CSRF (cross-site request forgery). How do they differ?
24. What is the OWASP (Open Worldwide Application Security Project) Top 10? Name at least five items.
25. ⭐ Brute force vs dictionary attack vs password spraying vs credential stuffing — how do you tell them apart in logs?
26. What is a zero-day vulnerability?
27. What are CVE (Common Vulnerabilities and Exposures), CVSS (Common Vulnerability Scoring System), and CWE (Common Weakness Enumeration)?
28. ⭐ Explain the Cyber Kill Chain. Name all seven stages.
29. ⭐ What is MITRE ATT&CK? Difference between tactics, techniques, and procedures (TTPs).
30. ⭐ IOC (indicator of compromise) vs IOA (indicator of attack) — difference, with examples.
31. What is the Pyramid of Pain? Why are hashes at the bottom and TTPs at the top?
32. Explain lateral movement, privilege escalation, and persistence. Give one technique for each.
33. ⭐ How does ransomware work end to end? What are the first three things you do when it is detected on a host?
34. What is a C2 (command and control) server? What is beaconing and how would you spot it in logs?
35. Explain the TLS (Transport Layer Security) handshake at a high level.
36. ⭐ Antivirus vs EDR (endpoint detection and response) vs XDR (extended detection and response).
37. What is DLP (data loss prevention)?
38. What is sandboxing? When would you detonate a file in a sandbox?
39. ⭐ MD5 vs SHA-1 vs SHA-256. Why is MD5 considered broken? How do you use a file hash during an investigation?
40. What is a living-off-the-land attack? Name some LOLBins (living-off-the-land binaries) — e.g. PowerShell, certutil, rundll32.
41. What is data exfiltration? Name common exfiltration channels.
42. What is an APT (advanced persistent threat)?

---

## 2. Networking

### 2.1 Models and Core Concepts

43. ⭐ Explain the OSI (Open Systems Interconnection) model — all seven layers, with one protocol and one attack per layer.
44. ⭐ OSI model vs TCP/IP model — how do the layers map?
45. ⭐ TCP (Transmission Control Protocol) vs UDP (User Datagram Protocol) — differences, and which applications use each.
46. ⭐ Explain the TCP three-way handshake. How does a connection close (four-way teardown)?
47. What are the TCP flags (SYN, ACK, FIN, RST, PSH, URG)? What does a flood of RST or SYN-only packets suggest?
48. ⭐ What happens, step by step, when you type a URL in a browser and press Enter?
49. What is encapsulation? Segment vs packet vs frame.
50. What is TTL (time to live)? How does traceroute use it?

### 2.2 Addressing

51. ⭐ What is an IP address? IPv4 vs IPv6.
52. ⭐ Public vs private IP. List the private IPv4 ranges (RFC 1918).
53. What is a subnet mask? What does /24 mean? How many usable hosts in a /24, /26, /30?
54. ⭐ MAC (media access control) address vs IP address — difference, and which layer each works at.
55. What is a loopback address? What is APIPA (Automatic Private IP Addressing, 169.254.x.x) and what does it tell you?
56. ⭐ What is NAT (network address translation)? What is PAT (port address translation)?
57. What is a default gateway?

### 2.3 Protocols

58. ⭐ List the common ports and their protocols: 20/21, 22, 23, 25, 53, 67/68, 80, 110, 123, 135, 137–139, 143, 161/162, 389, 443, 445, 636, 1433, 3306, 3389.
59. ⭐ How does DNS (Domain Name System) resolution work? Recursive vs iterative query.
60. DNS record types — A, AAAA, CNAME, MX, TXT, PTR, NS, SOA.
61. ⭐ When does DNS use TCP instead of UDP?
62. ⭐ What is DHCP (Dynamic Host Configuration Protocol)? Explain the DORA process (Discover, Offer, Request, Acknowledge).
63. ⭐ What is ARP? How does ARP poisoning work?
64. What is ICMP (Internet Control Message Protocol)? How do ping and traceroute use it? Why do some networks block it?
65. ⭐ HTTP vs HTTPS. What does the S actually add?
66. ⭐ HTTP status code classes — 1xx, 2xx, 3xx, 4xx, 5xx. What do 200, 301, 302, 401, 403, 404, 500, 503 mean? Which ones matter in web attack investigation?
67. HTTP methods — GET, POST, PUT, DELETE, HEAD, OPTIONS. Which are risky if left enabled?
68. SSH (Secure Shell) vs Telnet. Why is Telnet insecure?
69. FTP vs SFTP vs FTPS.
70. SMTP vs POP3 vs IMAP — what each does and their ports.
71. ⭐ What are SPF (Sender Policy Framework), DKIM (DomainKeys Identified Mail), and DMARC (Domain-based Message Authentication, Reporting and Conformance)?
72. What is SMB (Server Message Block)? Why is port 445 exposed to the internet dangerous? (Think WannaCry / EternalBlue.)
73. What is RDP (Remote Desktop Protocol)? Why is it a common attack target?
74. What are LDAP (Lightweight Directory Access Protocol) and Kerberos? How does Kerberos authentication work at a high level?
75. What is SNMP (Simple Network Management Protocol)? Why are v1/v2c insecure?
76. What is NTP (Network Time Protocol)? Why is time sync critical for a SOC?

### 2.4 Devices and Architecture

77. ⭐ Hub vs switch vs router — difference and OSI layer of each.
78. What is a VLAN (virtual local area network)? Why is it used for security?
79. ⭐ What is a DMZ (demilitarized zone)? What do you place in it?
80. ⭐ What is a VPN (virtual private network)? IPsec VPN vs SSL VPN. Site-to-site vs remote access.
81. ⭐ Forward proxy vs reverse proxy. What logs does a proxy give you that a firewall does not?
82. What is a load balancer?
83. What is network segmentation and why does it limit lateral movement?
84. What is a honeypot?

### 2.5 Network Security and Analysis

85. ⭐ What is port scanning? Explain TCP connect scan vs SYN (half-open) scan. How does a port scan look in firewall logs?
86. ⭐ What is Wireshark? Write display filters for: a specific IP, a specific port, only HTTP, only DNS, only SYN packets.
87. Packet capture (PCAP) vs NetFlow — what does each give you?
88. What is DNS tunneling? How do you detect it?
89. What is DNS poisoning / DNS spoofing?
90. What is a DGA (domain generation algorithm)? How would such domains look in DNS logs?
91. What are the signs of beaconing in network traffic?
92. What is IP spoofing? What is MAC spoofing?
93. East-west vs north-south traffic — what is the difference and why does it matter for detection?

---

## 3. SOC — Role, Tools, and Process

### 3.1 SOC Basics

94. ⭐ What is a SOC (security operations centre)? What does it do?
95. ⭐ What are the roles of L1, L2, and L3 analysts? What exactly does L1 do day to day?
96. ⭐ What is the difference between an event, an alert, and an incident?
97. ⭐ Explain true positive, false positive, true negative, and false negative — with an example of each. Which is the most dangerous and why?
98. ⭐ What is alert triage? Walk through how you triage an alert.
99. When do you escalate to L2? What information must the escalation contain?
100. What is a playbook / runbook?
101. What is an SLA (service level agreement) in a SOC? What are MTTD (mean time to detect) and MTTR (mean time to respond)?
102. What is alert fatigue? How is it reduced?
103. What is a shift handover and what must it include?
104. What makes a good incident ticket? What fields do you fill in?

### 3.2 SIEM and Logs

105. ⭐ What is a SIEM (security information and event management) system? How does it work — collection, parsing, normalisation, correlation, alerting?
106. ⭐ Name SIEM tools you know (Splunk, IBM QRadar, Microsoft Sentinel, Elastic, ArcSight, Wazuh). Which have you used hands-on?
107. ⭐ What log sources feed a SIEM? Which are the most valuable and why?
108. What is a correlation rule / use case? Give an example rule for brute-force detection.
109. What is log normalisation and parsing? Why is it needed?
110. What is SOAR (security orchestration, automation and response)? SIEM vs SOAR.
111. SIEM vs EDR vs XDR — where does each fit?
112. Can you write a basic search query? (Splunk SPL — Search Processing Language, or KQL — Kusto Query Language: failed logins by user in the last 24 hours.)
113. What is a baseline? Why do you need one for anomaly detection?

### 3.3 Windows and Linux Logs

114. ⭐ Which Windows Event IDs must you know? Explain: 4624, 4625, 4634, 4648, 4672, 4688, 4720, 4722, 4724, 4728/4732, 4740, 4768, 4769, 4776, 1102, 7045.
115. ⭐ What are Windows logon types? Explain type 2, 3, 4, 5, 7, 10. What does a type 10 from an external IP mean?
116. Where are Windows logs stored? Security vs System vs Application log.
117. What is Sysmon (System Monitor)? Which Sysmon Event IDs are useful (1, 3, 7, 11, 13, 22)?
118. Where are Linux logs? What is in /var/log/auth.log (or /var/log/secure), /var/log/syslog, /var/log/messages?
119. What is syslog? What port does it use?
120. How would you spot suspicious PowerShell activity? (Encoded commands, download cradles, execution policy bypass.)

### 3.4 Incident Response

121. ⭐ Explain the incident response lifecycle — NIST (National Institute of Standards and Technology) four phases, and SANS six steps (Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned).
122. ⭐ Containment vs eradication vs recovery — difference, with examples.
123. What is chain of custody? Why does it matter?
124. What is the order of volatility in evidence collection?
125. Why should you NOT immediately power off an infected machine?
126. What is a post-incident review / lessons learned?

### 3.5 Phishing and Email Analysis

127. ⭐ A user reports a suspicious email. Walk through your full analysis.
128. ⭐ Which email header fields do you check? (From, Return-Path, Reply-To, Received chain, Message-ID, X-Originating-IP, SPF/DKIM/DMARC results.)
129. How do you safely analyse a suspicious URL and a suspicious attachment?
130. How do you find out who else received the same email and who clicked?
131. What is BEC (business email compromise)?

### 3.6 Threat Intelligence and Tools

132. ⭐ Which OSINT (open-source intelligence) tools do you use for investigation? (VirusTotal, AbuseIPDB, urlscan.io, Any.Run, Hybrid Analysis, Shodan, WHOIS, MXToolbox, Cisco Talos.)
133. VirusTotal shows 2 of 70 engines flagging a file. Is it malicious? How do you decide?
134. What is threat intelligence? Strategic vs tactical vs operational.
135. What is threat hunting? How does it differ from alert-driven monitoring?
136. What is a vulnerability scanner (Nessus, Qualys, OpenVAS)? Is a scan alert from the internal scanner IP a true positive?

---

## 4. Scenario Questions (L1 panels lean heavily on these)

137. ⭐ You see 500 failed logins (4625) followed by one success (4624) for the same account from the same IP. What do you do?
138. ⭐ Multiple failed logins across many accounts from one IP, only a few attempts per account. What attack is this? Next steps?
139. ⭐ An endpoint is beaconing to a known-malicious IP every 60 seconds. Walk through your response.
140. ⭐ EDR flags `powershell.exe -enc <base64>` spawned by `winword.exe`. What is happening? What do you check?
141. ⭐ A user clicked a phishing link and entered credentials. What are your immediate actions?
142. A user logs in from Chennai and 20 minutes later from Germany. What is this called (impossible travel)? How do you validate it?
143. Ransomware note appears on one workstation. First five actions, in order?
144. Firewall shows a large outbound data transfer at 02:00 from a finance server to an unknown external IP. How do you investigate?
145. You see a spike in DNS queries with long random subdomains to a single domain. What do you suspect?
146. Antivirus quarantined a file successfully. Is the incident closed? Why or why not?
147. An admin account was created (4720) and added to Domain Admins (4728) outside business hours. What do you do?
148. Security log cleared (1102) on a server. Why is this serious?
149. You get 50 alerts at once at the start of your shift. How do you prioritise?
150. You are fairly sure an alert is a false positive but not certain. What do you do?
151. A web server log shows `' OR 1=1 --` and `UNION SELECT` in request parameters. What is it? How do you tell if it succeeded? (Status codes, response sizes.)
152. A senior manager asks you to whitelist a blocked site urgently. How do you handle it?

---

## 5. HR / Role-Fit Questions (short, but always asked)

153. ⭐ Why do you want to work in a SOC? Why L1?
154. ⭐ Are you comfortable with 24x7 rotational shifts, including nights and weekends?
155. How do you keep yourself updated on new threats? (Name actual sources.)
156. Tell me about a recent cyber attack or breach in the news and what went wrong.
157. Describe your home lab or any hands-on practice (TryHackMe, LetsDefend, Blue Team Labs, CyberDefenders).
158. Which certifications do you have or plan to take? (CompTIA Security+, CEH — Certified Ethical Hacker, Google Cybersecurity, Microsoft SC-200, Splunk Core User.)
159. How do you handle repetitive work and pressure during a live incident?
160. Where do you see yourself in three years — L2, threat hunting, incident response, or detection engineering?

---

## Prep Priority (if short on time)

1. All ⭐ questions in Section 3 and Section 4 — this is where L1 candidates get selected or rejected.
2. Ports list (Q58), OSI model (Q43), TCP handshake (Q46), DNS (Q59), DHCP (Q62).
3. Windows Event IDs and logon types (Q114, Q115).
4. Phishing walkthrough (Q127, Q128) — be able to narrate it end to end without pausing.
5. Kill Chain, MITRE ATT&CK, IOC vs IOA (Q28–Q30).
