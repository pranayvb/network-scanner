# network-scanner

# Network Scanner

A simple yet effective network scanner built using Python for Linux-based operating systems. This tool allows users to quickly scan a target IP range and identify active hosts in the network. It is designed to be used from the command line and can scan entire subnets efficiently.

## How It Works
This script uses the ARP protocol to identify live hosts. It sends an ARP request to each IP in the target range, and when a device responds, it captures the response to extract its IP and MAC address. This approach works well because ARP is essential in local networks to map IP addresses to MAC addresses, and any active device will respond to ARP requests.

## Features
- Scans for live hosts in the specified IP range.
- Lightweight and easy to use.
- Designed for Linux OS, leveraging Python's standard libraries.
  
## Requirements
- Python 3.x
- Scapy (for sending and receiving network packets)
  

#to use -

## To run it in terminal go to the directory where u saved it :
-cd <directory>
-python3 network_scanner -h
  

  
## usage: network_scanner.py [-h] [-t TARGET]

optional arguments:
  -h, --help            show this help message and exit
  -t TARGET, --target 
   - TARGET Target IP range.
  

  -eg :
  python3 network_scanner.py -t 192.168.13.1/24


  
