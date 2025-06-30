# Task-5-Capture-and-Analyze-Network-Traffic-Using-Wireshark

##  Objective

Capture live network packets using Wireshark, apply protocol filters, and analyze common network traffic types such as DNS, ICMP, and TCP.

##  Tools Used

- **Wireshark** (Packet capture tool)
- **Command Prompt** (for ping operations)
- **Google Chrome** (or any web browser)

## Steps Performed

1. Installed Wireshark and Npcap (packet capture driver).
2. Ran Wireshark as Administrator.
3. Started packet capture on the active network interface (Wi-Fi).
4. Generated traffic by:
   - Visiting a website in the browser
   - Pinging `8.8.8.8` using Command Prompt (`ping 8.8.8.8`)
5. Stopped the capture after about 1 minute.
6. Applied filters:
   - `icmp` – to view ping packets
   - `dns` – to see domain name resolution
   - `tcp` – to check web or secure traffic (HTTPS)
7. Saved the capture as: `network_capture.pcapng`
8. Analyzed protocols and summarized results

## Protocols Identified

| Protocol | Description                                                                                                                                         |
|----------|-------------                                                                                                                                        |
| **ICMP** | Used for network diagnostics (e.g., ping). ICMP Echo Request/Reply packets were captured when pinging 8.8.8.8.                                      |
| **DNS**  | Domain Name System queries were captured when accessing websites. Shows how domain names are resolved to IP addresses.                              |
| **TCP**  | Transmission Control Protocol – observed for most reliable connections, especially in web communication. TLS (encrypted HTTPS) was present as well. |

##  Files Included

- `network_capture.pcapng` – Packet capture file containing recorded traffic.



