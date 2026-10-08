```
(root㉿kali)-[~/Desktop/tryhackme/HH]
└─# nmap -sV -sC 10.49.184.196 
Starting Nmap 7.95 ( https://nmap.org ) at 2026-08-05 15:32 EDT
Nmap scan report for 10.49.184.196
Host is up (0.047s latency).
Not shown: 998 closed tcp ports (reset)
PORT     STATE SERVICE VERSION
22/tcp   open  ssh     OpenSSH 9.6p1 Ubuntu 3ubuntu13.18 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   256 58:93:1c:b0:06:cf:f9:d6:93:51:6c:c4:7f:f6:2c:69 (ECDSA)
|_  256 e8:4d:4c:33:c5:33:56:fd:7c:1e:a0:98:04:2d:ff:d1 (ED25519)
5000/tcp open  http    Gunicorn
| http-title: Byte Lotus \xE2\x80\x94 Room Service
|_Requested resource was /login
|_http-server-header: gunicorn
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 9.20 seconds
````
```
[view source page]

(Staff ID): concierge
    
(Passphrase): StayNoticed2024!
```





