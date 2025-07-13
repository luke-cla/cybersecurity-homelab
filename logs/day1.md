# Log 1 – Raspberry Pi 3 Honeypot Setup

## Objective
Begin building a segmented cybersecurity homelab by configuring a Raspberry Pi 3 B+ as a honeypot inside a DMZ network segment using OpenCanary.

## Hardware Used
- Raspberry Pi 3 B+
- 32GB microSD card
- USB-C card reader
- Ethernet cable
- Monitor and keyboard (for initial setup)
- Old Acer laptop (used to flash the SD card and run SSH)

## Software Installed on Pi 3
- Raspberry Pi OS Lite
- OpenCanary (lightweight honeypot framework)
- Core tools for management and testing `nmap`, `net-tools`, `vim`, `curl`, `htop`

## Network Configuration
- Static IP assigned on local subnet
- Configured for both `wlan0` (Wi-Fi) and `eth0` (Ethernet)
- SSH access verified over Ethernet

## OpenCanary Setup
- Installed with `pip` in a virtual environment
- Custom `opencanary.conf` file created and edited
- Enabled select services (e.g., HTTP, FTP) to simulate a vulnerable target
- Disabled SSH to avoid conflicts with actual remote access
- OpenCanary started successfully with no errors
- Log generation verified

## Next Steps
- Begin setup of Raspberry Pi 5 as the SIEM and monitoring system
- Design a basic network segmentation diagram
- Add the OpenCanary config file to the repository for reference
