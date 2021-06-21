# Nmap-TryHackMe

## Introduction

### Deploy the machine!
<details>
  <summary>Answer</summary>

  ```
   No Answer needed
  ```
</details>


### What networking constructs are used to direct traffic to the right application on a server?
<details>
  <summary>Answer</summary>

  ```
   Ports
  ```
</details>

### How many of these are available on any network-enabled computer?
<details>
  <summary>Answer</summary>

  ```
   65535
  ```
</details>

### [Research] How many of these are considered "well-known"? (These are the "standard" numbers mentioned in the task)
<details>
  <summary>Answer</summary>

  ```
   1024
  ```
</details>


## Nmap Switches
### What is the first switch listed in the help menu for a 'Syn Scan' (more on this later!)?
<details>
  <summary>Answer</summary>

  ```
   -sS
  ```
</details>

### Which switch would you use for a "UDP scan"?
<details>
  <summary>Answer</summary>

  ```
   -sU
  ```
</details>

### If you wanted to detect which operating system the target is running on, which switch would you use?
<details>
  <summary>Answer</summary>

  ```
   -O
  ```
</details>

### Nmap provides a switch to detect the version of the services running on the target. What is this switch?
<details>
  <summary>Answer</summary>

  ```
   -sV
  ```
</details>

### The default output provided by nmap often does not provide enough information for a pentester. How would you increase the verbosity?

<details>
  <summary>Answer</summary>

  ```
   -v
  ```
</details>

### Verbosity level one is good, but verbosity level two is better! How would you set the verbosity level to two?

<details>
  <summary>Answer</summary>

  ```
   -vv
  ```
</details>

### What switch would you use to save the nmap results in three major formats?

<details>
  <summary>Answer</summary>

  ```
   -oA
  ```
</details>

### What switch would you use to save the nmap results in a "normal" format?

<details>
  <summary>Answer</summary>

  ```
   -oN
  ```
</details>

### A very useful output format: how would you save results in a "grepable" format?

<details>
  <summary>Answer</summary>

  ```
   -oG
  ```
</details>

### How would you activate this setting?

<details>
  <summary>Answer</summary>

  ```
   -A
  ```
</details>

### How would you set the timing template to level 5?

<details>
  <summary>Answer</summary>

  ```
   -T5
  ```
</details>

### How would you tell nmap to only scan port 80?

<details>
  <summary>Answer</summary>

  ```
   -p 80
  ```
</details>

### How would you tell nmap to scan ports 1000-1500?

<details>
  <summary>Answer</summary>

  ```
  -p 1000-1500
  ```
</details>

### How would you tell nmap to scan all ports?

<details>
  <summary>Answer</summary>

  ```
  -p-
  ```
</details>

### How would you activate a script from the nmap scripting library (lots more on this later!)?

<details>
  <summary>Answer</summary>

  ```
  --script
  ```
</details>

### How would you activate all of the scripts in the "vuln" category?

<details>
  <summary>Answer</summary>

  ```
 --script=vuln
  ```
</details>

## [Scan Types] Overview
<details>
  <summary>Answer</summary>

  ```
   No Answer needed
  ```
</details>

## [Scan Types] TCP Connect Scans
### Which RFC defines the appropriate behaviour for the TCP protocol?

<details>
  <summary>Answer</summary>

  ```
  RFC 793
  ```
</details>

### If a port is closed, which flag should the server send back to indicate this?

<details>
  <summary>Answer</summary>

  ```
   RST
  ```
</details>

## [Scan Types] SYN Scans
### There are two other names for a SYN scan, what are they?

<details>
  <summary>Answer</summary>

  ```
  half-open,stealth
  ```
</details>

### Can Nmap use a SYN scan without Sudo permissions (Y/N)?

<details>
  <summary>Answer</summary>

  ```
  N
  ```
</details>

## [Scan Types] UDP Scans
### If a UDP port doesn't respond to an Nmap scan, what will it be marked as?

<details>
  <summary>Answer</summary>

  ```
  open|filtered
  ```
</details>

### When a UDP port is closed, by convention the target should send back a "port unreachable" message. Which protocol would it use to do so?

<details>
  <summary>Answer</summary>

  ```
  ICMP
  ```
</details>


## [Scan Types] NULL, FIN and XMas
### Which of the three shown scan types uses the URG flag?

<details>
  <summary>Answer</summary>

  ```
  xmas
  ```
</details>

### Why are NULL, FIN and Xmas scans generally used?

<details>
  <summary>Answer</summary>

  ```
  firewall evasion
  ```
</details>

### Which common OS may respond to a NULL, FIN or Xmas scan with a RST for every port?

<details>
  <summary>Answer</summary>

  ```
  microsoft windows
  ```
</details>

## [Scan Types] ICMP Network Scanning
### How would you perform a ping sweep on the 172.16.x.x network (Netmask: 255.255.0.0) using Nmap? (CIDR notation)

<details>
  <summary>Answer</summary>

  ```
  nmap -sn 172.16.0.0/16
  ```
</details>

## [NSE Scripts] Overview
### What language are NSE scripts written in?

<details>
  <summary>Answer</summary>

  ```
  lua
  ```
</details>

### Which category of scripts would be a very bad idea to run in a production environment?

<details>
  <summary>Answer</summary>

  ```
  intrusive
  ```
</details>

## [NSE Scripts] Working with the NSE
### What optional argument can the ftp-anon.nse script take?

<details>
  <summary>Answer</summary>

  ```
  maxlist
  ```
</details>

## [NSE Scripts] Searching for Scripts
### Search for "smb" scripts in the /usr/share/nmap/scripts/ directory using either of the demonstrated methods.
What is the filename of the script which determines the underlying OS of the SMB server?

<details>
  <summary>Answer</summary>

  ```
  maxlist
  ```
</details>

### Read through this script. What does it depend on?

<details>
  <summary>Answer</summary>

  ```
  smb-brute
  ```
</details>

## Firewall Evasion
### Which simple (and frequently relied upon) protocol is often blocked, requiring the use of the -Pn switch?

<details>
  <summary>Answer</summary>

  ```
  ICMP
  ```
</details>

### Which Nmap switch allows you to append an arbitrary length of random data to the end of packets?

<details>
  <summary>Answer</summary>

  ```
  --data-length
  ```
</details>

## Practical
### Does the target (10.10.53.56)respond to ICMP (ping) requests (Y/N)?

<details>
  <summary>Answer</summary>

  ```
  N
  ```
</details>

### Perform an Xmas scan on the first 999 ports of the target -- how many ports are shown to be open or filtered?

<details>
  <summary>Answer</summary>

  ```
  999
  ```
</details>

### The answer will be in your scan results. Think carefully about which switches to use -- and read the hint before asking for help!

<details>
  <summary>Answer</summary>

  ```
  no response
  ```
</details>

### Perform a TCP SYN scan on the first 5000 ports of the target -- how many ports are shown to be open?

<details>
  <summary>Answer</summary>

  ```
  5
  ```
</details>

### Open Wireshark (see Cryillic's Wireshark Room for instructions) and perform a TCP Connect scan against port 80 on the target, monitoring the results.
Make sure you understand what's going on.

<details>
  <summary>Answer</summary>

  ```
  No answer needed.
  ```
</details>

### Deploy the ftp-anon script against the box. Can Nmap login successfully to the FTP server on port 21? (Y/N)

<details>
  <summary>Answer</summary>

  ```
  Y
  ```
</details>

## Conclusion
### Read the conclusion.

<details>
  <summary>Answer</summary>

  ```
  No answer needed.
  ```
</details>
