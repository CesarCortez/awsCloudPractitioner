# Networking and content delivery

## Introduction to Networking

- **Network** - A group of two or more computer systems linked together
- **Network Interface** - A network interface is a software interface to networking hardware. It is a collection of software and hardware components that enable communication between computers
- **IP Address** - A unique string of numbers separated by periods that identifies each computer using the Internet Protocol to communicate over a network
- **Subnet** - A logical subdivision of an IP network
- **Route Table** - A set of rules, often viewed in table format, that is used to determine where data packets traveling over an Internet Protocol (IP) network will be directed
- **Internet Gateway** - A network component that connects an internal network with the Internet
- **VPC** - A virtual private cloud (VPC) is a virtual network dedicated to your AWS account
- **CIDR** - Classless Inter-Domain Routing (CIDR) is a method for allocating IP addresses and routing Internet Protocol packets. Standard CIDR notation is a slash (/) followed by the number of bits in the network mask.
- **NAT** - Network Address Translation (NAT) is the process where a network device, usually a firewall, assigns a public address to a computer (or group of computers) inside a private network
- **Elastic IP** - An Elastic IP address is a static IPv4 address designed for dynamic cloud computing
- **Security Group** - A security group acts as a virtual firewall for your instance to control inbound and outbound traffic
- **IPv4**  32-bit address
- **IPv6** 128-bit address
- **OSI Model** The Open Systems Interconnection model is a conceptual model that characterizes and standardizes the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology: 7 layers (Physical, Data Link, Network, Transport, Session, Presentation, Application).
- **TCP/IP** The Internet protocol suite is the conceptual model and set of communications protocols used in the Internet and similar computer networks. It is commonly known as TCP/IP because the foundational protocols in the suite are the Transmission Control Protocol (TCP) and the Internet Protocol (IP).
- **DNS** The Domain Name System is a hierarchical and decentralized naming system for computers, services, or other resources connected to the Internet or a private network. It associates various information with domain names assigned to each of the participating entities.


## Amazon Virtual Private Cloud (VPC)

- A virtual private cloud (VPC) is a virtual network dedicated to your AWS account
- It is logically isolated from other virtual networks in the AWS Cloud
- You can launch your AWS resources, such as Amazon EC2 instances, into your VPC
- You can specify an IP address range for the VPC, add subnets, associate security groups, and configure route tables.
- You can use both IPv4 and IPv6 for most resources in your VPC
- You can create a VPC with a single public subnet, a VPC with public and private subnets (NAT), or a VPC with public and private subnets and hardware VPN access to your on-premises network (NAT + VPN)
- Belongs to a single region. You can create subnets in multiple Availability Zones.
- Networks and gateways.
- Layers of security: Security groups and network access control lists (ACLs)

## Subnets

- A subnet is a range of IP addresses in your VPC
- You can launch AWS resources into a specified subnet
## IP Addressing

- IPv4 addresses are 32-bit addresses
- IPv6 addresses are 128-bit addresses
- IPv4 addresses are typically represented in dot-decimal notation, consisting of four decimal numbers, each ranging from 0 to 255, separated by dots, e.g.,
- IPv6 addresses are represented as eight groups of four hexadecimal digits separated by colons, e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334
- CIDR notation is a compact representation of an IP address and its associated routing prefix

## Reserved IP Addresses

- The first four IP addresses and the last IP address in each subnet CIDR block are not available for you to use, and cannot be assigned to an instance
- Network address: The IP address of the network border
- Network gateway address: The IP address of the network gateway

## Types of public IP addresses

- **IPv4 public IP addresses** are reachable from the internet
- **IPv6 public IP addresses** are reachable from the internet
- **Elastic IP addresses** are static IPv4 addresses designed for dynamic cloud computing. An Elastic IP address is associated with your AWS account. With an Elastic IP address, you can mask the failure of an instance or software by rapidly remapping the address to another instance in your account

## Elastic network interfaces

- An elastic network interface is a logical networking component in a VPC that represents a virtual network card
- It can include the following attributes:
  - A primary private IPv4 address from the IPv4 address range of your VPC
  - One or more secondary private IPv4 addresses from the IPv4 address range of your VPC
  - One Elastic IP address per private IPv4 address
  - One public IPv4 address, which can be auto-assigned to the network interface for eth0 when you launch an instance, or assigned later
  - One or more IPv6 addresses
  - One or more security groups
  - A MAC address
  - A source/destination check flag
  - A description

  ## Route Tables

    - A route table contains a set of rules, called routes, that are used to determine where network traffic is directed
    - Each subnet in your VPC must be associated with a route table; the table controls the routing for the subnet
    - A subnet can only be associated with one route table at a time, but you can associate multiple subnets with the same route table
    - The main route table for a VPC is created at the same time as the VPC
    - One to one relationship between a subnet and a route table

## VPC Networking options

- **Internet Gateway** - An internet gateway is a horizontally scaled, redundant, and highly available VPC component that allows communication between instances in your VPC and the internet (IPv4 and IPv6). It therefore imposes no availability risks or bandwidth constraints on your network traffic. 
- **NAT Gateway** - A NAT gateway is a highly available, managed Network Address Translation (NAT) service for your resources in a private subnet to access the internet (IPv4 only). It enables instances in a private subnet to connect to the internet, but prevents the internet from initiating a connection with those instances.
- **NAT Instance** - You can create a NAT instance in your VPC in order to enable instances in a private subnet to connect to the internet (IPv4 only). A NAT instance routes traffic from the instances in the private subnet to the internet, and then sends the response back to the instances. When traffic goes to the internet, the source IPv4 address is replaced with the NAT instance's address and similarly, when the response traffic goes to those instances, the NAT instance translates the address back to those instances' private IPv4 addresses. NAT instances are not supported for IPv6 traffic—use an egress-only internet gateway instead.

## VPC Sharing

- You can share your VPC with another AWS account, or you can share a VPC that another AWS account owns with your account.

## VPC Peering

- A VPC peering connection is a networking connection between two VPCs that enables you to route traffic between them privately. Instances in either VPC can communicate with each other as if they are within the same network. You can create a VPC peering connection between your own VPCs, or with a VPC in another AWS account within a single region.

## AWS Direct Connect

- AWS Direct Connect is a cloud service solution that makes it easy to establish a dedicated network connection from your premises to AWS. Using AWS Direct Connect, you can establish private connectivity between AWS and your datacenter, office, or colocation environment, which in many cases can reduce your network costs, increase bandwidth throughput, and provide a more consistent network experience than Internet-based connections.

## VPC Security

- **Security groups** act at the instance level, not the subnet level. Therefore, each instance in a subnet in your VPC could be assigned to a different set of security groups. If you don't specify a particular group at launch time, the instance is automatically assigned to the default security group for the VPC.
- **Network ACLs (Network access comtrol list)** act at the subnet level. Therefore, each instance in a subnet in your VPC could be associated with a different network ACL; however, a single network ACL can be associated with multiple subnets. If you don't explicitly associate a network ACL with a subnet, the subnet is automatically associated with the default network ACL.

## Amazon Route 53

- Amazon Route 53 is a highly available and scalable cloud Domain Name System (DNS) web service. It is designed to give developers and businesses an extremely reliable and cost-effective way to route end users to Internet applications by translating names like www.example.com into the numeric IP addresses like.
- Amazon Route 53 effectively connects user requests to infrastructure running in AWS – such as Amazon EC2 instances, Elastic Load Balancing load balancers, or Amazon S3 buckets – and can also be used to route users to infrastructure outside of AWS. You can use Amazon Route 53 to configure DNS health checks to route traffic to healthy endpoints or to independently monitor the health of your application and its endpoints. Amazon Route 53 Traffic Flow makes it easy for you to manage traffic globally through a variety of routing types, including Latency Based Routing, Geo DNS, and Weighted Round Robin—all of which can be combined with DNS Failover in order to enable a variety of low-latency, fault-tolerant architectures. Using Amazon Route 53 Traffic Flow’s simple visual editor, you can easily manage how your end-users are routed to your application’s endpoints—whether in a single AWS region or distributed around the globe. Amazon Route 53 also offers Domain Name Registration – you can purchase and manage domain names such as example.com and Amazon Route 53 will automatically configure DNS settings for your domains.

1. **simple routing** - Simple routing lets you route internet traffic to a single resource.
2. **weighted routing** - Weighted routing lets you split your traffic based on different weights assigned to the routes.
3. **latency-based routing** - Latency-based routing lets you route your traffic based on the lowest network latency for your end user.
4. **failover routing** - Failover routing lets you route your traffic based on the health of your endpoints.
5. **geolocation routing** - Geolocation routing lets you choose the resources that serve your traffic based on the geographic location of your users.
6. **multivalue answer routing** - Multivalue answer routing lets you configure Amazon Route 53 to return multiple values, such as IP addresses for your web servers, in response to DNS queries. You can specify multiple values for almost any record, but multivalue answer routing also lets you check the health of each resource, so Amazon Route 53 returns only values for healthy resources. If all the resources are unhealthy, Amazon Route 53 can return up to eight healthy records using multivalue answer routing.
7. **geoproximity routing** - Geoproximity routing lets Amazon Route 53 route traffic to your resources based on the geographic location of your users and your resources. You can also optionally choose to route more traffic or less to a given resource by specifying a value, known as a bias. A bias expands or shrinks the size of the geographic region from which traffic is routed to a resource.

## Amazon CloudFront

- Amazon CloudFront is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers globally with low latency, high transfer speeds, all within a developer-friendly environment.
- CloudFront is integrated with AWS – both physical locations that are directly connected to the AWS global infrastructure, as well as other AWS services. CloudFront works seamlessly with services including AWS Shield for DDoS mitigation, Amazon S3, Elastic Load Balancing or Amazon EC2 as origins for your applications, and Lambda@Edge to run custom code closer to customers’ users and to customize the user experience. Lastly, if you use AWS origins such as Amazon S3, Amazon EC2 or Elastic Load Balancing, you don’t pay for any data transferred between these services and CloudFront.

![CloudFront](../img/CloudFront.JPG)
![CloudFront2](../img/CloudFront2.JPG)