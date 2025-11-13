# 1-Task
The primary goal of this task was to learn and practice basic network reconnaissance by discovering open ports on devices within the local network using Nmap to understand the network's exposure to potential security risks
Microsoft Windows [Version 10.0.26100.6899]
C:\Users\User>ipconfig
Windows IP Configuration
Wireless LAN adapter Local Area Connection* 1:
Media State
: Media disconnected
Connection-specific DNS Suffix :
Wireless LAN adapter Local Area Connection* 2:
Media State
: Media disconnected
Connection-specific DNS Suffix :
Wireless LAN adapter Wi-Fi:
Connection-specific DNS Suffix :
Link-local IPv6 Address
IPv4 Address.
: 192.168.248.81
Subnet Mask
: 255.255.255.0
Default Gateway
: fe80::ffe6:bd98:3652:6d58%5
: 192.168.248.254
Ethernet adapter Bluetooth Network Connection:
Media State
: Media disconnected
Connection-specific DNS Suffix :
C:\Users\User>nmap -sS 192.168.248.0/24
Starting Nmap 7.98 (https://nmap.org) at 2025-11-13 21:50 +0530
Nmap scan report for 192.168.248.254
Host is up (0.0043s latency).
Not shown: 999 closed tcp ports (reset)
PORT STATE SERVICE
53/tcp open domain
MAC Address: FA:04:59:63:02:F6 (Unknown)
Nmap scan report for 192.168.248.81
Host is up (0.00052s latency).
Not shown: 996 closed tcp ports (reset)
PORT STATE SERVICE
135/tcp open msrpc
139/tcp open netbios-ssn
445/tcp open microsoft-ds
3306/tcp open mysql
Nmap done: 256 IP addresses (2 hosts up) scanned in 6.47 seconds
