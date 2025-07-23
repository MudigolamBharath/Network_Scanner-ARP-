# Network_Scanner-ARP
🔍 Simple Network Scanner with Python & Scapy
A lightweight and effective Network Scanner script written in Python using Scapy. This tool scans a local network to identify connected devices by sending ARP requests and capturing the responses.

🧠 What It Does
This script:

Broadcasts ARP requests on the specified IP range (e.g., 192.168.1.1/24)

Collects replies from active hosts

Displays IP and MAC addresses of connected devices in a neat format

🛠️ How It Works

from scapy.all import ARP, Ether, srp
ARP is used to query devices for their MAC address

Ether is used to send a broadcast

srp() sends and receives packets at layer 2

📋 Output Example:
Available devices in the network:
IP                  MAC
192.168.1.2         00:11:22:**:**:**
192.168.1.5         aa:bb:**:**:**
🚀 How to Run
Clone the repo:

git clone https://github.com/MudigolamBharathNetwork_Scanner-ARP-.git
cd network-scanner
Install dependencies:

pip install scapy
Run the script (root/sudo might be required):

sudo python3 scanner.py
⚠️ Disclaimer
This tool is intended for educational and ethical use only. Do not use it to scan networks without proper authorization.
