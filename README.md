# Web-Server-Infrastructure
Web Server infrastructure ready to be deployed in AWS.

## Infrastructure Components

Here I'm going to describe different components in our basic architecture.

### Network Components
As part of the Network we have the following components described in network.yml
* One VPC where all our components will be located.
* Three AZ to locate our subnets.
* Three Public Subnets, two of them are used to locate Load Balancer and Nat services for our servers. the other one is used for our jumpServer(server for debugginh purposes).
* Two Private Subnets to locate our ASG . This is done for security reasons.
* As part of the Network components we also define our route tables to specify public/private subnets.

### Compute Components
As part of the Network we have the following components described in server.yml
* Security Groups to associate our servers and load balancer.
* Load balancer to manage the traffic in our servers.
* Instance profile to manage permission in aws services for the servers.

## Infrastructure Diagram

![alt text](https://github.com/ederfduran/Web-Server-Infrastructure/blob/master/InfrastuctureDiagram.png?raw=true)
