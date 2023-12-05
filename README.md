# Network Intrusion Detection System (NIDS) Project

## Overview

This project implements a robust and extensible Network Intrusion Detection System (NIDS) using Python and Scapy. The NIDS is designed to detect and respond to potential threats in network traffic, providing a layer of defense for your network infrastructure.

## Features

### 1. Signature-Based Detection

The NIDS uses signature patterns to identify known threats in network traffic. Signature patterns can include specific strings, patterns, or characteristics associated with malicious activities.

### 2. Logging and Reporting

All detected threats are logged to provide detailed information about the nature of the potential security incidents. Additionally, the system generates periodic reports summarizing network activity, helping security analysts understand the threat landscape.

### 3. AlienVault OTX Integration

The NIDS integrates with AlienVault Open Threat Exchange (OTX) to enhance its detection capabilities. Threat intelligence feeds from OTX are leveraged to dynamically update the signature database, ensuring that the system stays current with the latest threat information.

### 4. Scheduled Updates

To stay proactive against emerging threats, the NIDS schedules regular updates to fetch the latest threat intelligence data. This ensures that the system's signature database is continually updated and reflective of the evolving threat landscape.

### 5. Simulated Threats

The system provides tools and scripts to simulate various types of network activities, including port scanning, malicious payloads, and Denial of Service (DoS) attacks. This allows users to test the NIDS under controlled conditions.





## Prerequisites

- Python
- Scapy
- Requests (for fetching threat data from AlienVault OTX)
- Homebrew (for installing additional tools like hping)

## Setup and Usage








