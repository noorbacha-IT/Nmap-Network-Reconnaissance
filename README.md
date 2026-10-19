# Nmap-Network-Reconnaissance
Hands-on Nmap covering network reconnaissance, host discovery, ARP, ICMP, TCP probing, IP ranges, and network scanning fundamentals.
Hands-on cybersecurity and networking exploring Nmap, host discovery, network scanning, ARP, ICMP, TCP probing, and IP addressing.

## Overview

This repository documents practical exercises and learning notes related to network reconnaissance and host discovery. It includes work from networking assignments and supporting lab experiments designed to develop a better understanding of how devices can be discovered and analyzed on a network.

The goal is to build practical knowledge of network visibility, reconnaissance techniques, and the fundamentals of network security.

## Objectives

- Understand the fundamentals of network reconnaissance.
- Explore host discovery and network reachability.
- Study ARP requests and their role in local network communication.
- Learn about ICMP-based host discovery.
- Understand TCP SYN and TCP ACK probing.
- Practice IP address ranges and CIDR notation.
- Learn how reverse DNS lookups work.
- Record scan results and interpret observations.
- Understand the importance of authorized and responsible scanning.

## Tools and Technologies

- **Nmap** — Network exploration and host discovery.
- **Wireshark / packet analysis tools** — For observing network traffic when used in the relevant lab.
- **Virtual or simulated networks** — For controlled networking exercises.
- **Command-line tools** — For running commands and documenting results.



## Topics Covered

### 1. Host Discovery

Study methods used to determine whether hosts are reachable on a network and understand how discovery results can vary depending on network configuration and filtering.



### 2. ARP Analysis

Explore ARP requests in a simulated local network and observe which devices receive or process the requests.

**Learning focus:**
- MAC address resolution
- Local network communication
- ARP request behavior
- Network topology and packet visibility

<img width="975" height="501" alt="image" src="https://github.com/user-attachments/assets/8f902b24-b834-4fc7-9f72-8465474fdf62" />

### 3. ICMP-Based Discovery

Review Nmap's ICMP discovery options:

| Option | Purpose |
|---|---|
| `-PE` | ICMP echo request discovery |
| `-PP` | ICMP timestamp request discovery |
| `-PM` | ICMP address mask request discovery |

The actual response depends on host configuration, firewall rules, and network policies.

<img width="975" height="289" alt="image" src="https://github.com/user-attachments/assets/979af635-7c3e-4fc3-bb9c-015a5e11b63e" />


### 4. TCP-Based Discovery

Explore TCP probes used for host discovery.

| Option | Purpose |
|---|---|
| `-PS` | TCP SYN discovery probe |
| `-PA` | TCP ACK discovery probe |
| `-PS23` | TCP SYN discovery probe targeting port 23 |

These options help demonstrate how TCP-based probes can provide information about host reachability. They do not, by themselves, establish that a system is vulnerable.



### 5. IP Addressing and CIDR

Practice interpreting network ranges and CIDR notation.

Example from the assignment:

- Address: `10.10.12.13/29`
- Corresponding network: `10.10.12.8/29`
- Address range: `10.10.12.8`–`10.10.12.15`
- Conventional usable host range: `10.10.12.9`–`10.10.12.14`


This example illustrates how a subnet prefix determines the size of a network.

<img width="975" height="157" alt="image" src="https://github.com/user-attachments/assets/2e576792-6f7f-4935-81e0-2f1d46f30641" />
<img width="975" height="423" alt="image" src="https://github.com/user-attachments/assets/2878dab3-d7d2-4ba2-bede-c0d9ebb657ee" />

### 6. Reverse DNS Lookup

Learn about the Nmap `-R` option, which requests reverse DNS resolution for target IP addresses.

Reverse DNS results depend on available DNS records and resolver configuration.

<img width="974" height="523" alt="image" src="https://github.com/user-attachments/assets/887b80e6-a1e2-41fc-8ecb-098d64a0049d" />

<img width="975" height="363" alt="image" src="https://github.com/user-attachments/assets/5a3ae360-b28c-4f0f-8c8f-f7f1ba164155" />



## Disclaimer

This repository is intended for educational purposes and professional portfolio development. All practical scanning must be performed only on systems, networks, or lab environments that I own or am explicitly authorized to assess.

