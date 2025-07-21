---
title: 'Thesis'
date: 2025-07-04
type: post

design:
  spacing: '5rem'

# Note: `username` refers to the user's folder name in `content/authors/`
---

# PhD Thesis: Untangling Neural Networks

In this thesis, we \`\`untangle'' neural networks, in a broad and metaphorical sense of the word: uncovering the implicit inductive biases imposed on them during training and adapting neural networks to make them more controllable. We aim to advance the science of deep learning, so that we expand our knowledge and understanding of deep learning’s inductive biases and of levers on neural networks’ size and representations in general.

Find my thesis here: 

## Understanding Redundancy in Neural Networks

In Chapter4 we demonstrate that for our feed-forward models and tasks, as the model architecture increases in size, the absolute number of unprunable parameters increases, but the proportion of unprunable parameters is relatively stable. In other words, if we keep a task constant, but increase the architecture size, the network uses up more parameters to implement a solution. This means that the proportion of redundant parameters is relatively fixed, regardless of architecture size. We find that neural networks may have an implicit inductive bias towards density. See [The Propensity for Density in Feed-forward Models](https://arxiv.org/abs/2410.14461).

Additionally, Appendix A presents an evolutionary algorithm, Neuroevolutionary Ticket Search (NeTS), which finds efficient subnetworks in feed-forward or convolutional DNN architectures,  
by learning a mask and network parameters in tandem. This means that redundant parameters are already identified during training. See [Finding Sparse Initialisations using Neuroevolutionary Ticket Search (NeTS)](https://direct.mit.edu/isal/proceedings/isal2023/35/110/116859).

## Redundant and Harmful Parameters

In Chapter 5 we investigate the effects of removing bits from binary intermediate representations on out-of-distribution performance in a model trained to solve an unsupervised task. Our approach starts from the intuition that for high-entropy features in a model's training distribution, it will have learned a more robust understanding for when the feature is relevant. We find that the generalizability (to performance on out-of-distribution data) of neural networks can be enhanced by eliminating low entropy neurons. See [Low-Entropy Latent Variables Hurt Out-of-Distribution Performance](https://arxiv.org/abs/2305.12238).

Additionally, Appendix C introduces a machine unlearning method that removes neurons based on their importance for a targeted capability relative to their importance for general network performance. Our findings reveal that both feed-forward and attention neurons in LLMs are specialized; that is, for specific tasks, certain neurons are more crucial than others. Neurons that are specialized to do well on dangerous tasks (such as coding or generating toxic text) can be removed to improve the overall safety of a model. See [Dissecting Language Models: Machine Unlearning via Selective Pruning](https://arxiv.org/abs/2403.01267).

## Translating a Neural Network Into a More Interpretable Architecture

In Chapter 6 and Appendix E we translate a neural network into a different representation that provides a functionally equivalent implementation.

In Chapter 6 we show that for every ReLU network there exists a functionally equivalent KAN, and vice versa. KANs are more difficult to train, but more interpretable. Our translation method sheds light on the relationship between well studied ReLU networks and KANs. See [Relating Piecewise Linear Kolmogorov Arnold Networks to ReLU Networks](https://arxiv.org/abs/2503.01702).

Additionally, Appendix E provides a method for rewriting a deep ReLU network as a functionally identical three-layer network with weights valued in the extended reals. This shallow network is a white-box model in that for every parameter we know what role it serves. In other words, we ReLU networks can be translated to more interpretable representations that are functionally equivalent. See [Any Deep ReLU Network is Shallow](https://arxiv.org/abs/2306.11827).

