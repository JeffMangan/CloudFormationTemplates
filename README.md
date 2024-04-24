## NAT Gateway & NAT Instance yaml templates

### Overview
This repo provides to yaml templates, one for an AWS NAT Gatewway and one for a NAT Instance.  I wanted to avoid paying the cost of NAT Gateway in my non-production environments.

### NAT Gateway
- **Managed Service**: AWS NAT Gateway is a managed service designed to provide Internet connectivity to EC2 instances in private subnets while blocking inbound traffic from the Internet.
- **Cost**: NAT Gateways are more expensive than NAT Instances as they charge per hour and for each gigabyte of data processed.
- **Ease of Use**: As a fully managed service, it requires minimal setup and ongoing maintenance effort, making it ideal for teams without specialized network management skills.

### NAT Instance
- **EC2-based Solution**: A NAT Instance is an EC2 instance configured to perform Network Address Translation. It's suitable for providing Internet connectivity to private subnets.
- **Cost**: Typically cheaper than a NAT Gateway because it leverages the EC2 pricing model, which is more flexible. However, costs can vary based on the instance type and traffic.
- **Management Effort**: Requires more setup and manual configuration (e.g., setting up the routing tables, ensuring high availability). It demands consistent management and monitoring, making it more labor-intensive than using a NAT Gateway.

### Cost vs. Effort Trade-off
- **NAT Gateway**: Higher cost but significantly reduces management overhead and offers better availability and bandwidth scalability.
- **NAT Instance**: More cost-effective but requires a higher degree of manual setup, management, and monitoring (ideal for non production environments).



