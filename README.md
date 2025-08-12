Day 02

Installing Kali Linux on Oracle VirtualBox:

There are primarily 3 things Needed to install Kali linux on a Windows Host Machine.
1. Downloading Kali linux VirtualBox Image.(https://cdimage.kali.org/kali-2025.2/kali-linux-2025.2-virtualbox-amd64.7z)
2. Downloading 'Oracle VirtualBox'. It is a general-purpose full virtualization software.(https://download.virtualbox.org/virtualbox/7.1.12/VirtualBox-7.1.12-169651-Win.exe)
3. Downloading '7Zip'. It is a free and open-source file archiver with a high compression ratio. We are gonna use this for extracting the downloaded zip file.(https://www.7-zip.org/a/7z2500-x64.exe)

Note: Ensure you Have a minimum of 10-15 Gbs of Space in your Storage.

Step 1:
Installing Oracle VirtualBox on Windows host Machine.
1. Execute the downloaded VirtualBox installer.
2. Click on 'Yes' to provide the Administrator privilages needed.
3. Once Installer Dialogue box pops up click on 'Next'.
4. 'Custom Setup' page arrives. I suggest you don't do anything and press on 'Next'.
At the bottom left corner of the dialogue box defines the place where the software is gonna be installed.
5. Next "Warning! Network Interface' Page appears. Press 'Yes' to Continue.
6. Next "Missing Dependencies" Pages appears. Press 'Yes' to continue.
7. Next "Ready to install" Pages appears. Press 'Install'.
8. Click on 'Finish' and The VirtualBox is installed in your Host Machine.

TrobbleShooting Problems Occured during and after The installation of Oracle VirtualBox:
Problem 1
Missing 'Microsoft Visual C++ 2015-2022 Redistributable (x64) - 14.44.35211'
1. Click on the link to Download The dependency. https://aka.ms/vs/17/release/vc_redist.x64.exe and Install it.
2. Relauch the Oracle VirtualBox installer and Follow step 1.

 Problem 2
 AMD-V is diasabled in the BIOS(or by the Host OS)
1. Reboot Your System into Bios.
    To Enter into BIOS ,Check Your device model and Google for bios Key for that     Model. BIOS Key for some of the Famous Laptop's are Mentioned below.
      Dell: F2 or F12
Lenovo: F2 or Fn + F2 (for laptops), F1 (for desktops and all-in-ones), or the       Novo button
      Acer: F2 or DEL
      HP: Esc or F10
2. Navigate to Advance Setting Menu and search for Virtualization or SVM mode and Enable it.
    

Step 2:
Installing 7Zip tool.
1.Right click on downloaded 7Zip installer and "Run as Administrator".
2.An installer Diaglogue box appears, Click on 'Install'.
3.Click on 'Close' after installation.

Step 3:
Extracting the Downloaded Kali Linux VirtualBox Image Zip File.
1.Navigate to Directory where You have Downloaded the Kali Linux VirtualBox Image Zip file.
2.Right click on the Zip file and click on 'Show more options'. Move Your Cursor close to the 7Zip option and click on 'Extract here'.
3. It will take some time extracting the File after that the Extracting Taskj is Complete.

Step 4:Loading the Kali Linux VirtualBox image File.
1.It is Recommended to Make a Seperate pertetion in your Disk drive for Keeping Kali linux.(10-15 Gbs will be fine)(https://www.youtube.com/watch?v=HGqo17dGk0E)
2.Copy the Extracted Kali Linux VirtualBox image File to the new partetion.
3.Open the folder and you will find 2 files types, 1.VirtualBox Machine Defination and 2.Virtual Disk Image File.You have to double click on 'VirtualBox Machine Defination' Type file.
4. Oracle VirtualBox opens, Click on 'Start' to Turn on the Virtual Machine. Its going to take a when u are booting it for the First time.
5. After sucessful booting, Enter Username and password as 'kali'.




DAY 3

Linux provides a powerful set of commands to manage files and directories efficiently. To begin with, you can navigate the file system using commands like pwd, which prints the current working directory, and cd, which is used to change directories. For instance, cd Documents moves into the Documents folder, cd .. moves up to the parent directory, and simply typing cd brings you back to your home directory.

To view files and directories in the current location, you can use ls. Adding options enhances its functionality: ls -l shows detailed information including permissions and file sizes, ls -a reveals hidden files, ls -lh presents human-readable sizes, and ls -R lists contents recursively. Creating files and directories is also straightforward. The touch command is used to create empty files (e.g., touch file.txt), while mkdir creates new directories. For creating nested directories in one go, mkdir -p dir1/dir2 is used.

Copying and moving files is handled with cp and mv. For example, cp file.txt backup.txt makes a copy of a file, and cp -r dir1 dir2 copies an entire directory recursively. The mv command is used to move or rename files and directories. So, mv old.txt new.txt renames a file, and mv file.txt /home/user/docs moves it to another location.

To delete files, rm is used. A simple rm file.txt deletes a file, while rm -r folder/ removes a directory and all its contents. To remove an empty directory, rmdir is used. If you want to delete files without confirmation prompts, rm -f will force the deletion. Additionally, the stat command displays detailed file information such as size and timestamps, while file identifies the type of file based on its content.

Using these commands, users can fully manage their file system from the terminal with speed and precision. Remember, using the Tab key for auto-completion and adding options to commands (like -l, -r, or -a) can save a lot of time and reduce typing errors.
Loading the Kali Linux VirtualBox image File.
1.It is Advised to Create a Seperate pertetion in your Disk drive for Storing Kali linux.(10-15 Gbs would be sufficient)(https://www.youtube.com/watch?v=HGqo17dGk0E)
2.Copy the Extracted Kali Linux VirtualBox image File to the new partetion.
3. Open the folder and you will get 2 file types, 1.VirtualBox Machine Defination and 2.Virtual Disk Image File.Du need to double click on 'VirtualBox Machine Defination' Type file.
4. Oracle VirtualBox gets opened, Click on 'Start' to Turn on the Virtual Machine.Its going to take a when u are booting it for the First time.
5. After sucessful booting, Enter Username and password as 'kali'.

DAY 4

### 1. **IPv4 (Internet Protocol version 4)**

* **Definition**: IPv4 is the fourth version of the Internet Protocol used to identify devices on a network using an addressing system.
* **Address Format**: 32-bit address (e.g., `192.168.1.1`)
* **Total Addresses**: About **4.3 billion** unique addresses.
* **Structure**: Written in **dot-decimal notation** (four numbers separated by dots).
* **Limitation**: Because of the growing number of internet devices, IPv4 addresses are running out.

---

### 2. **IPv6 (Internet Protocol version 6)**

* **Definition**: IPv6 is the newer version of the Internet Protocol designed to replace IPv4.
* **Address Format**: 128-bit address (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`)
* **Total Addresses**: Around **340 undecillion** (virtually unlimited).
* **Structure**: Written in **hexadecimal** and separated by colons.
* **Advantage**: Solves the IPv4 exhaustion problem and offers better routing and security features.

---

### 3. **MAC ID (Media Access Control Address)**

* **Definition**: A MAC ID (or MAC address) is a **unique hardware identifier** assigned to a network interface card (NIC) by the manufacturer.
* **Format**: 48-bit address, usually shown as `00:1A:2B:3C:4D:5E`
* **Purpose**: Used for identifying devices within a **local network (LAN)**.
* **Cannot Be Changed**: It's a physical address tied to the device (though it can be spoofed).

---

### 4. **TCP (Transmission Control Protocol)**

* **Definition**: TCP is a **connection-oriented** protocol that ensures **reliable communication** between two devices.
* **Features**:

  * Data is sent in a sequence.
  * Ensures data reaches correctly (error checking).
  * Slower but **more reliable**.
* **Examples**: Used in applications like **web browsing (HTTP/HTTPS)**, **email (SMTP)**, and **file transfers (FTP)**.

---

### 5. **UDP (User Datagram Protocol)**

* **Definition**: UDP is a **connectionless** protocol used for fast, **non-reliable communication**.
* **Features**:

  * No error checking or guaranteed delivery.
  * Much **faster** than TCP.
* **Examples**: Used in **video streaming**, **online gaming**, and **VoIP (Voice over IP)**.

---

### Comparison Table:

| Feature     | TCP                        | UDP                         |
| ----------- | -------------------------- | --------------------------- |
| Connection  | Connection-oriented        | Connectionless              |
| Speed       | Slower                     | Faster                      |
| Reliability | High (guaranteed delivery) | Low (no delivery guarantee) |
| Use Case    | Email, Web browsing        | Gaming, Streaming           |

---
### 🔍 **Reconnaissance in Cybersecurity**

**Definition**:
**Reconnaissance** is the **first phase** of the ethical hacking or cyberattack lifecycle. It involves **gathering information** about a target system, network, or organization **before launching an attack**. Think of it like a thief studying a building before breaking in.

---

### 🧠 **Purpose of Reconnaissance**

* To **understand the target's environment**
* Identify **vulnerabilities**, **open ports**, **IP addresses**, **technologies used**
* Reduce chances of **detection** during the actual attack
* Plan effective attacks or penetration tests

---

### 🛠️ **Types of Reconnaissance**

| Type              | Description                                                                                                                      |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| **Passive Recon** | Collecting info **without interacting** directly with the target. Example: looking at social media, WHOIS data, Google searches. |
| **Active Recon**  | Directly engaging with the target to gather information. Example: scanning networks, pinging devices, port scanning.             |

---

### 🔧 **Common Recon Tools**

| Tool             | Use                                                            |
| ---------------- | -------------------------------------------------------------- |
| **Nmap**         | Network scanning, open ports, services                         |
| **Wireshark**    | Packet analysis (network traffic)                              |
| **theHarvester** | Email, subdomain, and employee information gathering           |
| **Maltego**      | Visual link analysis for people, companies, domains, and IPs   |
| **Google Dorks** | Using advanced search techniques to find sensitive information |

---

### 🧾 **Examples of Information Collected**

* IP address ranges
* Subdomains
* Open ports
* Software versions
* Employee names or emails
* DNS records

---

### ⚠️ **Why It Matters**

In ethical hacking, reconnaissance helps in:

* Finding weak points before an attacker does
* Strengthening defenses proactively
* Simulating real-world attack planning for better security

---
DAY 5
---

**Low Privilege User**
A low privilege user is an account with minimal access rights and permissions, typically restricted to basic system usage such as opening approved applications, reading allowed files, and performing non-administrative tasks. This follows the *Principle of Least Privilege (PoLP)*, which aims to reduce security risks by limiting what each user can do. Even if compromised, such an account cannot directly make critical system changes or access sensitive data, helping contain potential damage. An example is a standard employee account without administrator rights.

---

**Security Operations Center (SOC)**
A Security Operations Center (SOC) is a dedicated team or facility responsible for continuously monitoring, detecting, analyzing, and responding to cybersecurity threats in an organization. SOC analysts use tools such as SIEM systems, intrusion detection systems (IDS), and firewall logs to identify suspicious activities. The SOC’s main functions include real-time threat monitoring, incident response, threat intelligence gathering, and reporting on security incidents for compliance and management. Operating 24/7, SOCs act as the nerve center of an organization’s cybersecurity defense.

---

**Data Exfiltration**
Data exfiltration refers to the unauthorized transfer of sensitive data from within a network to an external destination, often carried out by malicious insiders or external attackers. This can happen through methods such as malware sending data over the internet, unauthorized copying to USB drives, or sending confidential information via email. Data exfiltration is a serious security breach as it can lead to financial loss, reputational damage, and legal consequences. Preventive measures include data loss prevention (DLP) tools, encryption, strict access controls, and continuous monitoring of data movements.

---

**Privilege Escalation**
Privilege escalation is the process of gaining higher access rights than initially granted, often exploited by attackers after obtaining entry into a low privilege account. There are two main types: *vertical escalation*, where a standard user gains administrative or root privileges, and *horizontal escalation*, where a user gains access to another user’s resources without higher privileges. Common techniques include exploiting software vulnerabilities, misconfigured permissions, and stealing credentials. Successful privilege escalation can lead to full system control, disabling of security measures, and easier execution of further attacks.





