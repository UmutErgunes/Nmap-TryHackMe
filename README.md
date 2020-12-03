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



