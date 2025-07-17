# Hack The Box – Fawn Walkthrough

## 🔐 Challenge Info
- Name: Fawn
- Difficulty: Easy
- OS: Linux
- IP: 10.10.xx.xx (change based on instance)
- Skills: FTP enumeration, anonymous login

## 🛠️ Tools Used
Nmap
FTP
Kali Linux

## 🧭 Walkthrough

### 🔎 Step 1: Enumeration
nmap 10.10.xx.xx -sCV

Found FTP open on port 21...

### 🚪 Step 2: Access FTP
bash
Copy
Edit
ftp 10.10.xx.xx
### Login anonymously
📁 Step 3: Download File
bash
Copy
Edit
get important_file.txt
### Submit Flag (Do NOT paste it here)
Successfully submitted the flag!


