# Using-NIST-Cybersecurity-Framework

## Incident Report Analysis

### Summary
Recently, there was a report to the Cybersecurity Team that the organization’s network services suddenly stopped responding due to an incoming flood of ICMP packets. Normal internal network traffic could not access any network resources.

### Identify
The company’s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the company’s network through a distributed denial of service (DDoS) attack.

### Protect
To address this security event, the network security team implemented: 

1) A new firewall rule to limit the rate of incoming ICMP packets
2) Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets
3) Network monitoring software to detect abnormal traffic patterns
4) An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics

### Detect
To detect new unauthorized access attacks in the future, the team will use a firewall logging tool and an intrusion detection system (IDS) to monitor all incoming traffic.

### Respond
The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services.

### Recover
The team will recover the deleted data by restoring the database from the previous verified backup. We also informed the users that the system will be restored gradually to avoid cloud misconfiguration. This will help in hardening the OS from future attacks.
