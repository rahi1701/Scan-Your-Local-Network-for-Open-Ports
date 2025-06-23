# Scan-Your-Local-Network-for-Open-Ports

Learn to discover open ports on devices in your local network to understand network exposure.

Run nmap tool to perform TCP SYN Scan.

Use below Command for check open port in your network

        nmap -sS 192.168.1.0/24 

In the code -s switch determines the type of scan to perform.

-sS for SYN Scan.

Insted of 192.168.1.0/24 use your network rang.
