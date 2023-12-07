# Network Intrusion Detection System (NIDS)

## Overview

This project implements a simple Network Intrusion Detection System (NIDS) using Python and Scapy. The NIDS is designed to capture and analyze network packets, detect potential threats based on predefined signatures.

## Requirements

- Python 3.x
- Scapy


## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/gegediallo12/nids-project.git
    cd nids-project
    ```

2. Create and activate a virtual environment:

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3. Install required packages:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Start the NIDS to capture and analyze packets:

    ```bash
    python NIDS.py
    ```

2. Observe the console for alerts and packet details.

3. Optionally, simulate network activities for testing:

    - Use tools like Nmap for port scanning:

        ```bash
        nmap -Pn 192.168.0.1
        ```

    - Use hping3 to simulate ICMP traffic:

        ```bash
        hping3 --icmp 192.168.0.1
        ```

## Configuration

- Signature Database: Edit the `signature_database` list in `NIDS.py` to customize threat signatures.
- AlienVault OTX: Replace the placeholder API key (`otx_api_key`) and pulse URL (`otx_url`) with your actual OTX API key and pulse URL.

## External Threat Feeds Integration

Integrate your NIDS with external threat intelligence feeds to enhance detection capabilities. Leverage threat feeds to update your signature database dynamically.

## Logging and Reporting

Improve logging mechanisms to store detailed information about detected threats. Generate periodic reports summarizing network activity and potential security incidents.

## Schedule Updates

Schedule regular updates to fetch the latest threat intelligence data and update your NIDS signature database. This ensures that your system remains up-to-date with the latest threat information.

## Troubleshooting

If you encounter issues with dependencies, ensure that you have installed the required packages and activated the virtual environment.

## Code Explanation

The `NIDS.py` script includes the following key components:

### Signature-Based Detection

The `signature_database` list defines various threat signatures, such as ICMP Echo Reply, ICMP Packets, Malware, DoS, and Port Scan.

### AlienVault OTX Configuration

Configure the AlienVault OTX API key (`otx_api_key`) and pulse URL (`otx_url`) to fetch threat data.

### Traffic Analysis

The `packet_callback` function is called for each captured packet, checking against the defined signatures and logging alerts.

### Fetching Threat Data

The `fetch_threat_data` function fetches threat data from AlienVault OTX using the configured API key and pulse URL.

### Updating Signature Database

The `update_signature_database` function is a placeholder for logic to process threat data and update the signature database.

### Packet Capture

Packet capture is initiated using Scapy's `sniff` function on the 'en0' interface.

---












