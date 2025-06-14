# Scanning-and-Enumerating-a-Local-Network-with-Nmap-on-Kali-Linux

This project demonstrates how to perform network scanning and enumeration using Nmap on Kali Linux. It covers discovering active hosts, identifying open ports and services, and fingerprinting operating systems on a local network.

# Project Goals

- Learn how to use Nmap for network reconnaissance
- Understand different types of Nmap scans
- Enumerate services and detect OS and device types
- Develop a basic understanding of local network topologies

# Environment & Tools
• Base OS: Kali Linux 2023.x (Debian-based)
• Virtualization: VMware Workstation / VirtualBox (if applicable)
• Network Setup: Local Area Network (Wi-Fi or Ethernet)
• Main Tool: Nmap 7.94

# Installation

Nmap is preinstalled within Kali Linux. To verify the installation use: 
sudo apt-get update && sudo apt-get install nmap
![unnamed (1)](https://github.com/user-attachments/assets/7725d338-1043-4970-8782-f8c71d5948a1)

# Process

Scan Number 1: Basic Network Scan
Command: nmap 192.168.231.0/24 (List of active devices with IP and Port)

Expected Output:
![unnamed (2)](https://github.com/user-attachments/assets/b31f9870-9084-4010-b850-989b73f00841)

Scan Number 2: Scanning for a specific port
Command: nmap -p 80 192.168.231.0/24 (List of devices with specific port ie. 80)

Expected Output:
![unnamed (3)](https://github.com/user-attachments/assets/2a713466-09be-4c0b-bec4-eb1a1edb1ac5)

Scan Number 3: Service Version Detection
Command: nmap -sV 192.168.231.0/24 (Lists all of the ports with their service and version details)

Expected Output:
![unnamed (4)](https://github.com/user-attachments/assets/6d9fd596-18b0-40ca-b279-cb38f912567c)
![unnamed (5)](https://github.com/user-attachments/assets/bb9e2157-2b21-4ae8-8b4a-7a0adac9e6de)

Scan Number 4: Operation System Detection
Command: sudo nmap -O 192.168.231.0/24 (Lists the operating systems of the listed networks)

Expected Output:
![unnamed (6)](https://github.com/user-attachments/assets/4c693378-82aa-4064-83ad-b4bdb46fc6e7)
![unnamed (7)](https://github.com/user-attachments/assets/95e57994-70a3-4c68-9e2f-dc5625a023c5)

Scan Number 5: Aggressive Scan 
Command: sudo nmap -A 192.168.231.0/24 (Lists everything, including OS, version, scripts and traceroute)

Expected Output: 
![unnamed (8)](https://github.com/user-attachments/assets/43cdaae3-1044-4c60-b5b3-2f2d0e32609a)
![unnamed (9)](https://github.com/user-attachments/assets/3ae4bb3d-bbd9-4fee-b24d-282aa29228ff)
![unnamed (10)](https://github.com/user-attachments/assets/7a2a493f-14a4-400c-b0ae-9c9ad5f41910)


