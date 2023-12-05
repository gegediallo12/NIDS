# Network Intrusion Detection System (NIDS) Project

## Introduction

This project implements a simple Network Intrusion Detection System (NIDS) using Python and Scapy. The NIDS is designed to detect specific network activities based on signature patterns.

## Features

- **Signature-Based Detection:** The system uses signature patterns to identify potential threats in network traffic.

- **Logging and Reporting:** Detailed information about detected threats is logged, and periodic reports summarizing network activity and potential security incidents are generated.

- **Integration with AlienVault OTX:** The NIDS can fetch threat intelligence data from AlienVault OTX and dynamically update the signature database.

- **Scheduled Updates:** Regular updates are scheduled to fetch the latest threat intelligence data and keep the NIDS signature database up-to-date.

- **Simulated Threats:** The system can be tested by simulating different types of network activities, such as port scanning and DoS attacks.





## Prerequisites

- Python
- Scapy
- Requests (for fetching threat data from AlienVault OTX)
- Homebrew (for installing additional tools like hping)

## Setup and Usage





