---
title: "Counterfactual experience augmented off-policy reinforcement learning"
collection: publications
category: manuscripts
permalink: /publication/cea
# excerpt: ''
date: 2025-07-07
venue: 'Neurocomputing'
# slidesurl: 'https://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://www.sciencedirect.com/science/article/abs/pii/S0925231225006897'
bibtexurl: 'https://bowen1911.github.io/files/cea.bib'
citation: 'Lee S, Gong Y, Deng C. Counterfactual experience augmented off-policy reinforcement learning[J]. Neurocomputing, 2025, 637: 130017.'
---
Reinforcement learning control algorithms face significant challenges due to out-of-distribution and inefficient exploration problems. While model-based reinforcement learning enhances the agent’s reasoning and planning capabilities by constructing virtual environments, training such virtual environments can be very complex. In order to build an efficient inference model and enhance the representativeness of learning data, we propose the Counterfactual Experience Augmentation (CEA) algorithm. CEA leverages variational autoencoders to model the dynamic patterns of state transitions and introduces randomness to model non-stationarity. This approach focuses on expanding the learning data in the experience pool through counterfactual inference and performs exceptionally well in environments that follow the bisimulation assumption. Environments with bisimulation properties are usually represented by discrete observation and action spaces, we propose a sampling method based on maximum kernel density estimation entropy to extend CEA to various environments. By providing reward signals for counterfactual state transitions based on real information, CEA constructs a complete counterfactual experience to alleviate the out-of-distribution problem of the learning data, and outperforms general SOTA algorithms in environments with difference properties. Finally, we discuss the similarities, differences and properties of generated counterfactual experiences and real experiences. The code is available at [https://github.com/Aegis1863/CEA](https://github.com/Aegis1863/CEA).
