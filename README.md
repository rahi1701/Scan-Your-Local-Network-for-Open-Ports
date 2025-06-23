# Scan-Your-Local-Network-for-Open-Ports

Learn to discover open ports on devices in your local network to understand network exposure.

Run nmap tool to perform TCP SYN Scan.

Use below Command for check open port in your network

        nmap -sS 10.0.2.15/24 

Insted of 10.0.2.15/24 use your network rang.

In the code -s switch determines the type of scan to perform.

-sS for SYN Scan.

Result for my nmap scanning 

\\        
┌──(kali㉿kali)-[~]
└─$ nmap -sS 10.0.2.15/24
Starting Nmap 7.95 ( https://nmap.org ) at 2025-06-23 06:41 EDT
Nmap scan report for 10.0.2.2
Host is up (0.0029s latency).
Not shown: 997 filtered tcp ports (no-response)
PORT     STATE SERVICE
135/tcp  open  msrpc
445/tcp  open  microsoft-ds
5900/tcp open  vnc
MAC Address: 52:55:0A:00:02:02 (Unknown)

Nmap scan report for 10.0.2.3
Host is up (0.0035s latency).
Not shown: 999 filtered tcp ports (net-unreach)
PORT   STATE SERVICE
53/tcp open  domain
MAC Address: 52:55:0A:00:02:03 (Unknown)

Nmap scan report for 10.0.2.15
Host is up (0.0000020s latency).
All 1000 scanned ports on 10.0.2.15 are in ignored states.
Not shown: 1000 closed tcp ports (reset)

Nmap done: 256 IP addresses (3 hosts up) scanned in 7.26 seconds
