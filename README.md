# Cybersecurity Lab Setup | Week 01

**VirtualBox • Kali Linux • Network Configuration**

## Overview

This project documents my Week 1 cybersecurity internship task with NETWORKWALKS. I configured a virtual cybersecurity lab using Oracle VirtualBox and Kali Linux to build a foundation for hands-on cybersecurity learning and authorized security testing.

## Objectives

- Set up Kali Linux in VirtualBox.
- Configure a NAT Network with the `10.0.0.0/24` subnet.
- Assign the required IP address to Kali Linux.
- Enable clipboard sharing and drag-and-drop.
- Configure a shared folder between the host and virtual machine.
- Verify network connectivity and internet access.
- Document the lab configuration and setup process.

## Tools Used

| Tool | Purpose |
|---|---|
| Oracle VirtualBox | Virtual machine management |
| Kali Linux | Cybersecurity testing environment |
| NAT Network | Virtual network configuration |
| Linux networking commands | Network verification |

## Lab Configuration

| Component | Configuration |
|---|---|
| Virtualization Platform | Oracle VirtualBox |
| Virtual Machine | Kali Linux |
| Network Mode | NAT Network |
| Network Name | `NatNetwork` |
| Network Subnet | `10.0.0.0/24` |
| Kali Linux IP Address | `10.0.0.2/24` |
| Shared Folder | Host `/downloads` folder |
| Clipboard Sharing | Enabled |
| Drag and Drop | Enabled |

## Setup Procedure

### 1. Configure VirtualBox

Installed and prepared Oracle VirtualBox to run the Kali Linux virtual machine.

### 2. Set Up Kali Linux

Imported and configured Kali Linux as the virtual machine for the cybersecurity lab. After the fresh setup, I took a snapshot named `my fresh kali` so I can restore the clean state at any time.

<img width="1356" height="651" alt="Kali linux" src="https://github.com/user-attachments/assets/cc724f76-641f-416b-8f49-0b6445ce2b41" />


### 3. Configure the NAT Network

Created a NAT Network with the following settings:

- **Network Name:** `NatNetwork`
- **IPv4 Subnet:** `10.0.0.0/24`
- **DHCP Server:** Enabled

Configured the Kali Linux virtual machine to use this network.

<img width="1366" height="768" alt="Nat Network" src="https://github.com/user-attachments/assets/8d777676-1634-4a2e-aaf1-6ea4bd8ad624" />


### 4. Configure the IP Address

Configured the required Kali Linux IPv4 address using the manual method:

```text
IP Address: 10.0.0.2
Subnet Mask: 255.255.255.0
Gateway: 10.0.0.1
DNS Server: 10.0.0.1
```

<img width="1356" height="651" alt="Wired Connection" src="https://github.com/user-attachments/assets/2c9ea903-10a2-4382-a899-bb4b16887589" />


Verified the network configuration using:

```bash
ip a
```

<img width="1356" height="651" alt="ip" src="https://github.com/user-attachments/assets/93603873-6775-47b4-bcac-8715477daf30" />


### 5. Enable Virtual Machine Integration

Configured clipboard sharing, drag-and-drop, and a shared folder to improve file transfer between the host machine and Kali Linux.

### 6. Verify Network Connectivity

Used the following commands to check the network configuration and connectivity:

```bash
ip a
ping 10.0.0.1
ping 8.8.8.8
```

These commands help verify the IP address, gateway reachability, and internet connectivity. Successful results should be confirmed in the running lab.

## Key Learnings

- Virtualization and virtual machine management
- NAT Network configuration
- IPv4 addressing and subnet masks
- Linux network troubleshooting
- Host-to-VM file sharing
- Technical documentation

## Ethical Use

This lab is intended for educational purposes and authorized security testing. Any future testing will be conducted only on systems I own or have explicit permission to assess.

## Project Information

- **Program:** NETWORKWALKS Cybersecurity Internship
- **Week:** 01
- **Project:** Cybersecurity Lab Setup
- **Technologies:** VirtualBox and Kali Linux

## Author

**Sumrah Al Kareem**

BS Cybersecurity and Digital Forensics Student  
GitHub: [My GitHub Profile](https://github.com/sumrah-alkareem)
