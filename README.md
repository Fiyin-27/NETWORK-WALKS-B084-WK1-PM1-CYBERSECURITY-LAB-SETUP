<div align="center">

# 🔐 Cybersecurity Lab Setup

Building a virtual environment for cybersecurity learning and ethical hacking practice.

</div>

---

## 📌 Project Overview

This project documents the setup of a cybersecurity laboratory using VirtualBox and Kali Linux.

The purpose is to create a virtual environment for learning and practicing cybersecurity concepts, including networking security,vulnerability assessment and authorized penetration-testing activities.

The lab uses a private NAT Network with the address range `10.0.0.0/24`, while Kali Linux is assigned the IP address `10.0.0.2/24`. This setup provides a foundation for adding more virtual machines in the future for authorized security testing.

The environment will also support future cybersecurity projects and practical exercises.

## 🎯 Objectives
The main objectives of this project are to:

- Install 7-Zip to extract and manage virtual machines
- Install and configure VirtualBox.
- Build a dedicated NAT Network using the `10.0.0.0/24` address range.
- Download and set up Kali Linux.
- Configure Kali Linux with the static IP address `10.0.0.0/24`.
- Test the network configuration to confirm connectivity and DNS resolution.
- Confirm that Kali Linux can access the internet.
- Save a clean snapshot of the virtual machine to make it easier to restore the environment if needed.
- Record the setup steps and configurations for future reference.
- Establish a reliable virtual lab for upcoming cybersecurity experiments and practical exercises.

## 🛠️ Tools and Technologies

| Tool | Purpose |
|---|---|
| VirtualBox | Running virtual machines |
| Kali Linux | Cybersecurity learning environment |
| 7-Zip | Extracting compressed files |
| NAT Network | Virtual network configuration |
| GitHub | Documenting and sharing the project |

## ⚙️ Lab Configuration

| Component | Configuration |
|---|---|
| 🖥️ Host OS | Windows 10 |
| 🧰 Hypervisor | VirtualBox 7.2 |
| ⚡ Processor | Intel Core i7 |
| 🌐 Virtual Network | NAT Network |
| 🐉 Security OS | Kali Linux
| 📡 Network Address | `10.0.0.0/24` |
| 🐧 Kali Linux IP Address | `10.0.0.2/24` |
| 🚪 Default Gateway | `10.0.0.1` |
| 🌍 DNS Server | 8.8.8.8 |
| 📸 VM Snapshot | Required |

## 🏗️ Lab Architecture

The lab consists of:

- **Host machine:** My physical laptop running the host operating system.
- **VirtualBox:** The virtualization software.
- **Kali Linux:** The virtual machine used for cybersecurity practice.
- **NAT Network:** The virtual network connecting the lab to external networks.

Additional virtual machines may be added for future exercises.

## 🪜 Lab Setup Procedure

### Step 1: Install 7-Zip

Download and install 7-Zip if required to extract the Kali Linux virtual machine files.

Download: https://7-zip.org/download.html

### Step 2: Install VirtualBox

Download and install VirtualBox on the host computer.

Download: https://www.virtualbox.org/wiki/Downloads

### Step 3: Create the NAT Network

Create a NAT Network in VirtualBox with the required subnet:

`10.0.0.0/24`

This network will provide the virtual networking environment for the lab.

### Step 4: Set Up Kali Linux

Download Kali Linux from its official website and import the virtual machine into VirtualBox.

Download: https://www.kali.org/get-kali/

Configure the virtual machine's network adapter to use the created NAT Network.


##  Step 5: Configure the IP Address

Configure Kali Linux to use the required IP address:

```text
IP Address: 10.0.0.2
CIDR:       /24
```

Check the network settings, gateway, DNS configuration, and connectivity.


Check the network settings, gateway, DNS configuration, and connectivity.

### Step 6: Configure Shared Features

Enable the required VirtualBox features:

- Shared clipboard
- Drag-and-drop
- Shared folder for the host's `/downloads` folder

Verify that these features work as intended.

### Step 7: Test Connectivity

Use appropriate network commands to verify the configuration.

Check the IP address:

```bash
ip addr
```

Check the routing table:

```bash
ip route
```

Test gateway connectivity:

```bash
ping 10.0.0.1
```

Test internet connectivity:

```bash
ping 8.8.8.8
```

Test domain name resolution:

```bash
nslookup networkwalks.com
```

The results should be recorded after running the commands. If a test fails, investigate the network configuration before marking it successful.

### Step 8: Take a Virtual Machine Snapshot

After the lab has been configured and verified, create a VirtualBox snapshot.

A snapshot provides a recovery point that can be used to return the virtual machine to its saved state.

## 📸 Screenshots

Screenshots documenting the practical work will be stored in the `screenshots` folder.

| Screenshot | Description |
|---|---|
| `virtual-box-installation.png` | VirtualBox installation |
| `kali-linux.png` | Kali Linux virtual machine |
| `nat-network.png` | NAT Network configuration |
| `network-config.png` | Network configuration |
| `ip-configuration.png` | Kali Linux IP address |
| `shared-folder.png` | Shared folder settings |
| `drag-drop.png` | Clipboard and drag-and-drop settings |
| `test.png` | Connectivity testing |

The filenames above are suggested examples. Use the exact names of the screenshots you upload.

## 🔍 Verification Checklist

- [ ] VirtualBox installed.
- [ ] Kali Linux imported and running.
- [ ] NAT Network configured.
- [ ] Required IP address configured.
- [ ] Internet connectivity tested.
- [ ] Shared folder configured.
- [ ] Clipboard and drag-and-drop tested.
- [ ] Virtual machine snapshot created.
- [ ] Screenshots uploaded to GitHub.

## 🧠 What I Aim to Learn

Through this project, I aim to improve my understanding of:

- Virtualization and virtual machines.
- Basic network configuration.
- IPv4 addressing and subnetting.
- NAT Network functionality.
- Kali Linux administration.
- Cybersecurity lab preparation.
- Technical documentation using GitHub.

## 🔐 Ethical Use

This lab is intended for educational purposes and authorized security testing only. Any future security assessments should be conducted on systems I own or have explicit permission to test.

## 📚 References

- VirtualBox: https://www.virtualbox.org/wiki/Downloads
- Kali Linux: https://www.kali.org/get-kali/
- 7-Zip: https://7-zip.org/download.html

---

**Project:** WK1-PM1  
**Module:** Cybersecurity Lab Setup  
**Environment:** VirtualBox and Kali Linux


