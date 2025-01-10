# Networking Refresher

- IP Addresses
- MAC Addresses
- TCP, UDP, and the Three-Way Handshake
- Common Ports and Protocols
- The OSI Model
- Subnetting

## IP Addresses (Layer 3)
- Routing
- ifconfig or ip -a
- ipv4 = 32bit 
- ipv6 = 128bit
- private ip class for ipv4
	- A(10.0.0.0) \network^ ; /hosts^^
	- B |network ; |hosts
	- C(192.168.0.0) /network ; \hosts (household)
	- loopback

## MAC Addresses (Layer 2)
- Switching
- address for network interface
- 'ether' in ifconfig
	- first three pairs = identifiers

## TCP, UDP and Three-Way Handshake (Layer 4)
- Transport
- Transmission Control Protocol -> connection oriented [HTTP, HTTPS, FTP, SSH]
- User Datagram Protocol -> connectionless [Streaming, DNS, VoIP]
- Three-Way Handshake
	1. SYN (hello there!)
	2. SYN ACK (general kenobi!!!)
	3. ACK (lightsaber battle)

## Common Ports and Protocols
TCP
- FTP (21)
- SSH (22)
- Telnet (23)
- SMTP (25)
- DNS (53)
- HTTP (80)/HTTPS (443)
- POP3 (110)
- SMB (139[old] + 445[new]) : **very imp as pentester** : eg. Wannacry
- IMAP (143)
- LDAP (389)
- SMB (445)
- FTPS (990)
- MySQL (3306)
- RDP (3389)

UDP 
- DNS (53)
- DHCP (67,68)
- TFTP (69)
- NTP (123)
- SNMP (161)
- LDAP (389)

## OSI Model
 
- Physical (data cables, cat6)
- Datalink (switching, MAC Addr)
- Network (IP addr, routing)
- Transport (TCP/UDP)
- Session (session management)
- Presentation (JPEG, MOV)
- Application (HTTP, SMTP)

## Subnetting
- 32 bit
- BOOORING



^\ - down arrow
^^/ - up arrow