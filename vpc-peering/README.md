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
<br/><br/>
<img width="1174" height="595" alt="Screenshot 2026-04-28 170853" src="https://github.com/user-attachments/assets/f03760c9-97d8-48f9-9e1d-be9a56ed3b7a" />


