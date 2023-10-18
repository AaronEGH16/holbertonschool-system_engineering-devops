# Distributed web infrastructure:

![Example of Distributed Infrastructure](https://github.com/AaronEGH16/holbertonschool-system_engineering-devops/blob/main/web_infrastructure_design/1-distributed_web:infrastructure.jpg)

## Infrastructure Explanation

### Load Balancer:
Added to distribute traffic load across multiple servers, ensuring efficient resource utilization and improving availability.
### Distribution Algorithm:
The load balancer is configured with a weighted distribution algorithm to allocate load based on the capacity of the servers, thus optimizing performance.
### Load Balancer Configuration:
It has been configured to allow an Active-Active environment, where all servers are active and responding to traffic, improving availability and recoverability.
### Primary-Replica Database Cluster:
Implemented to improve redundancy and fault tolerance. The primary node handles write operations, while the secondary nodes (replicas) are used for read operations, thus distributing the load.
### Difference between Primary and Replica node:
The primary node is responsible for write and update operations while the replica nodes are used for read operations. This improves the performance and scalability of the system.

## Problems with Infrastructure

### Single Points of Failure (SPOF):
It is not specified how SPOFs are addressed. To improve availability, it is essential to identify and eliminate any single point of failure that could disrupt system operation.
### Security Problems:
The lack of firewall and the absence of HTTPS represent security problems. A firewall is crucial to control and monitor traffic, and HTTPS encrypts communication to protect data during transfer.
### Lack of Monitoring:
The lack of monitoring tools makes it difficult to identify and quickly resolve problems. Implementing a monitoring system is essential to monitor performance, detect potential problems, and ensure system integrity.