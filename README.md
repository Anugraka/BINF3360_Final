# BINF3360_Final
Motif Discovery Benchmarking Project

This project compares four motif discovery methods: Greedy Motif Search, Randomized Motif Search, Gibbs Sampling, and an Entropy-Based Position Projection (EPP) method using DNA sequences from gene expression data in multiple sclerosis (MS). The goal is to compare how deterministic and stochastic methods perform in terms of motif quality, sequence similarity, and computation time.

Dataset: The dataset is derived from GEO dataset GSE135511 and processed using GEO2R differential expression analysis. Genes were filtered based on statistical significance and functional similarity (protein binding category via STRING). Corresponding DNA sequences were used as input for motif discovery.

Methods: All algorithms were run on the same input sequences with a fixed motif length (k = 9). Gibbs Sampling used 1000 iterations. Each method produced a set of predicted motifs for comparison.

Evaluation: Algorithms were compared using likelihood scores from a combined profile matrix, hamming distance to a consensus motif, pairwise Hamming distances between motifs, runtime, and memory usage.

Tools: Python, NumPy, Pandas, Matplotlib, Memory Profiler
