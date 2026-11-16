## 1. Introduction to Computer Networks

A computer network is a set of interconnected devices (nodes) that share data and resources using agreed rules called protocols.

- Nodes: computers, servers, phones, routers, switches
- Links: wired (copper, fiber) or wireless (Wi-Fi, cellular)
- Goals: resource sharing, communication, reliability, scalability

## 2. Types of Networks

- PAN (Personal Area Network): a few meters, e.g. Bluetooth between phone and earbuds
- LAN (Local Area Network): a home, office, or campus
- MAN (Metropolitan Area Network): a city-wide network
- WAN (Wide Area Network): spans countries; the Internet is the largest WAN

## 3. Network Topologies

The physical or logical layout of a network.

- Bus: all devices share a single cable; cheap, but one break stops everything
- Star: all devices connect to a central switch; easy to manage, but the switch is a single point of failure
- Ring: each device connects to two neighbors; data travels in a loop
- Mesh: devices connect to many others; highly reliable but expensive
- Tree: hierarchy of star networks
- Hybrid: a combination of the above

## 4. OSI Model

A 7-layer reference model that splits networking into functions.

- Layer 7, Application: user-facing services (HTTP, FTP, SMTP)
- Layer 6, Presentation: encryption, compression, formatting (SSL/TLS, JPEG)
- Layer 5, Session: opens, manages, closes sessions (NetBIOS, RPC)
- Layer 4, Transport: end-to-end delivery and reliability (TCP, UDP)
- Layer 3, Network: logical addressing and routing (IP, ICMP)
- Layer 2, Data Link: node-to-node delivery, MAC addressing (Ethernet, Wi-Fi)
- Layer 1, Physical: raw bits over the medium (cables, hubs)

Memory trick (top to bottom): All People Seem To Need Data Processing.

## 5. TCP/IP Model

The practical model the Internet actually uses, with 4 layers:

1. Application (covers OSI layers 5 to 7): HTTP, DNS, SMTP
2. Transport: TCP, UDP
3. Internet: IP, ICMP, ARP
4. Network Access (covers OSI layers 1 and 2): Ethernet, Wi-Fi

## 6. Network Devices

- Hub: broadcasts data to all ports (Layer 1)
- Switch: forwards frames using MAC addresses (Layer 2)
- Router: connects different networks, forwards packets using IP addresses (Layer 3)
- Modem: converts digital and analog signals for ISP connections
- Access Point: provides Wi-Fi access to a wired network
- Firewall: filters traffic based on security rules
- Gateway: connects networks that use different protocols

## 7. IP Addressing

- IPv4: 32-bit address, written as 192.168.1.1; about 4.3 billion addresses
- IPv6: 128-bit address, written in hexadecimal; solves IPv4 exhaustion
- Classes (IPv4): A (1-126), B (128-191), C (192-223), D (multicast), E (reserved)
- Private ranges: 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16
- Subnetting: dividing a network into smaller ones using a subnet mask, e.g. /24 = 255.255.255.0
- MAC address: 48-bit hardware address, fixed to the network card

## 8. Transport Layer: TCP vs UDP

- Connection: TCP is connection-oriented; UDP is connectionless
- Reliability: TCP guarantees delivery with retransmission; UDP gives no guarantee
- Ordering: TCP is ordered; UDP is not ordered
- Speed: TCP is slower; UDP is faster
- Use cases: TCP for web, email, file transfer; UDP for streaming, gaming, DNS, VoIP
- TCP three-way handshake: SYN, then SYN-ACK, then ACK

## 9. Application Layer Protocols

- HTTP/HTTPS: web pages (ports 80/443)
- FTP: file transfer (ports 20/21)
- SMTP / POP3 / IMAP: email (ports 25 / 110 / 143)
- DNS: translates domain names to IP addresses (port 53)
- DHCP: automatically assigns IP addresses (ports 67/68)
- SSH: secure remote login (port 22)
- Telnet: unencrypted remote login (port 23)

## 10. Routing and Switching

- Static routing: routes set manually by an administrator
- Dynamic routing: routers learn routes automatically
- RIP: distance-vector, uses hop count
- OSPF: link-state, uses cost; common inside organizations
- BGP: path-vector, used between ISPs on the Internet
- Switching techniques: circuit switching, packet switching, message switching

## 11. Error Detection and Flow Control

- Parity bit: simple single-bit error check
- Checksum: sum-based verification used in IP, TCP, UDP
- CRC (Cyclic Redundancy Check): strong check used in Ethernet
- Flow control: stops a fast sender from overwhelming a slow receiver (stop-and-wait, sliding window)
- Congestion control: TCP slows down when the network is overloaded

## 12. Network Security

- Encryption: symmetric (AES) and asymmetric (RSA)
- Firewalls: block unauthorized traffic
- VPN: encrypted tunnel over a public network
- SSL/TLS: secures data between browser and server
- Common attacks: phishing, DDoS, man-in-the-middle, spoofing, sniffing
- Core goals (CIA): Confidentiality, Integrity, Availability

## 13. Wireless Networks

- Wi-Fi (IEEE 802.11): WLAN standard; bands include 2.4 GHz and 5 GHz
- Bluetooth: short-range personal networks
- Cellular: 4G (LTE) and 5G for mobile data
- Security protocols: WEP (broken), WPA2, WPA3 (current best)

## 14. Key Terms to Remember

- Bandwidth: maximum data capacity of a link
- Throughput: actual data rate achieved
- Latency: delay for data to travel from source to destination
- Packet: unit of data at the network layer
- Frame: unit of data at the data link layer
- Port: number identifying an application on a host
- Socket: IP address plus port number
- Client-Server vs Peer-to-Peer: centralized vs distributed resource sharing
EOF