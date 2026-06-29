# Extending Graph Network Simulators for Particle-Based Simulations of Transient Flow Problems
[The Journal of Computational Science](https://www.scimagojr.com/journalsearch.php?q=19700174607&tip=sid)

## Paper Status
**Status:** [Accepted](https://www.sciencedirect.com/science/article/pii/S1877750326001493)

**Paper Url:**  [https://doi.org/10.1016/j.jocs.2026.102931](https://doi.org/10.1016/j.jocs.2026.102931)


> **Note:** This paper is now available online.

## Citation

If you find this work useful, please cite the preprint:

```bibtex
@article{DHARMA2026102931,
title = {Extending graph network simulators for particle-based simulations of transient flow problems},
journal = {Journal of Computational Science},
pages = {102931},
year = {2026},
issn = {1877-7503},
doi = {https://doi.org/10.1016/j.jocs.2026.102931},
url = {https://www.sciencedirect.com/science/article/pii/S1877750326001493},
author = {Dody Dharma and Peter K. Jimack and He Wang},
keywords = {Fluid dynamics, Surrogate model, Graph network simulator, Self-supervised learning, Graph attention operator, Vorticity conservation},
abstract = {We extend the Graph Network Simulator (GNS) framework for transient flow problems by treating its processor layer as a tunable design axis. On a common training harness — a six-component physics-informed loss covering acceleration, velocity, position, density, divergence, and vorticity, with dual acceleration/velocity prediction and distributed training with mini-batch noise injection — we evaluate two complementary processor instantiations against vanilla GNS and a non-graph external baseline (the full SFBC pipeline): GNS with the Self-Supervised Graph Attention Operator (GNS-SSGAT), and GNS with a Fourier Basis Convolution layer adapted from SFBC (GNS-FBC). Across two-dimensional lid-driven cavity and curl-noise benchmarks we find that processor choice produces systematically different physical-fidelity profiles, with each instantiation dominating in a different physics regime: GNS-SSGAT achieves the lowest vorticity-field MSE and the highest Pearson correlation on a Material-Point-Method (MPM) semi-compressible regime, while GNS-FBC dominates vorticity-field MSE, Pearson correlation, KL divergence, and long-rollout particle-distribution stability on a harder FLIP/APIC incompressible-liquid regime. Both clearly outperform vanilla GNS and the external SFBC baseline on their respective target regimes, and together they characterise the processor layer as a useful design axis for accurate and stable surrogate modelling of transient flow problems.}
}
```

## About

This repository contains the code for the vorticity network — a graph network-based surrogate model for vorticity conservation in particle-based simulations of transient flow problems.
