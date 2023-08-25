# Distributed Web Infrastructure

![Alt](https://raw.githubusercontent.com/B3zaleel/0x09-web_infrastructure_design/main/1-distributed_web_infrastructure.jpg)

## Description

* For every additional element, why you are adding it?

A load balancer is a device that acts as a reverse proxy and distributes network or application traffic across a number of servers. Load balancers are used to increase the capacity (concurrent users) and reliability of applications. 

* What distribution algorithm your load balancer is configured with and how it work ?

The HAProxy load balancer is configured with the Round Robin distribution algorithm. 
works by using each server behind the load balancer in turns, according to their weights. It’s also probably the smoothest and most fair algorithm as the servers’ processing time stays equally distributed. As a dynamic algorithm, Round Robin allows server weights to be adjusted on the go.

* Is your load-balancer enabling an Active-Active or Active-Passive setup, explain the difference between both ?

The HAProxy load-balancer is enabling an Active-Passive setup rather than an Active-Active setup. In an Active-Active setup, the load balancer distributes workloads across all nodes in order to prevent any single node from getting overloaded. Because there are more nodes available to serve, there will also be a marked improvement in throughput and response times. On the other hand, in an Active-Passive setup, not all nodes are going to be active (capable of receiving workloads at all times). In the case of two nodes, for example, if the first node is already active, the second node must be passive or on standby. The second or the next passive node can become an active node if the preceding node is inactive.

* How a database Primary-Replica (Master-Slave) cluster works ?

A Primary-Replica setup configures one server to act as the Primary server and the other server to act as a Replica of the Primary server. However, the Primary server is capable of performing read/write requests whilst the Replica server is only capable of performing read requests. Data is synchronized between the Primary and Replica servers whenever the Primary server executes a write operation.

* What is the difference between the Primary node and the Replica node in regard to the application ?

The Primary node is responsible for all the write operations the site needs whilst the Replica node is capable of processing read operations, which decreases the read traffic to the Primary node.
