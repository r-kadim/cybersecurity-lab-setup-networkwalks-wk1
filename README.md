# NETWORKWALKS-RKADIM-B084-WK1-PM1-CYBERSECURITY-LAB-SETUP

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ver-Virtualbox%20v7.2.22-0070C0?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Kali%20Linux-v2026.3-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Linux-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Penetration%20Testing-C00000?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub-404040?style=flat-square&labelColor=0070C0&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Ethical%20Hacking-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
</p>

##
This is my first project on GitHub setting up a Cybersecurity Lab environment using Virtualbox with Kalilinux.
##
The purpose of this lab is basically to setup a cyber security lab environment using the system you currently have to practice and experiment with cybersecurity principles using Virtualbox.

##  Lab Configuration
*   **Host OS:** Windows 10 Home
*   **Host RAM:**  16.0 GB (15.8 GB usable)
*   **Processor:** Intel Core i7-11800H @ 2.3 GHz
*   **Graphics:** NVIDIA RTX 3060 Laptop GPU (6 GB), Intel(R) UHD Graphpics (128 MB)
*   **Storage:** Micron 3400 477 GB NVMe M.2 SSD, Western Digital WD10SPX 932 GB HDD
*   **Hypervisor:**  VirtualBox 7.2.22
*   **Security OS:**  Kali Linux 2026.3
*   **Kali RAM:** 2048 MB
*   **Virtual Network** NAT Network
*   **Network Address:**  10.0.0.0/24
*   **Kali IP Address:**  10.0.0.2/24
*   **DNS Server:**  10.0.0.1

### Step 1 . Download and Install 7-Zip or similar.
7-Zip is installed to extract the Kali Linux virtual machine package for VirtualBox, which typically is distributed as a `.7z` compressed file.

**Tool:** 7-Zip, WinRar

### Step 2 . Download and Install VirtualBox.
VirtualBox was installed as the virtual machine environment to run the Kali Linux operating system.

**Tool:** VirtualBox 7.2.22

### Step 3. Create NAT Network in VirtualBox using the IP Address 10.0.0.0/24.


#### Configuration

| Network Name      | NAT Network  |
| ------------------| -------------|
| IPv4 Prefix       | 10.0.0.0/24  |
| DHCP              | Enabled      |
| IPv6              | Disabled     |

<img width="341.5" height="230" alt="NAT Network 1" src="https://github.com/user-attachments/assets/8fae0a78-0903-474b-84e1-aa0fbd367ba5" />

<img width="960" height="500" alt="NAT Network 2" src="https://github.com/user-attachments/assets/ae296777-1571-4c98-80c5-d3ed413dec78" />

### Step 4 . Download and Import Kali Linux to VirtualBox.
Go to https://www.kali.org/get-kali/#kali-platforms and click Virtual Machines. 
<img width="960" height="446" alt="Kali web" src="https://github.com/user-attachments/assets/d45a4581-fbc6-48c5-af65-3be32d95b0d8" />

Click VirtualBox and wait for it to complete downloading.

<img width="960" height="447" alt="Kali web 2" src="https://github.com/user-attachments/assets/ef0bd7f2-6e33-47ef-927a-c66ac41934de" />

Extract the Kali Linux download file using 7-Zip or WinRAR and import the extracted folder to VirtualBox. 
<img width="483" height="393" alt="Kali Import" src="https://github.com/user-attachments/assets/b67bada3-ed65-4b15-8f51-c587770d8864" />

<img width="513" height="332" alt="Kali Import 2" src="https://github.com/user-attachments/assets/192c877d-edd0-4a0e-8b23-c7ccbab062d1" />

Successful import should look like the image below.

<img width="960" height="511" alt="Kali sucessful Import " src="https://github.com/user-attachments/assets/1bec4630-84d2-4fb9-8501-394541255433" />

**Tool:** Kali Linux


### Step 5 . Setup the IP Configuration in the Kali Linux virtual machine in Virtualbox.

<img width="640" height="400" alt="VirtualBox_kali-linux-2026 3-virtualbox-amd64_30_10_2026_01_33_41" src="https://github.com/user-attachments/assets/195c6059-8f13-4229-a75d-8de67026979c" />

Click edit connections and double click Wired Connection 1. Open IPv4 Settings tab

<img width="640" height="400" alt="VirtualBox_kali-linux-2026 3-virtualbox-amd64_30_10_2026_01_40_38" src="https://github.com/user-attachments/assets/0ab090ee-a43c-4e27-9a88-4954b0d52461" />

Assigned the following settings in IPv4 Settings in Kali.

### Kali Network Settings
| IP Address | 10.0.0.2|
| :--- | :--- | 
| Subnet Mask | 255.255.255.0 |
| Gateway | 10.0.0.1 |
| DNS| 10.0.0.1 |

<img width="640" height="400" alt="VirtualBox_kali-linux-2026 3-virtualbox-amd64_30_10_2026_01_45_03" src="https://github.com/user-attachments/assets/0623e325-e161-4bcc-9ff7-ae968c46af67" />

Confirm internet is working in Kali Linux.

<img width="640" height="400" alt="VirtualBox_kali-linux-2026 3-virtualbox-amd64_30_10_2026_02_13_02" src="https://github.com/user-attachments/assets/fd60e64e-2910-4399-9f97-9f9ae0f233a8" />

**Tool:** VirtualBox 7.2.22, Kali Linux

### Step 6. Take a snapshot of Kali Linux.

The snapshot is the clean baseline you can go back to if by chance something breaks in future labs.

<img width="960" height="515" alt="Snapshot" src="https://github.com/user-attachments/assets/9020381d-13a8-4c46-a926-f0e423ee99fc" />

##  Tools & Resources

- **7-Zip:** [https://7-zip.org/download.html](https://7-zip.org/download.html)
- **VirtualBox:** [https://virtualbox.org/wiki/Downloads](https://virtualbox.org/wiki/Downloads)
- **Kali Linux:** [https://kali.org/get-kali](https://kali.org/get-kali)

## 👤 Author
**Rajesh Kadim**\
Cybersecurity Intern B084

LinkedIn: https://www.linkedin.com/in/rajesh-kadim/

##  Project Information
Program Name: Cybersecurity at Networkwalks | **Week:** 01 | Project: Cybersecurity & Pentesting Lab Setup | **Repository:** GitHub

