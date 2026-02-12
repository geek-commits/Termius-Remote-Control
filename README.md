# Termius Remote Control Portfolio  
  
**Author:** Gadi Josephat Daniel  
**Project Status:** Success  
**Tools:** Termius, SSH, Python, SFTP  
  
## 1. Project Overview  
This repository documents my competency in remote server management. Using Termius as my client, I successfully established a local SSH environment on macOS to execute two key tasks:  
1.  **Remote Service Deployment:** Hosting a local web server accessed by external devices.  
2.  **Secure File Manipulation:** Modifying critical files remotely via SFTP overwrite.  
  
---  
  
## 2. Execution Log  
  
### Task A: Local Network Web Server  
**Objective:** Launch a network service and verify accessibility from a separate mobile client.  
  
* **Command Used:** `python3 -m http.server 8000`  
* **Protocol:** TCP/IP (Localhost)  
* **Verification:** Accessed the server via iPhone at `192.168.1.125:8000`.  
  
**Evidence:**  
*Successful Handshake between Server (Mac) and Client (iPhone)*  
![Web Server Proof](proof_web_server.jpg)  
  
---  
  
### Task B: The "Overwrite" Attack (SFTP)  
**Objective:** Modify a protected file on the remote server without direct terminal editing access.  
  
* **Method:**  
    1.  Located target file `notes.pdf` in `/Secret_Project`.  
    2.  Created a local replica with modified payload ("COMPROMISED by Gadi").  
    3.  Forced an **SFTP Overwrite** to inject the new file into the remote directory.  
  
**Evidence:**  
*Step 1: Locating the target in Termius SFTP Interface*  
![SFTP Interface](proof_sftp_interface.jpg)  
  
*Step 2: Verification of the compromised file content*  
![Text Modification](proof_text_modified.png)  
  
---  
  
## 3. Technical Conclusion  
This project demonstrates functional proficiency in:  
* **Port Forwarding & Listening:** Understanding how port 8000 broadcasts on a LAN.  
* **SFTP Management:** Managing remote file systems using GUI-based SSH tools.  
* **Network Addressing:** Configuring local IP static routing.  
