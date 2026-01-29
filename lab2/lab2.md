# Lab 2: Network Commands for Testing and Troubleshooting

## Objective
To familiarize with essential network commands used for testing and troubleshooting network connectivity issues.

## Required Tools
- A computer with Command Line Interface (CLI) access  
- Network connection (wired or wireless)

## Network Commands

### Syntax and Usage of Common Network Commands

#### 1. ping
- **Syntax:**  
  `ping [hostname or IP address]`
- **Usage:**  
  Tests the reachability of a host on an IP network and measures the round-trip time for messages sent from the source to the destination computer.

---

#### 2. ipconfig (Windows) / ifconfig (Linux)
- **Syntax:**  
  `ipconfig` or `ifconfig`
- **Usage:**  
  Displays current TCP/IP network configuration values and refreshes DHCP and DNS settings.

---

#### 3. tracert (Windows) / traceroute (Linux)
- **Syntax:**  
  `tracert [hostname or IP address]`  
  `traceroute [hostname or IP address]`
- **Usage:**  
  Determines the route taken by packets to reach a specific host by listing all intermediate routers.

---

#### 4. netstat
- **Syntax:**  
  `netstat -a` or `netstat -n`
- **Usage:**  
  Displays active TCP connections, listening ports, Ethernet statistics, and more.

---

#### 5. nslookup
- **Syntax:**  
  `nslookup [hostname]`
- **Usage:**  
  Queries the Domain Name System (DNS) to obtain domain name or IP address mapping information.

---

#### 6. arp
- **Syntax:**  
  `arp -a`
- **Usage:**  
  Displays and modifies the IP-to-Physical (MAC) address translation table used by ARP.

---

#### 7. telnet
- **Syntax:**  
  `telnet [hostname or IP address] [port]`
- **Usage:**  
  Connects to a remote host using the Telnet protocol, useful for testing connectivity to specific ports.  

> *No output due to installation issue.*

---

#### 8. netsh wlan (Windows)
- **Syntax:**  
  `netsh wlan show profiles`  
  `netsh wlan connect name=[profile name]`
- **Usage:**  
  Manages wireless network profiles and connections on Windows systems.

---

#### 9. pathping
- **Syntax:**  
  `pathping [hostname or IP address]`
- **Usage:**  
  Combines the functionality of ping and tracert to provide information about network latency and packet loss at each hop.

---

#### 10. route print
- **Syntax:**  
  `route print`
- **Usage:**  
  Displays the current IP routing table on the local machine.

---

#### 11. getmac
- **Syntax:**  
  `getmac`
- **Usage:**  
  Displays the MAC addresses of network adapters on the local machine.

---

#### 12. nbtstat
- **Syntax:**  
  `nbtstat -a [hostname]`
- **Usage:**  
  Displays NetBIOS over TCP/IP statistics, including the NetBIOS name table of a remote computer.

---

#### 13. whois
- **Syntax:**  
  `whois [domain name]`
- **Usage:**  
  Retrieves registration information about a domain name from the WHOIS database.  

> *Some outputs were not displayed due to recognition error.*

---

## Procedure
1. Open the Command Line Interface (CLI) on your computer.
2. Use the `ipconfig` or `ifconfig` command to check the current network configuration.
3. Execute the listed commands and observe their outputs.

## Output
All outputs are attached along with the syntax and usage of the respective commands.

## Conclusion
This lab provided hands-on experience with various network commands essential for diagnosing and troubleshooting network issues. The commands learned in this lab can be effectively applied in real-world network troubleshooting scenarios.

