# Security Fundamentals

This page introduces fundamental security concepts. Controls are used as a guideline for protecting an organization's assets.

# <span style="font-size: 26px;">Physical Controls</span>

Physical controls aim to prevent unauthorized access to a building or areas inside. This is accomplished by implementing deterrents and monitoring and access controls. 

- Detterent Example: a warning sign about beware of dog

- Monitoring Example: CCTV watching one or several points of interest on the property

- Access Example: gates or locks

These are important because it's over. Hackers will win if they walk into your data center and directly connect to the assets. 

# <span style="font-size: 26px;">Network Security Controls</span>

- Network Intrusion Detection (NIDS): software or physical devices that generate alerts that require humans to investigate. 

- Network Intrusion Prevention (NIPS): software that will take action automatically. 

- Firewall: used for network separation and restricts traffic. Typically, one will be positioned to limit traffic from the internet to the network.

# <span style="font-size: 26px;">Endpoint Security Controls</span>

Endpoint controls provide insight into real-time actions on assets such as servers, desktops, and more. 

- Host Intrusion Prevention (HIPS): software installed on the endpoint that will take action without human intervention once malicious activity has occurred

- Antivirus: There are two types: signature and behavioral. Signature checks previously known malware from the "signature" assigned to it. Behavior requires a set baseline; anything above that threshold triggers an alert.

- Log Monitoring: An endpoint can be configured to send logs to an SIEM (Security Information and Event Manager). The data is tested against rules for potentially malicious behavior. This requires human intervention.

- Endpoint Detection and Response: agents run on assets, collect logs, monitor activity, and take action. They display data in different categories on a dashboard. 

# <span style="font-size: 26px;">Email Security Controls</span>

- Spam Filters: software that scans emails for malicious content and takes action to preventing them from an employees inbox

- Data Loss Prevention (DLP): prevents information such as financial or PII (personally identifiable information) from being leaked. Actions are also automated.

- Security Awareness Training: a mandatory program for all employees to educate them to be vigilant about actions over the internet.

# <span style="font-size: 26px;">Useful Networking Commands</span>

- ipconfig: shows network details and configuration of the host. included are the IP address, gateway and DNS

- "ip -a" shows ip address of the device

- "ip r list" shows the routing table on the device

- "ip link set dev [device name] [up/down]" will set the device network configuration up or down

- "traceroute" shows the PATH to an ip address

- "traceroute -p" shows the path with a specific port

- "Dig" and "Nslookup" are commands to query dns domains for Windows and Linux

- "dig [domain]" to query domain for A (address) records

- "dig [domain] MX" to query for mail exchange records

- "dig [domain] ANY" to query for all records

- Netstat is a command to show all current TCP and UDP network connections

- "netstat -a" shows all active connections and listening ports on the system

- "netstat -a -b" same as above but adds the process executing it

- "netstat -s -p -tcp -f" shows the statistics (-s) for protocols (-p) TCP (-tcp) in the format FQDN (-f) (fully qualified domain name)

- NMAP (Network Mapper) is a tool used to conduct network discovery. It can reveal ports, services, devices, operating systems and more.

- "-sv" service detection

- "V" verbosity level (how much information)

- "-O" operating system detection

- "-sC" to run default scripts

- "-Pn" removes host discovery to scan regardless

- "-sS" TCP SYN Scan for stealth and quickness

- "-sT" TCP Connect scan for complete handshake

- "-sU" UDP connect scan

- "-sA" TCP ACK scan to check for firewalls

- Well-known ports and services

-  20,21 FTP transfer files between systems

-  22 SSH (Secure Shell) connects to host with encryption

-  23 Telnet connection to host without encryption

-  25 SMTP (Simple Mail Transfer Protocol) sends emails to external servers (transport only)

-  53 DNS (Domain Name Server) uses relational databases to transfer machine ip addresses to human readable names. (IP addresses to Hostnames, 8.8.8.8 becomes google.com)

-  67,68 DHCP (Dynamic Host Configuration Protocol) automatically assigns ip addresses to machines in the environment

-  80,443 HTTP/HTTPS Insecure and Secure web protocols for retrieving content

-  514 UDP Syslog information that gets sent to the SIEM

-  3389 RDP Microsoft protocol to connect to other hosts
