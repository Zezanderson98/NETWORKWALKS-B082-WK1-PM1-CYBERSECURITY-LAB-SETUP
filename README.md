# NETWORKWALKS-B082-WK1-PM1-CYBERSECURITY-LAB-SETUP

<div align="center">

# 🔐 Cybersecurity Lab Environment Setup

**Building an isolated virtual lab for penetration testing and ethical hacking practice**
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ver-Virtualbox%20v7.2-0070C0?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Kali%20Linux-v2026.2-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Linux-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Network-10.0.0.0%2F24-238F89?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Penetration%20Testing-C00000?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Virtualization-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/GitHub-404040?style=flat-square&labelColor=0070C0&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Kali%20Linux-404040?style=flat-square&labelColor=C00000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/NetworkWalks-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ethical%20Hacking-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Anderson%20Edaiyo%20-C00000?style=flat-square" />
</p>

---

## 📌 Project Overview

This project focuses on setting up a **virtual cybersecurity and penetration-testing laboratory** using VirtualBox and Kali Linux.

The purpose of the lab is to create a controlled environment where cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly.

The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.

---


## 🎯 Objectives

The main objectives of this project are to:

- Install and configure VirtualBox.
- Install/import Kali Linux as a virtual machine.
- Create a private **NAT Network** for the cybersecurity lab.
- Configure network connectivity for Kali Linux.
- Assign a consistent IP address to the Kali VM.
- Verify network connectivity and DNS resolution.
- Take a clean VM snapshot for recovery.
- Document the complete setup process.
- Prepare the environment for future cybersecurity projects.

---

## 🛡️ Purpose of the Lab

The lab provides an isolated and controlled environment for cybersecurity learning and authorized security testing.

It can be used for activities such as:

- Network reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Web security testing
- Exploitation practice
- Security-tool experimentation

⚠️ **Important:** This laboratory must only be used for systems that you own or have explicit permission to test. Do not use the lab or its tools to attack unauthorized systems.

---

## 🏗️ Lab Architecture

![](1-screenshot-title-image.png)


Additional target machines can be added to the same virtual network in future projects.

---

## ⚙️ Lab Configuration

| 🧩 Component       | ⚙️ Configuration   |
| ------------------ | ------------------  |
| 🖥️ Host OS         | Windows 10 Pro         |
| 🧠 Host RAM        | 8 GB               |
| ⚡ Processor       | Intel(R) Pentium(R)      |
| 🧰 Hypervisor      | VirtualBox 7.2  |
| 🐉 Security OS     | Kali Linux 2026.2  |
| 🧠 Kali RAM        | 2048 MB            |
| 🌐 Virtual Network | NAT Network        |
| 📡 Network Address | 10.0.0.0/24        |
| 🐧 Kali IP Address | 10.0.0.2/24        |
| 🚪 Default Gateway | 10.0.0.1           |
| 🌍 DNS Server      | 8.8.8.8            |
| 🔮 Future VM Range | 10.0.0.3–10.0.0.99 |

---

# 🔐 Cybersecurity Lab Environment Setup
**Course Tag:** TASK WK1-PM1  
**Academy Module:** Networkwalks Academy Portfolio  
**Developer:** <!-- Type your full name here -->  
**Intern Identifier:** <!-- Type your student ID here -->  

---

## 📌 Project Overview

This project focuses on setting up a **virtual cybersecurity and penetration-testing laboratory** using VirtualBox and Kali Linux.

The purpose of the lab is to create a controlled environment where cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly.

The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.

---

## 🎯 Objectives

The main objectives of this project are to:
- Install required system dependencies and hypervisor layers.
- Create a private **NAT Network** for the cybersecurity lab.
- Install and configure a Kali Linux virtual machine.
- Set up a consistent, manual IP address configuration.
- Verify end-to-end network connectivity and internet reachability.
- Capture a baseline system state snapshot for recovery.

---

## 🏗️ Lab Architecture

📸 **My Architecture Blueprint:**  
<!-- Insert your personal screen capture of the network diagram layout here. Keep your file path clean, e.g., ![](images/my_network_diagram.png) -->

---

## ⚙️ Lab Configuration

*   **Host Operating System:** <!-- Type your host OS version here, e.g., Windows 11 Pro -->
*   **Host System Memory:** <!-- Type your actual host RAM here, e.g., 16 GB DDR4 -->
*   **Processor Engine:** <!-- Type your CPU model here, e.g., Intel Core i7-12700H -->
*   **Hypervisor Engine:** VirtualBox 7.x
*   **Security Distribution OS:** Kali Linux (Pre-built VM Instance)
*   **Virtual Machine Memory:** <!-- Type the RAM capacity assigned to your VM, e.g., 2048 MB -->
*   **Virtual Network Array:** NAT Network (`NatNetwork`)
*   **Subnet CIDR Range:** `10.0.0.0/24`
*   **Static Endpoint Assignment:** `10.0.0.2/24`
*   **Default System Gateway:** `10.0.0.1`
*   **Target DNS Nameserver:** `8.8.8.8`

---

# 🪜 Lab Setup Procedure

## Step 1. Install System Dependencies & 7-Zip
Before setting up the virtual machine platform, I configured the underlying Windows environment with the proper prerequisites to ensure core virtualization frameworks compile successfully without throwing runtime error flags.

*   **Microsoft Visual C++ Redistributable Package:** Installed the visual runtime engine required by VirtualBox to run stable kernel tasks on Windows hosts.
    *   [Official Microsoft VC++ Redistributable Direct Download (x64)](https://aka.ms)
*   **7-Zip File Extraction Utility:** Installed the file manager engine to safely open compressed archives.
    *   [Official 7-Zip Utility Download](https://7-zip.org)

---

## Step 2. Install VirtualBox
I deployed the host virtualization hypervisor platform to manage local sandbox operating system images.

*   **Hypervisor Component Link:** [Official Oracle VirtualBox Downloads Hub](https://virtualbox.org)

---

## Step 3. Create the NAT Network
I initialized a specialized isolated virtual local area network inside the hypervisor environment interface.

*   **Network Name:** `NatNetwork`
*   **IPv4 Subnet Prefix:** `10.0.0.0/24`
*   **DHCP Allocator Engine:** Enabled
*   **IPv6 Protocol Paths:** Disabled

> 🖼️ **My Custom NAT Network Interface Config:**  
> <!-- Place your VirtualBox NATNetwork preferences screenshot here. Keep your file path clean, e.g., ![](images/my_network_setup.png) -->

This specific network architecture was chosen to ensure multiple security boxes launched later can smoothly map inter-guest connectivity strings while sharing a secure outbound gateway bridge to the internet.

---

## Step 4. Import Kali Linux
I pulled down the pre-configured system appliance instance package straight from the official distribution mirrors and imported the image into the VirtualBox architecture array.

*   **Attacker Distribution Image Link:** [Official Kali Linux Pre-Built VM Download](https://kali.org)

### My Applied Machine Settings:
*   **Network Mapping:** Attached to `NAT Network` using the newly defined `NatNetwork` block.
*   **Adapter Profile:** `Intel PRO/1000 MT Desktop`
*   **Guest Additions:** Configured **Bidirectional** setting flags for clipboard data sharing paths and drag-and-drop operations.
*   **FileSystem Shared Folders:** Mounted a direct path connection mapping my physical machine's `/downloads` folder into the virtual machine's local tree structure.

> 🖼️ **My VM Settings Dashboard:**  
> <!-- Place a screenshot of your specific VM Settings panels here, showing Advanced Clipboard features and network attachments. -->

---

## Step 5. Configure the Kali Linux Network
To prevent dynamic lease changes during successive vulnerability evaluations, I manually changed the Linux configuration setup profiles from automated tracking to hardcoded static endpoints.

*   **Manual Assigned Address:** `10.0.0.2`
*   **Network Segment Mask:** `255.255.255.0`
*   **Upstream Gateway Pathway:** `10.0.0.1`
*   **Primary DNS Resolver Server:** `8.8.8.8`

> 🖼️ **My Manual Connection Modification Screenshot:**  
> <!-- Place a screenshot here showing YOUR manual network connection modifications layout open inside Kali Linux. -->

---

## Step 6. Create a Clean VM Snapshot
Once the network installation framework verified successfully, I immediately generated a pristine environment state snapshot capture point.

*   **My Saved Milestone Label Name:** <!-- Type what you actually named your snapshot, e.g., Clean Kali - Network Setup -->

This snapshot functions as the stable baseline configuration marker for my security testing lab environment, ensuring I can restore the system parameters instantly if any future tasks damage system dependencies.

---

# 🔎 Lab Verification

| ✅ Test                        | 🧾 Command                      | 🎯 Expected Result              |
| ----------------------------- | ------------------------------- | ------------------------------- |
| 🌐 Check IP address           | `ip a`                          | Correct Kali IP displayed       |
| 📡 Test gateway               | `ping 10.0.0.1`                 | Successful replies              |
| 🌍 Test Internet connectivity | `ping 8.8.8.8`                  | Successful replies              |
| 🔎 Test DNS resolution        | `nslookup networkwalks.com`     | Domain resolves                 |
| 🧰 Verify Nmap                | `nmap --version`                | Nmap version displayed          |
| 🔄 Verify snapshot            | Restore snapshot and run `ip a` | Baseline configuration restored |

### My Shell Console Diagnostics Readout:
<!-- 
👉 INSTRUCTION: 
Run these commands in your live terminal, copy the actual text output from your screen, and paste it inside the code blocks below.
-->

```bash
# Diagnostic Run A: Active IP Verification
ip address show eth0
```
```text
<!-- PASTE THE EXACT, REAL TEXT OUTPUT FROM YOUR OWN KALI TERMINAL HERE -->
```

```bash
# Diagnostic Run B: Outbound Data Bridge Audit
ping -c 4 8.8.8.8
ping -c 4 google.com
```
```text
<!-- PASTE THE REAL PING PRINTOUT FROM YOUR SCREEN HERE SHOWING 0% PACKET LOSS -->
```

> 🖼️ **My Verified Diagnostic Terminal Snapshot:**  
> <!-- Place a screenshot of your live terminal window displaying these successful commands here. -->

---

# 🐞 Problems Encountered & Solutions

<!-- 
👉 INSTRUCTION:
Write 2-3 short sentences about what actually went wrong during your day. Did your internet disconnect? Did you get a BIOS error? Did you misspell a network name? Write it completely in your own words.
-->

### Technical Anomaly Encountered:
<!-- Describe your problem here. Example: "When I saved my manual settings, my upper taskbar internet icon completely disappeared and I couldn't reach any website." -->

### Resolution Process Executed:
<!-- Explain how you solved it. -->
```bash
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
sudo nmcli connection down "Wired connection 1"
sudo nmcli connection up "Wired connection 1"
```

---



---

# 💡 What I Learned

Through this project, I learned how to create and configure a virtual environment for cybersecurity practice.

The most important concepts I learned include:

### 1. NAT vs NAT Network

A standard NAT configuration and a NAT Network serve different purposes.

A NAT Network allows multiple VMs connected to the same virtual network to communicate with one another while providing network address translation for external connectivity.

This makes it useful for building a multi-machine cybersecurity laboratory.

### 2. Virtual Machine Networking

I learned how VirtualBox virtual network adapters connect virtual machines to different types of networks and how network configuration affects communication between machines.

### 3. Static IP Configuration

I learned how to configure and verify IPv4 addressing, subnet masks, gateways, and DNS settings in Kali Linux.

### 4. VM Snapshots

I learned that a clean snapshot should be created **before performing risky or experimental activities**.

This provides a known-good recovery point for future cybersecurity exercises.

### 5. Documentation

I learned that documenting commands, configuration, screenshots, problems, and solutions is an important part of a professional cybersecurity project.

---

# 🔐 Security & Ethical Use

This laboratory is intended strictly for education purposes only.

---

# 🔗 Tools & Resources

- **7-Zip:** [https://7-zip.org/download.html](https://7-zip.org/download.html)
- **VirtualBox:** [https://virtualbox.org/wiki/Downloads](https://virtualbox.org/wiki/Downloads)
- **Kali Linux:** [https://kali.org/get-kali](https://kali.org/get-kali)

---

# 👤 Author

**Anderson Edaiyo**\
Cybersecurity Professional B082

LinkedIn: [https://www.linkedin.com/in/anderson-edaiyo-bab74117b)

---

## 📌 Project Information

**Program Name:** Cybersecurity at Networkwalks | **Week:** 01 | **Project:** Cybersecurity & Pentesting Lab Setup | **Repository:** GitHub

# 📂 Engineering Journal: Custom Security Sandbox Deployment
**Project Reference:** TASK WK1-PM1  
**Curriculum Stream:** Networkwalks Portfolio Matrix  
**Systems Engineer:** <!-- Input your full name here -->  
**Intern Identifier:** <!-- Input your student token here -->  

---

## 📝 1. Individual Environmental Scope

The objective of this engineering task was to initialize an out-of-band virtual workspace dedicated to secure software security validation. By separating guest host networking components away from my main physical desktop setup, I can safely run local network diagnostic routines while ensuring the guest terminal retains outbound internet transit routing capabilities.

---

## ⚙️ 2. Physical Host Resource Inventory

Prior to downloading software packages or configuring virtual adapters, I audited my local computer to confirm it possessed adequate hardware capability to handle multi-instance virtualization without dropping connection tables:

*   **Processor Engine:** <!-- Type your specific CPU model here, e.g., Intel Core i5-11400H -->
*   **Volatile Memory Available:** <!-- Type your host RAM size here, e.g., 16 GB DDR4 -->
*   **Solid State Storage Space:** <!-- Type your drive capacity here, e.g., 1TB NVMe M.2 SSD -->
*   **Host Environment OS:** <!-- Type your base operating system version here, e.g., Windows 11 Home -->

---

## 🏗️ 3. Environment Architecture Layout

To establish a clear structural design of my localized testing environment before carrying out the configuration tasks, I referenced and tracked the baseline operational blueprint layout below:

📸 **My Screen Evidence (Topology Diagram):**  
<!-- Insert your personal screen capture of the network diagram layout here. Keep your file path clean, e.g., ![](images/my_network_diagram.png) -->

---

## 📦 4. Software Source & System Prerequisites

To ensure proper deployment validation and avoid installation failure flags due to missing dynamic link libraries (.dll), I verified and installed all baseline system runtimes before initializing the hypervisor engine.

### Prerequisites & Dependencies
*   **Data Extraction Utility:** Deployed the open-source 7-Zip archiver engine to manage `.7z` virtual hardware images.
    *   [Official 7-Zip Download Engine](https://7-zip.org)
*   **Windows Subsystem Runtime Dependency:** Installed the **Microsoft Visual C++ 2019/2022 Redistributable Package (x64)**. This runtime environment is strictly required by VirtualBox 7.x to execute system virtualization hooks on a Windows host OS.
    *   [Official Microsoft VC++ Redistributable Direct Link](https://aka.ms)

### Primary Virtualization Platforms
*   **Hypervisor Kernel:** Selected Oracle VirtualBox 7.x as the core bare-metal type-2 management platform.
    *   [Official Oracle VirtualBox Downloads Hub](https://virtualbox.org)
*   **Offensive Guest Workspace:** Sourced the pre-packaged VirtualBox Open Virtualization Archive (`.ova`) image directly from the official Kali repository.
    *   [Official Kali Linux VM Images Hub](https://kali.org)

---

## 🌐 5. Custom Segment Configuration (NATNetwork)

Instead of utilizing standard bridging nodes, I built a dedicated network virtualization layer to safely keep all lab traffic internal to this specific network card segment.

> ### Subnet Configurations Applied:
> - **Virtual Network Label:** `NatNetwork`
> - **Subnet Range:** `10.0.0.0/24`
> - **Local IP Distribution (DHCP):** Enabled
> - **IPv6 Global Unicast Paths:** Disabled

📸 **My Screen Evidence (NAT Prefs Panel):**  
<!-- Insert your personal snapshot of the VirtualBox network preferences dashboard here. Example: ![](images/my_network_properties.png) -->

---

## 🐉 6. Attack Terminal Provisioning (Kali Linux)

I deployed the official Kali Linux virtual image onto the designated segment and modified the virtual hardware containers to permit direct data sharing workflows.

*   **System RAM Provisioned:** <!-- Type the RAM capacity assigned to your VM, e.g., 2048 MB -->
*   **Network Mapping Profile:** Attached to: `NAT Network` | Name: `NatNetwork` | Adapter: `Intel PRO/1000 MT Desktop`
*   **Runtime File Shares:** Enabled bidirectional system clipboard tracking alongside shared filesystem directory bindings pointing to my local host machine's `/downloads` partition directory.

📸 **My Screen Evidence (VM Advanced Settings):**  
<!-- Insert a screenshot showing your unique Kali Linux VirtualBox configuration profile here. -->

---

## 🎛️ 7. Static Network Hardcoding

To maintain structural consistency for subsequent tracking and mapping tasks, I manually locked down the interface adapters inside the virtual environment rather than leaving them dynamic:

```text
Target Node Address:  10.0.0.2
Subnet Segment Mask:  255.255.255.0 (/24)
Local Network Gateway: 10.0.0.1
Primary DNS Resolver: 8.8.8.8
```

📸 **My Screen Evidence (Manual IPv4 Panel):**  
<!-- Insert a screenshot here showing YOUR manual network connection modifications layout open inside Kali Linux. -->

---

## 🔬 8. Verification and Local Interface Checks

To prove the manual configuration updates were written correctly to the network controller, I initiated a series of diagnostic terminal commands inside the Linux environment.

<!-- 
👉 INSTRUCTION FOR MAXIMUM portfolio AUTHENTICITY: 
Open your live terminal, execute these routines, and copy/paste your actual textual output inside the boxes below!
-->

### Network Interface Readout:
```bash
ip address show eth0
```
```text
<!-- PASTE THE EXACT LIVE READOUT FROM YOUR OWN KALI LINUX TERMINAL SCREEN HERE -->
```

### End-to-End Route Validation:
```bash
ping -c 4 8.8.8.8
ping -c 4 google.com
```
```text
<!-- PASTE THE RAW ICMP RESULTS FROM YOUR SCREEN HERE TO SHOW ZERO PACKET LOSS -->
```

📸 **My Screen Evidence (Terminal Run):**  
<!-- Insert a screenshot of your active terminal window capturing the successful ping readouts here. -->

---

## 🩹 9. Logged Operational Obstacles & Fixes

<!-- 
👉 REMINDER:
State the real, organic typos or errors you hit today in your own words.
-->

### Real-World Bug Encountered:
<!-- Describe your personal issue here. Example: "Upon updating the interface settings to manual mode, my terminal dropped all outward connections and couldn't resolve external web paths." -->

### Resolution Process Implemented:
<!-- Explain how you manually brought it back up. Example: "I entered the terminal interface and appended the recommended NetworkManager modification arguments to clear the DAD threshold timeout block, cycled the connection parameters, and restored operational continuity." -->

```bash
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
sudo nmcli connection down "Wired connection 1"
sudo nmcli connection up "Wired connection 1"
```

---

## 💾 10. Safe State Recovery (Baseline Snapshots)

To establish a clear recovery path prior to executing potential vulnerability assessments down the road, I finalized a full system point snapshot inside the hypervisor architecture dashboard.

*   **My Custom Snapshot Identifier Tag:** <!-- Type what you personally named the system snapshot point, e.g., Wk1_Fresh_Deployment -->

📸 **My Screen Evidence (Hypervisor Snapshot Manager):**  
<!-- Insert a snapshot of your VirtualBox snapshot workspace layout highlighting your saved milestone tree. -->

---

## ⚖️ 11. Repository Licensing

This deployment documentation and project log tracking are distributed openly under the terms of the MIT License framework. Check the root level `LICENSE` document file for details.


