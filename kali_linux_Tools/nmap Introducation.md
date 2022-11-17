<h1 align = 'center'>nmap 使用示例</h1>
以详细模式扫描 （），启用操作系统检测、版本检测、脚本扫描和跟踪路由 （），并针对目标 IP 进行版本检测 （）：-v-A-sV192.168.1.1

root@kali:~# nmap -v -A -sV 192.168.1.1

Starting Nmap 6.45 ( http://nmap.org ) at 2014-05-13 18:40 MDT
NSE: Loaded 118 scripts for scanning.
NSE: Script Pre-scanning.
Initiating ARP Ping Scan at 18:40
Scanning 192.168.1.1 [1 port]
Completed ARP Ping Scan at 18:40, 0.06s elapsed (1 total hosts)
Initiating Parallel DNS resolution of 1 host. at 18:40
Completed Parallel DNS resolution of 1 host. at 18:40, 0.00s elapsed
Initiating SYN Stealth Scan at 18:40
Scanning router.localdomain (192.168.1.1) [1000 ports]
Discovered open port 53/tcp on 192.168.1.1
Discovered open port 22/tcp on 192.168.1.1
Discovered open port 80/tcp on 192.168.1.1
Discovered open port 3001/tcp on 192.168.1.1


e:
──(root㉿kali)-[/home/kali]
└─# nmap -v -A -sV 192.168.253.5
Starting Nmap 7.92 ( https://nmap.org ) at 2022-11-17 09:36 EST
NSE: Loaded 155 scripts for scanning.
NSE: Script Pre-scanning.
Initiating NSE at 09:36
Completed NSE at 09:36, 0.00s elapsed
Initiating NSE at 09:36
Completed NSE at 09:36, 0.00s elapsed
Initiating NSE at 09:36
Completed NSE at 09:36, 0.00s elapsed
Initiating Ping Scan at 09:36
Scanning 192.168.253.5 [4 ports]
Completed Ping Scan at 09:36, 0.05s elapsed (1 total hosts)
Initiating Parallel DNS resolution of 1 host. at 09:36
Completed Parallel DNS resolution of 1 host. at 09:36, 0.17s elapsed
Initiating SYN Stealth Scan at 09:36
Scanning 192.168.253.5 [1000 ports]
Completed SYN Stealth Scan at 09:36, 9.31s elapsed (1000 total ports)
Initiating Service scan at 09:36
Initiating OS detection (try #1) against 192.168.253.5
Initiating Traceroute at 09:36
Completed Traceroute at 09:36, 0.02s elapsed
Initiating Parallel DNS resolution of 2 hosts. at 09:36
Completed Parallel DNS resolution of 2 hosts. at 09:36, 0.24s elapsed
NSE: Script scanning 192.168.253.5.
Initiating NSE at 09:36
Completed NSE at 09:36, 0.03s elapsed
Initiating NSE at 09:36
Completed NSE at 09:36, 0.00s elapsed
Initiating NSE at 09:36
Completed NSE at 09:36, 0.00s elapsed
Nmap scan report for 192.168.253.5
Host is up (0.00075s latency).
All 1000 scanned ports on 192.168.253.5 are in ignored states.
Not shown: 1000 filtered tcp ports (no-response)
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
Device type: WAP|general purpose
Running: Actiontec embedded, Linux 2.4.X|3.X
OS CPE: cpe:/h:actiontec:mi424wr-gen3i cpe:/o:linux:linux_kernel cpe:/o:linux:linux_kernel:2.4.37 cpe:/o:linux:linux_kernel:3.2 cpe:/o:linux:linux_kernel:4.4
OS details: Actiontec MI424WR-GEN3I WAP, DD-WRT v24-sp2 (Linux 2.4.37), Linux 3.2, Linux 4.4
Network Distance: 2 hops

TRACEROUTE (using port 80/tcp)
HOP RTT     ADDRESS
1   0.20 ms 192.168.116.2
2   0.24 ms 192.168.253.5

NSE: Script Post-scanning.
Initiating NSE at 09:36
Completed NSE at 09:36, 0.00s elapsed
Initiating NSE at 09:36
Completed NSE at 09:36, 0.00s elapsed
Initiating NSE at 09:36
Completed NSE at 09:36, 0.00s elapsed
Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 11.33 seconds
           Raw packets sent: 2036 (91.010KB) | Rcvd: 1955 (78.474KB)
