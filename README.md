# Cybersecurity Week 2 Projects

**Projects:** W2-PM4 — Footprinting & Reconnaissance with theHarvester; W2-PM5 — Network Scanning with Zenmap  
**Author:** `[ESTHER TAFADZWA MADZIWA]`  
**Date:** `[13 November 2026]`

## Overview

This repository documents two educational cybersecurity practicals:

1. **theHarvester:** query public sources for information associated with `microsoft.com`, following the project guide.
2. **Zenmap:** identify my local network configuration, discover responding hosts on my own/authorized LAN, review available IP/MAC address information, and export a network topology.

> **Scope and ethics:** These activities are for educational purposes. Network discovery must be limited to a network you own or have explicit permission to assess. The report records reconnaissance and host discovery only; it does not claim that a vulnerability was confirmed.

## Tools

- Kali Linux terminal
- [theHarvester](https://github.com/laramies/theHarvester)
- Windows Command Prompt (`ipconfig`)
- [Zenmap / Nmap](https://nmap.org/download.html)

## Project 1 — Footprinting with theHarvester (W2-PM4)

### Task 1: Baidu source

Command used in the lab:

```bash
theHarvester -d microsoft.com -l 1000 -b baidu
```

**Purpose:** Search the specified domain using Baidu, with the result limit set to 1,000.

**My observations:** 

### Task 2: All sources

Command used in the lab:

```bash
theHarvester -d microsoft.com -l 50 -b all
```

**Purpose:** Search the specified domain using all sources supported by the installed version, with the result limit set to 50.



## Project 2 — Network Scanning with Zenmap (W2-PM5)

### Procedure

1. Installed/opened Zenmap on Windows.
2. Used `ipconfig` in Command Prompt to identify my local IPv4 address and subnet.
3. Entered my actual local subnet into Zenmap.
4. Selected **Ping Scan** to discover hosts responding on the authorized local network.
5. Recorded the scan's host count and the IP addresses; recorded MAC addresses where available from the scan or local system information.
6. Opened **Topology**, enabled the legend, and exported the topology as a PDF.

### My results

| Item | My observed result |
|---|---|
| Local IPv4 address | `[192.168.56.1]` |
| Subnet mask / prefix | `[255.255.255.0]` | |
| Number of responding hosts | `[1]` |

### Discovered hosts

Replace these placeholders with your own results. Do not copy example addresses from the lab guide unless they match your actual scan.

| Host / device | IP address | MAC address (if observed) |
|---|---|---|
| `[Host 1]` | `[192.168.56.1]` | `[MAC : not available]` || | |



## Key Learning Outcomes

- Practiced querying public information sources with theHarvester.
- Compared the use of one specified source with an all-sources query.
- Learned to identify local IP configuration and subnet information.
- Practiced a Zenmap Ping Scan and documented responding hosts.
- Exported a network topology for reporting.
- Learned that discovery results are observations, not proof of a vulnerability.

## Limitations

Results depend on the data sources available at the time and on local network configuration. A host may not respond to a Ping Scan, and the absence of a response does not prove that a device is absent. These practicals did not include exploitation or vulnerability validation.


## Author

`[Esther Tafadzwa Madziwa]`  
# Penetration-Testing-Report
