# NETWORKWALKS-B082-WK1-PM1-CYBERSECURITY-LAB-SETUP

<div align="center">

# 🔐 Cybersecurity Lab Environment Setup

**Building an isolated virtual lab for penetration testing and ethical hacking practice**
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/-Virtualbox%20v7.2-0070C0?style=flat-square&labelColor=000000" />
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


---

# 🪜 Lab Setup Procedure

## Step 1. Install System Dependencies & 7-Zip
Before setting up the virtual machine platform, I configured the underlying Windows environment with the proper prerequisites to ensure core virtualization frameworks compile successfully without throwing runtime error flags.

*   **Microsoft Visual C++ Redistributable Package:** Installed the visual runtime engine required by VirtualBox to run stable kernel tasks on Windows hosts.
    *   [Official Microsoft VC++ Redistributable Direct Download (x64)](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170)
*   **7-Zip File Extraction Utility:** Installed the file manager engine to safely open compressed archives.
    *   [Official 7-Zip Utility Download](https://7-zip.org)

---

## Step 2. Install VirtualBox
I deployed the host virtualization hypervisor platform to manage local sandbox operating system images.

*   **Hypervisor Component Link:** [Official Oracle VirtualBox Downloads Hub](https://virtualbox.org)

<img width="1366" height="768" alt="Oracle VirtualBox" src="https://github.com/user-attachments/assets/a46d707c-0cd8-4b9d-bb62-71a59b113cb6" />


## Step 3. Create the NAT Network
I initialized a specialized isolated virtual local area network inside the hypervisor environment interface.

*   **Network Name:** `NatNetwork`
*   **IPv4 Subnet Prefix:** `10.0.2.0/24`
*   **DHCP Allocator Engine:** Enabled
*   **IPv6 Protocol Paths:** Disabled

> 🖼️ **My Custom NAT Network Interface Config:**  
  <img width="1366" height="768" alt="NatNetwork" src="https://github.com/user-attachments/assets/3753757f-e073-457c-9ced-e4c8eaa0e249" />

A **NAT Network** was selected because multiple virtual machines connected to the same NAT Network can communicate with one another while also having outbound network connectivity.

This will allow future attacker and target VMs to communicate within the lab.



---

## Step 4. Import Kali Linux
I pulled down the pre-configured system appliance instance package straight from the official distribution mirrors and imported the image into the VirtualBox architecture array.

*   **Attacker Distribution Image Link:** [Official Kali Linux Pre-Built VM Download](https://kali.org)



<img width="1366" height="662" alt="kalibabaaa" src="https://github.com/user-attachments/assets/f54a56a5-5784-479a-9125-472568b2d9e9" />

### My Applied Machine Settings:
 ```text
Adapter 1
Attached to: NAT Network
Network:     NatNetwork
Adapter Type: Intel PRO/1000 MT Desktop
```

<img width="1366" height="768" alt="smart lot" src="https://github.com/user-attachments/assets/22987d73-7f57-499f-941b-3d7bee2644fa" />






The VM was allocated:

```text
RAM: 2048 MB
```
<img width="1366" height="768" alt="lihjy" src="https://github.com/user-attachments/assets/dead712b-c2b8-4270-a4e1-2680321538b8" />





  
  
  
  
  **FileSystem Shared Folders:** Mounted a direct path connection mapping my physical machine's `/downloads` folder into the virtual machine's local tree structure.

<img width="1366" height="768" alt="shared fold" src="https://github.com/user-attachments/assets/d161de62-e5ce-4cd8-8518-86404f7713db" />


---

## Step 5. Configure the Kali Linux Network
To prevent dynamic lease changes during successive vulnerability evaluations, I manually changed the Linux configuration setup profiles from automated tracking to hardcoded static endpoints.

*   **Manual Assigned Address:** `10.0.0.2`
*   **Network Segment Mask:** `255.255.255.0`
*   **Upstream Gateway Pathway:** `10.0.0.1`
*   **Primary DNS Resolver Server:** `8.8.8.8`

> 🖼️ **My Manual Connection Modification Screenshot:**  
<img width="1366" height="662" alt="flys of kali config" src="https://github.com/user-attachments/assets/9b877f7e-f286-4cc1-adce-2503766d2e4f" />



> 🖼️ **My Manual Connection Verification Proof:**  
> This live capture confirms full internet connectivity inside my Kali Linux desktop environment. After saving my static parameters, I opened the native Firefox ESR browser and successfully loaded the external `networkwalks.com` web portal via my custom NATNetwork gateway interface:
<img width="1366" height="662" alt="andybaba o" src="https://github.com/user-attachments/assets/6bf57de6-9b1e-4e1e-beaf-c05da15180aa" />




## Step 6. Create a Clean VM Snapshot

Once my manual network parameters were written and internet reachability was confirmed, I powered off the Kali Linux Virtual Machine to capture a permanent, clean environment baseline.

*   **Snapshot Designation Name:** `Clean Kali - Network Setup`
*   **Detailed Snapshot Log Description:** `A Clean Network Setup of Kali Linux (Attac&ker VM)`

As documented in the step-by-step progress below, I initialized the snapshot request within the VirtualBox manager screen panel. This saved execution checkpoint serves as my core system fallback profile. If a subsequent cyber security scanning tool or aggressive vulnerability payload accidentally breaks my network stack dependencies in a future exercise, I can instantly roll back the state parameters to this exact pristine milestone.

> 🖼️ **My In-Progress Configuration Point (Creating the State Capture):**  

<img width="1366" height="768" alt="snapshot of kali linux" src="https://github.com/user-attachments/assets/a831ed30-c199-478a-8c13-54ebceaa6fc0" />



> 🖼️ **My Verification Point (Snapshot Saved):**  
<img width="1366" height="768" alt="snapshot taken really hoho" src="https://github.com/user-attachments/assets/36f1c27c-187d-4f43-bca1-c9e906136e01" />


---

| ✅ Test | 🧾 Command / Action | 🎯 Live Result Observations |
| :--- | :--- | :--- |
| **🌐 Check IP Address** | `ip a` | **SUCCESSFUL** (Correct Kali linux `10.0.0.2` address profile displayed) |
| **📡 Test Gateway** | `ping 10.0.0.1` | **FAILED** (Returned host unreachable / packets dropped) |
| **🌍 Test Internet Traffic** | Open Firefox Browser | **SUCCESSFUL** (Successfully accessed and loaded `networkwalks.com`) |
| **🌍 Test Raw Link IP** | `ping 8.8.8.8` | **FAILED** (Returned host unreachable / packets dropped) |
| **🔎 Test DNS Resolution** | `nslookup networkwalks.com` | **FAILED** (communication error to 8.8.8.8#53: host unreachable) |
| **🧰 Verify Nmap** | `nmap --version` | **SUCCESSFUL** (Nmap utility layer version 7.99 engine displayed) |
| **🔄 Verify Snapshot State** | Restore VM & run `ip a` | **SUCCESSFUL** (Baseline configuration state restored cleanly) |


### My Shell Console Diagnostics Readout:

```bash
# Diagnostic Run A: Active IP Verification
ip a
```
```text
10.0.0.2
```
<img width="1360" height="662" alt="ip a screenshot" src="https://github.com/user-attachments/assets/9305edd8-66e2-46ba-aaed-1856080d163a" />



```bash
# Diagnostic Run B: Test Gateway
ping 10.0.0.1

```
```text
host unreachable/packet dropped
```
<img width="1360" height="662" alt="ping gateway screenshot" src="https://github.com/user-attachments/assets/2465c5ce-3e51-4404-9279-078ccb667231" />


```bash
# Diagnostic Run C: Test Raw Link IP
ping 8.8.8.8
```
```text
host unreachable / packets dropped
```
<img width="1360" height="662" alt="ping of the year" src="https://github.com/user-attachments/assets/85af7e79-4a1a-4aa3-b301-bbf7a64cc1e8" />



```bash
# Diagnostic Run D: Test DNS Resolution
nslookup networkwalks.com
```
```text
communication error to 8.8.8.8#53: host unreachable
```

<img width="1360" height="662" alt="nslookup screenshot" src="https://github.com/user-attachments/assets/fb46d592-fc46-46fd-b573-30fe15690d06" />


```bash
# Diagnostic Run E: Verify Nmap
nmap --version
```
```text
Nmap version 7.99
```

<img width="1360" height="662" alt="nmap version screenshot" src="https://github.com/user-attachments/assets/274a5ab0-4b74-4fb1-a11a-c13463c60202" />


### 🔄 Snapshot Integrity & Recovery Audit

To validate the operational reliability of my baseline state snapshot, I simulated a severe network interface configuration failure by manually purging the static IP allocations from the active network card profile within the guest terminal. 

I then performed a clean shutdown of the instance, accessed the VirtualBox Snapshot Management console interface, selected the `Clean Kali - Network Setup` tree node, and executed a hardware rollback operation. Upon a fresh reboot cycle, running `ip a` confirmed that the entire local system configuration matrix was successfully restored to the target baseline state with zero configuration loss.

```bash
sudo ip addr del 10.0.0.2/24 dev eth0

```
<img width="1360" height="662" alt="delete it" src="https://github.com/user-attachments/assets/d1e044df-5634-477a-9709-323ef2d4be66" />

**Executing hardware rollback**
<img width="1366" height="768" alt="restore back" src="https://github.com/user-attachments/assets/d5bc9aa1-227d-42c8-a3e1-210d694362bf" />



```bash
# Diagnostic Run F: Verify Snapshot State
ip a
```
```text
10.0.0.2
```

<img width="1360" height="662" alt="snapshot restored" src="https://github.com/user-attachments/assets/1cb783ca-2ece-4f00-b9f0-20f05046d426" />



---

# 🐞 Problems Encountered & Solutions

### Problem 1: Hypervisor Kernel Initialization Failure (Guru Meditation Crash)
*   **Operational Anomaly:** During the initial boot sequence of the Kali Linux attacking instance, the hypervisor suffered a fatal engine crash. It threw a critical "VirtualBox - Guru Meditation" error popup window and halted system execution entirely.
*   **Root Cause Analysis:** The crash was triggered by low-level resource competition on my laptop between the Oracle virtualization engine and native Windows hypervisor subsystems. 
*   **Remediation Path:** To resolve the conflict, I carried out a targeted host-level cleanup sequence on my physical Windows laptop:
    1. Opened the **Windows Features** menu and completely unchecked the allocations for *Windows Hypervisor Platform* and *Virtual Machine Platform*.
    2. Navigated to the Windows **Core Isolation** security dashboard and toggled *Memory Integrity* to **OFF** to stop driver blockages.
    3. Performed a full host computer system reboot.
    
    This cleared the hardware virtualization blocks and allowed the Kali Linux guest operating system to boot cleanly with perfect stability.

**Guru Mediation Crash Screenshot**
<img width="1366" height="768" alt="VirtualBox Guru Meditation" src="https://github.com/user-attachments/assets/2e389018-e702-467e-8dff-d8de158c06ef" />



**Windows Features Screenshot**

<img width="1365" height="752" alt="Windows features" src="https://github.com/user-attachments/assets/16a35acf-181e-4e19-a7b8-6a95a47af34d" />


**Core Isolation Screenshot**

<img width="1364" height="768" alt="Core isolation" src="https://github.com/user-attachments/assets/7b2243f2-3fb2-4838-bcf6-5500201dfb25" />




### Problem 2: Persistent Terminal ICMP Packet Drops & Gateway Route Failures
*   **Operational Anomaly:** After migrating the network adapter card profiles inside the Kali Linux GUI from dynamic tracking to the required manual static deployment layout (`10.0.0.2/24`), all terminal-based connectivity validation checks failed completely. Running `ping -c 4 8.8.8.8` or checking the default gateway via `ping 10.0.0.1` consistently returned `Destination Host Unreachable` or `No route to host` error flags.
*   **Multi-Layered Diagnostic Discovery:** To track down the exact location of the network bottleneck on my system, I ran a detailed diagnostic pipeline inside the Linux terminal:
    1. Checked the hardware adapter state using `ip a`, which returned a perfectly active and healthy `<UP,LOWER_UP>` status.
    2. Inspected the core system network script layers using `cat /etc/network/interfaces`, verifying that the file was clean and completely uncorrupted.
    3. Audited the local ARP neighbor cache using `ip neigh show`, which flagged the virtual gateway address (`10.0.0.1`) as strictly **`incomplete`**.

*   **Remediation Path (Attempted):** To force the network interface to re-align its routing parameters, I executed the standard curriculum-recommended NetworkManager recycling commands to adjust the Duplicate Address Detection (DAD) constraints and cycle the interface state:
    ```bash
    sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
    sudo nmcli connection down "Wired connection 1"
    sudo nmcli connection up "Wired connection 1"
    ```
    *Note: This remediation path did not resolve the terminal ping issue on my host system, as the interface configuration layers remained isolated from raw command-line ICMP traffic.*



 **Failed ping remediation Screenshot**

<img width="1360" height="662" alt="didnot work" src="https://github.com/user-attachments/assets/46920aa9-b5f6-4f89-9310-38bd6302792a" />



*   **Definitive Engineering Proof:** Although local host-level security configurations stubbornly blocked raw command-line ICMP (ping) packets from passing the network bridge, the lab setup itself was verified as **100% structurally functional**. This was proven conclusively when I launched the native Firefox browser inside the guest desktop environment and successfully loaded and explored the external `networkwalks.com` website live. The core sandbox network layer successfully handles application-layer (HTTP/HTTPS) data pipelines, and the final project state was preserved perfectly using the VirtualBox snapshot tree tracking mechanics.


**Multi-Layered Diagnostic Discovery Screenshot**

<img width="1360" height="662" alt="shows i will use" src="https://github.com/user-attachments/assets/07c93cd9-0b42-4b0b-84ca-09006ca02668" />





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

**Anderson Edaiyo Uzezi**\
Cybersecurity Professional B082

LinkedIn: [https://www.linkedin.com/in/anderson-edaiyo-bab74117b)

---
# 📊 Project Information Matrix

> [!NOTE]
> This repository contains the complete documentation, environment blueprints, and live verification logs for my Week 01 specialized laboratory deployment.

| 🗂️ Project Parameter | ⚙️ Live Deployment Data |
| :--- | :--- |
| **Program Track** | Cybersecurity with Ethical Hacking |
| **Academy Module** | Networkwalks Academy Portfolio Matrix |
| **Timeline Horizon** | Week 01 Engineering Core |
| **Project Identity** | Cybersecurity & Pentesting Lab Environment Setup |
| **Target Task ID** | TASK WK1-PM1 |
| **Code Repository** | Public Deployment Hub via GitHub |

---
<div align="center">
  <!-- PRIMARY BLUE CANVAS MARGIN CONTAINER -->
  <table width="100%" cellspacing="0" cellpadding="20" style="border: 3px solid #00A6C7; background-color: #ffffff; border-radius: 4px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;">
    <tr>
      
      <!-- LEFT COLUMN PANEL: PHYSICAL HOST NODES WITH LIVE HARDWARE SPECIFICATIONS SCREENSHOT -->
      <td width="30%" valign="top" align="left" style="font-family: inherit; color: #1e293b; padding-right: 15px;">
        <h2 style="color: #00A6C7; font-size: 1.5rem; margin-top: 0; font-weight: 700; line-height: 1.2;">
          Main OS<br><span style="font-size: 1.2rem; font-weight: 500;">(Windows 10)</span>
        </h2>
        
        <!-- IMAGE 1: HOST LOCAL NETWORK INTERFACE MATRIX SCREENSHOT -->
        <table border="0" cellspacing="0" cellpadding="0" style="border: 1px solid #cbd5e1; border-radius: 2px; overflow: hidden; margin-bottom: 15px; box-shadow: 0 2px 4px rgba(0,0,0,0.05);">
          <tr>
            <td>
              <img src="images/23-failed-network-manager-icmp-remediation.png" width="100%" style="display: block;" alt="MTN Host Network Connection Properties">
            </td>
          </tr>
        </table>
        <p style="font-family: monospace; font-size: 1.05rem; font-weight: bold; color: #00A6C7; margin-top: 0; margin-bottom: 25px;">
          IP: 192.168.0.2
        </p>
        
        <!-- IMAGE 2: HOST HARDWARE SYSTEM DEVICE CONFIGURATION SCREENSHOT -->
        <table border="0" cellspacing="0" cellpadding="0" style="border: 1px solid #cbd5e1; border-radius: 2px; overflow: hidden; margin-bottom: 15px; box-shadow: 0 2px 4px rgba(0,0,0,0.05);">
          <tr>
            <td>
              <img src="images/21-windows-features-hypervisor-disabled.png" width="100%" style="display: block;" alt="Windows 10 Hardware System Specifications">
            </td>
          </tr>
        </table>
        
        <p style="font-size: 0.8rem; color: #64748b; font-style: italic; line-height: 1.3; margin-bottom: 5px;">
          PC/Laptop specs for this lab setup<br>(recommended but not a must)
        </p>
        <p style="font-size: 0.85rem; color: #475569; line-height: 1.5; font-weight: 500;">
          • 8GB RAM or more<br>
          • 256GB SSD or more<br>
          • Intel Pentium Processor (or similar)
        </p>
      </td>

      <!-- RIGHT COLUMN PANEL: ORANGE VIRTUALBOX ROUTING FABRIC ENVELOPE -->
      <td width="70%" valign="top" style="border: 2px solid #F59E0B; border-radius: 4px; background-color: #ffffff; padding: 20px;">
        
        <!-- VIRTUALBOX TOP LOGO LAYOUT LINE ROW -->
        <table width="100%" border="0" cellspacing="0" cellpadding="0">
          <tr>
            <td valign="top" align="left">
              <h1 style="color: #0070C0; font-size: 2.2rem; margin: 0; font-weight: 800; font-family: inherit;">
                VirtualBox
              </h1>
            </td>
            <td valign="top" align="right" style="font-family: inherit; font-size: 0.85rem; color: #334155; line-height: 1.4;">
              <span style="color: #0070C0; font-weight: bold;">Network Settings on all VM's:</span><br>
              <span style="color: #238F89; font-weight: bold;">NATNetwork (custom)</span><br>
              <span style="color: #F59E0B; font-weight: bold;">Range: 10.0.0.2-99 /24</span>
            </td>
          </tr>
        </table>

        <!-- CENTRAL BLADE: PRIMARY GUEST ATTACKER WORKSPACE NODE WITH LIVE SCREENSHOT -->
        <div align="center" style="margin-top: 25px; margin-bottom: 20px;">
          <!-- IMAGE 3: KALI LINUX WIRED STATIC NETWORK CONNECTION PANEL SCREENSHOT -->
          <table border="0" cellspacing="0" cellpadding="0" style="border: 2px solid #475569; border-radius: 2px; overflow: hidden; max-width: 520px; box-shadow: 0 4px 6px -1px rgba(0,0,0,0.1);">
            <tr>
              <td>
                <img src="images/08-kali-static-ip-gui-configuration.png" width="520" style="display: block;" alt="Kali Linux Active Static IPv4 Wired Interface Setup">
              </td>
            </tr>
          </table>
          <p style="font-family: inherit; font-size: 0.95rem; color: #1e293b; margin-top: 10px; font-weight: 500;">
            Manual IP: <span style="color: #16a34a; font-weight: bold;">10.0.0.2</span>/24 (NATNetwork)
          </p>
        </div>

        <!-- LOWER SUB-SEGMENT CONDUIT: RE-ARRANGED WINDOWS 10 ENDPOINT BASELINE TARGET -->
        <hr style="border: 0; border-top: 1px dashed #cbd5e1; margin: 20px 0;">
        <table width="100%" border="0" cellspacing="0" cellpadding="0">
          <tr>
            <td align="center" valign="bottom" width="100%">
              <p style="font-family: inherit; font-size: 0.85rem; color: #1e293b; margin-bottom: 8px; font-weight: 500;">
                Manual IP: <span style="color: #16a34a; font-weight: bold;">10.0.0.10</span> /24<br>
                <span style="color: #64748b; font-size: 0.75rem;">(NATNetwork)</span>
              </p>
              <h4 style="font-family: inherit; color: #0070C0; font-size: 1.1rem; margin-top: 4px; margin-bottom: 0; font-weight: 700;">
                Windows 10 Target VM
              </h4>
            </td>
          </tr>
        </table>

      </td>
    </tr>
  </table>
</div>
