# Incident Report Analysis

**Framework:** NIST Cybersecurity Framework (CSF)
**Incident Type:** ICMP Flood – Denial of Service (DoS)

---

## Summary

The organization experienced a Denial of Service (DoS) attack based on an ICMP packet flood, which caused internal network services to become unavailable for approximately two hours. The incident occurred due to the lack of proper ICMP traffic filtering and rate-limiting rules on a misconfigured firewall. During the incident, the incident response team blocked ICMP traffic, temporarily disabled non-critical services, and restored essential network services. After containment, additional security controls were implemented to reduce the likelihood of similar incidents in the future.

---

## Identify

* Identification of a DoS attack targeting the internal network through ICMP flooding.
* Firewall misconfiguration that allowed unrestricted ICMP traffic.
* Insufficient preventive controls to mitigate denial-of-service attacks.
* Direct impact on the availability of critical network assets and internal services.

---

## Protect

* Implementation of firewall rules with ICMP **rate limiting**.
* Source IP address validation to mitigate **IP spoofing** attacks.
* Establishment of secure configuration policies for firewalls and network devices.
* Technical staff training focused on periodic security configuration reviews.

---

## Detect

* Deployment of network monitoring software to identify abnormal traffic patterns.
* Use of IDS/IPS systems to detect and filter suspicious ICMP traffic.
* Configuration of automated alerts for unusual spikes in ICMP packets.

---

## Respond

* Immediate blocking of ICMP traffic at the firewall to contain the attack.
* Temporary shutdown of non-critical network services.
* Prioritized restoration of essential services.
* Post-incident investigation to identify root causes and exploited vulnerabilities.

---

## Recover

* Full restoration of normal network operations.
* Permanent adjustments to firewall rules and security policies.
* Continuous use of monitoring and detection tools.
* Updates to the incident response plan based on lessons learned.

---

## Reflections / Notes

This incident highlighted the importance of a proactive approach to network security. While the NIST CSF provides a solid foundation for incident response, effective cybersecurity requires continuous monitoring, proper configuration management, and constant adaptation to emerging threats. Applying the framework in practice strengthened the organization’s network resilience and overall security posture.
