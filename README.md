Network Scanner - ARP
=====================

🔍 A Simple Network Scanner with Python & Scapy

A lightweight and effective network scanner script written in Python using Scapy.
This tool scans a local network to identify connected devices by sending ARP requests 
and capturing the responses.

------------------------------------------------
🧠 What It Does:
------------------------------------------------
- Broadcasts ARP requests on the specified IP range (e.g., 192.168.1.1/24)
- Collects replies from active hosts
- Displays IP and MAC addresses of connected devices in a neat table

------------------------------------------------
🛠️ How It Works:
------------------------------------------------
Uses the following Scapy modules:

from scapy.all import ARP, Ether, srp

- ARP: Sends queries to devices asking for their MAC addresses.
- Ether: Creates a broadcast Ethernet frame (to ff:ff:ff:ff:ff:ff).
- srp(): Sends and receives packets at Layer 2 (Data Link Layer).

------------------------------------------------
📋 Output Example:
------------------------------------------------
Available devices in the network:

IP Address         MAC Address
------------------------------------------
192.168.1.2        00:11:22:33:44:55
192.168.1.5        AA:BB:CC:DD:EE:FF

------------------------------------------------
🚀 How to Run:
------------------------------------------------
1. Clone the repository:
   git clone https://github.com/MudigolamBharath/Network_Scanner-ARP-.git
   cd Network_Scanner-ARP-

2. Install dependencies:
   pip install scapy

3. Run the script (use sudo/root if needed):
   sudo python3 scanner.py

------------------------------------------------
⚠️ Disclaimer:
------------------------------------------------
This tool is intended for educational and ethical use only.
Do NOT use it to scan networks without proper authorization.
Unauthorized scanning may be illegal.

