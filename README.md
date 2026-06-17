# Awesome Optimizers List

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![GitHub](https://img.shields.io/badge/GitHub-JiwenJ%2FAwesome--Optimizers-181717.svg?style=flat-square&logo=github)](https://github.com/JiwenJ/Awesome-Optimizers)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](./LICENSE)
[![Papers](https://img.shields.io/badge/Papers-187-b31b1b.svg?style=flat-square&logo=arxiv&logoColor=white)](./data/optimizers.csv)
[![Code Links](https://img.shields.io/badge/Code%20Links-52-2ea44f.svg?style=flat-square&logo=github)](./data/optimizers.csv)
[![Coverage](https://img.shields.io/badge/Years-2022--2026-6f42c1.svg?style=flat-square&logo=bookstack&logoColor=white)](./data/optimizers.csv)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/JiwenJ/Awesome-Optimizers/pulls)

Curated optimizer-design papers from `2022+`, ordered by exact publication or submission date in reverse chronological order.

- CSV: [data/optimizers.csv](./data/optimizers.csv)
- Weakly related Muon papers: [data/muon_weakly_related.csv](./data/muon_weakly_related.csv)
- Date source: arXiv `published` date for arXiv papers; source-page submission date for OpenReview/blog entries.
- Note: `SRON` is a legacy unsourced row without a paper URL, so its date remains month-level until the source paper is verified.

| Date | Optimizer Name | Summary |
| --- | --- | --- |
| 2026-06-16 | [MGUP](https://arxiv.org/abs/2606.17526) [Code](https://github.com/MaeChd/MGUP) | Selects a fixed fraction of parameters for larger momentum-gradient-aligned steps while giving the rest smaller nonzero updates; works as a plug-in wrapper for AdamW, Lion, and Muon with convergence guarantees and LLM training experiments. |
| 2026-06-15 | [Hyperball Optimization](https://arxiv.org/abs/2606.16899) | Constrains both weight-matrix and optimizer-update Frobenius norms to fixed constants around a base optimizer such as Adam or Muon; reports 20-30% token-equivalent speedups on Qwen3-style models up to 1.2B and better learning-rate transfer. |
| 2026-06-15 | [CacheMuon](https://arxiv.org/abs/2606.16371) | Caches temporally correlated polar-factor information from previous steps to precondition Muon's Newton-Schulz computation, reducing repeated orthogonalization cost while exposing a quality-efficiency trade-off. |
| 2026-06-12 | [Free Heavy-Tailed Lunch for Muon](https://arxiv.org/abs/2606.14560) | Gives heavy-tailed nonconvex theory showing matrix-valued non-Euclidean optimizers such as Muon and Scion can avoid dimension-dependent costs and achieve stronger stationarity guarantees than Euclidean methods. |
| 2026-06-11 | [Muon^p](https://arxiv.org/abs/2606.13867) | Interpolates between gradient descent and Muon by using fractional spectral-power updates U S^p V^T; derives practical low-degree bivariate matrix recurrences because fixed univariate polynomial iterations cannot compute the required powers. |
| 2026-06-11 | [LoRA-Muon](https://arxiv.org/abs/2606.12921) | Derives a Muon-style spectral steepest-descent rule on the low-rank LoRA manifold, paired with split weight decay, to reduce initialization and stepsize sensitivity and improve rank/width/depth learning-rate transfer. |
| 2026-06-09 | [FOGO](https://arxiv.org/abs/2606.10406) | Frames forgetting as step-level gradient interference, then spectrally orthogonalizes momentum updates and keeps a compact codebook of past directions so dominant minibatch gradients do not erase rare useful directions. |
| 2026-06-08 | [Muon Robust Transfer](https://arxiv.org/abs/2606.09658) | Evaluates pretrained models under corrupted image/text shifts and layer-wise probes, finding Muon-trained features more robust and transferable than Adam or SGD features across transformer and CNN settings. |
| 2026-06-07 | [OptMuon](https://arxiv.org/abs/2606.08783) | Combines Muon-style polar-factor directions with a trajectory-dependent AdaGrad-Norm coefficient schedule, turning orthogonalized momentum into a closed-loop method that calibrates update magnitudes from observed optimization history. |
| 2026-06-07 | [Muon Spectral Dynamics](https://arxiv.org/abs/2606.08388) | Analyzes Muon's polar update as a flat-spectrum, entropy-maximizing bias under alignment assumptions, deriving singular-value dynamics and showing how the update geometry changes noise behavior rather than merely rescaling gradients. |
| 2026-06-03 | [Why Muon Outperforms Adam: A Curvature Perspective](https://arxiv.org/abs/2606.04662) | Uses second-order Taylor decomposition to show Muon and Adam have similar first-order gain at matched validation loss, while Muon pays a smaller curvature penalty through lower normalized directional sharpness. |
| 2026-06-02 | [Spectral Scaling Laws of Muon](https://arxiv.org/abs/2606.04058) | Measures singular-value quantiles of Muon momentum matrices across model sizes and layers, identifying which directions finite Newton-Schulz misses and turning the spectra into layer-aware orthogonalization guidance. |
| 2026-06-02 | [Denoise First, Orthogonalize Later](https://arxiv.org/abs/2606.03899) | Models Muon momentum as a spectral filter that suppresses perturbation modes before orthogonalization, increasing the signal-perturbation gap and stabilizing the singular subspaces passed into Newton-Schulz/polar updates. |
| 2026-06-01 | [A Note on Stability for Orthogonalized Matrix Momentum](https://arxiv.org/abs/2606.01720) | Proves finite-round generalization bounds for client-sampled distributed optimization with orthogonalized matrix momentum, explicitly tracking heterogeneous client sampling and finite-step Newton-Schulz effects. |
| 2026-05-29 | [How Much Orthogonalization Does Muon Need?](https://arxiv.org/abs/2606.00371) | Studies relaxed low-precision Newton-Schulz schedules for Muon and shows cheaper partial orthogonalization can preserve training behavior, separating the need for useful spectral shaping from exact polar accuracy. |
| 2026-05-29 | [Softsign / SoftMuon](https://arxiv.org/abs/2605.31371) | Smooths sign-style optimizer directions and extends the idea to SoftMuon for matrix updates under heterogeneous parameter scales. |
| 2026-05-26 | [Entry-Wise Clipping for Muon](https://arxiv.org/abs/2605.27733) | Applies entry-wise clipping before spectral normalization to control heavy-tailed gradient noise and further improve Muon training efficiency. |
| 2026-05-26 | [Spectral Descent (SD/TSD)](https://arxiv.org/abs/2605.26977) | Studies Muon-type spectral descent and truncated variants for non-smooth optimization with convergence and recovery guarantees. |
| 2026-05-26 | [Muon Adversarial Training](https://arxiv.org/abs/2605.26929) | Analyzes Muon's spectral-norm stability ceiling and empirical behavior under adversarial training across architectures and threat models. |
| 2026-05-26 | [MONA](https://arxiv.org/abs/2605.26842) | Adds an EMA of gradient differences into Muon's gradient pipeline for curvature-aware acceleration in scalable LLM training. |
| 2026-05-26 | [MuCon](https://arxiv.org/abs/2605.26459) | Clips singular values of Muon-style update matrices as a spectral-norm-ball projection alternative to the polar direction. |
| 2026-05-25 | [EMA-Nesterov](https://arxiv.org/abs/2605.25395) | Stabilizes Nesterov-style lookahead using EMA-smoothed trajectory signals and can wrap deep-learning optimizers. |
| 2026-05-23 | [Muon in Vision Transformers](https://arxiv.org/abs/2605.24770) | Evaluates Muon for Vision Transformer training and analyzes how spectral orthogonalized updates interact with ViT optimization recipes. |
| 2026-05-22 | [Regularized Muon Flow](https://arxiv.org/abs/2605.23871) | Interprets regularized Muon as a mirror/prox update and derives Hamiltonian probability-gradient-flow dynamics for Muon-type training. |
| 2026-05-21 | [AMUSE](https://arxiv.org/abs/2605.22432) | Combines schedule-free style iterate averaging with Muon to improve stable gradient evaluation and anytime training behavior. |
| 2026-05-21 | [Layerwise Learning Rates (LLR)](https://arxiv.org/abs/2605.22297) | Assigns transformer-layer learning rates from heavy-tailed spectral estimates and reports speedups across AdamW and Muon pretraining runs. |
| 2026-05-19 | [LionMuon](https://arxiv.org/abs/2605.19811) | Alternates cheaper sign-based Lion steps with stronger Muon spectral steps to reduce average iteration cost. |
| 2026-05-19 | [Schatten-p Adaptive Optimization](https://arxiv.org/abs/2605.19781) | Dynamically selects Schatten-p norm LMO geometries to adapt between SGD-like and Muon-like update rules. |
| 2026-05-19 | [MiMuon](https://arxiv.org/abs/2605.19619) | Mixes Muon orthogonalized gradients with momentum SGD to improve generalization while retaining Muon-style convergence. |
| 2026-05-19 | [High-Pass Pion](https://arxiv.org/abs/2605.19282) | Replaces Muon's uniform spectral whitening with a high-pass promotion-and-suppression Newton-Schulz filter for VLA and RLVR. |
| 2026-05-18 | [Distance-Aware Muon](https://arxiv.org/abs/2605.18999) | Adapts the normalized Muon step scale using trajectory distance or descent certificates to reduce manual scale tuning. |
| 2026-05-18 | [Ringmaster LMO](https://arxiv.org/abs/2605.18174) | Extends asynchronous delayed-gradient training to LMO-based optimizers such as Muon for heterogeneous distributed systems. |
| 2026-05-18 | [Symmetry-Compatible Optimizers](https://arxiv.org/abs/2605.18106) | Assigns spectral row-norm and hybrid updates to parameter blocks according to their symmetry groups, extending Muon-style equivariance. |
| 2026-05-18 | [AMO](https://arxiv.org/abs/2605.17806) | Adapts Muon orthogonalization schedules per matrix based on geometry-dependent Newton-Schulz difficulty. |
| 2026-05-16 | [DynMuon](https://arxiv.org/abs/2605.17109) | Generalizes Muon with dynamic spectral shaping U Sigma^p V^T and tunes the spectrum exponent during training. |
| 2026-05-13 | [Muon Spectral Flattening](https://arxiv.org/abs/2605.13079) | Analyzes Muon's spectral flattening mechanism and links it to larger stable learning rates and faster convergence. |
| 2026-05-13 | [DP-Muon](https://arxiv.org/abs/2605.12994) | Combines per-example clipping, Gaussian noise, momentum, and Newton-Schulz orthogonalization for differentially private Muon training. |
| 2026-05-12 | [Spectral Preconditioning](https://arxiv.org/abs/2605.11850) | Develops constrained stochastic spectral preconditioning as a proximal extension of Muon and Scion under heavy-tailed noise. |
| 2026-05-12 | [Pion](https://arxiv.org/abs/2605.12492) | Uses non-additive left and right orthogonal transforms to preserve singular values while modifying Muon-style matrix updates. |
| 2026-05-12 | [MuonQ](https://arxiv.org/abs/2605.11396) [Code](https://github.com/YupengSu/MuonQ) | Quantizes Muon optimizer states to 4-bit precision using directional fidelity optimization to reduce memory while preserving training quality. |
| 2026-05-11 | [Error Whitening](https://arxiv.org/abs/2605.11316) | Explains Gauss-Newton's advantage as function-space error whitening and compares the induced dynamics against Newton, Adam, and Muon. |
| 2026-05-11 | [Freon/Kaon](https://arxiv.org/abs/2605.11181) | Tests Muon-like Schatten and randomized spectra to argue that alignment and descent potential matter more than exact geometry. |
| 2026-05-11 | [Muon Fine-tuning Transfer](https://arxiv.org/abs/2605.10468) | Studies optimizer mismatch when switching Adam-pretrained models to Muon and proposes procedures for Muon fine-tuning. |
| 2026-05-11 | [Optimizer-Induced Mode Connectivity](https://arxiv.org/abs/2605.09991) | Analyzes connected solution regions constrained by AdamW, Muon, and Lion-K optimizers to expose optimizer-dependent implicit regularization. |
| 2026-05-11 | [Muown](https://arxiv.org/abs/2605.10797) | Controls row norms to reduce spectral-norm drift and weight-decay sensitivity in Muon optimization. |
| 2026-05-11 | [SODA](https://arxiv.org/abs/2605.11172) | Wraps base optimizers including Muon with optimistic dual averaging and a theoretically grounded decay schedule to reduce weight-decay tuning. |
| 2026-05-10 | [Muon Phase Analysis](https://arxiv.org/abs/2605.09552) | Analyzes phases where stochastic spectral optimizers such as Muon outperform SignSGD on high-dimensional matrix problems. |
| 2026-05-10 | [Dimension-Free Muon Escape](https://arxiv.org/abs/2605.09331) | Analyzes Muon saddle-point escape and argues that spectral shaping can avoid dimension-dependent trapping effects. |
| 2026-05-10 | [Intrinsic Muon](https://arxiv.org/abs/2605.09238) | Extends Muon-style spectral LMO updates to Riemannian matrix manifolds and constrained parameter geometries. |
| 2026-05-09 | [ZO Partial Orthogonalization](https://arxiv.org/abs/2605.09034) | Adds Muon-like partial orthogonalization from power iteration to accelerate zeroth-order spectral optimization for LLM fine-tuning. |
| 2026-05-09 | [Muon Non-Convergence](https://arxiv.org/abs/2605.08980) | Shows Muon can fail to converge on convex Lipschitz functions, clarifying limits of smoothness-based Muon theory. |
| 2026-05-09 | [Muon-OGD](https://arxiv.org/abs/2605.08949) | Uses Muon-style spectral geometry for orthogonal-gradient projection in continual learning for LLMs. |
| 2026-05-09 | [Group Muon](https://arxiv.org/abs/2605.08933) | Applies Muon group-wise across attention heads and studies the trade-off between whitening gains and grouping-induced norm cost. |
| 2026-05-08 | [PolarAdamW](https://arxiv.org/abs/2605.07067) | Applies Muon's polar spectral control to AdamW-preconditioned directions to separate spectral control from Schur gauge equivariance. |
| 2026-05-08 | [OrScale-LM](https://arxiv.org/abs/2605.07815) | Adds layer-wise trust-ratio scaling to Muon for language-model training using the norm of the actual parameter-space update direction. |
| 2026-05-07 | [Orth-Dion](https://arxiv.org/abs/2605.16341) | Removes Dion's low-rank Muon geometric mismatch by orthogonalizing the compressed factor in distributed spectral optimization. |
| 2026-05-07 | [Nesterov Muon](https://arxiv.org/abs/2605.06884) | Analyzes Muon with Nesterov momentum under heavy-tailed noise and inexact randomized polar decomposition. |
| 2026-05-07 | [SignSGD/Muon Lower Bounds](https://arxiv.org/abs/2605.06615) [Code](https://github.com/Dingzhen230/SignSGD_Outperforms_SGD) | Derives l1-geometry lower bounds for SignSGD and extends the framework to matrix-domain Muon optimality. |
| 2026-05-07 | [Pro-KLShampoo](https://arxiv.org/abs/2605.06316) | Projects KL-Shampoo-style preconditioned directions through orthogonalization to recover whitening in a Muon-adjacent optimizer. |
| 2026-05-07 | [Implicit Gradient Transport](https://arxiv.org/abs/2605.05577) | Accelerates LMO-based optimizers such as Lion and Muon through implicit gradient transport without extra gradient evaluations. |
| 2026-05-05 | [Aurora](https://blog.tilderesearch.com/blog/aurora) [Code](https://github.com/tilde-research/aurora-release) | Adds diagonal equilibration to Muon-style polar updates to enforce more uniform row leverage for rectangular matrices while reducing to standard Muon on square matrices. |
| 2026-05-05 | [Nora](https://arxiv.org/abs/2605.03769) | Projects row-wise momentum onto the orthogonal complement of weights to stabilize norms and angular velocities with O(mn) matrix-optimizer complexity. |
| 2026-05-04 | [SignMuon](https://arxiv.org/abs/2605.16311) | Combines signSGD-style majority-vote communication with Muon polar-step updates for bandwidth-efficient distributed training. |
| 2026-04-27 | [SUDA-Muon](https://arxiv.org/abs/2604.23980) | Separates gossip-compatible communication from Muon's nonlinear matrix-sign step for fully decentralized Muon optimization. |
| 2026-04-16 | [CLion](https://arxiv.org/abs/2604.14587) | Applies cautious updates to Lion to improve generalization while preserving lightweight optimizer state and efficiency. |
| 2026-04-12 | [Federated Gluon](https://arxiv.org/abs/2604.10689) | Extends Muon-style LMO optimization to federated learning with communication-efficient Gluon updates. |
| 2026-04-11 | [Muon^2](https://arxiv.org/abs/2604.09967) | Adds Adam-style second-moment preconditioning before Muon orthogonalization to reduce Newton-Schulz iteration cost. |
| 2026-04-10 | [APT for MTL](https://arxiv.org/abs/2604.08939) | Balances advanced optimizer momentum with multi-task gradients and preserves Muon orthogonalization directions for MTL. |
| 2026-04-09 | [Adam-HNAG](https://arxiv.org/abs/2604.08742) | Reformulates Adam with a curvature-aware correction and provides accelerated convergence guarantees in the reported setting. |
| 2026-04-06 | [Muon Spectral Wasserstein Flow](https://arxiv.org/abs/2604.04891) | Models vanishing-momentum Muon as a spectral Wasserstein flow to study normalized matrix-update dynamics. |
| 2026-04-06 | [Muon-Accelerated Tensor GLM](https://arxiv.org/abs/2604.04726) | Applies Muon-style acceleration to low-separation-rank tensor generalized linear models. |
| 2026-04-05 | [SIFT/Subspace Control](https://arxiv.org/abs/2604.04231) | Turns constrained model steering into spectral interference-free training via subspace orthogonalization connected to Muon. |
| 2026-04-01 | [Newton-Muon](https://arxiv.org/abs/2604.01472) | Adds input-side Newton preconditioning to Muon and reduces training steps and wall-clock time in reported GPT-2 pretraining runs. |
| 2026-03-30 | [HyperP](https://arxiv.org/abs/2603.28743) | Transfers learning rates across width, depth, tokens, and MoE granularity under Frobenius-sphere constraints with Muon. |
| 2026-03-30 | [MuonEq](https://arxiv.org/abs/2603.28254) | Rebalances momentum before finite-step Newton-Schulz orthogonalization using lightweight row and column equilibration. |
| 2026-03-27 | [Sharp Capacity Scaling](https://arxiv.org/abs/2603.26554) | Analyzes how Muon and spectral optimizers recover associative-memory capacity through frequency-dependent spectral dynamics. |
| 2026-03-20 | [RMNP](https://arxiv.org/abs/2603.20527) [Code](https://anonymous.4open.science/r/RMNP-E8E1/) | Replaces Muon Newton-Schulz iteration with row-wise momentum normalization for O(mn) matrix preconditioning and lower preconditioning wall-clock overhead. |
| 2026-03-18 | [MUD](https://arxiv.org/abs/2603.17970) | Replaces Muon's polar update with a triangular whitening surrogate to reduce matrix-multiply overhead in transformer training. |
| 2026-03-16 | [Hyperparameter Scaling Laws](https://arxiv.org/abs/2603.15958) | Derives batch-size and horizon scaling rules for LMO-style optimizers including signSGD and Muon. |
| 2026-03-16 | [Muon Heavy-Tailed Convergence](https://arxiv.org/abs/2603.15059) | Proves Muon convergence for nonconvex Holder-smooth empirical risk under heavy-tailed stochastic noise. |
| 2026-03-15 | [SPECTRA](https://arxiv.org/abs/2603.14315) | Adds spectral clipping and optional pre-filtering to control update norms and sparse spectral noise in LLM training. |
| 2026-03-10 | [HTMuon](https://arxiv.org/abs/2603.10067) | Applies heavy-tailed spectral correction to Muon so updates preserve more weight-spectrum self-regularization. |
| 2026-03-10 | [Mousse](https://arxiv.org/abs/2603.09697) | Adds curvature-aware preconditioning to Muon to avoid uniform spectral steps across ill-conditioned directions. |
| 2026-03-10 | [MOGA](https://arxiv.org/abs/2603.09952) | Uses mean-normalized matrix operator norms to derive width-aware row/column-normalized updates and improve cross-width hyperparameter transfer. |
| 2026-03-04 | [NuMuon](https://arxiv.org/abs/2603.03597) | Adds a nuclear-norm constraint to Muon updates to improve weight compressibility while retaining favorable convergence behavior. |
| 2026-02-28 | [Muon Simplicity Bias](https://arxiv.org/abs/2603.00742) | Studies optimization biases introduced by Muon and identifies cases where its speed can trade off with simplicity bias. |
| 2026-02-28 | [MuonRec](https://arxiv.org/abs/2603.00416) [Code](https://anonymous.4open.science/r/MuonRec-E447) | Adapts Muon-style orthogonalized updates to recommender models and reduces training steps while improving final ranking quality over AdamW baselines. |
| 2026-02-27 | [LoRA-Pre](https://arxiv.org/abs/2602.24283) [Code](https://github.com/mrflogs/LoRA-Pre) | Reduces Adam and Muon optimizer-state memory through low-rank momentum regressors for LLM pretraining and fine-tuning. |
| 2026-02-26 | [LITE](https://arxiv.org/abs/2602.22681) [Code](https://github.com/SHUCHENZHU/LITE) | Accelerates Muon and SOAP by increasing flat-direction damping and learning rates in an anisotropic Riemannian view. |
| 2026-02-26 | [FlashOptim](https://arxiv.org/abs/2602.23349) [Code](https://github.com/databricks/flashoptim) | Reduces optimizer-state memory by more than 50% with quantized states and master-weight splitting while preserving model quality. |
| 2026-02-25 | [MUON+](https://arxiv.org/abs/2602.21545) [Code](https://github.com/K1seki221/MuonPlus) | Adds one post-polar normalization step to Muon and acts as a small Muon vNext-style improvement in reported LLM pretraining runs. |
| 2026-02-24 | [Spectral Conditions for muP](https://arxiv.org/abs/2602.20937) | Derives muP-style spectral conditions for transferring hyperparameters across optimizers including Shampoo and Muon. |
| 2026-02-19 | [ZO-Muon](https://arxiv.org/abs/2602.17155) | Combines zeroth-order subspace gradient estimation with Muon-style spectral orthogonalization for efficient fine-tuning. |
| 2026-02-19 | [NAMO](https://arxiv.org/abs/2602.17080) | Combines Muon-style orthogonalized momentum with Adam-type noise adaptation to improve stability at negligible extra cost. |
| 2026-02-18 | [Adam/Muon Implicit Bias](https://arxiv.org/abs/2602.16340) | Characterizes momentum steepest-descent bias for Adam, Muon, and Signum on smooth homogeneous networks. |
| 2026-02-18 | [SpecMuon](https://arxiv.org/abs/2602.16167) | Adds spectral guidance and mode-wise RSAV step control to stabilize Muon for scientific machine learning. |
| 2026-02-17 | [Magma](https://arxiv.org/abs/2602.15322) | Uses momentum-aligned gradient masking as a drop-in adaptive optimizer that outperforms Adam and Muon in reported LLM runs. |
| 2026-02-13 | [TrasMuon](https://arxiv.org/abs/2602.13498) | Adapts Muon step scaling through a trust-region mechanism for orthogonalized momentum optimizers. |
| 2026-02-12 | [Muon Quadratic Insights](https://arxiv.org/abs/2602.11948) | Uses simple quadratic models to explain Muon behavior and limits through spectral optimizer dynamics. |
| 2026-02-12 | [Mini-batch Steepest Descent Bias](https://arxiv.org/abs/2602.11557) | Analyzes stochastic steepest descent under entry-wise and Schatten norms covering SignSGD and Muon. |
| 2026-02-10 | [Clarifying Shampoo](https://arxiv.org/abs/2602.09314) | Reinterprets Shampoo as an adapted Muon-style update and explains its token-efficiency advantage over Muon. |
| 2026-02-09 | [Pion/Leon](https://arxiv.org/abs/2602.08232) | Derives adaptive matrix optimizers from smoothed nuclear-norm online learning with nonsmooth nonconvex guarantees. |
| 2026-02-08 | [TSR-Adam](https://arxiv.org/abs/2602.08007) | Uses two-sided low-rank synchronization to reduce Adam-family communication cost in distributed training. |
| 2026-02-07 | [Sign-Based Heavy-Tail Optimizers](https://arxiv.org/abs/2602.07425) | Explains why sign-based optimizers such as Lion and Muon work well under heavy-tailed gradient noise. |
| 2026-02-06 | [Unified Vector/Matrix Adaptivity](https://arxiv.org/abs/2602.06880) | Decouples variance and scale-invariant updates to bridge Adam-style vector updates with Muon-style matrix optimization. |
| 2026-02-06 | [Muon LoRA Spectral Growth](https://arxiv.org/abs/2602.06385) | Proves equal-rate spectral growth for Muon-style updates in LoRA matrix factorization settings. |
| 2026-02-05 | [Norm-Constrained Warm-Up](https://arxiv.org/abs/2602.05813) | Derives adaptive warm-up and scheduling behavior for norm-constrained optimizers including Muon and Lion. |
| 2026-02-05 | [Muon Associative Memory](https://arxiv.org/abs/2602.05725) | Studies Muon training dynamics and scaling laws in hierarchical associative-memory learning. |
| 2026-02-05 | [ADANA](https://arxiv.org/abs/2602.05298) | Adds logarithmic-time momentum and weight-decay schedules to AdamW-style optimization and compares against Muon. |
| 2026-02-04 | [Canzona](https://arxiv.org/abs/2602.06079) | Provides asynchronous load-balanced execution for distributed matrix optimizers such as Shampoo, Muon, and SOAP. |
| 2026-02-04 | [BeyondMuon](https://arxiv.org/abs/2602.04669) [Code](https://github.com/Ocram7/BeyondMuon) | Studies Muon as an endpoint of spectral update transformations and evaluates RMS-normalized variants. |
| 2026-02-03 | [PRISM Spectral Shaping](https://arxiv.org/abs/2602.03096) | Adds low-rank quasi-second-order anisotropic spectral shaping to Muon-style spectral descent. |
| 2026-02-03 | [Non-Euclidean GNS](https://arxiv.org/abs/2602.03001) | Derives adaptive batch-size rules from gradient-noise scales matched to signSGD and Muon geometries. |
| 2026-02-01 | [OLion](https://arxiv.org/abs/2602.01105) | Combines Lion-style sign momentum with spectral orthogonalization to approximate Hadamard-like matrix steps. |
| 2026-01-30 | [Spectra](https://arxiv.org/abs/2602.11185) | Suppresses dominant low-rank spectral spikes to improve LLM optimizer speed, memory, and downstream accuracy. |
| 2026-01-30 | [TEON](https://arxiv.org/abs/2601.23261) | Generalizes layer-wise Muon into tensorized orthonormalization across structured higher-order gradient tensors. |
| 2026-01-30 | [Spectral GD Phase Retrieval](https://arxiv.org/abs/2601.22652) | Shows spectral gradient descent avoids anisotropy-driven misalignment in phase-retrieval dynamics. |
| 2026-01-30 | [Mano](https://arxiv.org/abs/2601.23000) | Projects momentum onto the tangent space and constrains updates on a rotational Oblique manifold to reduce memory and compute in reported LLM training. |
| 2026-01-29 | [PRISM Matrix Functions](https://arxiv.org/abs/2601.22137) | Accelerates matrix square-root and orthogonalization iterations used inside Shampoo and Muon. |
| 2026-01-29 | [FISMO](https://arxiv.org/abs/2601.21750) | Combines Fisher-structured adaptivity with Muon-style momentum orthogonalization. |
| 2026-01-29 | [MCSD/SPEL](https://arxiv.org/abs/2601.21487) | Extends LMO-based spectral steepest descent to manifold-constrained optimization with scalable matrix-sign steps. |
| 2026-01-27 | [Muon Convergence Rates](https://arxiv.org/abs/2601.19400) | Improves nonconvex convergence guarantees for Muon without restrictive update-rule assumptions. |
| 2026-01-27 | [Muon with Newton-Schulz](https://arxiv.org/abs/2601.19156) | Proves practical finite-step Newton-Schulz Muon converges near the ideal SVD-polar rate. |
| 2026-01-21 | [Variance-Adaptive Muon](https://arxiv.org/abs/2601.14603) | Applies NSR-modulated and variance-scaled momentum before Muon orthogonalization to accelerate LLM pretraining. |
| 2026-01-20 | [Muon Spectral Orthogonalization](https://arxiv.org/abs/2601.13474) | Analyzes Muon's preconditioning benefits for matrix factorization and in-context learning of linear transformers. |
| 2026-01-18 | [IFNSO](https://arxiv.org/abs/2602.02500) | Replaces iterative Newton-Schulz orthogonalization with a learned iteration-free polynomial formulation. |
| 2026-01-13 | [Spectral Sphere Optimizer (SSO)](https://arxiv.org/abs/2601.08393) [Code](https://github.com/Unakar/Spectral-Sphere-Optimizer) | Constrains both weights and updates on a spectral sphere to improve LLM training stability and outperform AdamW and Muon in reported experiments. |
| 2026-01-04 | [Principled Muon under muP](https://arxiv.org/abs/2601.01306) | Enforces muP spectral conditions during training for matrix-based optimizers such as Muon. |
| 2025-12-18 | [MVR-Gluon](https://arxiv.org/abs/2512.16598) | Adds momentum variance reduction to the Gluon framework covering Muon, Scion, and other LMO optimizers. |
| 2025-12-15 | [HCM-LMO](https://arxiv.org/abs/2512.13227) | Extends Hessian-corrected momentum to arbitrary-norm LMO optimizers such as Muon, Scion, and Gluon. |
| 2025-12-10 | [Fanions](https://arxiv.org/abs/2512.09678) | Builds Ky-Fan dual-norm Muon variants including Fanions, F-Muon, and S-Muon for matrix optimization. |
| 2025-12-05 | [Matrix-Preconditioned Hyperparameter Transfer](https://arxiv.org/abs/2512.05620) | Studies muP-style scaling rules for Shampoo, SOAP, and Muon across Llama model sizes. |
| 2025-12-04 | [Turbo-Muon](https://arxiv.org/abs/2512.04632) | Preconditions Newton-Schulz orthogonalization to reduce Muon's matrix-multiplication overhead. |
| 2025-12-03 | [Spectral Gradient Conditions](https://arxiv.org/abs/2512.04299) | Derives layerwise conditions predicting when Muon-style spectral updates outperform Euclidean gradient steps. |
| 2025-10-07 | [NorMuon](https://arxiv.org/abs/2510.05491) [Code](https://github.com/zichongli5/NorMuon) | Combines Muon with neuron-wise normalization and second-order statistics to improve scalability and efficiency. |
| 2025-10-06 | [DP-Adam-AC](https://arxiv.org/abs/2510.05288) | Adds adaptive clipping to Adam-based private fine-tuning to improve the privacy-utility trade-off for localizable language models. |
| 2025-10-04 | [Hill-ADAM](https://arxiv.org/abs/2510.03613) | Alternates minimization and maximization phases to help Adam escape local minima in non-convex loss landscapes. |
| 2025-09-29 | [Conda](https://arxiv.org/abs/2509.24218) | Blends Adam-style adaptivity with column-normalized updates to improve optimization efficiency in LLM training. |
| 2025-09-19 | [AdaGrad++](https://openreview.net/forum?id=dHxM51W120) | A simple parameter-free AdaGrad variant with convergence guarantees that removes manual learning-rate tuning. |
| 2025-09-19 | [Adam++](https://openreview.net/forum?id=dHxM51W120) | A simple parameter-free Adam variant with convergence guarantees that removes manual learning-rate tuning. |
| 2025-09-03 | [KL-Shampoo / KL-SOAP](https://arxiv.org/abs/2509.03378) [Code](https://github.com/yorkerlin/KL-Methods) | Recasts Shampoo and SOAP second-moment estimation as KL-minimization and proposes KL-based structured preconditioners that remove Adam grafting overhead. |
| 2025-09-01 | [ZO Fine-Tuner](https://openreview.net/forum?id=2Dn4yHYLQJ) | Learns a zeroth-order optimizer for LLM fine-tuning and outperforms prior zeroth-order baselines across most tested model-task pairs. |
| 2025-09 | SRON | Uses row-wise gradient normalization for state-free LLM training to reduce optimizer-state overhead while stabilizing matrix updates. |
| 2025-07-15 | [AdaMuon](https://arxiv.org/abs/2507.11005) | Adds elementwise second-moment scaling and RMS-aligned rescaling to Muon to improve large-scale training efficiency. |
| 2025-06-20 | [SCALE](https://arxiv.org/abs/2506.16659) [Code](https://github.com/OptimAI-Lab/Minimalist_LLM_Pretraining) | A minimalist optimizer using column normalization and last-layer momentum that matches Adam with much lower memory in LLM pretraining. |
| 2025-06-08 | [SPlus](https://arxiv.org/abs/2506.07254) [Code](https://github.com/kvfrans/splus) | Uses stable whitening-style preconditioning to cut gradient steps and wall-clock time in reported neural network training runs. |
| 2025-05-27 | [PolarGrad](https://arxiv.org/abs/2505.21799) | Unifies matrix-gradient preconditioning and introduces polar-decomposition updates that outperform Adam and Muon in reported studies. |
| 2025-05-19 | [Gluon](https://arxiv.org/abs/2505.13416) | Generalizes Muon and Scion within an LMO framework and improves layer-wise large-model optimization in the reported setting. |
| 2025-04-07 | [Dion](https://arxiv.org/abs/2504.05295) [Code](https://github.com/microsoft/dion) | Distributed orthonormalized updates that reduce large-scale training overhead while preserving Muon-style gains. |
| 2025-02-24 | [COSMOS](https://arxiv.org/abs/2502.17410) [Code](https://github.com/lliu606/COSMOS) | A hybrid optimizer that applies SOAP to leading eigensubspaces and Muon to the remainder for memory-efficient LLM training. |
| 2025-02-24 | [D-Muon](https://arxiv.org/abs/2502.16982) [Code](https://github.com/MoonshotAI/Moonlight) | Scales Muon-style orthogonalized updates to distributed LLM training and improves compute efficiency over strong AdamW baselines. |
| 2025-02-11 | [Scion](https://arxiv.org/abs/2502.07529) [Code](https://github.com/LIONS-EPFL/scion) | Uses norm-constrained LMO updates that improve stability, memory efficiency, and hyperparameter transfer. |
| 2024-12-08 | [Muon](https://kellerjordan.github.io/posts/muon/) [Code](https://github.com/KellerJordan/Muon) | Uses orthogonalized matrix updates for hidden-layer weights and is typically paired with AdamW for non-matrix parameters. |
| 2024-12-02 | [PROFIT](https://arxiv.org/abs/2412.01930) | A specialized optimizer for deep fine-tuning that uses temporal gradient orthogonalization to improve post-convergence adaptation. |
| 2024-11-25 | [Cautious Optimizers](https://arxiv.org/abs/2411.16085) [Code](https://github.com/kyleliang919/C-Optim) | Adds a one-line cautious mask to momentum optimizers such as AdamW and Lion. |
| 2024-11-15 | [MARS](https://arxiv.org/abs/2411.10438) [Code](https://github.com/AGI-Arena/MARS) | Injects variance reduction into adaptive and sign-based optimizers and reports strong GPT-2 training gains. |
| 2024-11-11 | [Subset-Norm + Subspace-Momentum](https://arxiv.org/abs/2411.07120) [Code](https://github.com/timmytonga/sn-sm) | Combines subset-norm adaptivity with subspace momentum to sharply reduce optimizer-state memory while retaining strong LLM training performance. |
| 2024-11-05 | [ADOPT](https://arxiv.org/abs/2411.02853) [Code](https://github.com/iShohei220/adopt) | A modified Adam-family method with stronger convergence guarantees and improved practical stability. |
| 2024-10-25 | [COAT](https://arxiv.org/abs/2410.19313) [Code](https://github.com/NVlabs/COAT) | Compresses optimizer states and activations for memory-efficient FP8 training with near-lossless performance on large models. |
| 2024-10-21 | [LDAdam](https://arxiv.org/abs/2410.16103) [Code](https://github.com/IST-DASLab/LDAdam) | Performs Adam-style adaptive updates in low-dimensional subspaces to reduce memory footprint while exploring the full parameter space. |
| 2024-09-17 | [SOAP](https://arxiv.org/abs/2409.11321) [Code](https://github.com/nikhilvyas/SOAP) | Blends Shampoo-style preconditioning with Adam-style moment updates. |
| 2024-09-05 | [AdEMAMix](https://arxiv.org/abs/2409.03137) [Code](https://github.com/apple/ml-ademamix) | Mixes older-gradient EMAs into AdamW to improve token efficiency. |
| 2024-06-24 | [Adam-mini](https://arxiv.org/abs/2406.16793) [Code](https://github.com/zyushun/Adam-mini) | Uses fewer learning-rate groups to reduce optimizer memory with AdamW-like quality. |
| 2024-05-24 | [SF-AdamW (Schedule-Free)](https://arxiv.org/abs/2405.15682) [Code](https://github.com/facebookresearch/schedule_free) | Removes explicit learning-rate schedules and simplifies tuning while keeping AdamW-style behavior. |
| 2024-05-24 | [MicroAdam](https://arxiv.org/abs/2405.15593) [Code](https://github.com/IST-DASLab/MicroAdam) | Compresses optimizer-state updates to reduce memory overhead while preserving convergence quality. |
| 2024-05-21 | [FAdam](https://arxiv.org/abs/2405.12807) [Code](https://github.com/lessw2020/fadam_pytorch) | Uses diagonal empirical Fisher preconditioning to make Adam behave more like a lightweight natural-gradient optimizer. |
| 2023-12-04 | [AGD](https://arxiv.org/abs/2312.01658) [Code](https://github.com/intelligent-machine-learning/dlrover/tree/master/atorch/atorch/optimizers) | Auto-switches preconditioning based on stepwise gradient differences to balance adaptivity and efficiency. |
| 2023-10-16 | [AdaLOMO](https://arxiv.org/abs/2310.10195) [Code](https://github.com/OpenLMLab/LOMO) | Low-memory optimizer with adaptive learning rates for resource-constrained full-parameter LLM fine-tuning. |
| 2023-09-05 | [AdaPlus](https://arxiv.org/abs/2309.01966) [Code](https://github.com/guanleics/AdaPlus) | Adds Nesterov momentum and more precise stepsize control on top of AdamW-style updates. |
| 2023-07-28 | [CoRe](https://arxiv.org/abs/2307.15663) [Code](https://github.com/ReiherGroup/CoRe_optimizer) | All-in-one optimizer designed to work robustly across tasks with less retuning. |
| 2023-07-18 | [Adam+CM](https://arxiv.org/abs/2307.09638) [Code](https://github.com/chandar-lab/CMOptimizer) | Adds critical momenta to Adam-style updates to improve exploration and escape poor minima. |
| 2023-07-05 | [CAME](https://arxiv.org/abs/2307.02047) [Code](https://github.com/yangluo7/CAME) | Confidence-guided memory-efficient optimization for large-scale model training. |
| 2023-06-16 | [LOMO](https://arxiv.org/abs/2306.09782) [Code](https://github.com/OpenLMLab/LOMO) | Fuses gradient computation and parameter updates to enable low-memory full-parameter LLM fine-tuning. |
| 2023-06-09 | [Prodigy](https://arxiv.org/abs/2306.06101) [Code](https://github.com/konstmish/prodigy) | Parameter-free learner derived from D-Adaptation that reduces learning-rate tuning. |
| 2023-05-25 | [WSAM](https://arxiv.org/abs/2305.15817) [Code](https://github.com/intelligent-machine-learning/dlrover/tree/master/atorch/atorch/optimizers) | Revisits SAM with weighted sharpness to improve generalization while keeping optimization practical. |
| 2023-05-25 | [DoWG](https://arxiv.org/abs/2305.16284) [Code](https://github.com/AMorporkian/DoWG) | Universal parameter-free gradient method that extends DoG-style step-size adaptation with stronger empirical performance. |
| 2023-05-23 | [Sophia](https://arxiv.org/abs/2305.14342) [Code](https://github.com/Liuhong99/Sophia) | Scalable stochastic second-order optimizer for language-model pretraining. |
| 2023-05-09 | [UAdam](https://arxiv.org/abs/2305.05675) | Unified Adam-type framework that studies convergence behavior across a broad class of Adam-family methods. |
| 2023-02-16 | [FOSI](https://arxiv.org/abs/2302.08484) [Code](https://github.com/hsivan/fosi) | Combines first-order optimizers with second-order curvature information for faster convergence on difficult objectives. |
| 2023-02-13 | [Lion](https://arxiv.org/abs/2302.06675) [Code](https://github.com/google/automl/tree/master/lion) | Sign-based momentum optimizer discovered by symbolic search. |
| 2023-02-08 | [DoG](https://arxiv.org/abs/2302.12022) [Code](https://github.com/formll/dog) | Parameter-free dynamic step-size schedule that makes SGD-style optimization much less tuning-sensitive. |
| 2023-01-18 | [D-Adaptation](https://arxiv.org/abs/2301.07733) [Code](https://github.com/facebookresearch/dadaptation) | Learning-rate-free optimization for SGD, Adam, and AdaGrad variants. |
| 2022-11-17 | [VeLO](https://arxiv.org/abs/2211.09760) [Code](https://github.com/google/learned_optimization/tree/main/learned_optimization/research/general_lopt) | Learned optimizer trained at scale to transfer across tasks and architectures better than smaller learned optimizers. |
| 2022-10-21 | [Amos](https://arxiv.org/abs/2210.11693) [Code](https://github.com/google-research/jestimator) | Adam-style optimizer with adaptive decay and scale-aware weight decay. |
| 2022-10-12 | [AdaNorm](https://arxiv.org/abs/2210.06364) [Code](https://github.com/shivram1987/AdaNorm) | Corrects gradient-norm scaling to stabilize adaptive optimization for CNNs. |
| 2022-08-13 | [Adan](https://arxiv.org/abs/2208.06677) [Code](https://github.com/sail-sg/Adan) | Adaptive Nesterov momentum optimizer for faster and more stable deep-model training. |
| 2022-06-14 | [GradaGrad](https://arxiv.org/abs/2206.06900) | Non-monotone adaptive stochastic gradient method aimed at improving practical convergence over monotone variants. |

## Weakly Related / Adjacent Muon Papers

These papers mention, compare, or rely on Muon-style optimization, but their main contribution is broader than a standalone Muon-family optimizer.

- CSV: [data/muon_weakly_related.csv](./data/muon_weakly_related.csv)

| Date | Paper | Relation |
| --- | --- | --- |
| 2026-06-14 | [Schattor](https://arxiv.org/abs/2606.15702) | Proposes Schatten-family deep-learning optimizers that unify SGD and Muon geometry while remaining broader than a Muon-specific variant. |
| 2026-06-13 | [When to use Schatten-p Norm](https://arxiv.org/abs/2606.15268) | Analyzes regimes where Schatten-p geometries such as Muon's Schatten-infinity update are beneficial rather than proposing a Muon variant. |
| 2026-06-12 | [ZO Parameter-free LMO](https://arxiv.org/abs/2606.14970) | Develops zeroth-order parameter-free LMO fine-tuning methods adjacent to Muon-style geometry without proposing a Muon optimizer. |
| 2026-06-12 | [Zeta](https://arxiv.org/abs/2606.14187) | Introduces dual whitening via coordinate-adaptive preconditioning and positions Muon as a matrix-aware baseline. |
| 2026-06-11 | [Different Layers Different Manifolds](https://arxiv.org/abs/2606.13276) | Studies module-wise Stiefel and DGram geometry assignments through Manifold Muon rather than changing core Muon. |
| 2026-06-09 | [Overcoming Rank Collapse in Feedback Alignment](https://arxiv.org/abs/2606.11123) | Uses Muon as an orthogonalized-update mechanism to increase feedback-alignment signal rank rather than proposing a Muon variant. |
| 2026-06-04 | [PC Layer](https://arxiv.org/abs/2606.06470) | Evaluates polynomial weight preconditioning for LLM pretraining with both AdamW and Muon while focusing on architecture-level conditioning. |
| 2026-06-04 | [Double Preconditioning](https://arxiv.org/abs/2606.06418) | Frames Muon as one gradient-wise preconditioning option inside a broader test-time-performance optimization method. |
| 2026-06-02 | [Ultralytics YOLO26](https://arxiv.org/abs/2606.03748) | Uses a hybrid Muon-SGD optimizer in a real-time vision training recipe but contributes a model family rather than an optimizer. |
| 2026-06-01 | [WALL-WM](https://arxiv.org/abs/2606.01955) | Relies on Muon-optimizer-based large-scale pretraining infrastructure for world action modeling rather than introducing Muon mechanics. |
| 2026-05-30 | [Exploiting Weight-Space Symmetries for Approximating Curvature](https://arxiv.org/abs/2606.00442) | Uses weight-space symmetry choices to approximate curvature and recover Shampoo/Muon-like estimates in a broader optimizer geometry framework. |
| 2026-05-29 | [Mellum2 Technical Report](https://arxiv.org/abs/2605.31268) | Reports Muon under FP8 hybrid precision in a code-model pretraining recipe rather than contributing an optimizer method. |
| 2026-05-28 | [On the Optimizer Dependence of Neural Scaling Laws](https://arxiv.org/abs/2605.29387) | Studies how scaling-law behavior changes across optimizers and uses Matrix-Sign as a Muon-style proxy rather than proposing a Muon variant. |
| 2026-05-27 | [Parallax](https://arxiv.org/abs/2605.29157) | Uses Muon to unlock parameterized local linear attention capacity but the main contribution is an attention architecture rather than an optimizer. |
| 2026-05-26 | [How the Optimizer Shapes Learned Solutions in Equivariant Neural Networks](https://arxiv.org/abs/2605.27662) | Compares Muon and Adam in equivariant neural networks and analyzes learned solution structure rather than introducing a Muon optimizer. |
| 2026-05-26 | [The Stability of Singular Distribution](https://arxiv.org/abs/2605.26489) | Uses Muon and WSD as examples of spectral mechanisms shaping two-phase LLM pretraining dynamics rather than proposing an optimizer. |
| 2026-05-23 | [Momentum Streams for Optimizer-Inspired Transformers](https://arxiv.org/abs/2605.24425) | Uses Muon, SOAP, and Adam analogies to design Transformer blocks with architecture rather than optimizer as the main contribution. |
| 2026-05-20 | [Same Architecture, Different Capacity](https://arxiv.org/abs/2605.21803) | Compares Muon and AdamW representation spectral scaling laws while focusing on capacity diagnostics rather than a new optimizer. |
| 2026-05-18 | [Scale-Invariant Neural Network Optimization](https://arxiv.org/abs/2605.18528) | Studies norm geometry and heavy-tailed noise for scale-invariant optimizers such as Muon and Scion rather than proposing a Muon variant. |
| 2026-05-09 | [Navigating LLM Valley](https://arxiv.org/abs/2605.09176) | Surveys LLM optimizers including Muon and matrix-based methods rather than proposing a new optimizer. |
| 2026-05-07 | [Optimizer-Model Consistency](https://arxiv.org/abs/2605.06654) | Analyzes matching pretraining and finetuning optimizers and compares Muon/AdamW forgetting behavior rather than introducing a method. |
| 2026-04-16 | [Benchmarking Optimizers for MLPs in Tabular Deep Learning](https://arxiv.org/abs/2604.15297) | Benchmarks Muon against other optimizers for tabular MLPs, with empirical comparison rather than optimizer design as the main contribution. |
| 2026-04-02 | [Normalization-Optimizer Coupling](https://arxiv.org/abs/2604.01563) | Studies how normalization choices interact with Muon in LLM training rather than introducing a new optimizer. |
| 2026-03-30 | [Spectral Edge Dynamics](https://arxiv.org/abs/2603.28964) | Uses spectra of update windows to analyze neural training phase transitions rather than proposing an optimizer. |
| 2026-02-25 | [veScale-FSDP](https://arxiv.org/abs/2602.22437) | Supports block-structured and matrix-optimizer training systems including Muon but focuses on FSDP infrastructure. |
| 2026-02-07 | [Robust Scaling Laws for Optimizers](https://arxiv.org/abs/2602.07712) | Compares scaling laws across optimizers including Muon and Shampoo without introducing a new optimizer. |
| 2026-01-31 | [Data Distribution as an Optimizer Lever](https://arxiv.org/abs/2602.00576) | Studies whether data distribution can steer optimizer generalization behavior rather than proposing a Muon method. |
| 2026-01-14 | [Muon-Optimized Distillation and Quantization](https://arxiv.org/abs/2601.09865) | Uses Muon inside a model-refinement pipeline for LLM deployment rather than contributing an optimizer. |
| 2026-01-08 | [Learnable Multipliers](https://arxiv.org/abs/2601.04890) | Validates learnable matrix-layer scale multipliers with Adam and Muon but focuses on parameter scaling. |
| 2025-12-16 | [Optimizing Rank for INRs](https://arxiv.org/abs/2512.14366) | Uses Muon-like high-rank updates to improve implicit neural representations rather than designing an optimizer. |
