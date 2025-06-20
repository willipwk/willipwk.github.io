---
title: ManiFoundation Model for General-Purpose Robotic Manipulation of Contact Synthesis with Arbitrary Objects and Robots
authors:
- Zhixuan Xu
- Chongkai Gao
- Zixuan Liu
- Gang Yang
- Chenrui Tie
- Haozhuo Zheng
- Haoyu Zhou
- Weikun Peng
- Debang Wang
- Tianrun Hu
- Tianyi Chen
- Zhouliang Yu
- Lin Shao
date: '2024-10-14'
publishDate: '2025-06-20T00:41:09.821734Z'
publication_types: ["paper-conference"]
publication: '*2024 IEEE/RSJ International Conference on Intelligent Robots and Systems
  (IROS)*'
doi: 10.1109/IROS58592.2024.10801782
tags:
- Point cloud compression
- Foundation models
- Manipulators
- Distance measurement
- Robots
- Intelligent robots

abstract: To substantially enhance robot intelligence, there is a pressing need to develop a large model that enables general-purpose robots to proficiently undertake a broad spectrum of manipulation tasks, akin to the versatile task-planning ability exhibited by LLMs. The vast diversity in objects, robots, and manipulation tasks presents huge challenges. Our work introduces a comprehensive framework to develop a foundation model for general robotic manipulation that formalizes a manipulation task as contact synthesis. Specifically, our model takes as input object and robot manipulator point clouds, object physical attributes, target motions, and manipulation region masks. It outputs contact points on the object and associated contact forces or post-contact motions for robots to achieve the desired manipulation task. We perform extensive experiments both in the simulation and real-world settings, manipulating articulated rigid, rigid, and deformable objects that vary in dimensionality, ranging from one-dimensional objects like ropes to two-dimensional objects like cloth and extending to three-dimensional objects such as plasticine. Our model achieves average success rates of around 90%.

summary: We develop a foundation model on robotic manipulation via modeling contact points on the object.

links:
  - name: PDF
    url: uploads/manifoundation.pdf
  - name: arXiv
    url: https://arxiv.org/abs/2405.06964
  - name: Website
    url: https://manifoundationmodel.github.io/
  - name: Code
    url: https://github.com/NUS-LinS-Lab/ManiFM
---
