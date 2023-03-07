# *Intro to Distributed Systems*

Have you ever wondered how distributed systems work? Do you want to learn how to write code that spans multiple systems reliably without data loss, while staying performant? Then say no more - we'll be running an crash course where we'll be building highly available distributed system components together in a local environment on our laptops.

This course will span 2 weeks, meet 3 times a week, 2 hours per day. At the end of each week, we'll build and deeply understand a component in a simulated distributed system with full end to end testing. The course components we will be building will be modeled after [FlyIO Gossip Columns](https://fly.io/dist-sys/). 

Sessions will be held in-person at the office. Join [slack] #distributed-systems-learning if you're interested
in attending - schedules/details will be posted there.

## *Course Prerequisites*:
1. Golang programming knowledge
2. Fundamental Systems Knowledge (networking, concurrency, filesystems, locks)


## Goals:
1. Understand and apply concepts around reliability, consistency, and availability in a distributed system.
2. Learn to debug and root cause common distributed system failures.


## *What is unique about this course?
Students will gain *hands on experience with distributed systems*. Students will participate in the design,
implementation, assembly, configuration, benchmarking, and tests of a simulated distributed system
on their local machine. Students will learn how to evaluate and make trade-offs in distributed systems
and understand the effects of network failures and message loss, and ways to mitigate these scenarios.

## *What happens after finishing this course?
Congrats! You're a systems expert now (not). Jokes aside, this course is simply a brief intro to the fascinating
but complex world of distributed systems. Hopefully this course has piqued your curiousity. After this
course, we'll aim to continue this series once every 2 weeks, where we will actually dive into popular
distributed system recipes, tools, and frameworks used in production environments (e.g. Kafka, Consul, Vitess, Apache *insert popular project here*), and understand
when to apply these systems to real world applications. Stay tuned!

### *Week 1: Foundations of a distributed system
1. Setup dev environment (pre-requisites e.g. golang, jdk/jre, graphviz)
2. Understanding consistency, availability, and partition tolerance.
3. Intro to maelstrom workbench for learning distributed systems.
    a. Protocol for data transfer
    b. Generating test workloads
    c. Interpreting tests
    d. Intro to maelstrom's Golang API for building nodes in a distributed system
4. Building a simple echo server
5. Building a global unique id generator

By the end of this week, students will learn how to intrepret data loss, latency, and availability,
and also implement simple systems in Golang with maelstrom's Node API.

### *Week 2: Building a gossip-based broadcast system (used in p2p apps, service discovery, etc.)
1. Implementing a single node broadcast system that's able to gossip messages across all nodes in a cluster.
2. Improving the broadcast system to become a distributed implementation that allows replication of messages across a cluster with no network partitions.
3. Adding fault tolerance onto previous implementation - meaning it can work even with network partitions between cluster nodes.
4. Implement a data efficient mechanism to reduce network traffic. We'll need to make tradeoffs between efficiency and latency.

At the end of the second week, we've applied concepts around scalable, reliable, performant data replication, by implementing the gossip protocol.
