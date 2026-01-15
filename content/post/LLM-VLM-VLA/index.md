---
title: Why VLM and VLA are less powerful than LLM at present? 
summary: An interesting thought from the perspective of turing machine
date: 2025-12-25
authors:
  - admin
tags:
  - Thoughts
image:
  caption: 'Image generated from GPT'
---

This post comes from an interesting discussion with one of my friends. We were discussing why VLM currently still make a lot of mistakes, while LLM could give more accurate answers.

Here I consider a VLM is a model that takes in images / videos and text prompt, and outputs text or images / videos. So models that solve text-guided vision tasks are also considered as VLM, such as SAM3, GroundingDINO, etc.

### Data?

Data may be the answer we come up with at the first time. True, there may not be that many text-image pairs data to do pre-training or post-finetuning. I take a look at the tech report of Qwen3-VL. Here are two findings:
1. Associated tasks are kind of limited actually. Training data are associated with these tasks: image captioning, OCR, box-based and point-based grounding, counting, 3D VQA, 3D grounding, coding (like writing HTML or CSS), video captioning, video grounding, GUI understanding. All these tasks can be categorized into two types: question answer and grounding. But we know that there are much more diverse tasks beyond this collection, such as segmentation, tracking, image manipulation, etc. 
2. The amount of data is indeed uncomparable to LLM. VQA data is relatively abundant. OmniCorpus provides billions level of image-text data for VQA and image captioning. However, for grounding tasks, current dataset remains at millions level or even smaller. This evidence may answer why VLM tends to work better on captioning or VQA, comparing to grounding tasks.

For VLA, unfortunately, I haven't seen any billions level text-image-action dataset.

The following question is, if we scale up the amount of data, will VLM be as powerful as LLM? And how much data we need?

### A Computation Theory Perspective

Here I want to diverge a bit to talk about Turing Machine. We know that Turing Machine is the math model of computation. Everything runs on computers do not go beyond Turing Machine, so does VLM. Turing machine models computation as manipulation on a set of symbols. On our actual hardware, it is basically 0 and 1. Unfortunately, not all computable problem has polynomial-time algorithm. So we need some efficient approximate algorithms.

We can think natural language problem as manipulating language symbols. What I feel is, LLM is the approximate algorithm we find to solve natural language problem, by optimizing billions of parameters from numerous text data. And we find the function of mapping between of sets of language symbols.

How about VLM? We not only have language symbols, but also symbols for visual data. Let's consider symbols for visual data as RGB pixels. There are in total 256x256x256=2^24 different symbols. Now we want to find an approxiamte function of mapping two sets of language+visual symbols. I am afraid the desired function will be much more complex than just mapping between two sets of language symbols. 

I won't deny that neural network is extremely powerful that it can almost approximate any function we want. But we have to consider the effort of getting the desired function. If we simply consider LLM memorizes every text prompt and answer, the effort we need is almost all available text on the Internet. For VLM, the effort may be all available text plus visual data, which is far more larger than any dataset currently available.  

People may argue that for VLM we do not always need pixel level accuracy. So we can somehow reduce the size of the set of image symbols. Yes I agree. We human can infer correct message from incomplete or erroneous text or image, due to the information redundancy. But what if the user is a robot instead of human? 

The symbol set for VLA would be even larger than VLM. Now we need to add action symbols. What's worse, the user is a robot instead of human. At present, robots are not that robust when handling inaccurate input. When VLA outputs "move straightforward 1cm" but actually requiring to move 2cm to reach the goal, robots will move 1cm faithfully. Thus, I'm afraid the amount of data of finding a generalized VLA model for any action would beyond our imagination.

### Moravec's Paradox

Finally, I want to talk a bit more on Moravec's Paradox:
> it is comparatively easy to make computers exhibit adult level performance on intelligence tests or playing checkers, and difficult or impossible to give them the skills of a one-year-old when it comes to perception and mobility

If we take the perspective of turing machine, we may get some intuition of Moravec's Paradox. We human summarizes knowledge from real world into a compact set of symbols, which is language. But once we try to incoporate richer and low-level observation from real world such as visual data and action data, the set of symbol grows exponentially. As a consequence, the computation problem becomes much harder, and requires much larger amounts of data to find approximate algorithm to solve it.

Thanks for reading this blog post. These are some of my very high level thoughts and do not garuantee mathematically correctness.