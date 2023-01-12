# nmap_script
A bash script for nmap

This script will preform a scan on an IP. 

Here is the output from sql-scan:

Starting Nmap 7.80 ( https://nmap.org ) at 2023-01-12 08:19 CET
Nmap scan report for 172.16.21.86
Host is up (0.000080s latency).
Not shown: 965 filtered ports, 31 closed ports
PORT    STATE SERVICE
21/tcp  open  ftp
22/tcp  open  ssh
80/tcp  open  http
| http-sql-injection: 
|   Possible sqli for queries:
|     http://172.16.21.86:80/wp-includes/js/jquery/?C=D%3bO%3dA%27%20OR%20sqlspider
|     http://172.16.21.86:80/wp-includes/js/jquery/?C=S%3bO%3dA%27%20OR%20sqlspider
|     http://172.16.21.86:80/wp-includes/js/jquery/?C=M%3bO%3dA%27%20OR%20sqlspider
|_    http://172.16.21.86:80/wp-includes/js/jquery/?C=N%3bO%3dD%27%20OR%20sqlspider
443/tcp open  https
MAC Address: 00:0C:29:7B:45:69 (VMware)

Nmap done: 1 IP address (1 host up) scanned in 15.20 seconds
