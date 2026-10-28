# Lab-00-Basic-Network
Create 1 router, 1 switch, 4 PCs. Assign IPs and test ping.

## Objective
Build a simple office network using a Cisco router, switch, and multiple PCs. Configure IP addressing and verify connectivity between devices on the same LAN and across different networks through a router.

## Tools Used
Cisco Packet Tracer
Cisco 2960 Switch
Cisco ISR4321 Router
IPv4 Addressing
ICMP (Ping)
Basic Routing

## Network Topology
                PC2
                 |
                 |
PC0 -------- Switch0 -------- Router0 -------- PC3
                 |
                 |
                PC1

## Network Design
| Device        | IP Address   | Subnet Mask   | Default Gateway |
| ------------- | ------------ | ------------- | --------------- |
| Router G0/0/0 | 192.168.1.1  | 255.255.255.0 | N/A             |
| PC0           | 192.168.1.10 | 255.255.255.0 | 192.168.1.1     |
| PC1           | 192.168.1.11 | 255.255.255.0 | 192.168.1.1     |
| PC2           | 192.168.1.12 | 255.255.255.0 | 192.168.1.1     |

## Lan 2
| Device        | IP Address   | Subnet Mask   | Default Gateway |
| ------------- | ------------ | ------------- | --------------- |
| Router G0/0/1 | 192.168.2.1  | 255.255.255.0 | N/A             |
| PC3           | 192.168.2.10 | 255.255.255.0 | 192.168.2.1     |


## Steps Completed
Router Configuration

Configured:

GigabitEthernet0/0/0
GigabitEthernet0/0/1
IP addressing
Enabled interfaces using no shutdown
PC Configuration

Configured:

Static IP addresses
Subnet masks
Default gateways
Connectivity Testing

Validated:

Same-network communication
Cross-network routing
Gateway reachability
ICMP ping responses

## Validation
- PCs in the same VLAN can ping each other.
- PCs in different VLANs cannot communicate without routing.

## Screenshots
<img width="937" height="590" alt="image" src="https://github.com/user-attachments/assets/274cb6ea-b27a-4de2-aad8-348a96dbc6d9" />
<img width="473" height="293" alt="image" src="https://github.com/user-attachments/assets/c2c7e443-9038-4968-8b16-8d027fabad6a" />
<img width="785" height="337" alt="image" src="https://github.com/user-attachments/assets/5c7fe1cf-ccce-4399-ba78-596a92bb2bb6" />
<img width="766" height="242" alt="image" src="https://github.com/user-attachments/assets/8f005046-b002-4985-b3d0-f355f0a1d591" />





## Lessons Learned
Issue	Resolution
Router interfaces down	Used no shutdown
Incorrect subnetting	Corrected IP addressing
Missing default gateway	Added router IP as gateway
Ping timeout	Verified interfaces and gateway settings
