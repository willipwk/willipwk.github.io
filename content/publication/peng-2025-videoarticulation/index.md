---
title: Generalizable Articulated Object Reconstruction from Casually Captured RGBD
  Videos
authors:
- Weikun Peng
- Jun Lv
- Cewu Lu
- Manolis Savva
date: '2025-06-10'
publishDate: '2025-06-20T00:41:09.836157Z'
publication_types: ["article"]
publication: "arXiv"
abstract: Articulated objects are prevalent in daily life. Understanding their kinematic structure and reconstructing them have numerous applications in embodied AI and robotics. However, current methods require carefully captured data for training or inference, preventing practical, scalable, and generalizable reconstruction of articulated objects. We focus on reconstruction of an articulated object from a casually captured RGBD video shot with a hand-held camera. A casually captured video of an interaction with an articulated object is easy to acquire at scale using smartphones. However, this setting is quite challenging, as the object and camera move simultaneously and there are significant occlusions as the person interacts with the object. To tackle these challenges, we introduce a coarse-to-fine framework that infers joint parameters and segments movable parts of the object from a dynamic RGBD video. To evaluate our method under this new setting, we build a 20× larger synthetic dataset of 784 videos containing 284 objects across 11 categories. We compare our approach with existing methods that also take video as input. Experiments show that our method can reconstruct synthetic and real articulated objects across different categories from dynamic RGBD videos, outperforming existing methods significantly.

summary: We develop a method that can reconstruct articulated objects from casually captured RGBD videos.

tags:
- Articulate Object Reconstruction
- Dynamic Scene Understanding
- Video Understanding

featured: true

url_pdf: 'uploads/video2articulation.pdf'
links:
- name: arXiv
  url: https://arxiv.org/abs/2506.08334
url_project: 'https://3dlg-hcvc.github.io/video2articulation/'
url_video: 'https://youtu.be/x32Hn9BjSV0'
url_code: 'https://github.com/3dlg-hcvc/video2articulation'
url_dataset: 'https://huggingface.co/datasets/3dlg-hcvc/video2articulation'
---
