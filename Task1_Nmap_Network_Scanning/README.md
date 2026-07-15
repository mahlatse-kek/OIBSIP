## What is Nmap?

Nmap (Network Mapper) is a free, open-source tool used to discover hosts and services on a network by sending packets and analysing the responses. It’s one of the most widely used tools in cybersecurity for reconnaissance, inventory and security auditing.

## Why network scanning matters:

Scanning reveals what’s actually exposed on a network — open ports, running services, and operating system fingerprints which is the same information an attacker would gather before attempting an exploit. Security teams scan their own networks proactively to find and close these gaps first.

**Setup Windows**
	1.	Go to nmap.org/download.html and download the Windows installer (self-installer .exe).
	2.	Run it. If it asks to install/confirm Npcap, accept — you likely already have this from installing Wireshark for Task 8, since they share the same packet-capture driver.
	3.	Once installed, open Command Prompt or PowerShell — Nmap runs directly from there, no VM or WSL required.
	4.	Confirm it installed correctly:

nmap --version

Choosing a target to scan:

You must only scan a machine you own or control. The easiest legitimate target is your own laptop, scanned via its loopback address:

nmap 127.0.0.1

Summary For Steps:

# 1. Basic scan
nmap [target IP]

# 2. Service version scan
nmap -sV [target IP]

# 3. OS detection scan (Command Prompt/PowerShell as Administrator)
nmap -O [target IP]

## Findings: