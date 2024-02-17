****

# Demo

![alt text](./images/logo.gif?raw=true "Logo")


***Description:***

​	Introduction to nmap

***Related Hosting Links***

- *TryHackMe.com*
  - Hosted currently as a free room! Recommended for beginners.
  - Link: https://tryhackme.com/room/blue


***Instructions:***

- Start by first checking the IP address of the Kali (or other attack box) you are attacking from
  - ifconfig
  - ![alt text](./images/ifconfig.png?raw=true "ifconfig")
- Following finding the IP address of our attack box, we can move onto discovering the address of the vulnerable box we will be attacking. This can be done either via netdiscover or nmap. Nmap is demonstrated below with a few select flags added for vulnerability discovery.
  - nmap
  - ![alt text](./images/nmap-cmd.png?raw=true "nmap-cmd")
  - -vv : Very verbose
  - -sS : Syn scan (can also use -sV for version numbers)
  - --script vuln : Check for vulnerabilities using the nmap scripting engine
- After waiting a bit, we can see the our results have been generated:
  - ![alt text](./images/nmap-results-1.png?raw=true "nmap-results-1")
  - General port information
  - ![alt text](./images/nmap-results-2.png?raw=true "nmap-results-2")
  