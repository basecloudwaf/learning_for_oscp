# nmap
quoted from the man pages.
## Description
Nmap (Network Mapper) is an open source tool for network exploration and security auditing. It was designed to rapidly scan large networks, although it works fine against single hosts. Nmap uses raw IP packets in novel ways to determine what hosts are available on the network, what services those hosts are offering, what operating systems they are running, what type of packet filters/firewalls are in use, and dozens of other characteristics. While Nmap is commonly used for security audits, many systems and network administrators find it useful for routine tasks such as network inventory, managing service upgrade schedules, and monitoring host or service uptime.

The output from Nmap is a list of scanned targets, with supplemental information on each depending on the options used. Key among that information is the "interesting ports table" that table lists the port number and protocol, service name, and state. The state is either open, filtered, closed, or unfiltered. Open, means that an application on the target is listening for connection/packets on that port. Filtered, means that a firewall, filter, or other network obstacle is blocking the port so that Nmap cannot tell whether it is open or closed. Closed, ports have no application listening on them, though they could open up at any time. Posts are classified as unfiltered, when they are responsive to Nap's probes, but Nmap cannot determine whether they are open or closed. Nmap reports the state combinations open|filtered. and closed|filtered. when it cannot determine which of the two states describe a port. The port table may also include software version details when version detection has been requested. When an IP protocol scan is requested (-s0), Nmap provides information on supported IP protocols rather than listening ports.

In addition to the interesting ports table, Nmap can provide further information on targets, including reverse DNS names, operating system guesses, device types, and MAC addresses.

A typical Nmap scan is shown in Example 1. The only Nmap arguments used in this example are -A, to enable OS and version detection, script scanning, and traceroute; -T4 for faster execution; and then the hostname.

Example 1.A representative Nmap scan
`nmap -A -T4 scanme.nmap.org`

## OPTIONS SUMMARY
summary is printed when Nmap is run with no arguments. It helps people remember the most common options, but is no substitute for the in-depth in the rest of this manual.  

- -iL: Input from list of hosts/networks
- -iR: Choose random targets
- --exclude <host> Exclude hosts/networks
- --exl
<!--stackedit_data:
eyJoaXN0b3J5IjpbNzQ4MDQ5OTQ0LC0yMzM3Njg3NTEsLTE3MT
gwNzQwMTksLTgyNDA4NDU4NiwxNzM2NDY5OTg2LC0xMjQ5NzQ3
ODI3LDQ2NzY2Mzc2NiwtMTM3NzU1ODIyOCwxNzkzNjE4NDQ4LC
0yMDg4NzQ2NjEyXX0=
-->