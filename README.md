# Task 5: Capture and Analyze Network Traffic Using Wireshark

## Objective
Capture live network packets using Wireshark and analyze them to identify basic protocols such as TCP, DNS, UDP, and TLS.

## PCAP File Analyzed
**File Name**: `merged.pcap`

## Protocols Identified
- **TCP**: Reliable data transmission with connection handshakes.
- **UDP**: Fast, connectionless protocol observed in DNS.
- **DNS**: Resolves domain names into IPs.
- **TLS/HTTPS**: Secure HTTP communication through TLS handshake.
- **ICMP (if present)**: Used during ping operations.

## Key Observations
- Captured packets included DNS queries and TCP connections.
- TLS handshakes indicate HTTPS activity.
- Packets show both internal and external IP communication.

## Sample Packet Summary
| Source IP     | Destination IP | Protocol | Length |
|---------------|----------------|----------|--------|
| 192.168.1.23   | 8.8.8.8        | DNS      | 74     |
| 192.168.3.45   | 142.x.x.x      | TCP      | 66     |
| 142.164.34.12  | 192.168.x.x    | TCP      | 60     |
| 192.168.1.23   | 142.x.x.x      | TLS      | 125    |

## Summary
This task demonstrates the basics of network packet capture and analysis. Wireshark enabled protocol filtering and traffic breakdown which is useful for troubleshooting and learning network behavior.
