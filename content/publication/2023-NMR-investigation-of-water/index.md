---
title: "Profiling gem5 Simulator"
date: 2023-06-23
publishDate: 2023-06-23
authors: ["**Johnson Umeike**", "Neel Patel", "Alex Manley", "Amin Mamandipoor", "Heechul Yun", "Mohammad Alian"]
publication_types: ["2"]
abstract: "In this work, we set out to find the answers to the following questions: (1) Where are the bottlenecks in a state-of-the-art architectural simulator? (2) How much faster can architectural simulations run by tuning system configurations? (3) What are the opportunities in accelerating software simulation using hardware accelerators? We choose gem5 as the representative architectural simulator, run several simulations with various configurations, perform a detailed architectural analysis of the gem5 source code on different server platforms, tune both system and architectural settings for running simulations, and discuss the future opportunities in accelerating gem5 as an important application. Our detailed profiling of gem5 reveals that its performance is extremely sensitive to the size of the L1 cache. Our experimental results show that a RISC-V core with 32KB data and instruction cache improves gem5’s simulation speed by 31%∼61% compared with a baseline core with 8KB L1 caches. Our paper is the first step toward building specialized hardware and software environments for accelerating software-based simulators."
featured: true
publication: "ISPASS"
links:
  - icon_pack: fas
    icon: scroll
    name: Link
    url: 'https://ieeexplore.ieee.org/document/1015820'
---
