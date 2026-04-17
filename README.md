# Awesome Optimizers List

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![GitHub stars](https://img.shields.io/github/stars/JiwenJ/Awesome-Optimzers?style=flat-square&logo=github)](https://github.com/JiwenJ/Awesome-Optimzers/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](./LICENSE)
[![Papers](https://img.shields.io/badge/Papers-217-b31b1b.svg?style=flat-square&logo=arxiv&logoColor=white)](./data/all_entries.csv)
[![Code Links](https://img.shields.io/badge/Code%20Links-34-2ea44f.svg?style=flat-square&logo=github)](./data/all_entries.csv)
[![Coverage](https://img.shields.io/badge/Years-2022--2026-6f42c1.svg?style=flat-square&logo=bookstack&logoColor=white)](./data/optimizers.csv)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/JiwenJ/Awesome-Optimzers/pulls)

Here is a curated list of modern optimizers and their corresponding papers, codebases, and practical advantages.

Current scope:

- Start from `2022`
- Order by time in reverse chronological order
- Focus on deep learning and LLM-related optimizers
- `GitHub` is optional; entries without a public implementation are still included

> Full catalog: [data/all_entries.csv](./data/all_entries.csv)
>
> Curated subset: [data/optimizers.csv](./data/optimizers.csv)
>
> Imported reference subset: [data/reference_catalog.csv](./data/reference_catalog.csv)
> The README table below includes all `217` current `2022+` entries directly, even when no public code link is available.

| Optimizer Name | Paper | Date | Notes |
| --- | --- | --- | --- |
| HomeAdam | [HomeAdam: Adam and AdamW Algorithms Sometimes Go Home to Obtain Better Provable Generalization](https://arxiv.org/abs/2603.02649) | 2026-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FlashOptim | [FlashOptim: Optimizers for Memory-Efficient Training](https://arxiv.org/abs/2602.23349) | 2026-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DP-aware AdaLN-Zero | [DP-aware AdaLN-Zero: Taming Conditioning-Induced Heavy-Tailed Gradients in Differentially Private Diffusion](https://arxiv.org/abs/2602.22610) | 2026-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Spectral Sphere Optimizer (SSO) <a href="https://github.com/Unakar/Spectral-Sphere-Optimizer"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Controlled LLM Training on Spectral Sphere](https://arxiv.org/abs/2601.08393) | 2026-01 | Enforces spectral constraints on both weights and updates, improving stability and outperforming AdamW and Muon in reported LLM pretraining runs. |
| Ringleader ASGD | [First Provably Optimal Asynchronous SGD for Homogeneous and Heterogeneous Data](https://arxiv.org/abs/2601.02523) | 2026-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| NOVAK | [NOVAK: Unified adaptive optimizer for deep neural networks](https://arxiv.org/abs/2601.07876) | 2026-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FANoS | [FANoS: Friction-Adaptive Nos´e–Hoover Symplectic Momentum for Stiff Objectives](https://arxiv.org/pdf/2601.00889) | 2026-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DP-λCGD | [DP-λCGD: Efficient Noise Correlation for Differentially Private Model Training](https://arxiv.org/abs/2601.22334) | 2026-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ROOT | [ROOT: Robust Orthogonalized Optimizer for Neural Network Training](https://arxiv.org/abs/2511.20626) | 2025-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| HVAdam | [HVAdam: A Full-Dimension Adaptive Optimizer](https://arxiv.org/abs/2511.20277) | 2025-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DP-MicroAdam | [DP-MicroAdam: Private and Frugal Algorithm for Training and Fine-tuning](https://arxiv.org/abs/2511.20509) | 2025-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DP-AdamW-BC | [DP-AdamW: Investigating Decoupled Weight Decay and Bias Correction in Private Deep Learning](https://arxiv.org/abs/2511.07843) | 2025-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdamNX | [AdamNX: An Adam improvement algorithm based on a novel exponential decay mechanism for the second-order moment estimate](https://arxiv.org/abs/2511.13465) | 2025-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FedMuon | [FedMuon: Accelerating Federated Learning with Matrix Orthogonalization](https://arxiv.org/abs/2510.27403) | 2025-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AuON | [AuON: A Linear-time Alternative to Orthogonal Momentum Updates](https://arxiv.org/abs/2509.24320) | 2025-09 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ZetA | [ZETA: A HYBRID OPTIMIZER COMBINING RIEMANN ZETA SCALING WITH ADAM FOR ROBUST DEEP LEARNING](https://arxiv.org/abs/2508.02719) | 2025-08 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| NIRMAL | [COMPARATIVE ANALYSIS OF NOVEL NIRMAL OPTIMIZER AGAINST ADAM AND SGD WITH MOMENTUM](https://arxiv.org/abs/2508.04293) | 2025-08 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DLAS-R-FTC | [Distributed Optimization and Learning for Automated Stepsize Selection with Finite Time Coordination](https://arxiv.org/abs/2508.05887) | 2025-08 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ZO-SAH | [Subspace-based Approximate Hessian Method for Zeroth-Order Optimization](https://arxiv.org/abs/2507.06125) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SoftSignSGD | [SoftSignSGD(S3): An Enhanced Optimizer for Practical DNN Training and Loss Spikes Minimization Beyond Adam](https://arxiv.org/abs/2507.06464) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SCSAdamW | [Beyond First-Order: Training LLMs with Stochastic Conjugate Subgradients and AdamW](https://arxiv.org/abs/2507.01241) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| S-BFGS | [EFFICIENT STOCHASTIC BFGS METHODS INSPIRED BY BAYESIAN PRINCIPLES](https://arxiv.org/abs/2507.07729) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| LyAm | [LyAm: Robust Non-Convex Optimization for Stable Learning in Noisy Environments](https://arxiv.org/abs/2507.11262) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DOME | [Communication Efficient, Differentially Private Distributed Optimization using Correlation-Aware Sketching](https://arxiv.org/abs/2507.03545) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DEO | [Dimer-Enhanced Optimization: A First-Order Approach to Escaping Saddle Points in Neural Network Training](https://arxiv.org/abs/2507.19968) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Deco-SGD | [DeCo-SGD: Joint Optimization of Delay Staleness and Gradient Compression Ratio for Distributed SGD](https://arxiv.org/abs/2507.17346) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| adaNPAG | [Boosting Accelerated Proximal Gradient Method with Adaptive Sampling for Stochastic Composite Optimization *](https://arxiv.org/abs/2507.18277) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdaMuon | [ADAMUON: ADAPTIVE MUON OPTIMIZER](https://arxiv.org/abs/2507.11005) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Accelerated GRAAL | [NESTEROV FINDS GRAAL: OPTIMAL AND ADAPTIVE GRADIENT METHOD FOR CONVEX OPTIMIZATION](https://arxiv.org/abs/2507.09823) | 2025-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| VR-SZD | [A Structured Proximal Stochastic Variance Reduced Zeroth-order Algorithm](https://arxiv.org/abs/2506.23758) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| TAH-QUANT | [TAH-QUANT: Effective Activation Quantization in Pipeline Parallelism over Slow Network](https://arxiv.org/abs/2506.01352) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SPlus <a href="https://github.com/kvfrans/splus"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [A Stable Whitening Optimizer for Efficient Neural Network Training](https://arxiv.org/abs/2506.07254) | 2025-06 | Uses stable whitening-style preconditioning to cut both gradient steps and wall-clock time in reported transformer training runs. |
| pFedSOP | [pFedSOP : Accelerating Training Of Personalized Federated Learning Using Second-Order Optimization](https://arxiv.org/abs/2506.07159) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| NYSACT | [NYSACT: A SCALABLE PRECONDITIONED GRADIENT DESCENT USING NYSTRÖM APPROXIMATION](https://arxiv.org/abs/2506.08360) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| MAC | [MAC: AN EFFICIENT GRADIENT PRECONDITIONING USING MEAN ACTIVATION APPROXIMATED CURVATURE](https://arxiv.org/abs/2506.08464) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| LQ-SGD | [Trustworthy Efficient Communication for Distributed Learning using LQ-SGD Algorithm](https://arxiv.org/abs/2506.17974) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| HGM | [Hindsight-Guided Momentum (HGM) Optimizer: An Approach to Adaptive Learning Rates](https://arxiv.org/abs/2506.22479) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FZOO | [FZOO: Fast Zeroth-Order Optimizer for Fine-Tuning Large Language Models towards Adam-Scale Speed](https://arxiv.org/abs/2506.09034) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FedOne | [FedOne: Query-Efficient Federated Learning for Black-box Discrete Prompt Learning](https://arxiv.org/abs/2506.14929) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FedCurv | [Blockchain-Enabled Privacy-Preserving Second-Order Federated Edge Learning in Personalized Healthcare](https://arxiv.org/abs/2506.00416) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DAT-SGD | [Enhancing Parallelism in Decentralized Stochastic Convex Optimization](https://arxiv.org/abs/2506.00961) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ADAACT | [AN ADAPTIVE METHOD STABILIZING ACTIVATIONS FOR ENHANCED GENERALIZATION](https://arxiv.org/abs/2506.08353) | 2025-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| VRAdam | [A Physics-Inspired Optimizer: Velocity Regularized Adam](https://arxiv.org/abs/2505.13196) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| VAMO | [VAMO: Efficient Large-Scale Nonconvex Optimization via Adaptive Zeroth Order Variance Reduction](https://arxiv.org/abs/2505.13954) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SUMO | [SUMO: Subspace-Aware Moment-Orthogonalization for Accelerating Memory-Efficient LLM Training](https://arxiv.org/abs/2505.24749) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SKA-SGD | [STREAMING KRYLOV-ACCELERATED STOCHASTIC GRADIENT DESCENT](https://arxiv.org/abs/2505.07046) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| RaCO-DP | [Private Rate-Constrained Optimization with Applications to Fair Learning](https://arxiv.org/abs/2505.22703) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| QZO | [Fine-tuning Quantized Neural Networks with Zeroth-order Optimization](https://arxiv.org/abs/2505.13430) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| LightSAM | [LightSAM: Parameter-Agnostic Sharpness-Aware Minimization](https://arxiv.org/abs/2505.24399) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Kuramoto-FedAvg | [Kuramoto-FedAvg: Using Synchronization Dynamics to Improve Federated Learning Optimization under Statistical Heterogeneity](https://arxiv.org/abs/2505.19605) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| KO | [KO: Kinetics-inspired Neural Optimizer with PDE Simulation Approaches](https://arxiv.org/abs/2505.14777) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| KerZOO | [KerZOO: Kernel Function Informed Zeroth-Order Optimization for Accurate and Accelerated LLM Fine-Tuning](https://arxiv.org/abs/2505.18886) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DEC-LOC | [DES-LOC: Desynced Low Communication Adaptive Optimizers for Training Foundation Models](https://arxiv.org/abs/2505.22549) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AutoSGD | [AutoSGD: Automatic Learning Rate Selection for Stochastic Gradient Descent](https://arxiv.org/abs/2505.21651) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdamS | [AdamS: Momentum Itself Can Be A Normalizer for LLM Pretraining and Post-training](https://arxiv.org/abs/2505.16363) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Adam-Power | [GradPower: Powering Gradients for Faster Language Model Pre-Training](https://arxiv.org/abs/2505.24275) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ADAGB2 | [Fast Stochastic Second-Order Adagrad for Nonconvex Bound-Constrained Optimization](https://arxiv.org/abs/2505.06374) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AbsSADMM | [Stochastic ADMM with batch size adaptation for nonconvex nonsmooth optimization](https://arxiv.org/abs/2505.06921) | 2025-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| GeoDP-SGD | [Analyzing and Optimizing Perturbation of DP-SGD Geometrically](https://arxiv.org/abs/2504.05618) | 2025-04 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Dion <a href="https://github.com/microsoft/dion"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Dion: Distributed Orthonormalized Updates](https://arxiv.org/abs/2504.05295) | 2025-04 | Distributed orthonormalized updates that retain Muon-style gains while lowering large-scale training overhead. |
| BC-ADMM | [BC-ADMM: An Efficient Non-convex Constrained Optimizer with Robotic Applications](https://arxiv.org/abs/2504.05465) | 2025-04 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AlphaGrad | [AlphaGrad: Non-Linear Gradient Normalization Optimizer](https://arxiv.org/abs/2504.16020) | 2025-04 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ZO2 | [ZO2: Scalable Zeroth-Order Fine-Tuning for Extremely Large Language Models with Limited GPU Memory](https://arxiv.org/abs/2503.12668) | 2025-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SPARTA | [SPARTA: An Optimization Framework for Differentially Private Sparse Fine-Tuning](https://arxiv.org/abs/2503.12822) | 2025-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| PAdamP | [ADAPTIVE MOMENT ESTIMATION OPTIMIZATION ALGORITHM USING PROJECTION GRADIENT FOR DEEP LEARNING](https://arxiv.org/abs/2503.10005) | 2025-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FUSE-PV | [FUSE: First-Order and Second-Order Unified SynthEsis in Stochastic Optimization](https://arxiv.org/abs/2503.04204) | 2025-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FedCET | [Communication Efficient Federated Learning with Linear Convergence on Heterogeneous Data](https://arxiv.org/abs/2503.15804) | 2025-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DC-SGD | [DC-SGD: Differentially Private SGD with Dynamic Clipping through Gradient Norm Distribution Estimation](https://arxiv.org/abs/2503.22988) | 2025-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AsyncSAM | [ASYNCHRONOUS SHARPNESS-AWARE MINIMIZATION FOR FAST AND ACCURATE DEEP LEARNING](https://arxiv.org/abs/2503.11147) | 2025-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ASGO | [ASGO: Adaptive Structured Gradient Optimization](https://arxiv.org/abs/2503.20762) | 2025-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ADEF | [Accelerated Distributed Optimization with Compression and Error Feedback](https://arxiv.org/abs/2503.08427) | 2025-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Stable-SPAM | [Stable-SPAM: How to Train in 4-Bit More Stably than 16-Bit Adam](https://arxiv.org/abs/2502.17055) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Scion <a href="https://github.com/LIONS-EPFL/scion"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Training Deep Learning Models with Norm-Constrained LMOs](https://arxiv.org/abs/2502.07529) | 2025-02 | Norm-constrained LMO updates improve stability, memory efficiency, and hyperparameter transfer across model sizes. |
| SASSHA | [SASSHA: Sharpness-aware Adaptive Second-order Optimization with Stable Hessian Approximation](https://arxiv.org/abs/2502.18153) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| RACS | [Towards Efficient Optimizer Design for LLM via Structured Fisher Approximation with a Low-Rank Extension](https://arxiv.org/abs/2502.07752) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| R-AdaZO | [Refining Adaptive Zeroth-Order Optimization at Ease](https://arxiv.org/abs/2502.01014) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| QuZO | [QuZO: Quantized Zeroth-Order Fine-Tuning for Large Language Models](https://arxiv.org/abs/2502.12346) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| OCAR | [Online Curvature-Aware Replay: Leveraging 2nd Order Information for Online Continual Learning](https://arxiv.org/abs/2502.01866) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| MaZO | [MaZO: Masked Zeroth-Order Optimization for Multi-Task Fine-Tuning of Large Language Models](https://arxiv.org/abs/2502.11513) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| LORENZA | [LORENZA: Enhancing Generalization in Low-Rank Gradient LLM Training and Fine-Tuning via Efficient Zeroth-Order Adaptive SAM Optimization](https://arxiv.org/abs/2502.19571) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Interleaved-ShuffleG | [The Cost of Shuffling in Private Gradient Based Optimization](https://arxiv.org/abs/2502.03652) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Hessian-aware Scaling | [First-ish Order Methods: Hessian-aware Scalings of Gradient Descent](https://arxiv.org/abs/2502.03701) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FAdamGC | [Gradient Correction in Federated Learning with Adaptive Optimization](https://arxiv.org/abs/2502.02727) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| eagle | [EAGLE: EARLY APPROXIMATED-GRADIENT-BASED LEARNING RATE ESTIMATOR](https://arxiv.org/abs/2502.01036) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DPZV | [DPZV: Elevating the Tradeoff between Privacy and Utility in Zeroth-Order Vertical Federated Learning](https://arxiv.org/abs/2502.20565) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DiZO | [Harmony in Divergence: Towards Fast, Accurate, and Memory-efficient Zeroth-order LLM Fine-tuning](https://arxiv.org/abs/2502.03304) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| D-Muon <a href="https://github.com/MoonshotAI/Moonlight"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Muon is Scalable for LLM Training](https://arxiv.org/abs/2502.16982) | 2025-02 | Scales Muon-style orthogonalized updates to distributed LLM training and reports strong compute-efficiency gains over AdamW. |
| Coupled Adam | [Better Embeddings with Coupled Adam](https://arxiv.org/abs/2502.08441) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdaGC | [AdaGC: Improving Training Stability for Large Language Model Pretraining](https://arxiv.org/abs/2502.11034) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Adadiag | [Improving Adaptive Moment Optimization viaPreconditioner Diagonalization](https://arxiv.org/abs/2502.07488) | 2025-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ZOQO | [ZOQO: Zero-Order Quantized Optimization](https://arxiv.org/abs/2501.06736) | 2025-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| TeZO | [TeZO: Empowering the Low-Rankness on the Temporal Dimension in the Zeroth-Order Optimization for Fine-tuning LLMs](https://arxiv.org/abs/2501.19057) | 2025-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SPAM | [SPAM: SPIKE-AWARE ADAM WITH MOMENTUM RESET FOR STABLE LLM TRAINING](https://arxiv.org/abs/2501.06842) | 2025-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SGDO | [Overshoot: Taking advantage of future gradients in momentum-based stochastic optimization](https://arxiv.org/abs/2501.09556) | 2025-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| LT-ADMM | [Communication-Efficient Stochastic Distributed Learning](https://arxiv.org/abs/2501.13516) | 2025-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| HybridSGD | [Communication-Efficient, 2D Parallel Stochastic Gradient Descent for Distributed-Memory Optimization](https://arxiv.org/abs/2501.07526) | 2025-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| GWT | [Wavelet Meets Adam: Compressing Gradients for Memory-Efficient Training](https://arxiv.org/abs/2501.07237) | 2025-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| GCSAM | [GCSAM: Gradient Centralized Sharpness Aware Minimization](https://arxiv.org/abs/2501.11584) | 2025-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ELASTICZO | [ELASTICZO: A MEMORY-EFFICIENT ON-DEVICE LEARNING WITH COMBINED ZEROTH- AND FIRST-ORDER OPTIMIZATION](https://arxiv.org/abs/2501.04287) | 2025-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SWAN | [SWAN: SGD WITH NORMALIZATION AND WHITENING ENABLES STATELESS LLM TRAINING](https://arxiv.org/abs/2412.13148) | 2024-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SGD-SaI | [No More Adam: Learning Rate Scaling at Initialization is All You Need](https://arxiv.org/abs/2412.11768) | 2024-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Muon <a href="https://github.com/KellerJordan/Muon"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Muon: An optimizer for the hidden layers of neural networks](https://kellerjordan.github.io/posts/muon/) | 2024-12 | Uses orthogonalized matrix updates for hidden-layer weights and is commonly paired with AdamW for embeddings and heads. |
| MIAdam | [A Method for Enhancing Generalization of Adam by Multiple Integrations](https://arxiv.org/abs/2412.12473) | 2024-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Grams | [Grams: Gradient Descent with Adaptive Momentum Scaling](https://arxiv.org/abs/2412.17107) | 2024-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FedSTaS | [FedSTaS: Client Stratification and Client Level Sampling for Efficient Federated Learning](https://arxiv.org/abs/2412.14226) | 2024-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| EXADAM | [EXADAM: THE POWER OF ADAPTIVE CROSS-MOMENTS](https://arxiv.org/abs/2412.20302) | 2024-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| apollo | [APOLLO:SGD-LIKE MEMORY, ADAMW-LEVEL PERFORMANCE](https://arxiv.org/abs/2412.05270) | 2024-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Adam-Real | [Adam on Local Time: Addressing Nonstationarity in RL with Relative Adam Timesteps](https://arxiv.org/abs/2412.17113) | 2024-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Adam++ | [Towards Simple and Provable Parameter-Free Adaptive Gradient Methods](https://arxiv.org/abs/2412.19444) | 2024-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| MARS <a href="https://github.com/AGI-Arena/MARS"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [MARS: Unleashing the Power of Variance Reduction for Training Large Models](https://arxiv.org/abs/2411.10438) | 2024-11 | Injects variance reduction into AdamW-, Lion-, and Shampoo-style updates and reports clear GPT-2 training gains. |
| FSGDM | [ON THE PERFORMANCE ANALYSIS OF MOMENTUM METHOD: A FREQUENCY DOMAIN PERSPECTIVE](https://arxiv.org/abs/2411.19671) | 2024-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FedIvon | [Federated Learning with Uncertainty and Personalization via Efficient Second-order Optimization](https://arxiv.org/abs/2411.18385) | 2024-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Cautious Optimizers <a href="https://github.com/kyleliang919/C-Optim"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Cautious Optimizers: Improving Training with One Line of Code](https://arxiv.org/abs/2411.16085) | 2024-11 | A one-line cautious mask that can make AdamW-, Lion-, and momentum-style optimizers more stable and robust. |
| CAdam | [CAdam: Confidence-Based Optimization for Online Learning](https://arxiv.org/abs/2411.19647) | 2024-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AGS-GD | [Anisotropic Gaussian Smoothing for Gradient-based Optimization](https://arxiv.org/abs/2411.11747) | 2024-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ADOPT <a href="https://github.com/iShohei220/adopt"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [ADOPT: Modified Adam Can Converge with Any β2 with the Optimal Rate](https://arxiv.org/abs/2411.02853) | 2024-11 | A drop-in Adam-family variant with stronger convergence guarantees and improved practical stability. |
| A-GNB | [HELENE: HESSIAN LAYER-WISE CLIPPING AND GRADIENT ANNEALING FOR ACCELERATING FINETUNING LLM WITH ZEROTH-ORDER OPTIMIZATION](https://arxiv.org/abs/2411.10696) | 2024-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SuZero | [Zeroth-Order Fine-Tuning of LLMs in Random Subspaces](https://arxiv.org/abs/2410.08989) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SOAA | [EFFICIENT SECOND-ORDER NEURAL NETWORK OPTIMIZATION VIA ADAPTIVE TRUST REGION METHODS](https://arxiv.org/abs/2410.02293) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SAMPa | [SAMPa: Sharpness-aware Minimization Parallelized](https://arxiv.org/abs/2410.10683) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| OptiQ | [Second-Order Optimization via Quiescence](https://arxiv.org/abs/2410.08033) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| LOZO | [Enhancing zeroth-order fine-tuning for language models with low-rank structures](https://arxiv.org/abs/2410.07698) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| LeZO | [SIMULTANEOUS COMPUTATION AND MEMORY EFFICIENT ZEROTH-ORDER OPTIMIZER FOR FINE-TUNING LARGE LANGUAGE MODELS](https://arxiv.org/abs/2410.09823) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| LDAdam | [LDADAM: ADAPTIVE OPTIMIZATION FROM LOWDIMENSIONAL GRADIENT STATISTICS](https://arxiv.org/abs/2410.16103) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| INNAprop | [A SECOND-ORDER-LIKE OPTIMIZER WITH ADAPTIVE GRADIENT SCALING FOR DEEP LEARNING](https://arxiv.org/abs/2410.05871) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FGSAM | [Fast Graph Sharpness-Aware Minimization for Enhancing and Accelerating Few-Shot Node Classification](https://arxiv.org/abs/2410.16845) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| CaAdam | [CaAdam: Improving Adam optimizer using connection aware methods](https://arxiv.org/abs/2410.24216) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Addax | [Addax: Utilizing Zeroth-Order Gradients to Improve Memory Efficiency and Performance of SGD for Fine-Tuning Language Models](https://arxiv.org/abs/2410.06441) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdaRankGrad | [Adarankgrad: Adaptive gradient-rank and moments for memory-efficient llms training and fine-tuning](https://arxiv.org/abs/2410.17881) | 2024-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| WarpAdam | [WarpAdam: A new Adam optimizer based on Meta-Learning approach](https://arxiv.org/abs/2409.04244) | 2024-09 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SOAP <a href="https://github.com/nikhilvyas/SOAP"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [SOAP: Improving and Stabilizing Shampoo using Adam](https://arxiv.org/abs/2409.11321) | 2024-09 | Blends Shampoo-style preconditioning with Adam-style moment updates for stronger large-batch optimization. |
| RSGDM | [Reducing Bias in Deep Learning Optimization: The RSGDM Approach](https://arxiv.org/abs/2409.15314) | 2024-09 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FLeNS | [FLeNS: Federated Learning with Enhanced Nesterov-Newton Sketch](https://arxiv.org/abs/2409.15216) | 2024-09 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FedRepOpt | [FedRepOpt: Gradient Re-parametrized Optimizers in Federated Learning](https://arxiv.org/abs/2409.15898) | 2024-09 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdEMAMix <a href="https://github.com/apple/ml-ademamix"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [AdEMAMix](https://arxiv.org/abs/2409.03137) | 2024-09 | Mixes long-horizon EMA information into AdamW and improves training efficiency for large language models. |
| DOPPLER | [DOPPLER: Differentially Private Optimizers with Low-pass Filter for Privacy Noise Reduction](https://arxiv.org/abs/2408.13460) | 2024-08 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FADAS | [FADAS: Towards Federated Adaptive Asynchronous Optimization](https://arxiv.org/abs/2407.18365) | 2024-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| CRNAS | [Novel Optimization Techniques for Parameter Estimation](https://arxiv.org/abs/2407.04235) | 2024-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| BADM | [BADM: Batch ADMM for Deep Learning](https://arxiv.org/abs/2407.01640) | 2024-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ZoPro | [A Zeroth-Order Proximal Algorithm for Consensus Optimization](https://arxiv.org/abs/2406.09816) | 2024-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| HesScale | [Revisiting Scalable Hessian Diagonal Approximations for Applications in Reinforcement Learning](https://arxiv.org/abs/2406.03276) | 2024-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Fed-Sophia | [Fed-Sophia: A Communication-Efficient Second-Order Federated Learning Algorithm](https://arxiv.org/abs/2406.06655) | 2024-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Adam-mini <a href="https://github.com/zyushun/Adam-mini"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Adam-mini](https://arxiv.org/abs/2406.16793) | 2024-06 | Reduces optimizer memory by sharing update statistics across parameter groups while preserving AdamW-like quality. |
| SF-AdamW (Schedule-Free) <a href="https://github.com/facebookresearch/schedule_free"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [The Road Less Scheduled](https://arxiv.org/abs/2405.15682) | 2024-05 | Removes explicit learning-rate schedules and simplifies tuning while keeping AdamW-style behavior. |
| Q-Newton | [Q-Newton: Hybrid Quantum-Classical Scheduling for Accelerating Neural Network Training with Newton’s Gradient Descent](https://arxiv.org/abs/2405.00252) | 2024-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| MicroAdam <a href="https://github.com/IST-DASLab/MicroAdam"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [MicroAdam](https://arxiv.org/abs/2405.15593) | 2024-05 | Compresses Adam-style state updates to reduce memory pressure while keeping competitive convergence. |
| FAdam <a href="https://github.com/lessw2020/fadam_pytorch"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [FAdam: Adam is a natural gradient optimizer using diagonal empirical Fisher information](https://arxiv.org/abs/2405.12807) | 2024-05 | Uses diagonal empirical Fisher preconditioning to make Adam behave more like a lightweight natural-gradient optimizer. |
| Athena | [Athena: Efficient Block-Wise Post-Training Quantization for Large Language Models Using Second-Order Matrix Derivative Information](https://arxiv.org/abs/2405.17470) | 2024-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdaFisher | [ADAFISHER: ADAPTIVE SECOND ORDER OPTIMIZATION VIA FISHER INFORMATION](https://arxiv.org/abs/2405.16397) | 2024-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| 4-bit shampoo | [4-bit Shampoo for Memory-Efficient Network Training](https://arxiv.org/abs/2405.18144) | 2024-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| VSGD | [Variational Stochastic Gradient Descent for Deep Neural Networks](https://arxiv.org/abs/2404.06549) | 2024-04 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| MeZO-SVRG | [Variance-reduced Zeroth-Order Methods for Fine-Tuning Language Models](https://arxiv.org/abs/2404.08080) | 2024-04 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| BAdam | [BAdam: A Memory Efficient Full Parameter Optimization Method for Large Language Models](https://arxiv.org/abs/2404.02827) | 2024-04 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FAGH | [FAGH: Accelerating Federated Learning with Approximated Global Hessian](https://arxiv.org/abs/2403.11041) | 2024-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| F-SAM | [Friendly Sharpness-Aware Minimization](https://arxiv.org/abs/2403.12350) | 2024-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Adapprox | [Adapprox: Adaptive Approximation in Adam Optimization via Randomized Low-Rank Matrices](https://arxiv.org/abs/2403.14958) | 2024-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Sparse MeZO | [Sparse MeZO: Less Parameters for Better Performance in Zeroth-Order LLM Fine-Tuning](https://arxiv.org/abs/2402.15751) | 2024-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FedLion | [FEDLION: FASTER ADAPTIVE FEDERATED OPTIMIZATION WITH FEWER COMMUNICATION](https://arxiv.org/abs/2402.09941) | 2024-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SSAM | [Stabilizing Sharpness-aware Minimization Through A Simple Renormalization Strategy](https://arxiv.org/abs/2401.07250) | 2024-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| MSAM | [Momentum-SAM: Sharpness Aware Minimization without Computational Overhead](https://arxiv.org/abs/2401.12033) | 2024-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| MADA | [MADA: Meta-Adaptive Optimizers through hyper-gradient Descent](https://arxiv.org/abs/2401.08893) | 2024-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| ZO-AdaMU | [ZO-AdaMU Optimizer: Adapting Perturbation by the Momentum and Uncertainty in Zeroth-order Optimization](https://arxiv.org/abs/2312.15184) | 2023-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DP-AdamBC | [DP-AdamBC: Your DP-Adam Is Actually DP-SGD (Unless You Apply Bias Correction)](https://arxiv.org/abs/2312.14334) | 2023-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AGD <a href="https://github.com/intelligent-machine-learning/dlrover/tree/master/atorch/atorch/optimizers"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [AGD: an Auto-switchable Optimizer using Stepwise Gradient Difference for Preconditioning Matrix](https://arxiv.org/abs/2312.01658) | 2023-12 | Auto-switches preconditioning based on stepwise gradient differences to balance adaptivity and efficiency. |
| SGDF | [Signal Processing Meets SGD: From Momentum to Filter](https://arxiv.org/abs/2311.02818) | 2023-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| FESS-GDA | [Stochastic Smoothed Gradient Descent Ascent for Federated Minimax Optimization](https://arxiv.org/abs/2311.00944) | 2023-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Dice-SGD | [DIFFERENTIALLY PRIVATE SGD WITHOUT CLIPPING BIAS: AN ERROR-FEEDBACK APPROACH](https://arxiv.org/abs/2311.14632) | 2023-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Logit-DP | [DIFFERENTIALLY PRIVATE OPTIMIZATION FOR NONDECOMPOSABLE OBJECTIVE FUNCTIONS](https://arxiv.org/abs/2310.03104) | 2023-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdaLOMO <a href="https://github.com/OpenLMLab/LOMO"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [AdaLomo: Low-memory Optimization with Adaptive Learning Rate](https://arxiv.org/abs/2310.10195) | 2023-10 | Extends LOMO with adaptive learning rates for memory-constrained full-parameter LLM fine-tuning. |
| AdaPlus <a href="https://github.com/guanleics/AdaPlus"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [AdaPlus](https://arxiv.org/abs/2309.01966) | 2023-09 | Adds Nesterov momentum and finer stepsize control on top of AdamW-style optimization. |
| mL-BFGS | [mL-BFGS: A Momentum-based L-BFGS for Distributed Large-Scale Neural Network Optimization](https://arxiv.org/abs/2307.13744) | 2023-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| CoRe <a href="https://github.com/ReiherGroup/CoRe_optimizer"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [CoRe Optimizer: An All-in-One Solution for Machine Learning](https://arxiv.org/abs/2307.15663) | 2023-07 | Proposes a single optimizer intended to work robustly across tasks with less hyperparameter retuning. |
| CAME <a href="https://github.com/yangluo7/CAME"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [CAME: Confidence-guided Adaptive Memory Efficient Optimization](https://arxiv.org/abs/2307.02047) | 2023-07 | Reduces optimizer-state cost for large models while preserving the benefits of adaptive optimization. |
| Adam+CM <a href="https://github.com/chandar-lab/CMOptimizer"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Promoting Exploration in Memory-Augmented Adam using Critical Momenta](https://arxiv.org/abs/2307.09638) | 2023-07 | Adds critical momenta to Adam-style updates to encourage exploration and help escape sharp or poor minima. |
| Prodigy <a href="https://github.com/konstmish/prodigy"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Prodigy](https://arxiv.org/abs/2306.06101) | 2023-06 | A parameter-free optimizer derived from D-Adaptation that reduces or removes learning-rate tuning. |
| MultiAdam | [MultiAdam: Parameter-wise Scale-invariant Optimizer for Multiscale Training of Physics-informed Neural Networks](https://arxiv.org/abs/2306.02816) | 2023-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| look around | [Lookaround Optimizer: k steps around, 1 step average](https://arxiv.org/abs/2306.07684) | 2023-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| LOMO <a href="https://github.com/OpenLMLab/LOMO"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Full Parameter Fine-tuning for Large Language Models with Limited Resources](https://arxiv.org/abs/2306.09782) | 2023-06 | Fuses gradient computation and parameter updates to enable low-memory full-parameter LLM fine-tuning. |
| WSAM <a href="https://github.com/intelligent-machine-learning/dlrover/tree/master/atorch/atorch/optimizers"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Sharpness-Aware Minimization Revisited: Weighted Sharpness as a Regularization Term](https://arxiv.org/abs/2305.15817) | 2023-05 | Revisits SAM with weighted sharpness to improve generalization while keeping optimization practical. |
| UAdam | [UAdam: Unified Adam-Type Algorithmic Framework for Non-Convex Stochastic Optimization](https://arxiv.org/abs/2305.05675) | 2023-05 | Unifies Adam-type methods in one framework and studies convergence behavior under a broad non-convex stochastic setting. |
| Sophia <a href="https://github.com/Liuhong99/Sophia"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Sophia](https://arxiv.org/abs/2305.14342) | 2023-05 | A practical stochastic second-order optimizer for language-model pretraining with modest overhead. |
| MoMo | [MoMo: Momentum Models for Adaptive Learning Rates](https://arxiv.org/abs/2305.07583) | 2023-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| MeZO | [Fine-Tuning Language Models with Just Forward Passes](https://arxiv.org/abs/2305.17333) | 2023-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DoWG <a href="https://github.com/AMorporkian/DoWG"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [DoWG Unleashed: An Efficient Universal Parameter-Free Gradient Descent Method](https://arxiv.org/abs/2305.16284) | 2023-05 | A universal parameter-free gradient method that extends DoG-style step-size adaptation with stronger empirical performance. |
| ANSGD | [Learning across Data Owners with Joint Differential Privacy](https://arxiv.org/abs/2305.15723) | 2023-05 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| μ²-SGD | [DO STOCHASTIC, FEEL NOISELESS: STABLE STOCHASTIC OPTIMIZATION VIA A DOUBLE MOMENTUM MECHANISM](https://arxiv.org/abs/2304.04172) | 2023-04 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DP-Adam | [DP-ADAM: CORRECTING DP BIAS IN ADAM’S SECOND MOMENT ESTIMATION](https://arxiv.org/abs/2304.11208) | 2023-04 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AE-SAM | [AN ADAPTIVE POLICY TO EMPLOY SHARPNESS-AWARE MINIMIZATION](https://arxiv.org/abs/2304.14647) | 2023-04 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| GAM | [Gradient Norm Aware Minimization Seeks First-Order Flatness and ImprovesGeneralization](https://arxiv.org/abs/2303.03108) | 2023-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DP-FedSAM | [Make Landscape Flatter in Differentially Private Federated Learning](https://arxiv.org/abs/2303.11242) | 2023-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdaSAM | [AdaSAM: Boosting Sharpness-Aware Minimization with Adaptive Learning Rate and Momentum for Training Deep Neural Networks](https://arxiv.org/abs/2303.00565) | 2023-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SET-adam | [On Suppressing Range of Adaptive Stepsizes of Adam to Improve Generalisation Performance](https://arxiv.org/abs/2302.01029) | 2023-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Lion <a href="https://github.com/google/automl/tree/master/lion"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Symbolic Discovery of Optimization Algorithms](https://arxiv.org/abs/2302.06675) | 2023-02 | Uses sign-based momentum updates to offer a lightweight alternative to AdamW. |
| FOSI <a href="https://github.com/hsivan/fosi"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [FOSI: Hybrid First and Second Order Optimization](https://arxiv.org/abs/2302.08484) | 2023-02 | Combines first-order optimizers with second-order curvature information for faster convergence on difficult objectives. |
| FedLAP-DP | [FedLAP-DP: Federated Learning by Sharing Differentially Private Loss Approximations](https://arxiv.org/abs/2302.01068) | 2023-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DoG <a href="https://github.com/formll/dog"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [DoG is SGD's Best Friend: A Parameter-Free Dynamic Step Size Schedule](https://arxiv.org/abs/2302.12022) | 2023-02 | Provides a parameter-free dynamic step-size schedule that makes SGD-style optimization far less tuning-sensitive. |
| D-Adaptation <a href="https://github.com/facebookresearch/dadaptation"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [D-Adaptation](https://arxiv.org/abs/2301.07733) | 2023-01 | Learning-rate-free optimization for SGD, Adam, and AdaGrad variants with less manual tuning. |
| AdaFedAdam | [ACCELERATING FAIR FEDERATED LEARNING: ADAPTIVE FEDERATED ADAM](https://arxiv.org/abs/2301.09357) | 2023-01 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| RLEKF | [RLEKF: An Optimizer for Deep Potential with Ab Initio Accuracy](https://arxiv.org/abs/2212.06989) | 2022-12 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| VeLO <a href="https://github.com/google/learned_optimization/tree/main/learned_optimization/research/general_lopt"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [VeLO: Training Versatile Learned Optimizers by Scaling Up](https://arxiv.org/abs/2211.09760) | 2022-11 | A learned optimizer trained at scale to transfer across tasks and architectures better than small learned optimizers. |
| SkechySGD | [SketchySGD: Reliable Stochastic Optimization via Randomized Curvature Estimates](https://arxiv.org/abs/2211.08597) | 2022-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdaCGD | [Adaptive Compression for Communication-Efficient Distributed Training](https://arxiv.org/abs/2211.00188) | 2022-11 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| SketchedAMSGrad | [Communication-Efficient Adam-Type Algorithms for Distributed Data Mining](https://arxiv.org/abs/2210.07454) | 2022-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| DPIS | [DPIS: An Enhanced Mechanism for Differentially Private SGD with Importance Sampling](https://arxiv.org/abs/2210.09634) | 2022-10 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Amos <a href="https://github.com/google-research/jestimator"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Amos](https://arxiv.org/abs/2210.11693) | 2022-10 | Introduces scale-aware adaptive decay and weight decay for Adam-style optimization. |
| AdaNorm <a href="https://github.com/shivram1987/AdaNorm"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [AdaNorm](https://arxiv.org/abs/2210.06364) | 2022-10 | Stabilizes adaptive optimization by correcting gradient-norm scaling behavior. |
| tpSGD | [Learning with Local Gradients at the Edge](https://arxiv.org/abs/2208.08503) | 2022-08 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Adan <a href="https://github.com/sail-sg/Adan"><img alt="GitHub" src="https://img.shields.io/badge/-181717?style=flat-square&logo=github&logoColor=white" height="16"></a> | [Adan: Adaptive Nesterov Momentum Algorithm](https://arxiv.org/abs/2208.06677) | 2022-08 | Uses adaptive Nesterov momentum to speed up and stabilize deep-model training. |
| AdamMC | [Moment Centralization based Gradient Descent Optimizers for Convolutional Neural Networks](https://arxiv.org/abs/2207.09066) | 2022-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdaBFE | [BFE and AdaBFE: A New Approach in Learning Rate Automation for Stochastic Optimization](https://arxiv.org/abs/2207.02763) | 2022-07 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| GradaGrad | [Grad-GradaGrad? A Non-Monotone Adaptive Stochastic Gradient Method](https://arxiv.org/abs/2206.06900) | 2022-06 | Proposes a non-monotone adaptive stochastic gradient method aimed at improving practical convergence over monotone variants. |
| DP-SGD | [Normalized/Clipped SGD with Perturbation for Differentially Private Non-Convex Optimization](https://arxiv.org/abs/2206.13033) | 2022-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AClipped-dpSGD | [Efficient Private SCO for Heavy-Tailed Data via Averaged Clipping](https://arxiv.org/abs/2206.13011) | 2022-06 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| Aida | [A DNN Optimizer that Improves over AdaBelief by Suppression of the Adaptive Stepsize Range](https://arxiv.org/abs/2203.13273) | 2022-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AEGDM | [AN ADAPTIVE GRADIENT METHOD WITH ENERGY AND MOMENTUM](https://arxiv.org/abs/2203.12191) | 2022-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| AdamFamily | [AdaFamily: A family of Adam-like adaptive gradient methods](https://arxiv.org/abs/2203.01603) | 2022-03 | Imported from APRIL-AIGC/Awesome-Optimizer. |
| 0/1 Adam | [Maximizing Communication Efficiency for Large-scale Training via 0/1 Adam](https://arxiv.org/abs/2202.06009) | 2022-02 | Imported from APRIL-AIGC/Awesome-Optimizer. |

## Notes

- This list is paper-first; public implementations are linked when available.
- GitHub icons appear next to optimizer names when a public repository is available.
- The README table includes both the curated entries and the reference-imported entries directly; imported rows are marked by source in the `Notes` column.
- Broad survey repos such as `APRIL-AIGC/Awesome-Optimizer` also include optimizer-adjacent methods; this table keeps the current import aligned to the `2022+` reference scope you asked for.
- `Muon` and `D-Muon` are listed separately: the original `Muon` entry uses the canonical 2024 write-up, while `D-Muon` refers to the 2025 scalable LLM-training paper.
- Cross-check for missing modern entries was done against `APRIL-AIGC/Awesome-Optimizer`, `boshallen/Awesome-Optimizers`, `AidinHamedi/Optimizer-Benchmark`, and `Benchmarking Optimizers for Large Language Model Pretraining`.
- New entries should be added in reverse chronological order.
