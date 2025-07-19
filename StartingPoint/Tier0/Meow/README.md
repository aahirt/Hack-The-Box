# 🐱 Hack The Box — Meow Challenge

## 🔍 Overview
- **Challenge Name:** Meow
- **Difficulty:** Very Easy
- **Platform:** Linux
- **Type:** Starting Point
- **Topic:** Telnet, Enumeration

## 🧰 Tools Used
- `nmap`
- `telnet`
- `ftp` (to verify plaintext protocol)
- Basic shell commands

## 📚 What I Learned
- How to enumerate a public-facing telnet service
- SFTP stands for SSH File Transfer Protocol (or Secure File Transfer Protocol).It is a secure replacement for FTP.Unlike FTP, which sends credentials and data in plaintext, SFTP encrypts everything using the SSH (Secure Shell) protocol.It runs over port 22, the same as SSH
- Importance of disabling default or blank credentials
- How legacy protocols like Telnet are vulnerable to unauthorized access

## Commands Used
- nmap 10.129.40.145 -Pn
- Connect to the target via Telnet: telnet 10.129.40.145
- Tried possible login credentials without password entered(admin, root, user, guest)
- sussessful login with root as username
- ls
- cat flag.txt
- obtained the flag
