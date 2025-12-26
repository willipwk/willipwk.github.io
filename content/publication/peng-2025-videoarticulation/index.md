---
title: "iTACO: Interactable Digital Twins of Articulated Objects from Casually Captured RGBD Videos"
authors:
- admin
- Jun Lv
- Cewu Lu
- Manolis Savva
author_links:
- https://willipwk.github.io/
- https://lyuj1998.github.io/
- https://www.mvig.org/
- https://msavva.github.io/
date: '2025-06-10'
publishDate: '2025-06-20T00:41:09.836157Z'
publication_types: ["paper-conference"]
featured: true
publication: "3DV 2026"
abstract: "Articulated objects are prevalent in daily life. Interactable digital twins of such objects have numerous applications in embodied AI and robotics. Unfortunately, current methods to digitize articulated real-world objects require carefully captured data, preventing practical, scalable, and generalizable acquisition. We focus on motion analysis and part-level segmentation of an articulated object from a casually captured RGBD video shot with a hand-held camera. A casually captured video of an interaction with an articulated object is easy to obtain at scale using smartphones. However, this setting is challenging due to simultaneous object and camera motion and significant occlusions as the person interacts with the object. To tackle these challenges, we introduce iTACO: a coarse-to-fine framework that infers joint parameters and segments movable parts of the object from a dynamic RGBD video. To evaluate our method under this new setting, we build a dataset of 784 videos containing 284 objects across 11 categories that is 20 larger than available in prior work. We then compare our approach with existing methods that also take video as input. Our experiments show that iTACO outperforms existing articulated object digital twin methods on both synthetic and real casually captured RGBD videos."

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
