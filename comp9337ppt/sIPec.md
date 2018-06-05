# 2 network-layer confidentiality
between two network entities:
* sending entity encrypts datagram payload 
* all data sent from one entity to other would be hidden
* blanket coverage”

# 3-4 Virtual Private Networks (VPNs)
* institutions often want private networks for security but costly
* VPN: institution’s inter-office traffic is sent over public Internet instead
1. encrypted before entering public Internet
2. logically separate from other traffic

# 5 IPsec services
* Data integrity
* Origin authentication
* Replay attack prevention
* Confidentiality
* Two different offerings (AH and ESP)

# 6 Tunnel and Transport Modes
Transport Mode: protects IP Payload from layers above (Higher layer TCP, UDP,ICMP..)

Tunnel Mode: All of IP including header etc is encapsulated, new IP header is added by Firewall/Routers.
