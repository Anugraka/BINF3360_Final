# BINF3360_Final
Motif Discovery Benchmarking Project

This project compares four motif discovery algorithms—Greedy Motif Search, Randomized Motif Search, Gibbs Sampling, and an Entropy-Based Position Projection (EPP) algorithm—using gene expression–derived DNA sequences from multiple sclerosis (MS) data. The goal is to evaluate differences between deterministic and stochastic approaches in terms of motif quality, sequence similarity, and computational performance.

Dataset: The dataset is derived from GEO dataset GSE135511 and processed using GEO2R differential expression analysis. Genes were filtered based on statistical significance and functional similarity (protein binding category via STRING). Corresponding DNA sequences were used as input for motif discovery.

Methods: All algorithms were run on the same input sequences with a fixed motif length (k = 9). Gibbs Sampling used 1000 iterations. Each method produced a set of predicted motifs for comparison.

Evaluation: Algorithms were compared using likelihood scores from a combined profile matrix, hamming distance to a consensus motif, pairwise Hamming distances between motifs, runtime, and memory usage.

Tools: Python, NumPy, Pandas, Matplotlib, Memory Profiler
