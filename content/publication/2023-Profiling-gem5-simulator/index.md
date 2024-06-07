---
title: "Profiling gem5 Simulator"
date: 2023-06-23
publishDate: 2023-06-23
authors: ["**Johnson Umeike**", "Neel Patel", "Alex Manley", "Amin Mamandipoor", "Heechul Yun", "Mohammad Alian"]
publication_types: ["1"]
abstract: "In this work, we set out to find the answers to the following questions: (1) Where are the bottlenecks in a state-of-the-art architectural simulator? (2) How much faster can architectural simulations run by tuning system configurations? (3) What are the opportunities in accelerating software simulation using hardware accelerators? We choose gem5 as the representative architectural simulator, run several simulations with various configurations, perform a detailed architectural analysis of the gem5 source code on different server platforms, tune both system and architectural settings for running simulations, and discuss the future opportunities in accelerating gem5 as an important application. Our detailed profiling of gem5 reveals that its performance is extremely sensitive to the size of the L1 cache. Our experimental results show that a RISC-V core with 32KB data and instruction cache improves gem5’s simulation speed by 31%∼61% compared with a baseline core with 8KB L1 caches. Our paper is the first step toward building specialized hardware and software environments for accelerating software-based simulators."
featured: true
publication: "ISPASS 23'"
links:
  - icon_pack: fas
    icon: scroll
    name: Link
    url: 'https://ieeexplore.ieee.org/document/10158201'
---
title: "Profiling gem5 Simulator"
date: 2023-06-23
publishDate: 2023-06-23
authors: ["**Johnson Umeike**", "Siddharth Agarwal", "Nikita Lazarev", "Mohammad Alian"]
publication_types: ["1"]
abstract: "Full-system simulation of computer systems is critical for capturing the complex interplay between various hardware and software components in future systems. Modeling the
network subsystem is indispensable for the fidelity of full-system simulations due to the increasing importance of scale-out systems. Over the last decade, the network software stack has undergone major changes, with userspace networking stacks and dataplane networks rapidly replacing the conventional kernel network stack. Nevertheless, the current state-of-the-art architectural simulator, gem5, still employs kernel networking, which precludes realistic network application scenarios. In this work, we first demonstrate the limitations of gem5’s current network stack in achieving high network bandwidth. Then, we enable a userspace networking stack on gem5. We extend gem5’s NIC hardware model and device driver to support userspace device drivers running the DPDK framework. Additionally, we implement a network load generator hardware model in gem5 to generate various traffic patterns and perform per-packet timestamp and latency measurements without introducing packet loss. We develop a suite of six network-intensive benchmarks for stress testing the host network stack. These applications, based on DPDK, can run on both gem5 and real systems. Our experimental results show that enabling userspace networking improves gem5’s network bandwidth by 6.3× compared with the current Linux kernel software stack. We characterize the performance of DPDK benchmarks running on both a real system and gem5, and evaluate the sensitivity of the applications to various system and microarchitecture parameters. This work marks the first step in refactoring the networking subsystem in gem5."
featured: true
publication: "ISPASS 24'"
links:
  - icon_pack: fas
    icon: scroll
    name: Link
    url: 'https://ieeexplore.ieee.org/document/10158201'
---
