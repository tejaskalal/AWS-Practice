## VPC Peering

#### What is VPC Peering ?
VPC Peering is a networking feature that allows two Virtual Private Clouds (VPCs) to communicate with each other privately using internal IP addresses, as if they are part of the same network.

How It Works
-- Two VPCs establish a peering connection
-- You update route tables in both VPCs
-- Traffic flows using private IPs only
-- No need for gateways, VPNs, or public internet
