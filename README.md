# Security Fundamentals

This page introduces fundamental security concepts. Controls are used as a guideline for protecting an organization's assets.

# <span style="font-size: 26px;">Physical Controls</span>

Physical controls aim to prevent unauthorized access to a building or areas inside. This is accomplished by implementing deterrents and monitoring and access controls. 

- Detterent Example: a warning sign about beware of dog

- Monitoring Example: CCTV watching one or several points of interest on the property

- Access Example: gates or locks

These are important because it's over. Hackers will win if they walk into your data center and directly connect to the assets. 

# <span style="font-size: 26px;">Network Security Controls</span>

-Network Intrusion Detection (NIDS): software or physical devices that generate alerts that require humans to investigate. 

-Network Intrusion Prevention (NIPS): software that will take action automatically. 

-Firewall: used for network separation and restricts traffic. Typically, one will be positioned to limit traffic from the internet to the network.

# <span style="font-size: 26px;">Endpoint Security Controls</span>

Endpoint controls provide insight into real-time actions on assets such as servers, desktops, and more. 

-Host Intrusion Prevention (HIPS): software installed on the endpoint that will take action without human intervention once malicious activity has occurred

-Antivirus: There are two types: signature and behavioral. Signature checks previously known malware from the "signature" assigned to it. Behavior requires a set baseline; anything above that threshold triggers an alert.

-Log Monitoring: An endpoint can be configured to send logs to an SIEM (Security Information and Event Manager). The data is tested against rules for potentially malicious behavior. This requires human intervention.

-Endpoint Detection and Response: agents run on assets, collect logs, monitor activity, and take action. They display data in different categories on a dashboard. 

# <span style="font-size: 26px;">Email Security Controls</span>

-Spam Filters: software that scans emails for malicious content and takes action to preventing them from an employees inbox

-Data Loss Prevention (DLP): prevents information such as financial or PII (personally identifiable information) from being leaked. Actions are also automated.

-Security Awareness Training: a mandatory program for all employees to educate them to be vigilant about actions over the internet.
