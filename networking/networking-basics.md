Networking Fundamentals

1. What is a Network?

A network is a group of connected devices that communicate and share
information.

-   LAN: Local Area Network.
-   WAN: Wide Area Network.
-   Internet: A global network connecting devices worldwide.

2. IP Address

An IP address identifies a device or network interface on an IP network.

Example: 192.168.1.25

Common private IPv4 ranges:

-   10.0.0.0 – 10.255.255.255
-   172.16.0.0 – 172.31.255.255
-   192.168.0.0 – 192.168.255.255

Loopback address: 127.0.0.1

3. MAC Address

A MAC address is a link-layer address used for communication on a local
network.

Example: A4:5E:60:C2:19:7B

-   IP address: Used for communication across IP networks.
-   MAC address: Used for local network delivery.

4. Default Gateway

A default gateway is usually your router.

It forwards traffic from your local network to other networks.

Command: ip route

5. Ports and Services

A port identifies a communication endpoint used by an application or
service.

  Port    Common Service
  ------- ----------------
  20/21   FTP
  22      SSH
  25      SMTP
  53      DNS
  80      HTTP
  443     HTTPS
  3306    MySQL
  3389    RDP

Port numbers range from 0 to 65535.

6. DNS

DNS translates domain names into IP addresses.

Example: example.com → an IP address.

Useful command:

getent hosts example.com

7. DHCP

DHCP automatically provides network configuration to devices.

It can assign:

-   IP address
-   Subnet mask or prefix
-   Default gateway
-   DNS server

DORA process:

1.  Discover
2.  Offer
3.  Request
4.  Acknowledge

8. Subnetting and CIDR

A subnet mask separates the network portion from the host portion of an
IP address.

Example:

192.168.1.25/24

-   /24 means 24 network bits.
-   Subnet mask: 255.255.255.0
-   Network address: 192.168.1.0

9. TCP vs UDP

TCP:

-   Connection-oriented.
-   Reliable and ordered delivery.
-   Commonly used by HTTPS and SSH.

UDP:

-   Connectionless.
-   Does not provide TCP-style delivery guarantees.
-   Commonly used by DNS.

10. HTTP vs HTTPS

-   HTTP commonly uses port 80.
-   HTTPS commonly uses port 443.
-   HTTPS uses TLS to protect communication.

Common HTTP status codes:

-   200 — OK
-   301 — Moved Permanently
-   403 — Forbidden
-   404 — Not Found
-   500 — Internal Server Error

11. Useful Kali Networking Commands

  Command                       Purpose
  ----------------------------- -------------------------------------------
  ip addr                       Displays network interfaces and addresses
  ip -br addr                   Displays a brief interface summary
  ip route                      Displays routing information
  ss -lnt                       Displays listening TCP sockets
  ss -lun                       Displays listening UDP sockets
  ping -c 4 example.com         Sends four ping requests
  traceroute example.com        Displays network hops
  curl -I https://example.com   Displays HTTP response headers

Key Takeaway

Networking knowledge is essential for ethical hacking. Understanding IP
addresses, ports, protocols, DNS, and routing helps us understand how
systems communicate and how to assess their security.
