# Week 9 Presentation and Research DevOps

#### Bastion servers

- A bastion host is a special purpose computer on a network specifically designed and configured to withstand attacks.
- In the context of SSH for AWS, a bastion host is a server instance itself that you must SSH into before you are able to SSH into any of the other servers in your VPC.

#### Terraform modules

- A module is a container for multiple resources that are used together. Every Terraform configuration has at least one module, know as its root module, which consists of the resources defined in the .tf files in the main working directory.  
- Allow you to better organise your configuration code and make the code reusable.

#### DNS and Route53

- The <b>Domain Name System (DNS)</b> is the phonebook of the Internet. DNS translates domain names to IP addresses so browsers can load Internet resources.
- Amazon <b>Route53</b> is a highly available and scalable cloud DNS web service. It designed to give developers and businesses an extremely reliable and cost effective way to route end users to end to Internet applications by translating names like:
```
 www.example.com into numeric IP addresses like 192.0.2.1
```
 that computers use to connect to each other.

#### Load Balancing and Autoscaling and Honey pots

- <b>Load Balancer</b> is a device that acts as a reverse proxy and distributes network or application traffic across a number of servers. Load balancers are used to increase capacity (concurrent users) and reliability of applications.
- Automatically increase the size of your <b>Auto Scaling</b> group when demand goes up and decrease it when demand goes down.
- As capacity is increased or decreased, the Amazon EC2 instances being added or removed must be registered or deregistered with a <b>load balancer.</b>
- A <b>honey pot</b> is a computer security mechanism set to detect, deflect, or, in some manner, counteract attempts at unauthorised use of information systems.

#### Docker and Containerisation

- <b>Docker</b> is a <b>containerisation</b> platform that packages your application and all its dependencies together in the form of a docker container to ensure that your application works seamlessly in any environment.

#### Load balancing and N-tier & High availability

- N-tier architecture is a client-server architecture concept in software engineering where the presentation, processing and data management functions are both logically and physically separated.

![img](https://docs.microsoft.com/en-us/azure/architecture/guide/architecture-styles/images/n-tier-logical.svg)


#### DB replica sets

- What is it?
  - A group of mongod processes that maintain the same data set.
- Where is it?
  - MongoDB
- What are the mechanics of this?
  - Provide redundancy and hgh availability, are the basis for all production deployments.

#### Blue-Green deployments

- Blue-green deployment is a technique that reduces downtime and risk by running two identical production environments called <b>Blue</b> and <b>Green</b>.
- At any time, only one of the environments is live, with the live environment serving all production traffic. For this example, Blue is currently live and Green is idle.

#### What is ELK Stack?

https://www.elastic.co/what-is/elk-stack

```
E - Elasticsearch (A search and analytic engine)
L - Logstash (A server-side data processing pipeline that ingests data from multiple sources instantaneously, transforms it, and then sends it to "stash" like Elasticsearch)
K - Kibana (Lets users visualise data with charts and graphs in Elasticsearch)
```
## Security:

```
  - at a network level (network security is any activity designed to protect that usability and integrity of your network and data)
  - IP lists to block (https://zeltser.com/malicious-ip-blocklists/)
  - Blocking DDos attack (Distributed denial of swervice. The primary purpose of a DDoS attack is to simply overwhelm your web server and either cripple it or take it down)
  - Honey pots (counteract attempts at unauthorized use of information systems)
  - SQL injection? (SQL injection is a code injection technique that might destroy your database. SQL injection is one of the most common web hacking techniques.)
  - SQL injection protection? (https://www.hacksplaining.com/prevention/sql-injection)
```
