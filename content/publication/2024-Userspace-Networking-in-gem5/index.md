---
title: "Userspace Networking in gem5"
date: 2024-06-23
publishDate: 2024-06-23
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
