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
<br/><br/>
Associated the Route Table with the public subnet (vpc1-public-subnet) in VPC-1.
<br/>
<img width="1846" height="829" alt="Screenshot 2026-04-28 232749" src="https://github.com/user-attachments/assets/ff09dda5-2087-4691-b36b-48a443a3f03c" />
<br/><br/>
Created an Internet Gateway (IGW) and attached it to VPC-1 to enable internet access.
<br/>
<img width="1855" height="844" alt="Screenshot 2026-04-28 232832" src="https://github.com/user-attachments/assets/5a6f87e0-0f48-489f-9e48-04491d14a949" />
<br/>
<img width="1856" height="839" alt="Screenshot 2026-04-28 232856" src="https://github.com/user-attachments/assets/0ab86bbc-5f0a-418b-8047-28a810ba4a4f" />
<br/><br/>
Updated the Route Table by adding a route (0.0.0.0/0) pointing to the Internet Gateway.
<br/>
<img width="1848" height="837" alt="Screenshot 2026-04-28 232950" src="https://github.com/user-attachments/assets/58a328e1-d18f-4660-8079-00e7779bb23e" />
<br/><br/>
Launched an EC2 instance in VPC-1 using t3.micro instance type with auto-assign public IP enabled for internet access.
<br/>
<img width="1845" height="829" alt="Screenshot 2026-04-28 233153" src="https://github.com/user-attachments/assets/f8110921-3831-48fd-a9ed-340cf61b878e" />
<br/>
<img width="1854" height="830" alt="Screenshot 2026-04-28 233234" src="https://github.com/user-attachments/assets/fbea55c2-7c80-4376-9e15-d258e930ed59" />
<br/><br/>
Created a second VPC (my-vpc-2) with CIDR block 192.168.0.0/24 to define a separate private network.
<br/>
<img width="1852" height="850" alt="Screenshot 2026-04-28 234720" src="https://github.com/user-attachments/assets/0e901bfa-efc8-4196-a505-d9a83023dbc5" />
<br/><br/>
Created a subnet (vpc2-public-subnet) in my-vpc-2.
<img width="1853" height="840" alt="Screenshot 2026-04-28 234901" src="https://github.com/user-attachments/assets/2a2c984c-a981-424a-88a3-cd774195b0ef" />
<br/><br/>
Created a Route Table named vpc2-route-table in my-vpc-2.
<br/>
<img width="1848" height="851" alt="Screenshot 2026-04-28 234939" src="https://github.com/user-attachments/assets/6128134d-25b2-49f6-bbe6-88cca0c9bee9" />
<br/><br/>
Created an Internet Gateway (vpc2-IGW) for my-vpc-2.
<br/>
<img width="1840" height="827" alt="Screenshot 2026-04-28 235003" src="https://github.com/user-attachments/assets/39ee8a9b-2095-4887-9475-c5960002085c" />
<br/>
Attached Internet Gateway for network access to my-vpc-2
<img width="1851" height="846" alt="Screenshot 2026-04-28 235022" src="https://github.com/user-attachments/assets/e58fd82f-4ca4-4e13-95f9-89674e4162a6" />
<br/><br/>
Associated the vpc2-route-table with vpc2-public-subnet
<br/>
<img width="1856" height="857" alt="Screenshot 2026-04-28 235117" src="https://github.com/user-attachments/assets/0aee5f44-8e2d-476f-8372-749d5f89e03e" />
<br/><br/>
Updated the Route Table by adding a route (0.0.0.0/0) pointing to the Internet Gateway.
<br/>
<img width="1856" height="857" alt="Screenshot 2026-04-28 235117" src="https://github.com/user-attachments/assets/91b308e9-7f55-43d4-b0f9-3c20fd11954e" />
<br/><br/>
Launched an EC2 instance in VPC-1 using t3.micro instance type with auto-assign public IP enabled for internet access.
<img width="1849" height="820" alt="Screenshot 2026-04-28 235747" src="https://github.com/user-attachments/assets/09c3f6a5-bf8f-48de-a4d8-00bf01355e80" />
<br/>
<img width="1856" height="840" alt="Screenshot 2026-04-28 235827" src="https://github.com/user-attachments/assets/7c88afef-413a-46ce-abf4-bddb52e82303" />
<br/><br/>





















