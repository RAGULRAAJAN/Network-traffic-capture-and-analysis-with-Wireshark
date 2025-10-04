# Network-traffic-capture-and-analysis-with-Wireshark
## AIM:
To capture and analyze network traffic using Wireshark in order to observe protocols, packets, and potential anomalies.
## Requirements:
- **Hardware:**
    - Computer with internet access
    - Network adapter (Ethernet/Wi-Fi)
- **Software:**
    - Wireshark (latest stable version)
    - Sample PCAP files (optional for offline analysis)
## Architecture:
```mermaid
flowchart TD
    A[Network Interface Card] --> B[Wireshark Packet Capture Engine]
    B --> C[Packet Decoder & Protocol Analyzer]
    C --> D[Packet Display & Filtering Interface]
    D --> E[Investigator Analyzes Network Data]
    E --> F[Findings: IPs, Ports, Protocols, Anomalies]
```
## DESIGN STEPS:
### Step 1:
Install Wireshark on the system.

### Step 2:
Launch Wireshark and select the network interface (Ethernet/Wi-Fi).

### Step 3:
Start the capture, apply filters (like http, tcp, ip.addr == x.x.x.x) to analyze specific traffic, and stop the capture after observing relevant data.
### Step 4:
**Analyze traffic to identify:**
  - Source & Destination IP addresses
  - Protocols (HTTP, DNS, TCP, UDP, etc.)
  - Suspicious activities (e.g., unusual ports, repeated requests).
## PROGRAM:

Wireshark Packet Capture and Filter Usage
## 1. Open Wireshark and Select a Network Interface

<img width="1919" height="1079" alt="Screenshot 2025-10-04 140800" src="https://github.com/user-attachments/assets/184242fc-435d-4f64-8a57-a8ae325ff022" />
## 2. Start Capturing Packets

• Click the blue shark fin icon or double-click the interface. • Wireshark will start capturing all real-time traffic.
<img width="1919" height="1077" alt="Screenshot 2025-10-04 140854" src="https://github.com/user-attachments/assets/c76bb47e-f454-4b92-b697-3d85b286459c" />
## 3. Apply Filters to Focus on Specific Traffic
• Use filters like http, ip.addr == 192.168.1.1, or tcp.port == 80 in the top filter bar to narrow down results.
<img width="1919" height="1079" alt="Screenshot 2025-10-04 140938" src="https://github.com/user-attachments/assets/53dbdc94-5c92-42c8-9bba-5ce2392aece8" />
## 4. Analyze Packet Details
• Click on a packet to view its detailed breakdown including frame, Ethernet, IP, TCP/UDP layers, and data payload.
<img width="957" height="446" alt="Screenshot 2025-10-04 141020" src="https://github.com/user-attachments/assets/6cca46d2-dda5-472f-ad42-15540caae6f3" />
## 5. Export or Save the Capture
• Go to File > Save As to store the capture in .pcap format for future analysis.
<img width="1919" height="1079" alt="Screenshot 2025-10-04 141202" src="https://github.com/user-attachments/assets/deab9192-ad68-460d-ba2c-ed200b3b1bed" />

## OUTPUT:
Captured Packets with Protocol Analysis and Detailed Packet Info

## RESULT:
Network traffic was successfully captured and analyzed using Wireshark.
