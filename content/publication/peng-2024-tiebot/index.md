---
title: 'TieBot: Learning to Knot a Tie from Visual Demonstration through a Real-to-Sim-to-Real Approach'
authors:
- admin
- Jun Lv
- Yuwei Zeng
- Haonan Chen
- Siheng Zhao
- Jichen Sun
- Cewu Lu
- Lin Shao
date: 2024-11-06
publishDate: '2025-06-20T00:41:09.828583Z'
publication_types: ["paper-conference"]
featured: true
publication: '*Proceedings of The 8th Conference on Robot Learning (CoRL)*'
abstract: The tie-knotting task is highly challenging due to the tie’s high deformation
  and long-horizon manipulation actions. This work presents TieBot, a Real-to-Sim-to-Real
  learning from visual demonstration system for the robots to learn to knot a tie.
  We introduce the Hierarchical Feature Matching approach to estimate a sequence of
  tie’s meshes from the demonstration video. With these estimated meshes used as subgoals,
  we first learn a teacher policy using privileged information. Then, we learn a student
  policy with point cloud observation by imitating teacher policy. Lastly, our pipeline
  applies learned policy to real-world execution. We demonstrate the effectiveness
  of TieBot in simulation and the real world. In the real-world experiment, a dual-arm
  robot successfully knots a tie, achieving 50% success rate among 10 trials. Videos
  can be found on https://tiebots.github.io/.
summary: We develop a Real-to-Sim-to-Real approach that enables learning tie-knotting skills for robots.
tag:
- Learning from Human Demonstration
url_pdf: 'uploads/tiebot.pdf'
links:
- name: arXiv
  url: http://arxiv.org/abs/2407.03245
url_project: 'https://tiebots.github.io/'
---
