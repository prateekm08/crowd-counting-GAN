# Crowd Counting using Conditional Generative Adversarial Networks

This is a complete implementation of a recent crowd counting paper titled  [An end-to-end generative adversarial network for crowd counting under complicated scenes](http://ieeexplore.ieee.org/document/7986133/).

## Misc. Info

1. To construct the ground truth density map, instructions from the [MCNN paper](http://ieeexplore.ieee.org/document/7780439/) are followed. 

2. All pixels are multiplied by 2550, a number decided empirically, before feeding the data to the Conditional GAN. This increases the L1 distance between density maps generated and zero valued tensors thus helping the model to converge much faster.
