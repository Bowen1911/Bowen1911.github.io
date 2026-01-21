---
title: "MacLight: Multi-scene Aggregation Convolutional Learning for Traffic Signal Control"
collection: publications
category: conferences
permalink: /publication/maclight
# excerpt: ''
date: 2025-07-07
venue: "AAMAS '25: Proceedings of the 24th International Conference on Autonomous Agents and Multiagent Systems"
# slidesurl: 'https://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://dl.acm.org/doi/epdf/10.5555/3709347.3743758'
bibtexurl: 'https://bowen1911.github.io/files/maclight.bib'
citation: 'Lee S, Lyu H, Gong Y, et al. MacLight: Multi-scene Aggregation Convolutional Learning for Traffic Signal Control[J]. arXiv preprint arXiv:2412.15703, 2024.'
---
Reinforcement learning methods have proposed promising traffic signal control policy that can be trained on large road networks. Current SOTA methods model road networks as topological graph structures, incorporate graph attention into deep Q-learning, and merge local and global embeddings to improve policy. However, graph-based methods are difficult to parallelize, resulting in huge time overhead. Moreover, none of the current peer studies have deployed dynamic traffic systems for experiments, which is far from the actual situation.
In this context, we propose Multi-Scene Aggregation Convolutional Learning for traffic signal control (MacLight), which offers faster training speeds and more stable performance. Our approach consists of two main components. The first is the global representation, where we utilize variational autoencoders to compactly compress and extract the global representation. The second component employs the proximal policy optimization algorithm as the backbone, allowing value evaluation to consider both local features and global embedding representations. This backbone model significantly reduces time overhead and ensures stability in policy updates. We validated our method across multiple traffic scenarios under both static and dynamic traffic systems. Experimental results demonstrate that, compared to general and domian SOTA methods, our approach achieves superior stability, optimized convergence levels and the highest time efficiency. The code is under [https://github.com/Aegis1863/MacLight](https://github.com/Aegis1863/MacLight).