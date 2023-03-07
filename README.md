Intro to Distributed System Patterns

Have you ever wondered how distributed systems work? Do you want to learn how to write code that spans multiple systems reliably without data loss, while staying performant? Then say no more - we'll be running an crash course where we'll be building highly available distributed system components together in a local environment on our laptops.

This course will span 2 weeks, meet 3 times a week, 2 hours per day. At the end of each week, we'll build and deeply understand a component in a simulated distributed system with full end to end testing. The course components we will be building will be modeled after https://fly.io/dist-sys/. Please react to this message if you're interested in attending this learning series (tentatively starting 2 weeks from now) so that I can guage how much interest there is.

Course Prerequisites:
-Golang programming knowledge
-Fundamental Systems Knowledge (networking, concurrency, filesystems, locks)

Goals:
1. Understand and apply key concepts around reliability, consistency, and availability in a distributed system.
2. Learn to debug and root cause common distributed system failures.

What is unique about this course?
Students will gain *hands on experience with distributed systems*. Students will participate in the design,
implementation, assembly, configuration, benchmarking, and tests of a simulated distributed system
on their local machine. Students will deeply learn how to evaluate and make trade-offs in distributed systems
and understand the effects of network failures and message loss, and ways to mitigate these scenarios.

Week 1: Foundations of a distributed system
1. Setup dev environment (pre-requisites e.g. golang, jdk/jre, graphviz)
2. Understanding CAP theorem (consistency, availability, partition tolerance)
3. Intro to maelstrom workbench for learning distributed systems.
  a. Protocol for data transfer
  b. Generating test workloads
  c. Interpreting tests
  d. Built in services (e.g. network, data stores) that can be used for building complex distributed systems
4. Building a simple echo server
5. Building a global unique id generator

By the end of this week, students will learn how to load test, run logical tests,

Week 2: Building a gossip-based broadcast system
This week we'll learn how data can be replicated in a scalable, reliable, simple way, by implementing the gossip protocol.
1. Implementing a single node broadcast system that's able to gossip messages across all nodes in a cluster.
2. Improving the broadcast system to become a distributed implementation that allows replication of messages across a cluster with no network partitions.
3. Adding fault tolerance onto previous implementation - meaning it can work even with network partitions between cluster nodes.
