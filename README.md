# Smart Bill Guardian

## Project Overview
Smart Bill Guardian is a network-based bill monitoring and payment verification simulation developed using Cisco Packet Tracer.

The project demonstrates how network segmentation, routing, DHCP, access control and server-based monitoring can be implemented in an enterprise-style network.

## Objectives
- Separate customer, billing and payment networks using VLANs.
- Implement inter-VLAN routing using Router-on-a-Stick.
- Assign customer IP addresses using DHCP.
- Configure Access Control Lists (ACLs).
- Implement switch port security.
- Simulate bill monitoring and payment status verification.
- Demonstrate pending and successful transaction statuses.

## Network Architecture

### VLANs
| VLAN | Name | Network |
|---|---|---|
| VLAN 10 | CUSTOMERS | 192.168.10.0/24 |
| VLAN 20 | BILLING | 192.168.20.0/24 |
| VLAN 30 | PAYMENT | 192.168.30.0/24 |

### Devices
- Cisco 2911 Router
- Cisco 2960 Switch
- CUSTOMER1 PC
- CUSTOMER2 PC
- BILL-SERVER
- PAYMENT-SERVER

## IP Addressing

| Device | IP Address |
|---|---|
| Router VLAN 10 Gateway | 192.168.10.1 |
| Router VLAN 20 Gateway | 192.168.20.1 |
| Router VLAN 30 Gateway | 192.168.30.1 |
| BILL-SERVER | 192.168.20.10 |
| PAYMENT-SERVER | 192.168.30.10 |
| CUSTOMER1 | DHCP |
| CUSTOMER2 | DHCP |

## Technologies Implemented
- VLAN
- Router-on-a-Stick
- DHCP
- ACL
- Port Security
- HTTP
- Inter-VLAN Routing

## Bill Monitoring Simulation

### CUSTOMER1
- Bill Amount: Rs. 1500
- Payment Status: PENDING

### CUSTOMER2
- Bill Amount: Rs. 2200
- Payment Status: SUCCESS

## Servers

### BILL-SERVER
Provides simulated bill information and due-date reminders.

### PAYMENT-SERVER
Provides simulated transaction status and transaction history.

## Security
- VLAN segmentation
- ACL-based traffic control
- Switch port security

## Testing
Connectivity and webpage access were tested from the customer PCs using the Packet Tracer simulation.

## Disclaimer
This is an educational networking and payment monitoring simulation. It does not process actual payments or connect to real financial systems.


