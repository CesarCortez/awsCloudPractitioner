# Automatic scaling and monitoring 

## Elastic Load Balancing

Elastic Load Balancing automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, IP addresses, and Lambda functions. It can handle the varying load of your application traffic in a single Availability Zone or across multiple Availability Zones. Elastic Load Balancing offers three types of load balancers that all feature the high availability, automatic scaling, and robust security necessary to make your applications fault tolerant.

### 3 types of load balancers

- Application Load Balancer
  - Best suited for load balancing of HTTP and HTTPS traffic
    - Route traffic to targets based on content of the request
    - Support for one or more listeners
    - Support for HTTP/2 and WebSocket
    - OSI Layer 7 - Application Layer

- Network Load Balancer
    - Best suited for load balancing of TCP traffic where extreme performance is required
        - Handle millions of requests per second
        - Support for static IP or Elastic IP addresses
        - Support for TCP, TLS, and UDP
        - OSI Layer 4 - Transport Layer
- Classic Load Balancer
    - Legacy Elastic Load Balancer
    - Support for EC2-Classic
    - Application layer and network layer load balancing
