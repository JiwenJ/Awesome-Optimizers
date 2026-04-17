# Awesome-Optimzers

A curated list of optimizer papers from 2022 onward, with paper links, official or canonical GitHub implementations, and short descriptions.

Current scope:

- Start from `2022`
- Sort by time in reverse chronological order
- Focus on optimizers that are directly useful for deep learning and LLM training

If you later want the repository name corrected to `Awesome-Optimizers`, I can rename the local folder and adjust the title.

## Format

| Date | Optimizer | Paper | GitHub | Short Description |
| --- | --- | --- | --- | --- |
| 2025-04 | Dion | [arXiv](https://arxiv.org/abs/2504.05295) | [microsoft/dion](https://github.com/microsoft/dion) | Distributed orthonormalized updates that keep Muon-style benefits while reducing large-scale training overhead. |
| 2025-02 | Muon | [arXiv](https://arxiv.org/abs/2502.16982) | [MoonshotAI/Moonlight](https://github.com/MoonshotAI/Moonlight) | Scales orthogonalized updates to LLM training and improves compute efficiency over strong AdamW baselines. |
| 2024-11 | Cautious Optimizers | [arXiv](https://arxiv.org/abs/2411.16085) | [kyleliang919/C-Optim](https://github.com/kyleliang919/C-Optim) | A one-line mask for momentum optimizers such as AdamW and Lion to improve stability and speed. |
| 2024-09 | SOAP | [arXiv](https://arxiv.org/abs/2409.11321) | [nikhilvyas/SOAP](https://github.com/nikhilvyas/SOAP) | Combines Shampoo-style preconditioning with Adam-style moment updates for faster large-batch training. |
| 2024-09 | AdEMAMix | [arXiv](https://arxiv.org/abs/2409.03137) | [apple/ml-ademamix](https://github.com/apple/ml-ademamix) | Adds older-gradient EMA mixing to AdamW and reports markedly better token efficiency for LLM training. |
| 2024-06 | Adam-mini | [arXiv](https://arxiv.org/abs/2406.16793) | [zyushun/Adam-mini](https://github.com/zyushun/Adam-mini) | Uses fewer learning-rate groups than AdamW to reduce optimizer memory while keeping similar quality. |
| 2024-05 | Schedule-Free | [arXiv](https://arxiv.org/abs/2405.15682) | [facebookresearch/schedule_free](https://github.com/facebookresearch/schedule_free) | Removes explicit learning-rate schedules and aims for strong performance with simpler tuning. |
| 2024-05 | MicroAdam | [arXiv](https://arxiv.org/abs/2405.15593) | [IST-DASLab/MicroAdam](https://github.com/IST-DASLab/MicroAdam) | Compresses optimizer-state updates to reduce memory overhead while preserving Adam-like convergence. |
| 2023-09 | AdaPlus | [arXiv](https://arxiv.org/abs/2309.01966) | [guanleics/AdaPlus](https://github.com/guanleics/AdaPlus) | Adds Nesterov momentum and more precise stepsize adjustment on top of AdamW-style updates. |
| 2023-07 | CAME | [arXiv](https://arxiv.org/abs/2307.02047) | [yangluo7/CAME](https://github.com/yangluo7/CAME) | A confidence-guided memory-efficient optimizer designed to reduce optimizer-state cost for large models. |
| 2023-06 | Prodigy | [arXiv](https://arxiv.org/abs/2306.06101) | [konstmish/prodigy](https://github.com/konstmish/prodigy) | A parameter-free learner that extends D-Adaptation and reduces or removes learning-rate tuning. |
| 2023-05 | Sophia | [arXiv](https://arxiv.org/abs/2305.14342) | [Liuhong99/Sophia](https://github.com/Liuhong99/Sophia) | A scalable stochastic second-order optimizer for language-model pretraining with low extra cost. |
| 2023-02 | Lion | [arXiv](https://arxiv.org/abs/2302.06675) | [google/automl/lion](https://github.com/google/automl/tree/master/lion) | Sign-based momentum optimizer discovered by symbolic search, often used as a lighter AdamW alternative. |
| 2023-01 | D-Adaptation | [arXiv](https://arxiv.org/abs/2301.07733) | [facebookresearch/dadaptation](https://github.com/facebookresearch/dadaptation) | Learning-rate-free optimization for SGD, Adam, and AdaGrad variants. |
| 2022-10 | Amos | [arXiv](https://arxiv.org/abs/2210.11693) | [google-research/jestimator](https://github.com/google-research/jestimator) | Adam-style optimizer with adaptive learning-rate decay and weight decay motivated by scale invariance. |
| 2022-10 | AdaNorm | [arXiv](https://arxiv.org/abs/2210.06364) | [shivram1987/AdaNorm](https://github.com/shivram1987/AdaNorm) | Corrects gradient-norm scaling to stabilize adaptive optimization in CNN training. |
| 2022-08 | Adan | [arXiv](https://arxiv.org/abs/2208.06677) | [sail-sg/Adan](https://github.com/sail-sg/Adan) | Adaptive Nesterov momentum optimizer aimed at faster and more stable deep-model training. |

## Notes

- The list currently favors papers with a public implementation.
- Some entries point to the most canonical public code location rather than a standalone dedicated repository.
- New entries should be inserted in reverse chronological order.

## Data File

Structured version: [data/optimizers.csv](./data/optimizers.csv)

## Possible Next Steps

- Add tags such as `first-order`, `second-order`, `memory-efficient`, `lr-free`, `LLM`.
- Split the list into yearly sections once the table becomes longer.
- Add a simple contribution rule for accepting new optimizers.
