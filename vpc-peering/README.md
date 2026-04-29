## VPC Peering

#### What is VPC Peering ?
VPC Peering is a networking feature that allows two Virtual Private Clouds (VPCs) to communicate with each other privately using internal IP addresses, as if they are part of the same network.

#### How It Works
- Two VPCs establish a peering connection
- You update route tables in both VPCs
- Traffic flows using private IPs only
- No need for gateways, VPNs, or public internet

#### Key Features
- Private communication (no internet)
- Low latency (direct connection)
- High security
- Works across regions (in many cloud providers)

#### When to Use
- Microservices across different VPCs
- Connecting dev, staging, and prod environments
- Multi-account architecture in cloud

#### Project Architecture
<img width="2558" height="896" alt="architecutre" src="https://github.com/user-attachments/assets/fdfe2551-b52c-4315-972d-888f88d74de9" />

#### Project Overview
Created a Virtual Private Cloud (VPC-1) in AWS with CIDR block 10.0.0.0/16 to define the private network range.
<br/>
<img width="1847" height="817" alt="Screenshot 2026-04-28 193635" src="https://github.com/user-attachments/assets/723a429d-68a1-41f7-825f-bd987b04edd9" />
<br/><br/>
Created a subnet in VPC-1 with CIDR block 10.0.0.0/24 to segment the network.
<br/>
<img width="1850" height="853" alt="Screenshot 2026-04-28 193947" src="https://github.com/user-attachments/assets/0610802d-1194-4aa8-b18d-e20ec806b339" />
<br/><br/>
Created a Route Table and associated it with the subnet in VPC-1.
<br/>
<img width="1855" height="832" alt="Screenshot 2026-04-28 232630" src="https://github.com/user-attachments/assets/e9811383-8b78-416f-93f6-dee0c4a252c9" />










