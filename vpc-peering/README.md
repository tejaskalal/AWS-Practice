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
<br/>
<img width="2558" height="896" alt="architecutre" src="https://github.com/user-attachments/assets/fdfe2551-b52c-4315-972d-888f88d74de9" />


