# Generalization in GNNs: How Much Data Is Enough?
This project investigates a fundamental question in machine learning with graph neural networks (GNNs): How much training data is enough for GNNs to generalize well? We combine theoretical insights from learning theory with empirical experiments on real-world graph datasets to understand this relationship.

## Overview
Graph Neural Networks have shown strong performance across domains like molecular biology, social networks, and recommender systems. But unlike standard neural networks, how GNNs generalize with varying amounts of data is still poorly understood.

This project explores:

1. Theoretical bounds on data requirements using the VC dimension of GNNs

2. Empirical validation on six benchmark graph datasets

3. Surprising findings about when additional data stops being useful (i.e., saturation points)

## Key Takeaways
1. GNNs have sample complexity bounds that help predict when additional data will meaningfully improve generalization.

2. Models often saturate early—they generalize well with surprisingly little data on some datasets.

3. However, larger datasets don’t always guarantee better generalization without considering the graph structure and composition.

## Methods
We apply results from PAC learning and VC dimension theory to derive data efficiency bounds for GNNs. We run experiments on 6 public datasets (e.g., ENZYMES, NCI1, MCF-7) with controlled model complexity. We train GNNs using fixed architectures and measure generalization gaps across increasing data sizes.

The code is adapted from [Morris et al. (2023)](https://arxiv.org/abs/2301.11039).
