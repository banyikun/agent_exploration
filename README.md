
<h1 align="center">🔥 Awesome-Agent-Exploration

"Agent Exploration Toward Artificial General Intelligence"</h2>




<p align="center">
  <b>◇ Responder → Reasoner → Agent → Prospector → Ecosystem ◇</b>
    <br>
   <i><b>🚀 Exploration as the Transition Mechanism 🚀</b></i>
</p>

<p align="center"><img src="fig/5levels.png" width="900"/></p>



<p align="center">
  <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6748619"><img src="https://img.shields.io/badge/📄_Paper-SSRN-blue" alt="Paper"></a>
  <!-- <a href="#"><img src="https://img.shields.io/badge/🌐_Website-Project_Page-blue" alt="Website"></a> -->
  <a href="https://github.com/banyikun/epistemic_exploration"><img src="https://img.shields.io/badge/GitHub-Repository-181717?logo=github" alt="GitHub"></a>
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <a href="#"><img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License"></a>
  <a href="#"><img src="https://img.shields.io/badge/Maintained%3F-Yes-brightgreen.svg" alt="Maintained"></a>
  <a href="#"><img src="https://img.shields.io/badge/PRs-Welcome-orange.svg" alt="PRs Welcome"></a>
  </a>
  <a href=""><img src="https://img.shields.io/github/last-commit/banyikun/epistemic_exploration?color=lightgrey"></a>
</p>

<p align="center">
  <a href="https://github.com/banyikun/epistemic_exploration/stargazers"><img src="https://img.shields.io/github/stars/banyikun/epistemic_exploration?style=social" alt="GitHub stars"></a>
  <a href="https://github.com/banyikun/epistemic_exploration/network/members"><img src="https://img.shields.io/github/forks/banyikun/epistemic_exploration?style=social" alt="GitHub forks"></a>
  <a href="https://visitor-badge.laobi.icu/badge?page_id=banyikun.epistemic_exploration">
  <img src="https://visitor-badge.laobi.icu/badge?page_id=banyikun.epistemic_exploration" alt="Visitors">
  </a>
</p>

<h4 align="center">If you find our survey helpful, please give it a star ⭐ to show your support！Thank you:)

</h4>






## 📣 Notices

> 🔥 This is a curated paper list for the survey **"Epistemic Exploration Toward Artificial General Intelligence"**, covering exploration mechanisms across reasoning, embodied AI, world models, and multi-agent systems.

> 🔥 **Stay tuned for our full paper release, incorporating the latest developments.**

> **[Always] [Add your papers]** We welcome all related papers! If you find any missed or new work, please open a Pull Request or contact us.

> **[Always] [Maintain]** We will keep this list updated frequently!

---


## Citation

If you find this survey useful, please cite:

```bibtex
@article{ban2026epistemic,
  title  = {Agent Exploration Toward Artificial General Intelligence},
  author = {Ban, Yikun and Yang, Fengkai and Chen, Fangzheng and Wang, Yibo and Chen, Zhijun and Li, Zhongyi and Huang, Zixuan and Zhang, Xiaoyuan and Li, Gongxun and Chen, Zehao and others},
  year   = {2026},
  doi    = {10.5281/zenodo.20201414},
  url    = {https://doi.org/10.5281/zenodo.20201414}
}
```

---



## 📑 Table of Contents

- [📣 Notices](#-notices)
- [📑 Table of Contents](#-table-of-contents)
- [1. Overview](#1-overview)
  - [1.1 What is Epistemic Exploration?](#11-what-is-epistemic-exploration)
  - [1.2 Three Criteria](#12-three-criteria)
  - [1.3 Unified Epistemic Exploration Objective](#13-unified-epistemic-exploration-objective)
  - [1.4 Five-Level Trajectory Toward AGI](#14-five-level-trajectory-toward-agi)
  - [1.5 3×5 Taxonomy](#15-35-taxonomy)
- [2. Levels 1–2: Responder → Reasoner — Reasoning-Space Exploration](#2-levels-12-responder--reasoner--reasoning-space-exploration)
  - [2.1 Uncertainty-Driven Exploration](#21-uncertainty-driven-exploration)
  - [2.2 Competence-Driven Exploration](#22-competence-driven-exploration)
  - [2.3 Reachability-Driven Exploration](#23-reachability-driven-exploration)
- [3. Level 3: Reasoner → Agent — Perception- \& Action-Space Exploration](#3-level-3-reasoner--agent--perception---action-space-exploration)
  - [3.1 Digital Agents](#31-digital-agents)
    - [3.1.1 Uncertainty-Driven Exploration](#311-uncertainty-driven-exploration)
    - [3.1.2 Competence-Driven Exploration](#312-competence-driven-exploration)
    - [3.1.3 Reachability-Driven Exploration](#313-reachability-driven-exploration)
  - [3.2 Embodied Agents](#32-embodied-agents)
    - [3.2.1 Uncertainty-Driven Exploration](#321-uncertainty-driven-exploration)
    - [3.2.2 Competence-Driven Exploration](#322-competence-driven-exploration)
    - [3.2.3 Reachability-Driven Exploration](#323-reachability-driven-exploration)
- [4. Level 4: Agent → Prospector — Imagination-Space Exploration](#4-level-4-agent--prospector--imagination-space-exploration)
  - [4.1 Why: The Dual Exploration Problem](#41-why-the-dual-exploration-problem)
    - [4.1.1 Compounding Errors and Reality Drift](#411-compounding-errors-and-reality-drift)
    - [4.1.2 The Noise-Hijacking Trap](#412-the-noise-hijacking-trap)
    - [4.1.3 Fatal Detail Loss in Latent Space](#413-fatal-detail-loss-in-latent-space)
  - [4.2 Where: Exploration Across Different Spaces](#42-where-exploration-across-different-spaces)
    - [4.2.1 Simulated Future Rollouts](#421-simulated-future-rollouts)
    - [4.2.2 Counterfactual Hazard Zones](#422-counterfactual-hazard-zones)
    - [4.2.3 Latent Value Landscapes](#423-latent-value-landscapes)
    - [4.2.4 Action-Grounded Latent Manifolds](#424-action-grounded-latent-manifolds)
  - [4.3 How: Exploration Across World-Model Domains](#43-how-exploration-across-world-model-domains)
    - [4.3.1 Model-Based Reinforcement Learning (MBRL)](#431-model-based-reinforcement-learning-mbrl)
      - [Deterministic Dynamics and Iterative Exploration](#deterministic-dynamics-and-iterative-exploration)
      - [Uncertainty-Aware Exploration](#uncertainty-aware-exploration)
      - [From Pixels to Latent Planning: Representation Learning for World Models](#from-pixels-to-latent-planning-representation-learning-for-world-models)
      - [Imagination-Based Exploration: The Dreamer Family](#imagination-based-exploration-the-dreamer-family)
      - [Predictive Architectures: JEPA](#predictive-architectures-jepa)
    - [4.3.2 Video Generation as World Simulation](#432-video-generation-as-world-simulation)
      - [Model as Environment](#model-as-environment)
      - [Model as Agent](#model-as-agent)
      - [Inference as Exploration](#inference-as-exploration)
      - [Active Closed-Loop Simulation via World Action Models (WAMs)](#active-closed-loop-simulation-via-world-action-models-wams)
    - [4.3.3 Autonomous Driving: Vectorised and Occupancy Exploration](#433-autonomous-driving-vectorised-and-occupancy-exploration)
      - [Generative Foundations and End-to-End Latent Planning](#generative-foundations-and-end-to-end-latent-planning)
      - [Counterfactual Reasoning and Uncertainty Awareness](#counterfactual-reasoning-and-uncertainty-awareness)
      - [4D Occupancy Exploration and Physical Consistency](#4d-occupancy-exploration-and-physical-consistency)
      - [Closed-Loop Neural Simulation](#closed-loop-neural-simulation)
    - [4.3.4 Social Dynamics: Exploration in Strategic and Normative Environments](#434-social-dynamics-exploration-in-strategic-and-normative-environments)
- [5. Level 5: Prospector → Ecosystem — Coordination-Space Exploration](#5-level-5-prospector--ecosystem--coordination-space-exploration)
  - [5.1 Multi-Agent Orchestration](#51-multi-agent-orchestration)
    - [5.1.1 Rule-based Orchestration (Reachability-Driven)](#511-rule-based-orchestration-reachability-driven)
    - [5.1.2 Learnable Orchestration (Competence-Driven)](#512-learnable-orchestration-competence-driven)
    - [5.1.3 Reflection \& Information-Theoretic Orchestration (Uncertainty-Driven)](#513-reflection--information-theoretic-orchestration-uncertainty-driven)
    - [5.1.4 Memory \& Knowledge Substrate Exploration](#514-memory--knowledge-substrate-exploration)
  - [5.2 Agentic Ensemble Papers](#52-agentic-ensemble-papers)
    - [5.2.1 Ensemble-During-Inference Papers](#521-ensemble-during-inference-papers)
    - [5.2.2 Ensemble-After-Inference Papers](#522-ensemble-after-inference-papers)
    - [5.2.3 Ensemble-Before-Inference Papers](#523-ensemble-before-inference-papers)
    - [5.2.4 Cascaded-Based Papers](#524-cascaded-based-papers)
  - [5.3 MARL](#53-marl)
  - [5.4 Self-Evolving](#54-self-evolving)
- [6. Exploration Evaluation](#6-exploration-evaluation)
  - [Foundations](#foundations)
  - [Biological Exploration Parallels](#biological-exploration-parallels)
  - [Evaluation Principles](#evaluation-principles)
  - [Open Challenges](#open-challenges)
- [7. Citation](#7-citation)

---
<br>



## 1. Overview

### 1.1 What is Epistemic Exploration?

> **Epistemic exploration** is the agent's capacity to actively acquire information that reduces its uncertainty about the world, convert that reduction into durable policy improvement, and keep future acquisition possible.

Unlike undirected exploration (e.g., ε-greedy), epistemic exploration is *intentional*, *belief-driven*, and *multi-scale*: the agent reasons about which actions are most informative and plans multi-step information-gathering strategies across reasoning trajectories, tool-use policies, embodied sensorimotor loops, world-model rollouts, and multi-agent coordination protocols.


### 1.2 Three Criteria

<p align="center"><img src="fig/3criteria.png" width="800"/></p>
<p align="center"><i>Figure: Foundation of Epistemic Exploration — Why, What, and How.</i></p>

We ground epistemic exploration in **three jointly necessary criteria**, each addressing a distinct failure mode of static optimisation:

| Criterion | What It Does | Failure Mode Addressed | Explores... |
|:---------:|:-------------|:-----------------------|:------------|
| **C1: Information Gain** | Actively reduces epistemic uncertainty via belief-updating observations | *Belief Stagnation* — frozen internal model under distribution shift | ...where it knows least |
| **C2: Value Improvement** | Converts new information into durable policy improvement | *Value Stagnation* — local optima lock-in, surrogate misalignment | ...what it cannot yet do well |
| **C3: Epistemic Reachability** | Preserves positive visitation over belief-consistent regions | *Reachability Collapse* — irreversible contraction of behavioural diversity | ...where it might otherwise never go |

These form a closed loop: **gain information → convert to value → keep the capacity to gain information alive → ...**


### 1.3 Unified Epistemic Exploration Objective

The three criteria combine into a single constrained objective:

$$
\pi_{\mathfrak{A},t}^{*}
\=\
\underset{\underbrace{\pi_{\mathfrak{A}} \,\in\, \Pi_{\mathrm{reach}}(b_t)}_{\text{Reachability (C3)}}}{\arg\max}\
\underbrace{\mathbb{E}_{\theta \sim b_t} \Big[V^{\pi_{\mathfrak{A}}}_\theta(s_t, h_t)\Big]}_{\text{Value Improvement (C2)}}
\ +\ \beta \cdot
\underbrace{\mathbb{E}^{\pi_{\mathfrak{A}}}_{b_t} \left[\sum_{t'=t}^{\infty} \gamma^{\,t'-t}\,\mathcal{U}(s_{t'}, a_{t'};\, b_{t'})\right]}_{\text{Information Gain (C1)}}
$$


where $\mathcal{U}(s, a;\, b) = I(\theta;\, s', r \mid s, a, b)$ is epistemic uncertainty, and  $\Pi_{\mathrm{reach}}(b_t)$ is the reachability-feasible policy set.


**Reading the objective.** The three terms map one-to-one onto the three criteria:

- **Information-gain term (C1)** — expected cumulative epistemic uncertainty the agent anticipates resolving along its trajectory. 
- **Value Improvement (C2)** — expected cumulative reward under current beliefs; what a pure exploiter would maximise.
- **Reachability (C3)** — visitation must remain over every region plausibly relevant under beliefs, preventing short-term gains from foreclosing future learning.



### 1.4 Five-Level Trajectory Toward AGI

We propose exploration as the **transition mechanism** between five levels of increasing agent sophistication. Each level introduces a qualitatively new exploration space that the previous level cannot access:

| Transition | Exploration Space | What Becomes Explorable |
|:-----------|:------------------|:------------------------|
| **L1 → L2: Responder → Reasoner** | **Reasoning space** | Hypotheses, alternative reasoning trajectories, latent thought representations; self-verification and revision |
| **L2 → L3: Reasoner → Agent** | **Interaction space** | Embodied perception, tool invocation, memory management, closed-loop action under partial observability |
| **L3 → L4: Agent → Prospector** | **Imagination space** | Counterfactual futures in learned world models; the dual exploration problem across real and imagined environments |
| **L4 → L5: Prospector → Ecosystem** | **Coordination space** | Communication topologies, co-evolving role specialisations, shared representations, collaborative strategies |

### 1.5 3×5 Taxonomy

Our survey is organized as a **3×5 taxonomy** crossing three signal-driven methodologies with the five levels:

| | **L1 Responder** | **L2 Reasoner** | **L3 Agent** | **L4 Prospector** | **L5 Ecosystem** |
|---|---|---|---|---|---|
| **Uncertainty-Driven** | *— (single forward pass; no internal search)* | Token / step entropy, entropy-guided branching | Active SLAM, prediction variance, pose uncertainty | Ensemble disagreement in latent world models | Inter-agent disagreement, joint-belief uncertainty |
| **Competence-Driven** | *— (no learning loop at inference)* | Difficulty-adaptive curricula, self-verification, self-play | Skill bootstrapping, goal-conditioned self-play | Imagination-based skill discovery, learning-progress curricula | Emergent multi-agent self-play, co-evolving curricula |
| **Reachability-Driven** | *— (fixed output manifold)* | Beam diversity, anti-repetition, KL-to-reference trust regions | Go-Explore, coverage-maximising curricula | Latent-space diversity bonuses, action-entropy regularisation | Role-diversity bonuses, anti-convergence on coordination topologies |



---
<br>



## 2. Levels 1–2: Responder → Reasoner — Reasoning-Space Exploration

The transition from **Responder** to **Reasoner** requires exploration in *reasoning space*: branching over token sequences, reasoning trajectories, and latent thought representations. The agent must search for informative hypotheses rather than simply produce reactive outputs.

<p align="center"><img src="fig/level1_reasoner.png" width="850"/></p>
<p align="center"><i>Figure: Levels 1–2 Reasoning-Space Exploration — Why (entropy escalation & reward stagnation), Where (tokens → turns → latent trajectories), and How (uncertainty / competence / reachability-driven).</i></p>

<br>

### 2.1 Uncertainty-Driven Exploration

Methods that prioritise exploration at high-uncertainty branching points in the reasoning process:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-08 | **CURE** | Expands the training-state distribution at critical decision points to sustain exploration | [CURE: Critical-Token-Guided Re-Concatenation for Entropy-Collapse Prevention](https://arxiv.org/pdf/2508.11016) | [![GitHub Stars](https://img.shields.io/github/stars/bytedance/CURE?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/bytedance/CURE) |
| 2026-03 | **SPINE** | Preserves exploration by selectively updating high-entropy branch tokens | [SPINE: Token-Selective Test-Time Reinforcement Learning with Entropy-Band Regularization](https://arxiv.org/abs/2511.17938) | - |
| 2025-06 | **TreeRL** | Explores reasoning via on-policy tree search from uncertain intermediate states | [TreeRL: LLM Reinforcement Learning with On-Policy Tree Search](https://arxiv.org/abs/2506.11902) | [![GitHub Stars](https://img.shields.io/github/stars/THUDM/TreeRL?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/THUDM/TreeRL) |
| 2025-09 | **CE-GPPO** | Sustains exploration by preserving clipped-token gradients | [CE-GPPO: Coordinating Entropy via Gradient-Preserving Clipping Policy Optimization in Reinforcement Learning](https://arxiv.org/pdf/2509.20712) | - |
| 2025-10 | **STEER** | Preserves exploration by stabilizing token-level entropy change through adaptive reweighting | [Rethinking Entropy Interventions in RLVR: An Entropy Change Perspective](https://arxiv.org/pdf/2510.10150) | [![GitHub Stars](https://img.shields.io/github/stars/zz-haooo/STEER?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/zz-haooo/STEER) 
| 2025-10 | **AEPO** | Breaks the exploration bottleneck by directly controlling policy entropy through temperature-guided REINFORCE | [Arbitrary Entropy Policy Optimization Breaks The Exploration Bottleneck of Reinforcement Learning](https://arxiv.org/pdf/2510.08141) | [![GitHub Stars](https://img.shields.io/github/stars/597358816/AEPO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/597358816/AEPO) |
| 2025-11 | **ICPO** | Promotes exploration by combining verifiable rewards with confidence-based preference advantages | [ICPO: Intrinsic Confidence-Driven Group Relative Preference Optimization for Efficient Reinforcement Learning](https://arxiv.org/abs/2511.21005) | - |
| 2026-02 | **REAL** | Stabilizes exploration via balanced gradient allocation | [Rewards as labels: Revisiting rlvr from a classification perspective](https://arxiv.org/pdf/2602.05630) | - |

<br>

### 2.2 Competence-Driven Exploration

Methods that match problem difficulty to the model's evolving competence frontier:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-06 | **E2H** | Guides exploration through an easy-to-hard curriculum | [Curriculum Reinforcement Learning from Easy to Hard Tasks Improves LLM Reasoning](https://arxiv.org/abs/2506.06632) | [![GitHub Stars](https://img.shields.io/github/stars/divelab/E2H-Reasoning?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/divelab/E2H-Reasoning) |
| 2025-10 | **RLAAR** | Steers exploration through curriculum learning and rewarded abstention | [Verifiable Accuracy and Abstention Rewards in Curriculum RL to Alleviate Lost-in-Conversation](https://arxiv.org/pdf/2510.18731) | - |
| 2025-05 | **CDAS** | Explores the competence frontier by sampling problems matched to the model’s current ability | [Rethinking the Sampling Criteria in Reinforcement Learning for LLM Reasoning: A Competence-Difficulty Alignment Perspective](https://arxiv.org/pdf/2505.17652) | [![GitHub Stars](https://img.shields.io/github/stars/DeyangKong/CDAS?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/DeyangKong/CDAS) |
| 2026-01 | **HA-DW** | Reduces exploration imbalance by debiasing group-relative advantages across prompt difficulty | [Your Group-Relative Advantage Is Biased](https://arxiv.org/abs/2601.08521) | - |
| 2025-08 | **SvS** | Sustains exploration by self-synthesizing diverse but answer-equivalent problems during RLVR | [Beyond Pass@1: Self-play with Variational Problem Synthesis Sustains RLVR](https://arxiv.org/pdf/2508.14029) | [![GitHub Stars](https://img.shields.io/github/stars/MasterVito/SvS?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/MasterVito/SvS) |

<br>

### 2.3 Reachability-Driven Exploration

Methods that prevent irreversible contraction of reasoning trajectory distributions:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-10 | **TROLL** | Stabilizes exploration with principled trust-region updates instead of PPO-style clipping | [TROLL: Trust Regions improve Reinforcement Learning for Large Language Models](https://arxiv.org/abs/2510.03817) | - |
| 2024-04 | **ROPO** | Preserves useful exploration by downweighting noisy preference signals instead of overfitting to them | [ROPO: Robust Preference Optimization for Large Language Models](https://arxiv.org/abs/2404.04102) | - |
| 2025-05 | **KTAE** | Explores better by assigning credit to key reasoning tokens rather than whole rollouts | [KTAE: A Model-Free Algorithm to Key-Tokens Advantage Estimation in Mathematical Reasoning](https://arxiv.org/abs/2505.16826) | [![GitHub Stars](https://img.shields.io/github/stars/ZNLP/KTAE?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ZNLP/KTAE.git) |
| 2025-08 | **VRPRM** | Guides exploration with visual step-level rewards that encourage deeper reasoning paths | [VRPRM: Process Reward Modeling via Visual Reasoning](https://arxiv.org/abs/2508.03556) | - |
| 2026-01 | **RLVRR** | Turns sparse end rewards into a verifiable reward chain that supports broader open-ended exploration | [From Verifiable Dot to Reward Chain: Harnessing Verifiable Reference-based Rewards for Reinforcement Learning of Open-ended Generation](https://arxiv.org/abs/2601.18533) | [![GitHub Stars](https://img.shields.io/github/stars/YJiangcm/RLVRR?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/YJiangcm/RLVRR) |




---

<br>





## 3. Level 3: Reasoner → Agent — Perception- & Action-Space Exploration

At Level 3, the agent crosses from internal reasoning into **situated interaction with external environments**. Exploration unfolds in perception and action space, where every step incurs real cost.

### 3.1 Digital Agents

Agents operating in software-mediated environments (web, APIs, code interpreters):

#### 3.1.1 Uncertainty-Driven Exploration

Methods that acquire information under partial observability by prioritising uncertain states, tool calls, or capability boundaries:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2026-01 | **JitRL** | Uses count-based uncertainty bonuses to explore unseen state-action pairs | [Just-In-Time Reinforcement Learning: Continual Learning in LLM Agents Without Gradient Updates](https://arxiv.org/abs/2601.18510) | [![GitHub Stars](https://img.shields.io/github/stars/liushiliushi/JitRL?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/liushiliushi/JitRL) |
| 2023-05 | **RAP** | Explores alternative reasoning paths with MCTS and UCB guidance | [Reasoning with Language Model is Planning with World Model](https://doi.org/10.18653/v1/2023.emnlp-main.507) | [![GitHub Stars](https://img.shields.io/github/stars/Ber666/RAP?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Ber666/RAP) |
| 2024-08 | **Agent Q** | Expands high-value action trajectories via MCTS-guided exploration | [Agent Q: Advanced Reasoning and Learning for Autonomous AI Agents](https://arxiv.org/abs/2408.07199) | - |
| 2023-10 | **LAST** | Explores reasoning-action branches through language-agent tree search | [Language Agent Tree Search Unifies Reasoning Acting and Planning in Language Models](https://arxiv.org/abs/2310.04406) | [![GitHub Stars](https://img.shields.io/github/stars/lapisrocks/LanguageAgentTreeSearch?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/lapisrocks/LanguageAgentTreeSearch) |
| 2025-04 | **KnowSelf** | Explores capability boundaries by detecting uncertain self-knowledge | [Agentic Knowledgeable Self-awareness](https://arxiv.org/abs/2504.03553) | [![GitHub Stars](https://img.shields.io/github/stars/zjunlp/KnowSelf?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/zjunlp/KnowSelf) |
| 2025-01 | **Search-o1** | Explores external evidence when reasoning exposes knowledge uncertainty | [Search-o1: Agentic Search-Enhanced Large Reasoning Models](https://doi.org/10.18653/v1/2025.emnlp-main.276) | [![GitHub Stars](https://img.shields.io/github/stars/RUC-NLPIR/Search-o1?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/RUC-NLPIR/Search-o1) |
| 2025-04 | **TTRL** | Test-time RL via majority-voted pseudo-rewards turns inference disagreement into exploration | [TTRL: Test-Time Reinforcement Learning](https://arxiv.org/abs/2504.16084) | - |

#### 3.1.2 Competence-Driven Exploration

Methods that tame combinatorial tool-use spaces through curricula, process-level credit assignment, and self-generated training tasks:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-08 | **PilotRL** | Stages curricula to expand agent exploration from planning to tool use | [PilotRL: Training Language Model Agents via Global Planning-Guided Progressive Reinforcement Learning](https://arxiv.org/abs/2508.00344) | - |
| 2025-09 | **ReSum-GRPO** | Sustains long-horizon search exploration through context summarization | [ReSum: Unlocking Long-Horizon Search Intelligence via Context Summarization](https://arxiv.org/abs/2509.13313) | - |
| 2024-03 | **ETO** | Optimizes exploratory trial-and-error trajectories for agent learning | [Trial and Error: Exploration-Based Trajectory Optimization for LLM Agents](https://arxiv.org/abs/2403.02502) | [![GitHub Stars](https://img.shields.io/github/stars/Yifan-Song793/ETO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Yifan-Song793/ETO) |
| 2024-11 | **WebRL** | Self-evolving online curriculum from failure trajectories for web agents | [WebRL: Training LLM Web Agents via Self-Evolving Online Curriculum RL](https://arxiv.org/abs/2411.02337) | - |
| 2025-09 | **Planner-R1** | Uses dense process rewards to steer exploration toward feasible plans | [Planner-R1: Reward Shaping Enables Efficient Agentic RL with Smaller LLMs](https://arxiv.org/abs/2509.25779) | - |
| 2025-08 | **RLTR** | Rewards complete tool-use processes to improve exploratory planning | [Encouraging Good Processes Without the Need for Good Answers: Reinforcement Learning for LLM Agent Planning](https://arxiv.org/abs/2508.19598) | - |
| 2025-04 | **ReTool** | RL rewards strategic tool-invocation patterns, penalises redundant calls | [ReTool: Reinforcement Learning for Strategic Tool Use in LLMs](https://arxiv.org/abs/2504.11536) | - |
| 2025-05 | **GiGPO** | Assigns state-level credit across grouped rollouts for exploration | [Group-in-Group Policy Optimization for LLM Agent Training](https://arxiv.org/abs/2505.10978) | [![GitHub Stars](https://img.shields.io/github/stars/langfengQ/verl-agent?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/langfengQ/verl-agent) |
| 2025-11 | **Agent0-VL** | Evolves tool-integrated exploration through repeated reasoning cycles | [Agent0-VL: Exploring Self-Evolving Agent for Tool-Integrated Vision-Language Reasoning](https://arxiv.org/abs/2511.19900) | [![GitHub Stars](https://img.shields.io/github/stars/aiming-lab/Agent0?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/aiming-lab/Agent0) |
| 2025-05 | **Absolute Zero** | Uses proposer-solver self-play to explore new reasoning tasks | [Absolute Zero: Reinforced Self-play Reasoning with Zero Data](https://arxiv.org/abs/2505.03335) | [![GitHub Stars](https://img.shields.io/github/stars/LeapLabTHU/Absolute-Zero-Reasoner?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/LeapLabTHU/Absolute-Zero-Reasoner) |

#### 3.1.3 Reachability-Driven Exploration

Methods that preserve behavioural flexibility by regulating entropy or injecting useful off-policy experience:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-08 | **EGPO** | Adds entropy bonuses to encourage exploration in function-call reasoning | [Reasoning through Exploration: A Reinforcement Learning Framework for Robust Function Calling](https://arxiv.org/abs/2508.05118) | [![GitHub Stars](https://img.shields.io/github/stars/BingguangHao/RLFC?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/BingguangHao/RLFC) |
| 2025-09 | **EPO** | Regularizes entropy to sustain exploration in multi-turn agent RL | [EPO: Entropy-regularized Policy Optimization for LLM Agents Reinforcement Learning](https://arxiv.org/abs/2509.22576) | [![GitHub Stars](https://img.shields.io/github/stars/WujiangXu/EPO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/WujiangXu/EPO) |
| 2025-09 | **ENTROPO** | Uses entropy-enhanced preferences to diversify coding-agent exploration | [Building Coding Agents via Entropy-Enhanced Multi-Turn Preference Optimization](https://arxiv.org/abs/2509.12434) | - |
| 2026-03 | **RAPO** | Expands policy exploration with retrieval-augmented experience | [RAPO: Expanding Exploration for LLM Agents via Retrieval-Augmented Policy Optimization](https://arxiv.org/abs/2603.03078) | - |
| 2026-04 | **E³-TIR** | Branches from high-entropy prefixes to exploit exploratory experience | [E3-TIR: Enhanced Experience Exploitation for Tool-Integrated Reasoning](https://arxiv.org/abs/2604.09455) | [![GitHub Stars](https://img.shields.io/github/stars/yuki-younai/E3-TIR?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yuki-younai/E3-TIR) |

<br>

### 3.2 Embodied Agents

<p align="center"><img src="fig/level3_embodied.png" width="850"/></p>
<p align="center"><i>Figure: Level 3 Embodied Agent Exploration — Uncertainty-driven active perception, competence-driven navigation & RL & test-time compute, and reachability-driven reward engineering & constrained safety.</i></p>

Embodied agents operate in continuous, high-dimensional action spaces where every physical interaction consumes time, energy, and mechanical wear, and many actions are irreversible. The three exploration paradigms adapt to this setting as follows:

#### 3.2.1 Uncertainty-Driven Exploration

Before executing complex plans in open-ended environments, agents must overcome severe partial observability by actively controlling their sensors to maximise information gain, eliminating cognitive blind spots.

**Geometric & high-fidelity reconstruction.** Viewpoint selection for active mapping, information-theoretic coverage, and ensemble-disagreement-based exploration of dynamics.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2018-10 | **MAX** | Ensemble-disagreement drives active exploration of dynamics | [Model-Based Active Exploration](https://arxiv.org/abs/1810.12162) | [![GitHub Stars](https://img.shields.io/github/stars/nnaisense/MAX?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/nnaisense/MAX) |
| 2020-04 | **Active Neural SLAM** | Coverage-maximising hierarchical policies explore unknown occupancy maps | [Learning To Explore Using Active Neural SLAM](https://arxiv.org/abs/2004.05155) | [![GitHub Stars](https://img.shields.io/github/stars/devendrachaplot/Neural-SLAM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/devendrachaplot/Neural-SLAM) |
| 2021-03 | **APT** | Non-parametric entropy maximisation for unsupervised active pre-training | [Behavior From the Void: Unsupervised Active Pre-Training](https://arxiv.org/abs/2103.04551) | [![GitHub Stars](https://img.shields.io/github/stars/rll-research/url_benchmark?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/rll-research/url_benchmark) |
| 2023-12 | **Model-Free Active Exploration** | Information-theoretic lower-bound approximation for ensemble-based exploration | [Model-Free Active Exploration in Reinforcement Learning](https://proceedings.neurips.cc/paper_files/paper/2023/hash/a9f8d5a20d4d12f04b84fb8cd61c0800-Abstract-Conference.html) | - |
| 2024-10 | **ActiveSplat** | Gaussian-splat viewpoint exploration maximises reconstruction fidelity under a time budget | [ActiveSplat: High-Fidelity Scene Reconstruction through Active Gaussian Splatting](https://arxiv.org/abs/2410.21955) | [![GitHub Stars](https://img.shields.io/github/stars/Li-Yuetao/ActiveSplat?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Li-Yuetao/ActiveSplat) |

**Semantic & multi-modal active inference.** Probing the environment to disambiguate alternative scene-graph completions or to gather cross-modal (audio / language) evidence.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2023-11 | **Conan** | Active interactive exploration as Bayesian query to disambiguate latent scene state | [Active Reasoning in an Open-World Environment](https://arxiv.org/abs/2311.02018) | [![GitHub Stars](https://img.shields.io/github/stars/ariesssxu/Conan-Active-Reasoning?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ariesssxu/Conan-Active-Reasoning) |
| 2024-04 | **ActiveRIR** | Cross-modal audio-visual exploration for acoustic scene mapping (room impulse responses) | [ActiveRIR: Active Audio-Visual Exploration for Building Room Impulse Responses](https://arxiv.org/abs/2404.16216) | - |
| 2025-10 | **Active Semantic Perception** | Entropy-driven exploration over LLM-sampled scene graph hypotheses | [Active Semantic Perception](https://arxiv.org/abs/2510.05430) | [![GitHub Stars](https://img.shields.io/github/stars/grasp-lyrl/active_semantic_perception?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/grasp-lyrl/active_semantic_perception) |

#### 3.2.2 Competence-Driven Exploration

Competence-driven exploration spans two tightly coupled phases: the agent must first **navigate** to task-relevant states, then **manipulate** the environment to achieve its objectives. Both push beyond pre-trained priors at the frontier between what the agent can already do and what it cannot yet do.

**Objective-driven navigation.** Translating high-level language goals into executable subgoals and using semantic representations to prune the spatial search manifold.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2022-04 | **SayCan** | Affordance value-function reweights LLM-proposed action exploration | [Do As I Can, Not As I Say: Grounding Language in Robotic Affordances](https://arxiv.org/abs/2204.01691) | [![GitHub Stars](https://img.shields.io/github/stars/google-research/google-research?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/google-research/google-research) |
| 2022-07 | **Inner Monologue** | Closed-loop replanning via inner-speech feedback re-explores failed plans | [Inner Monologue: Embodied Reasoning through Planning with Language Models](https://arxiv.org/abs/2207.05608) | - |
| 2022-07 | **LM-Nav** | Goal-directed exploration over LLM-annotated topological graphs | [LM-Nav: Robotic Navigation with Large Pre-Trained Models of Language, Vision, and Action](https://arxiv.org/abs/2207.04429) | [![GitHub Stars](https://img.shields.io/github/stars/blazejosinski/lm_nav?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/blazejosinski/lm_nav) |
| 2022-10 | **VLMaps** | Open-vocabulary visual-language maps guide language-conditioned spatial exploration | [Visual Language Maps for Robot Navigation](https://arxiv.org/abs/2210.05714) | [![GitHub Stars](https://img.shields.io/github/stars/vlmaps/vlmaps?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/vlmaps/vlmaps) |
| 2023-10 | **LFG** | LLM semantic-priors prune frontier exploration toward goal-relevant regions | [Language Frontier Guide: LLM-Based Semantic Priors for Exploration](https://arxiv.org/abs/2310.10103) | [![GitHub Stars](https://img.shields.io/github/stars/Michael-Equi/lfg-nav?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Michael-Equi/lfg-nav) |
| 2024-10 | **Fisher-Info Planning** | MLLM-guided exploration balancing information gain vs. localisation risk (Fisher information) | [Multimodal LLM Guided Exploration and Active Mapping using Fisher Information](https://arxiv.org/abs/2410.17422) | [![GitHub Stars](https://img.shields.io/github/stars/JiangWenPL/multimodal-active?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/JiangWenPL/multimodal-active) |

**RL for VLA policy exploration.** Safely expanding manipulation boundaries via offline RL, online PPO/GRPO, and hybrid offline-to-online fine-tuning on Vision-Language-Action architectures.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2023-03 | **Cal-QL** | Calibrated offline value exploration enabling safe online fine-tuning | [Cal-QL: Calibrated Offline RL Pre-Training for Efficient Online Fine-Tuning](https://arxiv.org/abs/2303.05479) | - |
| 2023-09 | **Q-Transformer** | Scales autoregressive value-based exploration to static multi-task trajectories | [Q-Transformer: Scalable Offline RL via Autoregressive Q-Functions](https://arxiv.org/abs/2309.10150) | - |
| 2024-09 | **DPPO** | Formulates denoising trajectories as auxiliary MDP for stable PPO on diffusion policies | [Diffusion Policy Policy Optimization](https://arxiv.org/abs/2409.00588) | [![GitHub Stars](https://img.shields.io/github/stars/irom-princeton/dppo?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/irom-princeton/dppo) |
| 2024-09 | **FLaRe** | Large-scale online RL fine-tuning exploration on pretrained VLAs | [FLaRe: Achieving Masterful and Adaptive Robot Policies with Large-Scale RL Fine-Tuning](https://arxiv.org/abs/2409.16578) | [![GitHub Stars](https://img.shields.io/github/stars/JiahengHu/FLaRe?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/JiahengHu/FLaRe) |
| 2024-10 | **HIL-SERL** | Sample-efficient on-robot RL with human-in-the-loop interventions for dexterous tasks | [Precise and Dexterous Robotic Manipulation via Human-in-the-Loop RL](https://arxiv.org/abs/2410.21845) | [![GitHub Stars](https://img.shields.io/github/stars/rail-berkeley/hil-serl?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/rail-berkeley/hil-serl) |
| 2024-11 | **GRAPE** | Preference-aligned exploration generalises VLA policies to novel scenarios | [GRAPE: Generalizing Robot Policy via Preference Alignment](https://arxiv.org/abs/2411.19309) | - |
| 2025-02 | **ConRFT** | Consistency-regularised offline-to-online exploration (HIL-SERL + consistency) for diffusion VLA | [ConRFT: A Reinforced Fine-tuning Method for VLA Models via Consistency Policy](https://arxiv.org/abs/2502.05450) | [![GitHub Stars](https://img.shields.io/github/stars/cccedric/conrft?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/cccedric/conrft) |
| 2025-05 | **ReinboT** | RL amplifies VLA manipulation exploration via reward-guided offline alignment | [ReinboT: Amplifying Robot Visual-Language Manipulation with Reinforcement Learning](https://arxiv.org/abs/2505.07395) | [![GitHub Stars](https://img.shields.io/github/stars/COST-97/reinboT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/COST-97/reinboT) |
| 2025-05 | **VLA-RL** | Scalable PPO-based online action-space exploration for VLA policies | [VLA-RL: Towards Masterful and General Robotic Manipulation with Scalable RL](https://arxiv.org/abs/2505.18719) | [![GitHub Stars](https://img.shields.io/github/stars/GuanxingLu/vlarl?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/GuanxingLu/vlarl) |
| 2025-09 | **SimpleVLA-RL** | GRPO group-relative exploration scales VLA skill acquisition | [SimpleVLA-RL: Scaling VLA Training via Reinforcement Learning](https://arxiv.org/abs/2509.09674) | [![GitHub Stars](https://img.shields.io/github/stars/PRIME-RL/SimpleVLA-RL?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/PRIME-RL/SimpleVLA-RL) |
| 2025-09 | **Dual-Actor FT** | Dual-actor decoupling of exploration vs. exploitation for stable offline-to-online RL | [Dual-Actor Fine-Tuning of VLA Models](https://arxiv.org/abs/2509.13774) | - |
| 2025-10 | **π_RL** | First online PPO/GRPO RL fine-tuning for flow-matching VLA | [πRL: Online RL Fine-Tuning for Flow-Based Vision-Language-Action Models](https://arxiv.org/abs/2510.25889) | - |
| 2025-11 | **SRPO** | Self-refined exploration bridging static data and online rollouts | [SRPO: Self-Refined Policy Optimization for VLA](https://arxiv.org/abs/2511.15605) | [![GitHub Stars](https://img.shields.io/github/stars/SUSTechBruce/SRPO_MLLMs?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/SUSTechBruce/SRPO_MLLMs) |
| 2025-11 | **π*₀.₆** | Flow-matching VLA that learns from online experience via offline RL | [π*₀.₆: A VLA That Learns From Experience](https://arxiv.org/abs/2511.14759) | - |
| 2025-11 | **WMPO** | Pure world-model PPO enables safe online action-space exploration for VLA | [WMPO: World Model-Based Policy Optimization for VLA](https://arxiv.org/abs/2511.09515) | - |
| 2026-01 | **SOP** | Scalable online post-training infrastructure for fleet-scale VLA exploration | [SOP: Scalable Online Post-training for Generalist VLA Models](https://arxiv.org/abs/2601.03044) | - |
| 2026-02 | **GigaBrain-0.5M** | Foundation VLA learned directly from world-model-based RL at fleet scale | [GigaBrain-0.5M*: A VLA That Learns From World Model-Based RL](https://arxiv.org/abs/2602.12099) | - |
| 2026-04 | **π₀.₇** | Steerable flow VLA trained with diverse multimodal context for out-of-the-box generalist skills | [π₀.₇: a Steerable Generalist Robotic Foundation Model with Emergent Capabilities](https://arxiv.org/abs/2604.15483) | - |

**Test-time compute & cognitive search.** Moving the exploration burden from training to deployment via MCTS, flow-guided steering, test-time RL, and "System-2" deliberation before physical execution.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2024-10 | **V-GPS** | Offline value guidance steers generalist AR / diffusion VLA decoding at test time | [Steering Your Generalists: Improving Robotic Foundation Models via Value Guidance](https://arxiv.org/abs/2410.13816) | - |
| 2025-05 | **Hume** | System-2 deliberative exploration via continuous flow value guidance | [Hume: Introducing System-2 Thinking in Visual-Language-Action Model](https://arxiv.org/abs/2505.21432) | [![GitHub Stars](https://img.shields.io/github/stars/hume-vla/hume?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/hume-vla/hume) |
| 2025-08 | **MB-Search VLA** | Model-based MCTS over AR / Diffusion VLA imagines trajectories before acting | [Improving Pre-Trained VLA Policies with Model-Based Search](https://arxiv.org/abs/2508.12211) | - |
| 2025-09 | **VLA-Reasoner** | MCTS imagination-time exploration over autoregressive action trajectories | [VLA-Reasoner: Empowering VLA Models via Test-Time Monte Carlo Tree Search](https://arxiv.org/abs/2509.22643) | - |
| 2025-11 | **DeepThinkVLA** | Slow-thinking test-time exploration through deliberate chain-of-action reasoning | [DeepThink-VLA: From Language Reasoning to Action Reasoning](https://arxiv.org/abs/2511.15669) | [![GitHub Stars](https://img.shields.io/github/stars/OpenBMB/DeepThinkVLA?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/OpenBMB/DeepThinkVLA) |
| 2025-12 | **TACO** | Anti-exploration test-time steering via continuous normalising flows | [TACO: Steering VLA Models at Test-Time via Anti-Exploration](https://arxiv.org/abs/2512.02834) | [![GitHub Stars](https://img.shields.io/github/stars/breez3young/TACO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/breez3young/TACO) |
| 2026-01 | **TT-VLA** | Value-free on-the-fly test-time RL adapts VLA policies per-episode | [Test-Time VLA: On-the-Fly Adaptation for Embodied Policies](https://arxiv.org/abs/2601.06748) | - |
| 2026-02 | **Recurrent-Depth VLA** | Implicit test-time compute scaling via latent iterative reasoning (no explicit tokens) | [Recurrent-Depth VLA: Implicit Test-Time Compute Scaling of VLA via Latent Iterative Reasoning](https://arxiv.org/abs/2602.07845) | - |

#### 3.2.3 Reachability-Driven Exploration

Defining *what* to explore and preventing exploration from irreversibly foreclosing future options are the central reachability challenges for embodied agents.

**Automated reward engineering & curiosity.** LLM-driven reward synthesis and curiosity / curriculum mechanisms sustain broad exploration incentives in unbounded physical manifolds.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2018-10 | **RND** | Curiosity-driven exploration bonus via random network distillation | [Exploration by Random Network Distillation](https://arxiv.org/abs/1810.12894) | [![GitHub Stars](https://img.shields.io/github/stars/openai/random-network-distillation?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/openai/random-network-distillation) |
| 2020-02 | **Never Give Up** | Episodic + lifelong novelty bonuses sustain directed exploration across long horizons | [Never Give Up: Learning Directed Exploration Strategies](https://arxiv.org/abs/2002.06038) | - |
| 2023-06 | **Language-to-Rewards** | LLM synthesises dense language-conditioned reward for skill exploration | [Language to Rewards for Robotic Skill Synthesis](https://arxiv.org/abs/2306.08647) | [![GitHub Stars](https://img.shields.io/github/stars/google-deepmind/language_to_reward_2023?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/google-deepmind/language_to_reward_2023) |
| 2023-10 | **Eureka** | LLM-synthesised executable reward code evolves the explorable task manifold | [Eureka: Human-Level Reward Design via Coding Large Language Models](https://arxiv.org/abs/2310.12931) | [![GitHub Stars](https://img.shields.io/github/stars/eureka-research/eureka?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/eureka-research/eureka) |
| 2024-09 | **CurricuLLM** | LLM-designed curricula for progressive exploration of hard manipulation skills | [CurricuLLM: Automatic Task Curricula Design for Learning Complex Robot Skills using LLMs](https://arxiv.org/abs/2409.18382) | [![GitHub Stars](https://img.shields.io/github/stars/labicon/CurricuLLM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/labicon/CurricuLLM) |
| 2025-05 | **TeViR** | Text-to-video diffusion rewards enable efficient sparse-task exploration | [TeViR: Text-to-Video Reward with Diffusion Models for Efficient RL](https://arxiv.org/abs/2505.19769) | - |

**Constrained safety.** Learned safety zones, recovery policies, and hard safety constraints bound trajectories while preserving the agent's reachable state set.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2020-10 | **Recovery RL** | Learned recovery zones bound exploration without collapsing reachable set | [Recovery RL: Safe Reinforcement Learning with Learned Recovery Zones](https://arxiv.org/abs/2010.15920) | [![GitHub Stars](https://img.shields.io/github/stars/abalakrishna123/recovery-rl?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/abalakrishna123/recovery-rl) |
| 2024-04 | **RECOVER** | Neuro-symbolic failure detection bounds exploratory trajectories in manipulation | [RECOVER: Neuro-Symbolic Failure Recovery for Robotic Manipulation](https://arxiv.org/abs/2404.00756) | - |
| 2025-03 | **SafeVLA** | Constrained policy exploration under hard safety guarantees for VLA | [SafeVLA: Towards Safety Alignment of VLA Model via Constrained Learning](https://arxiv.org/abs/2503.03480) | [![GitHub Stars](https://img.shields.io/github/stars/PKU-Alignment/SafeVLA?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/PKU-Alignment/SafeVLA) |


---

<br>

## 4. Level 4: Agent → Prospector — Imagination-Space Exploration
<p align="center"><img src="fig/level4_worldmodel.png" width="850"/></p>
<p align="center"><i>Figure: Level 4 Imagination-Space Exploration — Why (the dual exploration problem), Where (simulated rollouts, hazard zones, latent value landscapes), and How (MBRL, video generation, autonomous driving, social dynamics)</i></p>

The Prospector internalises a **world model** and faces a **dual exploration problem**: simultaneously gathering real data to refine world model fidelity AND searching imagined trajectories to extract policies.

---

### 4.1 Why: The Dual Exploration Problem

#### 4.1.1 Compounding Errors and Reality Drift

World models act as recursive self-simulators where infinitesimal single-step errors compound exponentially over long imagined horizons, causing mental simulations to catastrophically diverge from reality. Agents must proactively probe epistemic boundaries and gather adversarial data that anchors "dreams" to physical constraints.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2023-01 | **DreamerV3**          | Explores long imagined rollouts with entropy-regularised actor to prevent premature convergence in sparse-reward settings | [Mastering Diverse Domains through World Models](https://arxiv.org/abs/2301.04104) | [![GitHub Stars](https://img.shields.io/github/stars/danijar/dreamerv3?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/danijar/dreamerv3)       |
| 2019-06 | **MBPO**               | Limits imagined rollout length to prevent compounding error accumulation; iterative policy–model alternation drives exploration of true dynamics | [When to Trust Your Model: Model-Based Policy Optimization](https://arxiv.org/abs/1906.08253) | [![GitHub Stars](https://img.shields.io/github/stars/jannerm/mbpo?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/jannerm/mbpo)            |
| 2018-05 | **PETS**               | Ensemble of probabilistic networks quantifies epistemic uncertainty; explores regions where ensemble predictions most disagree to anchor model to reality | [Deep Reinforcement Learning in a Handful of Trials using Probabilistic Dynamics Models](https://arxiv.org/abs/1805.12114) | [![GitHub Stars](https://img.shields.io/github/stars/kchua/handful-of-trials?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/kchua/handful-of-trials) |
| 2018-07 | **SLBO**               | Constructs return lower bound jointly optimised over policy and model; optimism under uncertainty encourages exploration of under-covered state–action regions | [Algorithmic Framework for Model-based Deep Reinforcement Learning with Theoretical Guarantees](https://arxiv.org/abs/1807.03858) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/slbo?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/slbo)   |
| 2018-07 | **STEVE**              | Stochastic ensemble value expansion explicitly propagates epistemic uncertainty across multi-step imagined rollouts… | [Sample-Efficient Reinforcement Learning with Stochastic Ensemble Value Expansion](https://arxiv.org/abs/1807.01675) | -                                                          |
| 2025-12 | **Long-Horizon MBRL**  | Identifies compounding error as the core bottleneck in offline long-horizon model-based RL… | [Long-Horizon Model-Based Offline Reinforcement Learning Without Conservatism](https://arxiv.org/abs/2512.04341) | [![GitHub Stars](https://img.shields.io/github/stars/twni2016/neubay?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/twni2016/neubay)         |
| 2025-12 | **Surprise-Robust WM** | Trains world models to explicitly handle out-of-distribution "surprise" inputs; surprise-resilient training reduces catastrophic reality drift when imagination enters unexplored regions of state space | [World Model Robustness via Surprise Recognition](https://arxiv.org/abs/2512.01119) | [![GitHub Stars](https://img.shields.io/github/stars/Bluefin-Tuna/WISER?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Bluefin-Tuna/WISER)      |


#### 4.1.2 The Noise-Hijacking Trap

Curiosity-driven agents waste exploration budgets on irreducible stochasticity (noisy-TV problem) rather than informative states. Disentangling aleatoric from epistemic uncertainty via reachability metrics and learning-progress monitoring is essential.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2020-05 | **Plan2Explore**                   | Maximises future ensemble disagreement in latent space for task-agnostic exploration; disagreement targets epistemic uncertainty, not irreducible noise | [Planning to Explore via Self-Supervised World Models](https://arxiv.org/abs/2005.05960) | [![GitHub Stars](https://img.shields.io/github/stars/ramanans1/plan2explore?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ramanans1/plan2explore)             |
| 2020-06 | **RIDES**                          | Reward-weighted state-reachability intrinsic motivation separates reachable novel states from high-entropy irreducible noise | [Active World Model Learning with Progress Curiosity](https://arxiv.org/abs/2007.07853) | [![GitHub Stars](https://img.shields.io/github/stars/MarcCote/thinker?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/MarcCote/thinker)                   |
| 2018-08 | **RND**                            | Random network distillation as epistemic novelty signal; highlights persistent failure to distinguish aleatoric from epistemic uncertainty in stochastic envs | [Exploration by Random Network Distillation](https://arxiv.org/abs/1810.12894) | [![GitHub Stars](https://img.shields.io/github/stars/openai/random-network-distillation?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/openai/random-network-distillation) |
| 2017-05 | **ICM**                            | Curiosity via self-supervised inverse/forward dynamics; forward-model prediction error as intrinsic reward to explore informative state transitions | [Curiosity-driven Exploration by Self-supervised Prediction](https://arxiv.org/abs/1705.05363) | [![GitHub Stars](https://img.shields.io/github/stars/pathak22/noreward-rl?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/pathak22/noreward-rl)               |
| 2025-09 | **Beyond Noisy-TVs**               | Systematically categorises sources of stochastic noise in exploration environments… | [Beyond Noisy-TVs: Noise-Robust Exploration Via Learning Progress Monitoring](https://arxiv.org/abs/2509.25438) | [![GitHub Stars](https://img.shields.io/github/stars/Akuna23Matata/LPM_exploration?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Akuna23Matata/LPM_exploration)      |
| 2017-11 | **Bayesian Uncertainties**         | Canonical treatment of aleatoric vs. epistemic uncertainty in deep networks… | [What Uncertainties Do We Need in Bayesian Deep Learning for Computer Vision?](https://arxiv.org/abs/1703.04977) | -                                                                     |
| 2019-10 | **Model-Based Active Exploration** | Explicitly optimises for epistemic information gain rather than prediction novelty… | [Model-Based Active Exploration](https://arxiv.org/abs/1810.12162) | [![GitHub Stars](https://img.shields.io/github/stars/nnaisense/MAX?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/nnaisense/MAX)                      |


#### 4.1.3 Fatal Detail Loss in Latent Space

Aggressive compression of high-dimensional sensory streams loses safety-critical details (motor vibrations, slippery surfaces, grip deformations). Physical stress-testing and structured latent representations force world models to encode functionally critical geometric realities.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2019-02 | **PlaNet**       | RSSM with deterministic + stochastic latent components; stochastic branch explores multiple plausible states rather than collapsing to a single deterministic prediction | [Learning Latent Dynamics for Planning from Pixels](https://arxiv.org/abs/1811.04551) | [![GitHub Stars](https://img.shields.io/github/stars/google-research/planet?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/google-research/planet) |
| 2018-03 | **World Models** | V–M–C architecture compresses pixels to latent then explores futures via RNN-based mental simulation; highlights information loss from pure deterministic latents | [World Models](https://arxiv.org/abs/1803.10122) | [![GitHub Stars](https://img.shields.io/github/stars/hardmaru/worldmodels?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/hardmaru/worldmodels)   |
| 2023-04 | **I-JEPA**       | Image Joint-Embedding Predictive Architecture… | [Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture](https://arxiv.org/abs/2301.08243) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/ijepa?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/ijepa) |


<br>

### 4.2 Where: Exploration Across Different Spaces

#### 4.2.1 Simulated Future Rollouts

Agents generate imagined trajectories to discover effective behaviours before physical execution, exploiting computational parallelism — thousands of hypothetical scenarios per second.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-09 | **DreamerV4**           | Shared world-model/policy backbone with phased training; first agent to obtain Minecraft diamonds from offline data via exhaustive imagined rollouts | [Training Agents Inside of Scalable World Models](https://arxiv.org/abs/2509.24527)                | -                                                               |
| 2020-11 | **MuZero**              | Learns latent dynamics supporting MCTS planning without pixel reconstruction; achieves superhuman performance by planning over imagined state sequences | [Mastering Atari, Go, Chess and Shogi by Planning with a Learned Model](https://arxiv.org/abs/1911.08265)                | [![GitHub Stars](https://img.shields.io/github/stars/werner-duvaud/muzero-general?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/werner-duvaud/muzero-general) |
| 2019-12 | **DreamerV1**           | RSSM-based latent world model; explores via action noise during environment interaction to broaden state-space coverage for model training | [Dream to Control: Learning Behaviors by Latent Imagination](https://arxiv.org/abs/1912.01603)                | [![GitHub Stars](https://img.shields.io/github/stars/danijar/dreamer?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/danijar/dreamer)              |
| 2020-10 | **DreamerV2**           | Discrete categorical latents + entropy-regularised actor; entropy bonus is explicit exploration regulariser preventing premature behavioural convergence | [Mastering Atari with Discrete World Models](https://arxiv.org/abs/2010.02193)                | [![GitHub Stars](https://img.shields.io/github/stars/danijar/dreamerv2?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/danijar/dreamerv2)            |
| 2019-03 | **Atari 100k (SimPLe)** | First video-prediction world model competitive with model-free RL at 100k environment steps; imagined rollouts from pixel-based world model enable sample-efficient exploration of Atari games | [Model-Based Reinforcement Learning for Atari](https://arxiv.org/abs/1903.00374)                | [![GitHub Stars](https://img.shields.io/github/stars/tensorflow/tensor2tensor?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/tensorflow/tensor2tensor)     |
| 2026-01 | **Ctrl-World**          | Controllable world model with structured latent decomposition… | [Ctrl-World: Controllable World Models with Structured Latent Decomposition (OpenReview)](https://openreview.net/forum?id=ctrl-world-2026) | [![GitHub Stars](https://img.shields.io/github/stars/Robert-gyj/Ctrl-World?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Robert-gyj/Ctrl-World)        |


#### 4.2.2 Counterfactual Hazard Zones

Safety-critical exploration probes operational failure boundaries before physical deployment; world models evaluate "what-if" counterfactuals without incurring real-world risk.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2023-01 | **DayDreamer** | Transfers Dreamer latent-imagination to physical robots; explores counterfactual hardware interactions in latent space before committing to unsafe real actions | [DayDreamer: World Models for Physical Robot Learning](https://arxiv.org/abs/2206.14176) | [![GitHub Stars](https://img.shields.io/github/stars/danijar/daydreamer?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/danijar/daydreamer)      |
| 2018-05 | **PETS**       | Probabilistic ensemble models epistemic uncertainty for planning; agents probe high-uncertainty regions to discover failure modes before physical execution | [Deep Reinforcement Learning in a Handful of Trials using Probabilistic Dynamics Models](https://arxiv.org/abs/1805.12114) | [![GitHub Stars](https://img.shields.io/github/stars/kchua/handful-of-trials?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/kchua/handful-of-trials) |
| 2024-10 | **ActSafe**    | Active safe exploration via worst-case trajectory imagination; uses constrained world model rollouts to identify unsafe counterfactual outcomes before committing to any real action | [ActSafe: Active Exploration with Safety Constraints for Reinforcement Learning](https://arxiv.org/abs/2410.09486) | [![GitHub Stars](https://img.shields.io/github/stars/yardenas/actsafe?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yardenas/actsafe)        |
| 2025-04 | **BUMEx**      | Boundary-uncertainty model exploration: identifies safety-critical boundary regions in the world model's state space and actively probes them with imagined counterfactual rollouts to discover latent… | [Smart Exploration in Reinforcement Learning using Bounded Uncertainty Models](https://arxiv.org/abs/2504.05978) | [![GitHub Stars](https://img.shields.io/github/stars/JvHulst/BUMEX?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/JvHulst/BUMEX)           |


#### 4.2.3 Latent Value Landscapes

In sparse-reward settings, agents construct internal value landscapes through intrinsic motivation, turning world-model predictive errors into exploration bonuses that guide search toward informative states.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2020-05 | **Plan2Explore**                   | World model ensemble disagreement as intrinsic reward; constructs a latent value landscape rewarding states where model uncertainty is highest | [Planning to Explore via Self-Supervised World Models](https://arxiv.org/abs/2005.05960) | [![GitHub Stars](https://img.shields.io/github/stars/ramanans1/plan2explore?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ramanans1/plan2explore)             |
| 2020-06 | **RIDES**                          | Reachability-weighted novelty bonus sculpts intrinsic value landscape to emphasise informative and accessible states | [Active World Model Learning with Progress Curiosity](https://arxiv.org/abs/2007.07853) | -                                                                     |
| 2018-10 | **RND**                            | Forward model prediction error on random network as novelty signal; constructs a pseudo-value landscape for count-free exploration in high-dimensional spaces | [Exploration by Random Network Distillation](https://arxiv.org/abs/1810.12894) | [![GitHub Stars](https://img.shields.io/github/stars/openai/random-network-distillation?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/openai/random-network-distillation) |
| 2017-05 | **ICM**                            | Self-supervised curiosity: forward-model error in latent feature space as exploration bonus, ignoring unpredictable environmental noise | [Curiosity-driven Exploration by Self-supervised Prediction](https://arxiv.org/abs/1705.05363) | [![GitHub Stars](https://img.shields.io/github/stars/pathak22/noreward-rl?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/pathak22/noreward-rl)               |
| 2025-03 | **Curiosity-Driven Imagination**   | Curiosity bonus directly inside the latent imagination loop: world model generates diverse hypothetical futures and rewards the agent for imagining states with high latent novelty, sculpting an… | [Curiosity-Driven Imagination: Discovering Plan Operators and Learning Associated Policies for Open-World Adaptation](https://arxiv.org/abs/2503.04931) | [![GitHub Stars](https://img.shields.io/github/stars/lorangpi/PRM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/lorangpi/PRM)                       |
| 2025-10 | **General Exploratory Bonus**      | Unified framework for count-free exploration bonuses in latent space… | [General Exploratory Bonus for Optimistic Exploration in RLHF](https://arxiv.org/abs/2510.03269) | [![GitHub Stars](https://img.shields.io/github/stars/WindyLee0822/GEB?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/WindyLee0822/GEB)                   |
| 2026-01 | **SuS (Surprise-based Successor)** | Surprise-modulated successor representations for exploration… | [SuS: Strategy-aware Surprise for Intrinsic Exploration](https://arxiv.org/abs/2601.10349) | [![GitHub Stars](https://img.shields.io/github/stars/mariklolik/sus?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/mariklolik/sus)                     |


#### 4.2.4 Action-Grounded Latent Manifolds

Latent spaces must be action-grounded "Embodied-Native" manifolds — every imagined future tightly coupled with executable motor commands — enabling structural robustness over purely visual manifolds.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-06 | **V-JEPA 2**  | Video-pretrained JEPA model enabling zero-shot robotic grasping; explores action-grounded latent manifold via abstract representation rather than pixel reconstruction | [V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning](https://arxiv.org/abs/2506.09985) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/jepa?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/jepa)               |
| 2025-06 | **WorldVLA**  | Unified autoregressive framework for text, image, and action generation; joint latent manifold treats physical actions and visual evolution as first-class citizens | [WorldVLA: Towards Autoregressive Action World Model](https://arxiv.org/abs/2506.21539) | [![GitHub Stars](https://img.shields.io/github/stars/alibaba-damo-academy/WorldVLA?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/alibaba-damo-academy/WorldVLA)       |
| 2024-04 | **V-JEPA**    | First pure-video self-supervised JEPA; latent prediction of masked spatiotemporal blocks produces rich action-predictive representations without pixel reconstruction | [Revisiting Feature Prediction for Learning Visual Representations from Video](https://arxiv.org/abs/2404.08471) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/jepa?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/jepa)               |
| 2019-02 | **PlaNet**    | RSSM latent manifold for planning; stochastic + deterministic components allow exploration over multiple plausible physical futures simultaneously | [Learning Latent Dynamics for Planning from Pixels](https://arxiv.org/abs/1811.04551) | [![GitHub Stars](https://img.shields.io/github/stars/google-research/planet?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/google-research/planet)              |
| 2025-01 | **AD-L-JEPA** | Autonomous driving latent-space JEPA: predicts action-conditioned future representations of driving scenes… | [Self-Supervised Representation Learning with Joint Embedding Predictive Architecture for Automotive LiDAR Object Detection](https://arxiv.org/abs/2501.04969) | [![GitHub Stars](https://img.shields.io/github/stars/haoranzhuexplorer/ad-l-jepa-release?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/haoranzhuexplorer/ad-l-jepa-release) |


<br>

### 4.3 How: Exploration Across World-Model Domains

#### 4.3.1 Model-Based Reinforcement Learning (MBRL)

##### Deterministic Dynamics and Iterative Exploration

The most direct approach minimises one-step prediction error iteratively; the policy and model alternate, with the updated policy exploring the environment to collect increasingly informative data.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2019-06 | **MBPO**   | Short imagined rollouts prevent compounding error; iterative model–policy alternation guides exploration toward regions of true dynamics not yet covered | [When to Trust Your Model: Model-Based Policy Optimization](https://arxiv.org/abs/1906.08253) | [![GitHub Stars](https://img.shields.io/github/stars/jannerm/mbpo?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/jannerm/mbpo)             |
| 2018-07 | **SLBO**   | Jointly maximises return lower bound over policy and model; optimism in model optimisation encourages exploration of state–action regions not yet well covered | [Algorithmic Framework for Model-based Deep Reinforcement Learning with Theoretical Guarantees](https://arxiv.org/abs/1807.03858) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/slbo?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/slbo)    |
| 2019-03 | **SimPLe** | Sequential policy optimisation in latent model: pixel-based video prediction model supports model-free policy gradient exploration… | [Model-Based Reinforcement Learning for Atari](https://arxiv.org/abs/1903.00374) | [![GitHub Stars](https://img.shields.io/github/stars/tensorflow/tensor2tensor?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/tensorflow/tensor2tensor) |


##### Uncertainty-Aware Exploration

Isolating epistemic uncertainty from aleatoric uncertainty guides exploration toward regions where the model is genuinely ignorant rather than inherently noisy.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2018-05 | **PETS**                                 | Probabilistic ensemble explicitly disentangles aleatoric vs. epistemic uncertainty via KL minimisation between ensemble members; explores where epistemic uncertainty is highest | [Deep Reinforcement Learning in a Handful of Trials using Probabilistic Dynamics Models](https://arxiv.org/abs/1805.12114) | [![GitHub Stars](https://img.shields.io/github/stars/kchua/handful-of-trials?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/kchua/handful-of-trials) |
| 2018-10 | **ME-TRPO**                              | Model-ensemble trust-region policy optimisation: uses N independently trained models and limits policy updates to regions where all models agree, preventing exploitation of epistemic uncertainty in… | [Model-Ensemble Trust-Region Policy Optimization](https://arxiv.org/abs/1802.10592) | [![GitHub Stars](https://img.shields.io/github/stars/thanard/me-trpo?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/thanard/me-trpo)         |
| 2019-10 | **Model-Based Active Exploration (MAX)** | Treats exploration as active learning: at each step selects actions that maximally reduce epistemic uncertainty under the ensemble… | [Model-Based Active Exploration](https://arxiv.org/abs/1810.12162) | [![GitHub Stars](https://img.shields.io/github/stars/nnaisense/MAX?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/nnaisense/MAX)           |


##### From Pixels to Latent Planning: Representation Learning for World Models

For high-dimensional pixel observations, representation learning compresses inputs into compact latents to enable tractable imagination-space exploration.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2020-05 | **Plan2Explore** | Novelty = future ensemble disagreement in RSSM latent space; task-agnostic exploration pre-trains a world model before any reward signal is available | [Planning to Explore via Self-Supervised World Models](https://arxiv.org/abs/2005.05960) | [![GitHub Stars](https://img.shields.io/github/stars/ramanans1/plan2explore?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ramanans1/plan2explore) |
| 2019-02 | **PlaNet**       | Pioneers RSSM: deterministic hidden state + stochastic Gaussian latent; stochastic branch forces imagination to explore multiple plausible environmental outcomes | [Learning Latent Dynamics for Planning from Pixels](https://arxiv.org/abs/1811.04551) | [![GitHub Stars](https://img.shields.io/github/stars/google-research/planet?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/google-research/planet) |
| 2018-03 | **World Models** | V–M–C architecture: VAE compresses pixels, RNN explores temporal structure in latent space, controller acts within learned representation | [World Models](https://arxiv.org/abs/1803.10122) | [![GitHub Stars](https://img.shields.io/github/stars/hardmaru/worldmodels?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/hardmaru/worldmodels)   |


##### Imagination-Based Exploration: The Dreamer Family

The Dreamer lineage demonstrates progressively sophisticated exploration within learned latent spaces, from action noise to entropy regularisation to phased world-model/policy co-training.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-09 | **DreamerV4**  | Phased training (WM pre-train → policy post-train) solves dual exploration problem; policy leverages WM priors for efficient exploration of long-horizon imagined trajectories | [Training Agents Inside of Scalable World Models](https://arxiv.org/abs/2509.24527) | -                                                     |
| 2023-01 | **DreamerV3**  | Percentile return normalisation stabilises exploration intensity across sparse and dense reward scales; adapts entropy regularisation automatically | [Mastering Diverse Domains through World Models](https://arxiv.org/abs/2301.04104) | [![GitHub Stars](https://img.shields.io/github/stars/danijar/dreamerv3?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/danijar/dreamerv3)  |
| 2020-10 | **DreamerV2**  | Discrete categorical latents + actor entropy bonus as explicit exploration regulariser; prevents premature policy collapse in imagined rollouts | [Mastering Atari with Discrete World Models](https://arxiv.org/abs/2010.02193) | [![GitHub Stars](https://img.shields.io/github/stars/danijar/dreamerv2?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/danijar/dreamerv2)  |
| 2019-12 | **DreamerV1**  | RSSM world model with action noise for environment exploration; broader state-space coverage improves quality of imagined training data | [Dream to Control: Learning Behaviors by Latent Imagination](https://arxiv.org/abs/1912.01603) | [![GitHub Stars](https://img.shields.io/github/stars/danijar/dreamer?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/danijar/dreamer)    |
| 2023-01 | **DayDreamer** | Transfers DreamerV2 to physical robots; latent imagination enables efficient hardware exploration without prohibitive real-world sample requirements | [DayDreamer: World Models for Physical Robot Learning](https://arxiv.org/abs/2206.14176) | [![GitHub Stars](https://img.shields.io/github/stars/danijar/daydreamer?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/danijar/daydreamer) |


##### Predictive Architectures: JEPA

JEPA shifts from pixel reconstruction to abstract latent prediction, naturally encouraging exploration over multiple plausible world interpretations rather than fitting a single deterministic output.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-06 | **V-JEPA 2** | Video-pretrained world model enabling zero-shot robotic deployment; latent-space exploration closes the loop between imagination and physical execution | [V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning](https://arxiv.org/abs/2506.09985) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/jepa?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/jepa)  |
| 2024-04 | **V-JEPA**   | First pure-video JEPA: predicts masked spatiotemporal block representations; abstract latent prediction explores rich spatiotemporal structure without pixel-level noise | [Revisiting Feature Prediction for Learning Visual Representations from Video](https://arxiv.org/abs/2404.08471) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/jepa?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/jepa)  |
| 2023-06 | **I-JEPA**   | Image JEPA: learns representations by predicting abstract features of masked image regions from context… | [Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture](https://arxiv.org/abs/2301.08243) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/ijepa?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/ijepa) |




#### 4.3.2 Video Generation as World Simulation

Large-scale video diffusion models have evolved from passive visual generators toward active world simulators; integrating RL transforms them from distribution-fitters into causal reasoning engines.

##### Model as Environment

Video generation models serve as physics engines, enabling RL agents to explore within generated "dreams" at zero physical cost.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2024-05 | **Genie**                   | Learns action-conditioned state transitions from unlabelled video; creates controllable virtual sandboxes for agent exploration without real-world interaction | [Genie: Generative Interactive Environments](https://arxiv.org/abs/2402.15391) | -                                                                   |
| 2024-03 | **UniSim**                  | Universal simulator of sensorimotor interactions; trains RL agents entirely in simulated video environments for safe long-tail exploration | [Video Language Planning](https://arxiv.org/abs/2310.10625) | -                                                                   |
| 2024-01 | **DriveDreamer**            | Driving-domain video world model conditioned on structured HD-map and traffic annotations… | [DriveDreamer: Towards Real-world-driven World Models for Autonomous Driving](https://arxiv.org/abs/2309.09777) | [![GitHub Stars](https://img.shields.io/github/stars/JeffWang987/DriveDreamer?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/JeffWang987/DriveDreamer)         |
| 2024-11 | **Genie 2**                 | Scalable interactive environment generator: produces persistent 3D-consistent game worlds from a single image prompt… | [Spherical maximal operators with fractal sets of dilations on radial functions](https://arxiv.org/abs/2412.09390) | -                                                                   |
| 2024-04 | **Video Language Planning** | Combines video generation with language-conditioned planning: generates goal-directed video plans as imagined futures, then executes them via a learned policy… | [Video Language Planning](https://arxiv.org/abs/2310.10625) | [![GitHub Stars](https://img.shields.io/github/stars/video-language-planning/vlp_code?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/video-language-planning/vlp_code) |


##### Model as Agent

RL directly optimises the video generation process itself, forcing the generative model to actively explore the generation space toward physically plausible outputs.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-01 | **Cosmos Policy** | Injects latent frames for video–action co-diffusion; RL reward guides generation to explore physically consistent action-conditioned futures | [Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning](https://arxiv.org/abs/2601.16163) | -                                                          |
| 2025-01 | **VideoDPO**      | DPO applied to video generation; preference data forces generative exploration toward spatiotemporally consistent physical trajectories | [STAR: Stepwise Task Augmentation with Relation Learning for Aspect Sentiment Quad Prediction](https://arxiv.org/abs/2501.16093) | [![GitHub Stars](https://img.shields.io/github/stars/CIntellifusion/VideoDPO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/CIntellifusion/VideoDPO) |
| 2026-01 | **TAGRPO**        | Token-level advantage-guided reward policy optimisation for video generation… | [TAGRPO: Boosting GRPO on Image-to-Video Generation with Direct Trajectory Alignment](https://arxiv.org/abs/2601.05729) | [![GitHub Stars](https://img.shields.io/github/stars/SkyworkAI/SkyReels-V1?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/SkyworkAI/SkyReels-V1)   |
| 2026-02 | **DreamZero**     | Zero-shot world model policy: directly uses a pre-trained video world model as a policy by selecting action sequences that steer imagined futures toward high-reward outcomes… | [World Action Models are Zero-shot Policies](https://arxiv.org/abs/2602.15922) | [![GitHub Stars](https://img.shields.io/github/stars/dreamzero0/dreamzero?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/dreamzero0/dreamzero)    |


##### Inference as Exploration

Video generation at inference time becomes dynamic search and planning — generating multiple trajectory candidates and filtering via physics verifiers, analogous to MCTS in imagination.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-01 | **Video-T1**                  | Test-time scaling for video generation: generates multiple candidate trajectories, uses verifiers to select the most physically consistent — inference as tree search | [Time-Dependent Radiation Transport Simulations of Infrared Echoes from Dust-Shrouded Luminous Transients](https://arxiv.org/abs/2501.13157) | [![GitHub Stars](https://img.shields.io/github/stars/THU-SI/Video-T1?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/THU-SI/Video-T1)           |
| 2026-01 | **WMReward (Inference-Time)** | Uses world model value estimates as verifier rewards at inference time… | [Inference-time Physics Alignment of Video Generative Models with Latent World Models](https://arxiv.org/abs/2601.10553) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/WMReward?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/WMReward) |
| 2026-02 | **DreamZero (Inference)**     | Leverages a frozen video world model at inference time to score action proposals via forward imagination… | [World Action Models are Zero-shot Policies](https://arxiv.org/abs/2602.15922) | [![GitHub Stars](https://img.shields.io/github/stars/dreamzero0/dreamzero?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/dreamzero0/dreamzero)      |


##### Active Closed-Loop Simulation via World Action Models (WAMs)

Exploration evolves from passive open-loop video generation to active closed-loop counterfactual simulation; WAMs treat physical actions and visual evolution as joint first-class citizens.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2026-03 | **FastWAM**         | Decouples video generation from policy inference; skips test-time future imagination entirely to achieve 190ms latency for real-time closed-loop action exploration | [Fast-WAM: Do World Action Models Need Test-time Future Imagination?](https://arxiv.org/abs/2603.16666) | [![GitHub Stars](https://img.shields.io/github/stars/yuantianyuan01/FastWAM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yuantianyuan01/FastWAM)        |
| 2025-06 | **WorldVLA**        | Unified autoregressive framework generating text, images, and actions; explores action-grounded latent manifold as joint first-class representation | [WorldVLA: Towards Autoregressive Action World Model](https://arxiv.org/abs/2506.21539) | [![GitHub Stars](https://img.shields.io/github/stars/alibaba-damo-academy/WorldVLA?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/alibaba-damo-academy/WorldVLA) |
| 2025-01 | **Cosmos Policy**   | Latent frame injection synchronises video and action co-diffusion; closed-loop counterfactual simulation with RL-guided physically consistent exploration | [Cosmos Policy: Fine-Tuning Video Models for Visuomotor Control and Planning](https://arxiv.org/abs/2601.16163) | -                                                                |
| 2026-02 | **DreamZero (WAM)** | Zero-shot WAM that couples a frozen video world model with a learned action decoder; closed-loop action exploration via iterative world-model querying without any task-specific fine-tuning | [World Action Models are Zero-shot Policies](https://arxiv.org/abs/2602.15922) | [![GitHub Stars](https://img.shields.io/github/stars/dreamzero0/dreamzero?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/dreamzero0/dreamzero)          |



#### 4.3.3 Autonomous Driving: Vectorised and Occupancy Exploration

Autonomous driving demands exploration of rare long-tail scenarios through imagination — real-world trial-and-error is prohibitive — requiring a transition from pixel imagination to structured occupancy representations.

##### Generative Foundations and End-to-End Latent Planning

Generative world models serve as data engines bridging the reality gap; exploration is conducted in compact latent spaces to bypass rendering burdens.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2024-01 | **DriveDreamer** | Driving world model synthesising future scenes conditioned on actions; explores diverse driving futures in latent space to validate plans before physical execution | [DriveDreamer: Towards Real-world-driven World Models for Autonomous Driving](https://arxiv.org/abs/2309.09777) | [![GitHub Stars](https://img.shields.io/github/stars/JeffWang987/DriveDreamer?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/JeffWang987/DriveDreamer)     |
| 2023-09 | **GAIA-1**       | Generative world model for autonomous driving; produces diverse imagined driving scenarios as a data engine for exploring rare safety-critical events | [GAIA-1: A Generative World Model for Autonomous Driving](https://arxiv.org/abs/2309.17080) | -                                                               |
| 2022-10 | **MILE**         | Model-based imitation learning in compact latent space; imagined rollouts in latent representation for sample-efficient exploration of driving behaviours | [Model-Based Imitation Learning for Urban Driving](https://arxiv.org/abs/2210.07729) | [![GitHub Stars](https://img.shields.io/github/stars/wayveai/mile?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/wayveai/mile)                 |
| 2024-12 | **DrivingWorld** | Spatiotemporal autoregressive world model for autonomous driving… | [DrivingWorld: Constructing World Model for Autonomous Driving via Video GPT](https://arxiv.org/abs/2412.19505) | [![GitHub Stars](https://img.shields.io/github/stars/YvanYin/DrivingWorld?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/YvanYin/DrivingWorld)         |
| 2025-06 | **GenAD**        | Generalised autonomous driving world model: trains a single generative model across diverse driving datasets… | [Minimal $(n-2)$-umbilic submanifolds of the Euclidean space](https://arxiv.org/abs/2505.11039) | [![GitHub Stars](https://img.shields.io/github/stars/wzzheng/GenAD?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/wzzheng/GenAD)                |
| 2024-03 | **Think2Drive**  | Converts a pre-trained world model into an online planner… | [Think2Drive: Efficient Reinforcement Learning by Thinking in Latent World Model for Quasi-Realistic Autonomous Driving (in CARLA-v2)](https://arxiv.org/abs/2402.16720) | [![GitHub Stars](https://img.shields.io/github/stars/Thinklab-SJTU/Bench2DriveZoo?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Thinklab-SJTU/Bench2DriveZoo) |
| 2023-06 | **UniAD**        | Unified autonomous driving framework integrating perception, prediction, and planning in a shared representation… | [Planning-oriented Autonomous Driving](https://arxiv.org/abs/2212.10156) | [![GitHub Stars](https://img.shields.io/github/stars/OpenDriveLab/UniAD?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/OpenDriveLab/UniAD)           |


##### Counterfactual Reasoning and Uncertainty Awareness

Action-conditioned generation enables safe exploration of "what-if" counterfactual outcomes; uncertainty quantification prevents the policy exploiting out-of-distribution hallucinations.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2024-01 | **Drive-WM**  | Action-conditioned multi-view video generation for driving; visualises consequences of hypothetical manoeuvres to explore safe counterfactual futures | [Personalized Autonomous Driving with Large Language Models: Field Experiments](https://arxiv.org/abs/2312.09397) | [![GitHub Stars](https://img.shields.io/github/stars/BraveGroup/Drive-WM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/BraveGroup/Drive-WM)                 |
| 2024-03 | **RealGen**   | Adversarial retrieval-augmented generation targeting safety-critical scenario boundaries; probes failure-mode hazard zones via adversarial imagination exploration | [RealGen: Retrieval Augmented Generation for Controllable Traffic Scenarios](https://arxiv.org/abs/2312.13303) | [![GitHub Stars](https://img.shields.io/github/stars/yejy53/RealGen?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yejy53/RealGen)                      |
| 2025-01 | **AD-L-JEPA** | Autonomous driving latent-space JEPA: predicts action-conditioned future driving representations… | [Self-Supervised Representation Learning with Joint Embedding Predictive Architecture for Automotive LiDAR Object Detection](https://arxiv.org/abs/2501.04969) | [![GitHub Stars](https://img.shields.io/github/stars/haoranzhuexplorer/ad-l-jepa-release?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/haoranzhuexplorer/ad-l-jepa-release) |
| 2024-06 | **Delphi**    | Dense latent point cloud world model for driving; probabilistic forecasting of future scene states enables uncertainty-aware exploration of counterfactual traffic evolutions | [Unleashing Generalization of End-to-End Autonomous Driving with Controllable Long Video Generation](https://arxiv.org/abs/2406.01349) | [![GitHub Stars](https://img.shields.io/github/stars/westlake-autolab/Delphi?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/westlake-autolab/Delphi)             |
| 2025-01 | **UncAD**     | Uncertainty-aware autonomous driving: estimates both epistemic and aleatoric uncertainty in world model predictions… | [Tightening the entropic uncertainty relations with quantum memory in a multipartite scenario](https://arxiv.org/abs/2501.02861) | [![GitHub Stars](https://img.shields.io/github/stars/pengxuanyang/UncAD?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/pengxuanyang/UncAD)                  |


##### 4D Occupancy Exploration and Physical Consistency

Shifting from 2D pixel generation to 4D occupancy grids combats depth/scale drift and provides collision-risk cost volumes for safe planning exploration.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2024-08 | **OccSora**              | Diffusion-based 4D occupancy generation; synthesises long-horizon occupancy sequences enabling exploration of temporally consistent physical futures | [OccSora: 4D Occupancy Generation Models as World Simulators for Autonomous Driving](https://arxiv.org/abs/2405.20337) | [![GitHub Stars](https://img.shields.io/github/stars/wzzheng/OccSora?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/wzzheng/OccSora)             |
| 2024-05 | **OccWorld**             | Vision-centric 3D occupancy world model for driving; forecasts occupancy evolution providing collision-risk cost volumes for safe spatial exploration | [OccWorld: Learning a 3D Occupancy World Model for Autonomous Driving](https://arxiv.org/abs/2311.16038) | [![GitHub Stars](https://img.shields.io/github/stars/wzzheng/OccWorld?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/wzzheng/OccWorld)            |
| 2025-01 | **Drive-OccWorld**       | Drives entirely in a 4D occupancy world: unified model for scene generation and ego-planning… | [Driving in the Occupancy World: Vision-Centric 4D Occupancy Forecasting and Planning via World Models for Autonomous Driving](https://arxiv.org/abs/2408.14197) | [![GitHub Stars](https://img.shields.io/github/stars/yuyang-cloud/Drive-OccWorld?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yuyang-cloud/Drive-OccWorld) |
| 2024-04 | **Copilot4D**            | Discretises 3D point cloud scenes into tokens and applies discrete diffusion for 4D world modelling… | [Copilot4D: Learning Unsupervised World Models for Autonomous Driving via Discrete Diffusion](https://arxiv.org/abs/2311.01017) | -                                                              |
| 2025-01 | **DynamicCity**          | Dynamic 4D city generation via HexPlane-based occupancy world model; generates temporally consistent large-scale urban occupancy sequences enabling exploration of rare urban environment configurations | [3D-Adapter: Geometry-Consistent Multi-View Diffusion for High-Quality 3D Generation](https://arxiv.org/abs/2410.18974) | [![GitHub Stars](https://img.shields.io/github/stars/3DTopia/DynamicCity?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/3DTopia/DynamicCity)         |
| 2025-04 | **Gaussian World Model** | 4D Gaussian splatting world model for autonomous driving… | [Transversely pumped laser driven particle accelerator](https://arxiv.org/abs/2501.11825) | [![GitHub Stars](https://img.shields.io/github/stars/zuosc19/GaussianWorld?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/zuosc19/GaussianWorld)       |


##### Closed-Loop Neural Simulation

Exploration evolves from static data augmentation to dynamic closed-loop systems where the policy actively interacts with neural simulators to probe decision boundaries.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2024-10 | **DriveArena**       | Creates reactive 4D worlds where the policy actively interacts with a neural simulator; enables closed-loop exploration of diverse reactive traffic scenarios | [DriveArena: A Closed-loop Generative Simulation Platform for Autonomous Driving](https://arxiv.org/abs/2408.00415) | [![GitHub Stars](https://img.shields.io/github/stars/PJLab-ADG/DriveArena?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/PJLab-ADG/DriveArena)     |
| 2024-09 | **SimGen**           | Cascaded diffusion for high-fidelity, controllable scenario augmentation; addresses long-tail exploration by generating rare safety-critical scenarios on demand | [SimGen: Simulator-conditioned Driving Scene Generation](https://arxiv.org/abs/2406.09386) | [![GitHub Stars](https://img.shields.io/github/stars/metadriverse/SimGen?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/metadriverse/SimGen)      |
| 2024-03 | **DrivingDiffusion** | Multi-view video diffusion for closed-loop driving simulation… | [DrivingDiffusion: Layout-Guided multi-view driving scene video generation with latent diffusion model](https://arxiv.org/abs/2310.07771) | [![GitHub Stars](https://img.shields.io/github/stars/shalfun/DrivingDiffusion?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/shalfun/DrivingDiffusion) |
| 2025-05 | **Raw2Drive**        | End-to-end closed-loop driving directly from raw sensor data… | [Raw2Drive: Reinforcement Learning with Aligned World Models for End-to-End Autonomous Driving (in CARLA v2)](https://arxiv.org/abs/2505.16394) | [![GitHub Stars](https://img.shields.io/github/stars/Thinklab-SJTU/Raw2Drive?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Thinklab-SJTU/Raw2Drive)  |
| 2023-06 | **TrafficBots**      | Multi-agent traffic simulation via conditional behaviour generation… | [TrafficBots: Towards World Models for Autonomous Driving Simulation and Motion Prediction](https://arxiv.org/abs/2303.04116) | [![GitHub Stars](https://img.shields.io/github/stars/zhejz/TrafficBots?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/zhejz/TrafficBots)        |
| 2025-04 | **DrivingSphere**    | Spherical-projection world model for full 360° closed-loop driving simulation; complete spatial coverage removes blind spots so policies train against surrounding agents in all directions | [DrivingSphere: Building a High-fidelity 4D World for Closed-loop Simulation](https://arxiv.org/abs/2411.11252) | [![GitHub Stars](https://img.shields.io/github/stars/yanty123/DrivingSphere?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yanty123/DrivingSphere)   |




#### 4.3.4 Social Dynamics: Exploration in Strategic and Normative Environments

Social environments introduce recursive exploration: probing social dynamics reshapes those very dynamics, requiring agents to reason counterfactually over beliefs, incentives, and equilibria.


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2024-01 | **VBench**        | Comprehensive benchmark evaluating world model quality including social regularity capture; provides metrics to assess whether exploration produces socially plausible behaviours | [VBench: Comprehensive Benchmark Suite for Video Generative Models](https://arxiv.org/abs/2311.17982) | [![GitHub Stars](https://img.shields.io/github/stars/Vchitect/VBench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Vchitect/VBench)                |
| 2020-08 | **Social-STGCNN** | Spatio-temporal graph CNN models pedestrian trajectory social forces; world model for social dynamics enabling exploration of crowd interaction counterfactuals | [Social-STGCNN: A Social Spatio-Temporal Graph Convolutional Neural Network for Human Trajectory Prediction](https://arxiv.org/abs/2002.11927) | [![GitHub Stars](https://img.shields.io/github/stars/abduallahmohamed/Social-STGCNN?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/abduallahmohamed/Social-STGCNN) |
| 2025-10 | **LCTGen**        | Language-conditioned traffic generation: natural-language scene specs, structured map retrieval, and multi-agent rollouts for counterfactual social traffic exploration | [Language Conditioned Traffic Generation](https://arxiv.org/abs/2307.07947) | [![GitHub Stars](https://img.shields.io/github/stars/Ariostgx/lctgen?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Ariostgx/lctgen)                |


---

<br>



## 5. Level 5: Prospector → Ecosystem — Coordination-Space Exploration

<p align="center"><img src="fig/level5_ecosystem.png" width="850"/></p>
<p align="center"><i>Figure: Level 5 Coordination-Space Exploration — Why (single-agent limitations), Where (communication, collaboration, role, deployment), and How (orchestration, ensemble, MARL, self-evolving agents).</i></p>

<!-- At the highest level, exploration enters **coordination space**: heterogeneous agents discover communication topologies, role specialisations, shared representations, and collaborative strategies. -->

At Level 5, exploration transcends the individual agent entirely. The object of exploration is no longer a reasoning trajectory, an action sequence, or an imagined future, but the *coordination structure* itself — communication protocols, collaboration topologies, role assignments, and collective knowledge substrates. The central question shifts from "how should a single agent explore?" to "how should a population of heterogeneous agents organise their joint exploration?"

This transition is not merely about scaling the number of agents. Single-agent systems face fundamental limitations in capability coverage, robustness, and adaptability when confronting tasks that require cross-domain knowledge, long-horizon planning, and multi-step verification. Static multi-agent architectures with fixed interaction pathways suppress structural exploration, restricting adaptability to dynamic environments. Domain-specific tasks demand structured collaboration with specialised roles and verification steps to reduce hallucinations and ensure executability. And unconstrained multi-agent deployment introduces substantial computational overhead, requiring resource-efficient coordination strategies. Level 5 addresses these challenges by making the organisation of intelligence itself — how agents communicate, coordinate, specialise, compose, and co-evolve — the target of exploration.


| Challenge | Description |
|:----------|:------------|
| **Scalable Coordination Exploration** | The search space is combinatorial, hierarchical, and dynamic—which agents to activate, what communication to establish, how information flows |
| **Ecosystem-Level Credit Assignment** | Disentangling behavioural contribution from structural contribution under sparse, delayed feedback |
| **Diversity vs. Convergence Tension** | Balancing ecological diversity against system-level coherence |
| **Role–Communication Co-evolution** | Jointly evolving functional specialisation and information exchange protocols |

<!-- **Key Systems & Methods:**

| Method | Key Contribution |
|:-------|:-----------------|
| **MetaGPT** | Structured multi-agent coordination with role-based workflows |
| **AutoGen** | Flexible conversational multi-agent framework |
| **CAMEL** | Communicative agents for mind exploration |
| **Multi-agent Debate** | Structured deliberation improving collective reasoning (Du et al.) |
| **Learnable orchestration** | RL-evolved coordination topologies, optimisable agent graphs | -->



### 5.1 Multi-Agent Orchestration

#### 5.1.1 Rule-based Orchestration (Reachability-Driven)

Methods that coordinate collaboration through pre-defined routing rules, role protocols, or structured workflows to guarantee deterministic reachability across agents:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2026-02 | **ORCH** | Explores many parallel analysis trajectories and merges them via a deterministic EMA-guided router to ensure reachable consensus in discrete-choice reasoning | [ORCH: Many Analyses, One Merge — A Deterministic Multi-Agent Orchestrator for Discrete-Choice Reasoning with EMA-Guided Routing](https://arxiv.org/abs/2602.01797) | - |
| 2025-11 | **MA-IR** | Deterministic multi-agent orchestration for high-quality incident response decision support | [Multi-Agent LLM Orchestration Achieves Deterministic, High-Quality Decision Support for Incident Response](https://arxiv.org/abs/2511.15755) | - |
| 2025-10 | **MOSAIC** | Task-intelligent orchestration routes specialised agents to explore scientific coding workflows within a rule-governed collaboration space | [MOSAIC: Multi-agent Orchestration for Task-Intelligent Scientific Coding](https://arxiv.org/abs/2510.08804) | - |
| 2025-06 | **AgentOrchestra** | Defines the reachable coordination space via a Tool-Environment-Agent (TEA) protocol, scaffolding scalable multi-agent exploration | [AgentOrchestra: Orchestrating Multi-Agent Intelligence with the Tool-Environment-Agent (TEA) Protocol](https://arxiv.org/abs/2506.12508) | - |
| 2025 | **Croto** | Cross-team communication rules carve out a reachable space of inter-team collaboration for multi-agent exploration | Multi-agent collaboration via cross-team orchestration | - |
| 2024-06 | **MACNET** | Predefined topological links bound the agent interaction graph that large-scale multi-agent collaboration can traverse | [Scaling Large Language Model-based Multi-Agent Collaboration](https://arxiv.org/abs/2406.07155) | - |
| 2023-08 | **MetaGPT** | Encodes SOPs as meta-programming so role-based workflows follow reliably reachable collaboration trajectories | [MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework](https://arxiv.org/abs/2308.00352) | - |
| 2023 | **AgentVerse** | Rule-driven collaboration scaffolds multi-agent exploration of emergent group behaviours within a reachable role space | [Agentverse: Facilitating Multi-Agent Collaboration and Exploring Emergent Behaviors](https://openreview.net/forum?id=EHg5GDnyq1) | - |

#### 5.1.2 Learnable Orchestration (Competence-Driven)

Methods that train orchestrators, meta-agents, or agent graphs to route tasks toward the most competent executors and expand multi-agent capability boundaries:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2026-01 | **MAS-Orchestra** | Expands multi-agent reasoning competence through holistic orchestration, with controlled benchmarks probing the explored system space | [MAS-Orchestra: Understanding and Improving Multi-Agent Reasoning Through Holistic Orchestration and Controlled Benchmarks](https://arxiv.org/abs/2601.14652) | - |
| 2025-05 | **Puppeteer-Puppet** | Evolves a puppeteer that explores dynamic orchestration strategies over puppet agents to extend collaborative competence | [Multi-Agent Collaboration via Evolving Orchestration](https://arxiv.org/abs/2505.19591) | - |
| 2025-04 | **W4S** | Trains a weak meta-agent to explore task decompositions and harness strong executor agents beyond its own competence | [Weak-for-Strong: Training Weak Meta-Agent to Harness Strong Executors](https://arxiv.org/abs/2504.04785) | - |
| 2024-04 | **CMAT** | Collaboration tuning expands small-model agent competence by exploring multi-agent interaction signals | [CMAT: A Multi-Agent Collaboration Tuning Framework for Enhancing Small Language Models](https://arxiv.org/abs/2404.01663) | - |
| 2024-02 | **GPTSwarm** | Treats language agents as optimizable computation graphs, enabling competence-driven search over prompts and inter-agent edges | [Language Agents as Optimizable Graphs](https://arxiv.org/abs/2402.16823) | - |

#### 5.1.3 Reflection & Information-Theoretic Orchestration (Uncertainty-Driven)

Methods that adapt orchestration policies through reflection feedback or information-theoretic uncertainty signals across long-horizon multi-agent tasks:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-09 | **Orchestrator** | Uses active inference to drive multi-agent exploration under epistemic uncertainty across long-horizon tasks | [Orchestrator: Active Inference for Multi-Agent Systems in Long-Horizon Tasks](https://arxiv.org/abs/2509.05651) | - |
| 2025-04 | **W4S** | Weak meta-agent explores orchestration policies over strong executors, guided by reflection on uncertain outcomes | [Weak-for-Strong: Training Weak Meta-Agent to Harness Strong Executors](https://arxiv.org/abs/2504.04785) | - |
| 2025-03 | **MAS-GPT** | Trains LLMs to synthesise multi-agent systems per query, exploring the system-design space conditioned on task uncertainty | [MAS-GPT: Training LLMs to Build LLM-based Multi-Agent Systems](https://arxiv.org/abs/2503.03686) | - |
| 2024-04 | **CMAT** | Reflective multi-agent tuning explores feedback-driven collaboration to calibrate small-agent competence under uncertainty | [CMAT: A Multi-Agent Collaboration Tuning Framework for Enhancing Small Language Models](https://arxiv.org/abs/2404.01663) | - |

#### 5.1.4 Memory & Knowledge Substrate Exploration

Methods that build self-evolving multi-agent systems on shared memory or knowledge substrates to support long-horizon specialisation and exploration:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-05 | **PiFlow** | Principle-aware orchestration grows a scientific knowledge substrate that guides multi-agent discovery exploration | [PiFlow: Principle-aware Scientific Discovery with Multi-Agent Collaboration](https://arxiv.org/abs/2505.15047) | [![GitHub Stars](https://img.shields.io/github/stars/amair-lab/PiFlow?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/amair-lab/PiFlow) |
| 2025-03 | **MedAgentSim** | Self-evolving clinical multi-agent simulation explores new cases by accumulating case-level memory as a shared substrate | [Self-Evolving Multi-Agent Simulations for Realistic Clinical Interactions](https://arxiv.org/abs/2503.22678) | [![GitHub Stars](https://img.shields.io/github/stars/MAXNORM8650/MedAgentSim?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/MAXNORM8650/MedAgentSim) |
| 2025 | **SEMC** | Self-evolving consultation grows a shared diagnostic knowledge base, expanding the reachable medical case space over time | A Self-Evolving Framework for Multi-Agent Medical Consultation Based on Large Language Models | - |
| 2025-02 | **MobileSteward** | Orchestrates app-oriented agents with self-evolving memory to explore cross-app instruction compositions | [MobileSteward: Integrating Multiple App-Oriented Agents with Self-Evolution to Automate Cross-App Instructions](https://arxiv.org/abs/2502.16796) | [![GitHub Stars](https://img.shields.io/github/stars/XiaoMi/MobileSteward?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/XiaoMi/MobileSteward) |
| 2025-01 | **Mobile-Agent-E** | Self-evolving mobile assistant explores complex tasks by accumulating reusable tips and shortcuts as a growing experience substrate | [Mobile-Agent-E: Self-Evolving Mobile Assistant for Complex Tasks](https://arxiv.org/abs/2501.11733) | [![GitHub Stars](https://img.shields.io/github/stars/X-PLUG/MobileAgent?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/X-PLUG/MobileAgent/tree/main/Mobile-Agent-E) |
| 2023-04 | **Generative Agents** | Interactive simulacra use memory-retrieval substrates to explore and surface emergent social behaviour over long horizons | [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442) | [![GitHub Stars](https://img.shields.io/github/stars/joonspk-research/generative_agents?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/joonspk-research/generative_agents) |


<br>


### 5.2 Agentic Ensemble Papers




#### 5.2.1 Ensemble-During-Inference Papers



Methods that explore how to combine or choose token candidates from multiple LLMs at each decoding step, either by merging next-token distributions or by selecting the token from one model directly:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-10 | **SAFE** | Only ensembles at a few well-chosen token steps to keep decoding stable and fast | [When to Ensemble: Identifying Token-Level Points for Stable and Fast LLM Ensembling](https://arxiv.org/abs/2510.15346) | - |
| 2025-10 | **CoRe** | Uses token and model agreement to downweight unreliable signals | [Harnessing Consistency for Robust Test-Time LLM Ensemble](https://arxiv.org/abs/2510.13855) | - |
| 2025-05 | **Transformer Copilot** | A Copilot learns from past token mistakes and fixes the Pilot’s logits | [Transformer Copilot: Learning from The Mistake Log in LLM Fine-tuning](https://arxiv.org/abs/2505.16270) | [![GitHub Stars](https://img.shields.io/github/stars/jiaruzouu/TransformerCopilot?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/jiaruzouu/TransformerCopilot) |
| 2025-02 | **ABE** | Makes different-vocabulary models agree on the same surface token before choosing it | [Token-level Ensembling of Models with Different Vocabularies](https://arxiv.org/abs/2502.21265) | [![GitHub Stars](https://img.shields.io/github/stars/mjpost/abe?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/mjpost/abe) |
| 2025-02 | **CITER** | Sends easy tokens to a small model and hard ones to a large model | [CITER: Collaborative Inference for Efficient Large Language Model Decoding with Token-Level Routing](https://arxiv.org/abs/2502.01976) | [![GitHub Stars](https://img.shields.io/github/stars/aiming-lab/CITER?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/aiming-lab/CITER) |
| 2024-10 | **UniTe** | Ensembles only the union of top-*k* tokens instead of the full vocabulary | [Determine-Then-Ensemble: Necessity of Top-k Union for Large Language Model Ensembling](https://arxiv.org/abs/2410.03777) | - |
| 2024-06 | **GaC** | Treats next-token generation like classification and averages token probabilities | [Breaking the Ceiling of the LLM Community by Treating Token Generation as a Classification for Ensembling](https://arxiv.org/abs/2406.12585) | [![GitHub Stars](https://img.shields.io/github/stars/yaoching0/GaC?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yaoching0/GaC) |
| 2024-04 | **DeePEn** | Maps different vocabularies into a shared space before merging token distributions | [Ensemble Learning for Heterogeneous Large Language Models with Deep Parallel Collaboration](https://arxiv.org/abs/2404.12715) | [![GitHub Stars](https://img.shields.io/github/stars/OrangeInSouth/DeePEn?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/OrangeInSouth/DeePEn) |
| 2024-04 | **PackLLM** | Gives more weight to models that fit the prompt better | [Pack of LLMs: Model Fusion at Test-Time via Perplexity Optimization](https://arxiv.org/abs/2404.11531) | [![GitHub Stars](https://img.shields.io/github/stars/cmavro/PackLLM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/cmavro/PackLLM) |
| 2024-04 | **EVA** | Learns vocabulary mappings so different models can ensemble token by token | [Bridging the Gap between Different Vocabularies for LLM Ensemble](https://arxiv.org/abs/2404.09492) | [![GitHub Stars](https://img.shields.io/github/stars/xydaytoy/EVA?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/xydaytoy/EVA) |
| 2024-02 | **-** | Uses a benign small model to pull token probabilities away from harmful outputs | [Purifying large language models by ensembling a small language model](https://arxiv.org/abs/2402.14845) | - |




Methods that explore how to generate, assess, and select short text spans from multiple LLMs during decoding, so that the best segment can be fed back for the next step:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-06 | **RLAE** | Adjusts model weights on the fly as generation goes on | [RLAE: Reinforcement Learning-Assisted Ensemble for LLMs](https://arxiv.org/abs/2506.00439) | - |
| 2024-12 | **SpecFuse** | Lets models draft short spans, then picks the best one for the next step | [SpecFuse: Ensembling Large Language Models via Next-Segment Prediction](https://arxiv.org/abs/2412.07380) | - |
| 2025-02 | **Speculative Ensemble** | Lets one model draft a span and others verify it for faster decoding | [Speculative Ensemble: Fast Large Language Model Ensemble via Speculation](https://arxiv.org/abs/2502.01662) | [![GitHub Stars](https://img.shields.io/github/stars/Kamichanw/Speculative-Ensemble?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Kamichanw/Speculative-Ensemble/) |
| 2024-09 | **SweetSpan** | Lets each model write a short span, then uses mutual scoring to choose one | [Hit the Sweet Spot! Span-Level Ensemble for Large Language Models](https://arxiv.org/abs/2409.18583) | - |
| 2024-07 | **Cool-Fusion** | Waits for a shared word boundary, then selects the best whole span | [Cool-Fusion: Fuse Large Language Models without Training](https://arxiv.org/abs/2407.19807) | - |




Methods that explore multiple reasoning steps across LLMs during multi-step problem solving, and choose the most promising next step or reasoning path along the way:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-11 | **CBS** | Explores many next reasoning steps, then keeps the ones backed by collective consensus | [Collaborative Beam Search: Enhancing LLM Reasoning via Collective Consensus](https://aclanthology.org/2025.emnlp-main.574/) | - |
| 2024-12 | **LE-MCTS** | Searches over next reasoning steps and keeps the path with the best process reward | [Ensembling Large Language Models with Process Reward-Guided Tree Search for Better Complex Reasoning](https://arxiv.org/abs/2412.15797) | - |

#### 5.2.2 Ensemble-After-Inference Papers


Methods that explore how to compare multiple complete responses after generation, either by selecting the single best answer or by choosing a strong subset for regeneration:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-12 | **LLM-PeerReview** | Lets LLM judges score candidate answers and picks the best-reviewed one | [Scoring, Reasoning, and Selecting the Best! Ensembling Large Language Models via a Peer-Review Process](https://arxiv.org/abs/2512.23213) | [![GitHub Stars](https://img.shields.io/github/stars/zeyuji/LLM-PeerReview?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/zeyuji/LLM-PeerReview) |
| 2025-10 | **LLMartini** | Aligns answer parts so users can compare and compose a final response | [LLMartini: Seamless and Interactive Leveraging of Multiple LLMs through Comparison and Composition](https://arxiv.org/abs/2510.19252) | - |
| 2025-10 | **Beyond Consensus** | Uses minority veto to stop overly agreeable judges from accepting bad answers | [Beyond Consensus: Mitigating the Agreeableness Bias in LLM Judge Evaluations](https://arxiv.org/abs/2510.11822) | [![GitHub Stars](https://img.shields.io/github/stars/ai-cet/paper-arxiv-llm-judge-calibration?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ai-cet/paper-arxiv-llm-judge-calibration) |
| 2025-10 | **OW/ISP** | Uses who agrees with whom, not just vote counts | [Beyond Majority Voting: LLM Aggregation by Leveraging Higher-Order Information](https://www.arxiv.org/abs/2510.01499) | - |
| 2025-09 | **FLAME** | Aggregates line-level annotations from several LLMs to rank bug locations | [Explainable Fault Localization for Programming Assignments via LLM-Guided Annotation](https://arxiv.org/pdf/2509.25676v1) | [![GitHub Stars](https://img.shields.io/github/stars/FLAME-FL/FLAME?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/FLAME-FL/FLAME) |
| 2025-09 | **CARGO** | Uses confidence-aware scoring to decide which model to trust more | [CARGO: A Framework for Confidence-Aware Routing of Large Language Models](https://arxiv.org/abs/2509.14899) | - |
| 2025-07 | **LENS** | Learns how much to trust each answer from internal states | [LENS: Learning Ensemble Confidence from Neural States for Multi-LLM Answer Integration](https://arxiv.org/abs/2507.23167) | - |
| 2025-05 | **EL4NER** | Merges small-LLM NER outputs and self-checks the final spans | [EL4NER: Ensemble Learning for Named Entity Recognition via Multiple Small-Parameter Large Language Models](https://arxiv.org/abs/2505.23038) | - |
| 2025-03 | **Symbolic-MoE** | Selects skill-matched experts and then combines their finished reasonings | [Symbolic Mixture-of-Experts: Adaptive Skill-based Routing for Heterogeneous Reasoning](https://arxiv.org/abs/2503.05641) | [![GitHub Stars](https://img.shields.io/github/stars/dinobby/Symbolic-MoE?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/dinobby/Symbolic-MoE/) |
| 2025-01 | **DFPE** | Keeps diverse strong models, filters weak ones, and reweights the rest | [DFPE: A Diverse Fingerprint Ensemble for Enhancing LLM Performance](https://arxiv.org/abs/2501.17479) | [![GitHub Stars](https://img.shields.io/github/stars/nivgold/DFPE?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/nivgold/DFPE) |
| 2025-01 | **DMoA** | Balances diversity and consistency before mixing answers | [Balancing Act: Diversity and Consistency in Large Language Model Ensembles](https://openreview.net/pdf?id=Dl6nkKKvlX) | - |
| 2024-12 | **Smoothie** | Picks the answer most supported by the others, without labels | [Smoothie: Label Free Language Model Routing](https://arxiv.org/abs/2412.04692) | [![GitHub Stars](https://img.shields.io/github/stars/HazyResearch/smoothie?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/HazyResearch/smoothie) |
| 2024-10 | **LLM-Forest** | Uses weighted voting across graph-guided prompt variants | [LLM-Forest: Ensemble Learning of LLMs with Graph-Augmented Prompts for Data Imputation](https://arxiv.org/abs/2410.21520) | [![GitHub Stars](https://img.shields.io/github/stars/Xinrui17/LLM-Forest?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Xinrui17/LLM-Forest) |
| 2024-10 | **LLM-TOPLA** | Selects a diverse top-*k* set before regeneration | [LLM-TOPLA: Efficient LLM Ensemble by Maximising Diversity](https://arxiv.org/abs/2410.03953) | [![GitHub Stars](https://img.shields.io/github/stars/git-disl/llm-topla?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/git-disl/llm-topla) |
| 2024-10 | **MLKF** | Fuses complementary reasoning from multiple LLMs into one answer | [Two Heads are Better than One: Zero-shot Cognitive Reasoning via Multi-LLM Knowledge Fusion](https://dl.acm.org/doi/abs/10.1145/3627673.3679744) | [![GitHub Stars](https://img.shields.io/github/stars/trueBatty/MLKF?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/trueBatty/MLKF) |
| 2024-08 | **URG** | Learns ranking and regeneration together | [URG: A Unified Ranking and Generation Method for Ensembling Language Models](https://aclanthology.org/2024.findings-acl.261/) | - |
| 2024-02 | **Agent-Forest** | Samples many answers and keeps the one most supported by voting | [More Agents Is All You Need](https://arxiv.org/abs/2402.05120) | [![GitHub Stars](https://img.shields.io/github/stars/MoreAgentsIsAllYouNeed/AgentForest?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/MoreAgentsIsAllYouNeed/AgentForest) |
| 2023-06 | **LLM-Blender** | Ranks answers first, then fuses the best few into one | [LLM-Blender: Ensembling Large Language Models with Pairwise Ranking and Generative Fusion](https://arxiv.org/abs/2306.02561) | [![GitHub Stars](https://img.shields.io/github/stars/yuchenlin/LLM-Blender?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yuchenlin/LLM-Blender) |
| 2023-05 | **MoRE** | Uses agreement among reasoning experts to choose an answer or abstain | [Getting MoRE out of Mixture of Language Model Reasoning Experts](https://arxiv.org/abs/2305.14628) | [![GitHub Stars](https://img.shields.io/github/stars/NoviScl/MoRE?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/NoviScl/MoRE) |





#### 5.2.3 Ensemble-Before-Inference Papers


Methods that route each query by predicting discrete model utility—such as whether a model is likely to be good enough, or which model is better than another under the query:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-10 | **DiSRouter** | Lets models help decide which peer should answer | [DISROUTER: Distributed Self-Routing for LLM Selections](https://arxiv.org/abs/2510.19208) | - |
| 2025-06 | **TagRouter** | Matches queries to model tags instead of training a heavy router | [TAGROUTER: Learning Route to LLMs through Tags for Open-Domain Text Generation Tasks](https://arxiv.org/abs/2506.12473) | - |
| 2025-06 | **Router-R1** | Learns multi-round routing to choose and combine models better | [Router-R1: Teaching LLMs Multi-Round Routing and Aggregation via Reinforcement Learning](https://arxiv.org/abs/2506.09033) | [![GitHub Stars](https://img.shields.io/github/stars/ulab-uiuc/Router-R1?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ulab-uiuc/Router-R1) |
| 2025-06 | **RadialRouter** | Builds a structured query view for more robust routing | [RadialRouter: Structured Representation for Efficient and Robust Large Language Models Routing](https://www.arxiv.org/abs/2506.03880) | - |
| 2025-05 | **RTR** | Chooses both the model and the reasoning style | [Route to Reason: Adaptive Routing for LLM and Reasoning Strategy Selection](https://arxiv.org/abs/2505.19435) | [![GitHub Stars](https://img.shields.io/github/stars/goodmanpzh/Route-To-Reason?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/goodmanpzh/Route-To-Reason) |
| 2024-12 | **Bench-CoE** | Routes queries using benchmark-based model strengths | [Bench-CoE: a Framework for Collaboration of Experts from Benchmark](https://arxiv.org/abs/2412.04167) | [![GitHub Stars](https://img.shields.io/github/stars/ZhangXJ199/Bench-CoE?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ZhangXJ199/Bench-CoE) |
| 2024-10 | **GraphRouter** | Uses graph structure to choose the best model | [GraphRouter: A Graph-based Router for LLM Selections](https://arxiv.org/abs/2410.03834) | [![GitHub Stars](https://img.shields.io/github/stars/ulab-uiuc/GraphRouter?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ulab-uiuc/GraphRouter) |
| 2024-09 | **Eagle** | Compares candidate models without extra router training | [Eagle: Efficient Training-Free Router for Multi-LLM Inference](https://arxiv.org/abs/2409.15518) | - |
| 2024-08 | **SelectLLM** | Scores each query and picks an efficient model | [SelectLLM: Query-Aware Efficient Selection Algorithm for Large Language Models](https://arxiv.org/abs/2408.08545) | - |
| 2024-06 | **RouteLLM** | Learns when a cheaper model can replace a stronger one | [RouteLLM: Learning to Route LLMs with Preference Data](https://arxiv.org/abs/2406.18665) | [![GitHub Stars](https://img.shields.io/github/stars/lm-sys/RouteLLM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/lm-sys/RouteLLM) |
| 2024-05 | **LLM Routing Lessons** | Shows which prompt cues help choose the right model | [Harnessing the Power of Multiple Minds: Lessons Learned from LLM Routing](https://arxiv.org/abs/2405.00467) | [![GitHub Stars](https://img.shields.io/github/stars/kvadityasrivatsa/llm-routing?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/kvadityasrivatsa/llm-routing) |
| 2024-04 | **Hybrid-LLM** | Balances answer quality and cost before choosing a model | [Hybrid LLM: Cost-Efficient and Quality-Aware Query Routing](https://arxiv.org/abs/2404.14618) | [![GitHub Stars](https://img.shields.io/github/stars/m365-core/hybrid_llm_routing?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/m365-core/hybrid_llm_routing) |
| 2024-03 | **ETR** | Routes expert tokens to the most suitable specialist model | [An Expert is Worth One Token: Synergizing Multiple Expert LLMs as Generalist via Expert Token Routing](https://arxiv.org/abs/2403.16854) | [![GitHub Stars](https://img.shields.io/github/stars/zjunet/ETR?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/zjunet/ETR) |
| 2024-01 | **Routoo** | Learns to send each query to the model most likely to work | [Routoo: Learning to Route to Large Language Models Effectively](https://arxiv.org/abs/2401.13979) | - |
| 2024 | **RouterDC** | Learns query embeddings that make routing easier | [RouterDC: Query-Based Router by Dual Contrastive Learning for Assembling Large Language Models](https://proceedings.neurips.cc/paper_files/paper/2024/hash/7a641b8ec86162fc875fb9f6456a542f-Abstract-Conference.html) | [![GitHub Stars](https://img.shields.io/github/stars/shuhao02/RouterDC?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/shuhao02/RouterDC) |
| 2023-11 | **ZOOTER** | Uses reward signals to pick the right expert model | [Routing to the Expert: Efficient Reward-guided Ensemble of Large Language Models](https://arxiv.org/abs/2311.08692) | - |
| 2023-08 | **FORC** | Chooses the cheapest model that is still good enough | [Fly-Swat or Cannon? Cost-Effective Language Model Choice via Meta-Modeling](https://arxiv.org/abs/2308.06077) | [![GitHub Stars](https://img.shields.io/github/stars/epfl-dlab/forc?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/epfl-dlab/forc) |
| 2023 | **Benchmark Routing** | Builds routing rules from benchmark-level model performance | [LLM Routing with Benchmark Datasets](https://openreview.net/forum?id=k9EfAJhFZc) | - |



Methods that route each query by predicting continuous model utility—such as performance scores, costs, latency, or combined rewards—so the router can make finer trade-offs:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-10 | **WebRouter** | Compresses web-agent prompts and routes with cost in mind | [WebRouter: Query-specific Router via Variational Information Bottleneck for Cost-sensitive Web Agent](https://arxiv.org/abs/2510.11221) | - |
| 2025-10 | **LLMRank** | Uses rich query features to rank which model should answer | [LLMRank: Understanding LLM Strengths for Model Routing](https://arxiv.org/abs/2510.01234) | - |
| 2025-05 | **Avengers** | Combines small models by routing queries to their strengths | [The Avengers: A Simple Recipe for Uniting Smaller Language Models to Challenge Proprietary Giants](https://arxiv.org/abs/2505.19797) | [![GitHub Stars](https://img.shields.io/github/stars/ZhangYiqun018/Avengers?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ZhangYiqun018/Avengers) |
| 2025-05 | **InferenceDynamics** | Profiles model skills and knowledge before routing | [InferenceDynamics: Efficient Routing Across LLMs through Structured Capability and Knowledge Profiling](https://arxiv.org/abs/2505.16303) | - |
| 2025-05 | **kNN Router** | Uses nearest past queries instead of a complex learned router | [Rethinking Predictive Modeling for LLM Routing: When Simple kNN Beats Complex Learned Routers](https://arxiv.org/abs/2505.12601) | - |
| 2025 | **RELM** | Learns recommendation and evaluation together for model selection | [Co-optimizing Recommendation and Evaluation for LLM Selection](https://openreview.net/pdf?id=gWi4ZcPQRl) | - |
| 2025-02 | **LLM Bandit** | Explores cheap options first and learns cost-aware routing online | [LLM Bandit: Cost-Efficient LLM Generation via Preference-Conditioned Dynamic Routing](https://arxiv.org/abs/2502.02743) | - |
| 2024-12 | **PickLLM** | Uses RL to pick the best model from context and budget cues | [PickLLM: Context-Aware RL-Assisted Large Language Model Routing](https://arxiv.org/abs/2412.12170) | - |
| 2024-08 | **TO-Router** | Predicts utility under latency and cost constraints | [TensorOpera Router: A Multi-Model Router for Efficient LLM Inference](https://arxiv.org/abs/2408.12320) | - |
| 2024-07 | **MetaLLM** | Wraps several models and picks one using predicted utility | [MetaLLM: A High-performant and Cost-efficient Dynamic Framework for Wrapping LLMs](https://arxiv.org/abs/2407.10834) | [![GitHub Stars](https://img.shields.io/github/stars/mail-research/MetaLLM-wrapper?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/mail-research/MetaLLM-wrapper/) |
| 2024-06 | **HomoRouter** | Routes queries among similar tools with fine-grained scoring | [Query Routing for Homogeneous Tools: An Instantiation in the RAG Scenario](https://arxiv.org/abs/2406.12429) | - |
| 2024-01 | **Blending** | Blends model strengths as a cheaper alternative to one giant model | [Blending Is All You Need: Cheaper, Better Alternative to Trillion-Parameters LLM](https://arxiv.org/abs/2401.02994) | - |

#### 5.2.4 Cascaded-Based Papers





Methods that explore an ordered chain of models—typically from cheaper/weaker ones to more capable/costlier ones—to decide whether a query can stop early, should defer upward, or should switch routes to obtain a better answer under a desired cost-performance trade-off:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-12 | **RoBoN** | Routes best-of-n samples across multiple LLMs, exploring which model adds the highest next-response gain via reward and agreement signals | [RoBoN: Routed Online Best-of-n for Test-Time Scaling with Multiple LLMs](https://arxiv.org/abs/2512.05542) | [![GitHub Stars](https://img.shields.io/github/stars/j-geuter/RoBoN?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/j-geuter/RoBoN) |
| 2025-09 | **Semantic Agreement** | Uses meaning-level agreement between model outputs to explore whether a query can stop at a smaller model or should defer upward | [Semantic Agreement Enables Efficient Open-Ended LLM Cascades](https://arxiv.org/abs/2509.21837) | - |
| 2025-04 | **EMAFusion** | Combines taxonomy routing, learned routing, and confidence-triggered escalation to explore the cheapest reliable model path for each query | [EMAFusion: A Self-Optimizing System for Seamless LLM Selection and Integration](https://arxiv.org/abs/2504.10681) | - |
| 2025-04 | **ModelSwitch** | Uses sample consistency to explore when repeated sampling should stay with the current model or switch to a complementary one | [Do We Truly Need So Many Samples? Multi-LLM Repeated Sampling Efficiently Scales Test-Time Compute](https://arxiv.org/abs/2504.00762) | [![GitHub Stars](https://img.shields.io/github/stars/JianhaoChen-nju/ModelSwitch?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/JianhaoChen-nju/ModelSwitch) |
| 2024-12 | **DER** | Treats expert selection as sequential route exploration, choosing the next LLM to add complementary knowledge with minimal compute | [Dynamic Ensemble Reasoning for LLM Experts](https://arxiv.org/abs/2412.07448) | - |
| 2024-10 | **Cascade Routing** | Unifies routing and cascading to explore the model chain only when quality estimates suggest extra capacity will pay off | [A Unified Approach to Routing and Cascading for LLMs](https://arxiv.org/abs/2410.10347) | [![GitHub Stars](https://img.shields.io/github/stars/eth-sri/cascade-routing?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/eth-sri/cascade-routing) |
| 2024-04 | **LM Cascades** | Uses token-level uncertainty to explore whether a generative response is reliable enough to stop or should be deferred to a larger model | [Language Model Cascades: Token-level Uncertainty and Beyond](https://arxiv.org/abs/2404.10136) | - |
| 2023-10 | **AutoMix** | Uses self-verification and POMDP routing to explore whether a weaker model is sufficient or a larger model is needed | [AutoMix: Automatically Mixing Language Models](https://arxiv.org/abs/2310.12963) | [![GitHub Stars](https://img.shields.io/github/stars/automix-llm/automix?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/automix-llm/automix) |
| 2023-10 | **Neural Caching** | Uses active selection to explore which queries a continuously distilled student can absorb and which should still go to the teacher | [Cache & Distil: Optimising API Calls to Large Language Models](https://arxiv.org/abs/2310.13561) | [![GitHub Stars](https://img.shields.io/github/stars/guillemram97/neural-caching?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/guillemram97/neural-caching) |
| 2023-10 | **MoT Cascade** | Uses weak-model answer consistency, enriched with CoT/PoT thought mixtures, to explore whether escalation is necessary | [Large Language Model Cascades with Mixture of Thoughts Representations for Cost-efficient Reasoning](https://arxiv.org/abs/2310.03094) | [![GitHub Stars](https://img.shields.io/github/stars/MurongYue/LLM_MoT_cascade?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/MurongYue/LLM_MoT_cascade) |
| 2023-10 | **EcoAssistant** | Explores a hierarchy of assistants, refining with execution feedback and backing off to stronger models only when needed | [EcoAssistant: Using LLM Assistant More Affordably and Accurately](https://arxiv.org/abs/2310.03046) | [![GitHub Stars](https://img.shields.io/github/stars/JieyuZ2/EcoAssistant?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/JieyuZ2/EcoAssistant) |
| 2023-05 | **FrugalGPT** | Explores budget-aware combinations of LLMs, adaptively choosing a query-specific cascade for cost-efficient accuracy | [FrugalGPT: How to Use Large Language Models While Reducing Cost and Improving Performance](https://arxiv.org/abs/2305.05176) | - |
| 2023-01 | **Confidence Deferral** | Clarifies when confidence-only deferral can explore the cascade effectively and when downstream-aware signals are required | [When Does Confidence-Based Cascade Deferral Suffice?](https://proceedings.neurips.cc/paper_files/paper/2023/hash/1f09e1ee5035a4c3fe38a5681cae5815-Abstract-Conference.html) | - |
| 2022-10 | **Model Cascading** | Explores early exit across models of increasing capacity, reserving large-model compute for harder inputs | [Model Cascading: Towards Jointly Improving Efficiency and Accuracy of NLP Systems](https://arxiv.org/abs/2210.05528) | - |


<br>

### 5.3 MARL
| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-12 | **SDAX** | Treats unsupervised skill discovery as high-level exploration and bi-level tunes diversity-vs-task rewards to learn agile locomotion behaviors | [Unsupervised Skill Discovery as Exploration for Learning Agile Locomotion](https://arxiv.org/abs/2508.08982) | - |
| 2025-09 | **CERMIC** | Calibrates curiosity with inferred peer-intention context to filter noisy novelty and reward high information-gain transitions in sparse-reward MARL | [Wonder Wins Ways: Curiosity-Driven Exploration through Multi-Agent Contextual Calibration](https://arxiv.org/abs/2509.20648) | [![GitHub Stars](https://img.shields.io/github/stars/PyyWill/CERMIC?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/PyyWill/CERMIC) |
| 2025-02 | **TEE** | Maximizes cross-agent trajectory entropy in a contrastive latent space via particle-based estimation, yielding intrinsic rewards for diverse coordinated exploration | [Toward Efficient Multi-Agent Exploration with Trajectory Entropy Maximization](https://arxiv.org/abs/2502.08365v1) | - |
| 2025-02 | **Consensus-Diversity Tradeoff** | Shows implicit consensus with partial disagreement can preserve exploration diversity and improve robustness in dynamic multi-agent settings | [The Hidden Strength of Disagreement: Unraveling the Consensus-Diversity Tradeoff in Adaptive Multi-Agent Systems](https://arxiv.org/abs/2502.16565) | [![GitHub Stars](https://img.shields.io/github/stars/wuzengqing001225/ConsensusDiversityTradeoffMAS?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/wuzengqing001225/ConsensusDiversityTradeoffMAS) |
| 2023-02 | **EMAX** | Uses per-agent value ensembles for UCB-guided exploration, low-variance ensemble targets, and majority-vote action selection to reduce miscoordination | [Ensemble Value Functions for Efficient Exploration in Multi-Agent Reinforcement Learning](https://arxiv.org/abs/2302.03439) | - |
| 2022-08 | **MACE** | Combines collaborative voxel mapping, global goal assignment, and time-aware safe-corridor planning for collision-safe multi-robot exploration of unknown spaces | [MACE: Multi-Agent Autonomous Collaborative Exploration of Unknown Environments](https://arxiv.org/abs/2208.06949) | - |
| 2021-12 | **MASAC** | Proposes a CTDE multi-agent soft actor-critic front-end for collaborative waypoint search, coupled with minimal-snap trajectory optimization for executable robot motion | [Multi-agent Soft Actor-Critic Based Hybrid Motion Planner for Mobile Robots](https://arxiv.org/abs/2112.06594) | - |
| 2021-11 | **EMC** | Uses prediction errors of induced individual Q-values as coordinated intrinsic rewards, plus episodic memory to reinforce informative experiences | [Episodic Multi-agent Reinforcement Learning with Curiosity-Driven Exploration](https://arxiv.org/abs/2111.11032) | [![GitHub Stars](https://img.shields.io/github/stars/kikojay/EMC?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/kikojay/EMC) |
| 2021-07 | **CMAE** | Selects shared exploration goals from entropy-scored projected state spaces and trains agents to reach them in a coordinated way | [Cooperative Exploration for Multi-Agent Deep Reinforcement Learning](https://arxiv.org/abs/2107.11444) | [![GitHub Stars](https://img.shields.io/github/stars/IouJenLiu/CMAE?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/IouJenLiu/CMAE) |
| 2019-10 | **MAVEN** | Introduces latent-variable hierarchical control to induce temporally committed exploration modes while retaining value-decomposition scalability | [MAVEN: Multi-Agent Variational Exploration](https://arxiv.org/abs/1910.07483) | [![GitHub Stars](https://img.shields.io/github/stars/AnujMahajanOxf/MAVEN?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/AnujMahajanOxf/MAVEN) |
| 2019-10 | **EITI/EDTI** | Encourages coordinated exploration by maximizing inter-agent influence, using mutual information (EITI) and value-of-interaction rewards (EDTI) | [Influence-Based Multi-Agent Exploration](https://arxiv.org/abs/1910.05512) | [![GitHub Stars](https://img.shields.io/github/stars/TonghanWang/EITI-EDTI?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/TonghanWang/EITI-EDTI) |
| 2017-05 | **ICM** | Defines curiosity as forward-model prediction error in inverse-dynamics features, promoting exploration without relying on extrinsic rewards | [Curiosity-driven Exploration by Self-supervised Prediction](https://arxiv.org/abs/1705.05363) | [![GitHub Stars](https://img.shields.io/github/stars/pathak22/noreward-rl?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/pathak22/noreward-rl) |




<br>


### 5.4 Self-Evolving

Methods that let agents or LLMs continuously improve themselves—via self-generated rewards, self-feedback critiques, self-curriculum, or RL on self-collected trajectories—turning the model into the source of its own training signal and expanding its capability frontier through self-driven exploration:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-11 | **AgentEvolver** | Self-evolves an LLM agent through self-questioning, self-navigating, and self-attributing modules so it generates its own tasks, trajectories, and credit signals for autonomous capability growth | [AgentEvolver: Towards Efficient Self-Evolving Agent System](https://arxiv.org/abs/2511.10395) | [![GitHub Stars](https://img.shields.io/github/stars/modelscope/AgentEvolver?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/modelscope/AgentEvolver) |
| 2025-05 | **SPA-RL** | Decomposes a long-horizon agent's final reward into per-step progress contributions, providing dense intermediate rewards that stabilise RL on sparse-reward tasks | [SPA-RL: Reinforcing LLM Agents via Stepwise Progress Attribution](https://arxiv.org/abs/2505.20732) | [![GitHub Stars](https://img.shields.io/github/stars/WangHanLinHenry/SPA-RL-Agent?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/WangHanLinHenry/SPA-RL-Agent) |
| 2025-05 | **GiGPO** | Adds an inner step-level group baseline on top of trajectory-level GRPO, enabling fine-grained credit assignment for multi-turn LLM agent training | [Group-in-Group Policy Optimization for LLM Agent Training](https://arxiv.org/abs/2505.10978) | [![GitHub Stars](https://img.shields.io/github/stars/langfengQ/verl-agent?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/langfengQ/verl-agent) |
| 2025-05 | **SRSI** | LLM acts as its own judge to score self-generated solutions and uses these self-rewards as RL signal, bootstrapping improvement without external labels | [Self Rewarding Self Improving](https://arxiv.org/abs/2505.08827) | - |
| 2025-03 | **DAPO** | Open-source large-scale LLM RL recipe introducing clip-higher, dynamic sampling, token-level policy-gradient loss, and overlong-reward shaping for stable scaling | [DAPO: An Open-Source LLM Reinforcement Learning System at Scale](https://arxiv.org/abs/2503.14476) | [![GitHub Stars](https://img.shields.io/github/stars/BytedTsinghua-SIA/DAPO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/BytedTsinghua-SIA/DAPO) |
| 2025-02 | **SiriuS** | Builds an experience library of successful multi-agent reasoning trajectories—augmented by re-trying and rewriting failed ones—and fine-tunes the agents on it for self-improvement | [SiriuS: Self-improving Multi-agent Systems via Bootstrapped Reasoning](https://arxiv.org/abs/2502.04780) | [![GitHub Stars](https://img.shields.io/github/stars/zou-group/sirius?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/zou-group/sirius) |
| 2024-11 | **WebRL** | Self-evolving online curriculum turns failed web tasks into new training instructions, paired with an outcome-supervised reward model and KL-constrained policy updates | [WebRL: Training LLM Web Agents via Self-Evolving Online Curriculum Reinforcement Learning](https://arxiv.org/abs/2411.02337) | [![GitHub Stars](https://img.shields.io/github/stars/THUDM/WebRL?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/THUDM/WebRL) |
| 2024-06 | **TextGrad** | Treats LLM-generated natural-language critiques as textual "gradients" and back-propagates them through compound AI systems to optimise prompts, code, and components end-to-end | [TextGrad: Automatic "Differentiation" via Text](https://arxiv.org/abs/2406.07496) | [![GitHub Stars](https://img.shields.io/github/stars/zou-group/textgrad?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/zou-group/textgrad) |
| 2024-06 | **DigiRL** | Two-stage offline-then-online autonomous RL with a VLM-based evaluator and an advantage-filtered curriculum to train robust Android device-control agents in the wild | [DigiRL: Training In-The-Wild Device-Control Agents with Autonomous Reinforcement Learning](https://arxiv.org/abs/2406.11896) | [![GitHub Stars](https://img.shields.io/github/stars/DigiRL-agent/digirl?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/DigiRL-agent/digirl) |
| 2024-03 | **Quiet-STaR** | Generalises STaR by sampling internal rationales at every token position and reinforcing the ones that improve next-token prediction, teaching LMs to "think" silently before speaking | [Quiet-STaR: Language Models Can Teach Themselves to Think Before Speaking](https://arxiv.org/abs/2403.09629) | [![GitHub Stars](https://img.shields.io/github/stars/ezelikman/quiet-star?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ezelikman/quiet-star) |
| 2024-02 | **GRPO** | Removes PPO's value network by using group-sampled rollouts to compute the baseline, enabling memory-efficient on-policy RL for LLMs (introduced in DeepSeekMath) | [DeepSeekMath: Pushing the Limits of Mathematical Reasoning in Open Language Models](https://arxiv.org/abs/2402.03300) | [![GitHub Stars](https://img.shields.io/github/stars/deepseek-ai/DeepSeek-Math?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/deepseek-ai/DeepSeek-Math) |
| 2024-01 | **SRLM** | LLM acts as its own judge via LLM-as-a-Judge prompting, generates preference pairs on its own outputs, and iteratively DPO-trains on them—removing the human reward bottleneck | [Self-Rewarding Language Models](https://arxiv.org/abs/2401.10020) | - |
| 2023-10 | **SELF** | Iterative self-evolution loop where the model self-critiques and self-refines its outputs in natural-language feedback, then fine-tunes on the improved data | [SELF: Self-Evolution with Language Feedback](https://arxiv.org/abs/2310.00533) | - |
| 2023-05 | **DPO** | Re-parameterises RLHF so the LM itself implicitly defines the reward, reducing alignment to a simple classification loss on preference pairs—no separate reward model or RL loop needed | [Direct Preference Optimization: Your Language Model is Secretly a Reward Model](https://arxiv.org/abs/2305.18290) | [![GitHub Stars](https://img.shields.io/github/stars/eric-mitchell/direct-preference-optimization?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/eric-mitchell/direct-preference-optimization) |
| 2023-04 | **RRHF** | Aligns LLMs to human preferences by sampling multiple candidate responses and applying a ranking loss based on their reward order, sidestepping the complexity of PPO | [RRHF: Rank Responses to Align Language Models with Human Feedback without Tears](https://arxiv.org/abs/2304.05302) | [![GitHub Stars](https://img.shields.io/github/stars/GanjinZero/RRHF?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/GanjinZero/RRHF) |
| 2023-03 | **Self-Refine** | Same LLM iteratively produces feedback on its own output and refines it across rounds, improving quality at inference time without any extra training or external supervision | [Self-Refine: Iterative Refinement with Self-Feedback](https://arxiv.org/abs/2303.17651) | [![GitHub Stars](https://img.shields.io/github/stars/madaan/self-refine?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/madaan/self-refine) |
| 2023-03 | **Reflexion** | Agent verbalises why a trial failed, stores the reflection in episodic memory, and uses it to guide subsequent trials—"verbal" reinforcement learning without weight updates | [Reflexion: Language Agents with Verbal Reinforcement Learning](https://arxiv.org/abs/2303.11366) | [![GitHub Stars](https://img.shields.io/github/stars/noahshinn/reflexion?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/noahshinn/reflexion) |
| 2022-03 | **STaR** | Generates rationales for problems, rationalises wrong answers given the correct one, and iteratively fine-tunes on rationales that yield correct answers, bootstrapping reasoning ability | [STaR: Bootstrapping Reasoning with Reasoning](https://arxiv.org/abs/2203.14465) | [![GitHub Stars](https://img.shields.io/github/stars/ezelikman/STaR?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ezelikman/STaR) |


---
<br>


## 6. Exploration Evaluation

### 6.1 Principles & Infrastructure

Exploration is not a primitive observable but an inferential claim about how an agent handles uncertainty, learning, and future choice. An adequate evaluation must separate exploratory behaviour from mere activity, benefit from base competence, and open-ended search from premature convergence.

**Three principles — what counts as exploring:**
- **C1 Information Gain.** The agent actively reduces uncertainty through directed information-seeking. Signals: uncertainty reduction, calibration improvement, informative state acquisition.
- **C2 Value Improvement.** The agent converts acquired information into improved competence. Signals: performance gains, sample-efficiency, boundary expansion on harder tasks.
- **C3 Epistemic Reachability.** The agent preserves access to plausible future states, actions, and hypotheses consistent with its current beliefs. Signals: coverage, behavioural diversity, anti-collapse.

**Five infrastructure components — how to construct an exploration evaluation:**
- **Task.** Design at the *competence boundary* — low one-shot pass@1 with a wide pass@1-to-pass@k gap; reward feedback-rich, revisable settings.
- **Metrics.** Pair coverage (pass@k, Unique@k), robustness (Maj@k, self-correction $\Delta_{\text{self}}$, Pass^k), and efficiency (search-budget normalised performance).
- **Grader.** Combine code-based, model-based (incl. process reward models), and human grading; reward informative failures, not only correct outcomes.
- **Outcome.** Three tiers — immediate task success, boundary-expansion premium $\Delta_{\text{explore}}$, transferable capability acquisition.
- **Environment.** Partial observability, backtracking, intermediate feedback, sufficient complexity, trial isolation, safety/sandboxing.

**Criterion–component mapping** (primary components per criterion):
- **C1 Information Gain** → **Metrics, Environment, Grader.** Measure uncertainty reduction; partial observability necessitates active information-seeking; PRMs grade process quality.
- **C2 Value Improvement** → **Outcome, Metrics, Grader.** Capture boundary expansion; measure pass@1 vs pass@k gap; recognise novel valid solutions.
- **C3 Epistemic Reachability** → **Task, Metrics, Environment.** Design multi-path tasks; measure diversity and coverage; ensure branching structure supports genuine choice.

<br>

### 6.2 Reasoning-Space Evaluation

Frontier reasoning suites, code benchmarks with executable feedback, and classical sparse-reward settings — together they expose the pass@1-to-pass@k gap, make self-correction $\Delta_{\text{self}}$ measurable, and diagnose entropy collapse and chain-of-thought shortening:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2024-11 | **FrontierMath** | Exposes the pass@1-to-pass@k gap at capability frontiers, measuring whether reasoning search reaches answers beyond one-shot competence | [FrontierMath: A Benchmark for Evaluating Advanced Mathematical Reasoning in AI](https://arxiv.org/abs/2411.04872) | - |
| 2024-02 | **OlympiadBench** | Probes whether extended reasoning chains resolve genuine uncertainty or merely rephrase prior content at olympiad-level difficulty | [OlympiadBench: A Challenging Benchmark for Promoting AGI with Olympiad-Level Bilingual Multimodal Scientific Problems](https://arxiv.org/abs/2402.14008) | [![GitHub Stars](https://img.shields.io/github/stars/OpenBMB/OlympiadBench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/OpenBMB/OlympiadBench) |
| 2025-01 | **Humanity's Last Exam** | Tests epistemic reachability by revealing which answers remain inaccessible even when exploratory reasoning branches are exhausted | [Humanity's Last Exam](https://www.lastexam.ai/) | [![GitHub Stars](https://img.shields.io/github/stars/centerforaisafety/hle?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/centerforaisafety/hle) |
| 2024-03 | **LiveCodeBench** | Adds executable feedback to reasoning evaluation, making self-correction gain directly measurable as a signal of productive exploration | [LiveCodeBench: Holistic and Contamination Free Evaluation of Large Language Models for Code](https://arxiv.org/abs/2403.07974) | [![GitHub Stars](https://img.shields.io/github/stars/LiveCodeBench/LiveCodeBench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/LiveCodeBench/LiveCodeBench) |
| 2023-10 | **SWE-bench** | Provides verifiable revision signals on real-world tasks, enabling direct measurement of whether reasoning exploration improves reachable solutions | [SWE-bench: Can Language Models Resolve Real-World GitHub Issues?](https://arxiv.org/abs/2310.06770) | [![GitHub Stars](https://img.shields.io/github/stars/SWE-bench/SWE-bench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/SWE-bench/SWE-bench) |
| 2024-10 | **MLE-bench** | Assesses whether iterative reasoning under ML engineering constraints translates into harder-problem success beyond single-attempt competence | [MLE-bench: Evaluating Machine Learning Agents on Machine Learning Engineering](https://arxiv.org/abs/2410.07095) | [![GitHub Stars](https://img.shields.io/github/stars/openai/mle-bench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/openai/mle-bench) |
| 2016-06 | **Montezuma's Revenge** | Diagnoses exploration pathologies in which novelty-driven coverage fails to reduce uncertainty or transfer to downstream reasoning tasks | [Unifying Count-Based Exploration and Intrinsic Motivation](https://arxiv.org/abs/1606.01868) | - |
| 2024-02 | **Craftax** | Exposes premature chain-of-thought collapse and entropy failure by testing whether open-ended exploration sustains distinct reasoning paths over time | [Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning](https://arxiv.org/abs/2402.16801) | [![GitHub Stars](https://img.shields.io/github/stars/MichaelTMatthews/Craftax?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/MichaelTMatthews/Craftax) |


<br>

### 6.3 Interaction-Space Evaluation

The Reasoner-to-Agent transition moves exploration from internal reasoning into external action. The failure mode is poor *controller selection* — exploring too late, overcommitting to one tool, or failing to reopen search when the current strategy stops being informative. The split between *digital* and *embodied* agents matters because their failure modes, benchmark families, and grading challenges diverge.

#### 6.3.1 Digital Agents

Heterogeneous-tool, dynamic-interface, and long-horizon research-workflow benchmarks that force the controller to reopen exploration when strategies stop being informative:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2023-11 | **GAIA** | Stresses tool selection and strategy switching across heterogeneous real-world tasks to evaluate information-gain-driven action-policy control | [GAIA: A Benchmark for General AI Assistants](https://arxiv.org/abs/2311.12983) | - |
| 2024-03 | **WorkArena** | Reveals whether the controller reopens exploration when web-based interfaces and subtask structures change across knowledge-work scenarios | [WorkArena: How Capable Are Web Agents at Solving Common Knowledge Work Tasks?](https://arxiv.org/abs/2403.07718) | [![GitHub Stars](https://img.shields.io/github/stars/ServiceNow/WorkArena?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ServiceNow/WorkArena) |
| 2024-04 | **OSWorld** | Tests whether multimodal agents reopen search and adapt action policies when open-ended computer-environment tasks shift tool demands | [OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments](https://arxiv.org/abs/2404.07972) | [![GitHub Stars](https://img.shields.io/github/stars/xlang-ai/OSWorld?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/xlang-ai/OSWorld) |
| 2024-05 | **AndroidWorld** | Probes dynamic controller reselection by varying app interfaces and subtask structure to expose failures of premature exploration collapse | [AndroidWorld: A Dynamic Benchmarking Environment for Autonomous Agents](https://arxiv.org/abs/2405.14573) | [![GitHub Stars](https://img.shields.io/github/stars/google-research/android_world?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/google-research/android_world) |
| 2025-02 | **MLGym** | Extends exploration evaluation to long research workflows where detecting failure early and reallocating budget across tool use and experimentation is central | [MLGym: A New Framework and Benchmark for Advancing AI Research Agents](https://arxiv.org/abs/2502.14499) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/MLGym?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/MLGym) |
| 2026-02 | **AIRS-Bench** | Assesses frontier agents' capacity to revise search strategies and reallocate reasoning budget across multi-phase AI research science tasks | [AIRS-Bench: A Suite of Tasks for Frontier AI Research Science Agents](https://arxiv.org/abs/2602.06855) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/airs-bench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/airs-bench) |
| 2019-10 | **Meta-World** | Exposes transfer of exploratory control across related task families to separate genuine meta-control from structural-similarity reuse | [Meta-World: A Benchmark and Evaluation for Multi-Task and Meta Reinforcement Learning](https://arxiv.org/abs/1910.10897) | [![GitHub Stars](https://img.shields.io/github/stars/Farama-Foundation/Metaworld?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Farama-Foundation/Metaworld) |

#### 6.3.2 Embodied Agents

Navigation platforms, manipulation suites, and integrated embodied benchmarks that make active sensing, recovery, and behavioural diversity observable under physical cost and partial observability:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2019-04 | **Habitat** | Tests whether agent locomotion and viewpoint selection reduce spatial uncertainty under partial observability across navigation tasks | [Habitat: A Platform for Embodied AI Research](https://arxiv.org/abs/1904.01201) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/habitat-lab?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/habitat-lab) |
| 2021-06 | **Habitat 2.0** | Extends navigation evaluation to rearrangement manipulation, measuring whether active sensing improves physical interaction beyond familiar locomotion routes | [Habitat 2.0: Training Home Assistants to Rearrange their Habitat](https://arxiv.org/abs/2106.14405) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/habitat-lab?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/habitat-lab) |
| 2020-04 | **RoboTHOR** | Evaluates sim-to-real transfer fidelity so that coverage and path-efficiency gains in simulation reflect genuine sensorimotor uncertainty reduction | [RoboTHOR: An Open Simulation-to-Real Embodied AI Platform](https://arxiv.org/abs/2004.06799) | [![GitHub Stars](https://img.shields.io/github/stars/allenai/ai2thor?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/allenai/ai2thor) |
| 2022-06 | **ProcTHOR** | Procedurally generated houses test whether exploratory policies generalise across novel layouts rather than collapsing onto memorised routes | [ProcTHOR: Large-Scale Embodied AI Using Procedural Generation](https://arxiv.org/abs/2206.06994) | [![GitHub Stars](https://img.shields.io/github/stars/allenai/procthor?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/allenai/procthor) |
| 2019-12 | **ALFRED** | Benchmarks whether instruction-grounded information gathering and recovery improve long-horizon task competence across object-centric, cluttered, partially observable household settings | [ALFRED: A Benchmark for Interpreting Grounded Instructions for Everyday Tasks](https://arxiv.org/abs/1912.01734) | [![GitHub Stars](https://img.shields.io/github/stars/askforalfred/alfred?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/askforalfred/alfred) |
| 2021-08 | **BEHAVIOR** | Measures whether agents maintain behavioural diversity and recovery across everyday household activities in interactive ecological environments | [BEHAVIOR: Benchmark for Everyday Household Activities in Virtual, Interactive, and Ecological Environments](https://arxiv.org/abs/2108.03332) | [![GitHub Stars](https://img.shields.io/github/stars/StanfordVL/behavior?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/StanfordVL/behavior) |
| 2024-03 | **BEHAVIOR-1K** | Scales embodied evaluation to 1,000 activities, revealing whether exploratory competence and recovery persist across radically varied task distributions | [BEHAVIOR-1K: A Human-Centered, Embodied AI Benchmark with 1,000 Everyday Activities and Realistic Simulation](https://arxiv.org/abs/2403.09227) | [![GitHub Stars](https://img.shields.io/github/stars/StanfordVL/BEHAVIOR-1K?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/StanfordVL/BEHAVIOR-1K) |
| 2024-06 | **RoboCasa** | Large-scale everyday manipulation tasks probe whether information gathering from cluttered scenes yields value improvement in generalist robot policies | [RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots](https://arxiv.org/abs/2406.02523) | [![GitHub Stars](https://img.shields.io/github/stars/robocasa/robocasa?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/robocasa/robocasa) |
| 2025-01 | **EmbodiedEval** | Unified protocol evaluates whether multimodal LLM agents maintain navigation, interaction, and spatial uncertainty reduction across heterogeneous embodied tasks | [EmbodiedEval: Evaluate Multimodal LLMs as Embodied Agents](https://arxiv.org/abs/2501.11858) | [![GitHub Stars](https://img.shields.io/github/stars/thunlp/EmbodiedEval?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/thunlp/EmbodiedEval) |
| 2025-02 | **EmbodiedBench** | Comprehensive vision-driven benchmark tests whether coverage, recovery, and behavioural diversity persist rather than collapsing after first successful multimodal policy | [EmbodiedBench: Comprehensive Benchmarking Multi-Modal Large Language Models for Vision-Driven Embodied Agents](https://arxiv.org/abs/2502.09560) | [![GitHub Stars](https://img.shields.io/github/stars/EmbodiedBench/EmbodiedBench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/EmbodiedBench/EmbodiedBench) |
| 2025-10 | **RoboBench** | Integrated suite assesses whether embodied-brain LLMs preserve epistemic reachability across navigation, manipulation, and instruction-following under unified protocols | [RoboBench: A Comprehensive Evaluation Benchmark for Multimodal Large Language Models as Embodied Brain](https://arxiv.org/abs/2510.17801) | [![GitHub Stars](https://img.shields.io/github/stars/lyl750697268/RoboBench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/lyl750697268/RoboBench) |

<br>

### 6.4 Imagination-Space Evaluation

Open-ended MBRL suites and planning-focused benchmarks that separate "can imagine futures" from "futures are coherent" from "futures actually help real control":

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2024-02 | **Craftax** | Tests whether world-model-based exploration converts imagined rollouts into genuine epistemic gains across sparse-reward, open-ended tasks where simulation advantage is measurable | [Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning](https://arxiv.org/abs/2402.16801) | [![GitHub Stars](https://img.shields.io/github/stars/MichaelTMatthews/Craftax?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/MichaelTMatthews/Craftax) |
| 2022-06 | **MineDojo** | Evaluates whether embodied agents leverage internal simulation to reduce real interaction cost in long-horizon, open-ended environments requiring broad counterfactual reasoning | [MineDojo: Building Open-Ended Embodied Agents with Internet-Scale Knowledge](https://arxiv.org/abs/2206.08853) | [![GitHub Stars](https://img.shields.io/github/stars/MineDojo/MineDojo?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/MineDojo/MineDojo) |
| 2022-10 | **Avalon** | Probes whether model-based planners maintain epistemic reachability across procedurally generated worlds rather than collapsing onto narrow imagined trajectories | [Avalon: A Benchmark for RL Generalization Using Procedurally Generated Worlds](https://arxiv.org/abs/2210.13417) | [![GitHub Stars](https://img.shields.io/github/stars/Avalon-Benchmark/avalon?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Avalon-Benchmark/avalon) |
| 2022-06 | **PlanBench** | Isolates planning-layer failures by testing whether agents reason coherently about action and change independently of aggregate task-reward signals | [PlanBench: An Extensible Benchmark for Evaluating Large Language Models on Planning and Reasoning about Change](https://arxiv.org/abs/2206.10498) | [![GitHub Stars](https://img.shields.io/github/stars/karthikv792/LLMs-Planning?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/karthikv792/LLMs-Planning) |
| 2024-06 | **ActionReasoningBench** | Separates reasoning-about-change errors from world-model inaccuracy by benchmarking causal action inference with and without ramification constraints | [ActionReasoningBench: Reasoning about Actions with and without Ramification Constraints](https://arxiv.org/abs/2406.04046) | [![GitHub Stars](https://img.shields.io/github/stars/izuminka/reasoning_about_actions?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/izuminka/reasoning_about_actions) |
| 2024-12 | **EgoPlan-Bench2** | Assesses whether multimodal planners generate logically coherent imagined futures that translate to improved real-world sequential control outcomes | [EgoPlan-Bench2: A Benchmark for Multimodal Large Language Model Planning in Real-World Scenarios](https://arxiv.org/abs/2412.04447) | [![GitHub Stars](https://img.shields.io/github/stars/qiulu66/EgoPlan-Bench2?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/qiulu66/EgoPlan-Bench2) |

### 6.5 Coordination-Space Evaluation

Classical multi-agent RL suites and newer language-agent collaboration benchmarks that test whether communication reduces joint uncertainty rather than producing superficial agreement:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2019-02 | **SMAC** | Tests whether decentralised agents reduce joint uncertainty through tactical coordination rather than relying on a single dominant agent | [The StarCraft Multi-Agent Challenge](https://arxiv.org/abs/1902.04043) | [![GitHub Stars](https://img.shields.io/github/stars/oxwhirl/smac?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/oxwhirl/smac) |
| 2019-02 | **Hanabi** | Measures belief sharing and disagreement resolution among agents reasoning under hidden-information constraints central to collective exploration | [The Hanabi Challenge: A New Frontier for AI Research](https://arxiv.org/abs/1902.00506) | [![GitHub Stars](https://img.shields.io/github/stars/google-deepmind/hanabi-learning-environment?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/google-deepmind/hanabi-learning-environment) |
| 2019-10 | **Overcooked** | Evaluates whether tight human-AI coupling produces genuine information transfer or merely stable role labels masking brittle epistemic division | [On the Utility of Learning about Humans for Human-AI Coordination](https://arxiv.org/abs/1910.05789) | [![GitHub Stars](https://img.shields.io/github/stars/HumanCompatibleAI/overcooked_ai?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/HumanCompatibleAI/overcooked_ai) |
| 2025-03 | **MultiAgentBench** | Benchmarks LLM agents on collaboration and competition tasks, exposing free-riding and duplicated effort that obscure true collective information gain | [MultiAgentBench: Evaluating the Collaboration and Competition of LLM Agents](https://arxiv.org/abs/2503.01935) | [![GitHub Stars](https://img.shields.io/github/stars/ulab-uiuc/MARBLE?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ulab-uiuc/MARBLE) |
| 2023-10 | **Sotopia** | Assesses whether social interaction and norm-sensitive role behaviour measurably reduce joint uncertainty rather than producing superficial verbal agreement | [SOTOPIA: Interactive Evaluation for Social Intelligence in Language Agents](https://arxiv.org/abs/2310.11667) | [![GitHub Stars](https://img.shields.io/github/stars/sotopia-lab/sotopia?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/sotopia-lab/sotopia) |
| 2024-11 | **Magentic-One** | Probes multi-agent orchestration to determine whether task decomposition improves search coverage or consolidates epistemic work in a single orchestrator | [Magentic-One: A Generalist Multi-Agent System for Solving Complex Tasks](https://arxiv.org/abs/2411.04468) | [![GitHub Stars](https://img.shields.io/github/stars/microsoft/autogen?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/microsoft/autogen) |
| 2025-02 | **MLGym** | Evaluates research-agent collaboration on decomposition quality and information sharing across long horizons, testing whether specialisation reduces redundancy | [MLGym: A New Framework and Benchmark for Advancing AI Research Agents](https://arxiv.org/abs/2502.14499) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/MLGym?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/MLGym) |
| 2026-02 | **AIRS-Bench** | Measures frontier research agents on long-horizon coordination tasks, revealing whether role diversity is preserved or collapses into premature consensus | [AIRS-Bench: A Suite of Tasks for Frontier AI Research Science Agents](https://arxiv.org/abs/2602.06855) | [![GitHub Stars](https://img.shields.io/github/stars/facebookresearch/airs-bench?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/facebookresearch/airs-bench) |

### Biological Exploration Parallels
- **Sensory-motor embodiment** → Lévy flights, whisking, saccades
- **Intrinsic curiosity** → Dopaminergic information prediction errors
- **Meta-control** → Locus coeruleus-norepinephrine regulation
- **Cognitive simulation** → Hippocampal preplay sequences
- **Social exploration** → Swarm intelligence, Theory of Mind

### Open Challenges
- Open-domain scalable exploration for reasoning beyond verifiable tasks
- Safe exploration with predictive world action models
- Causal and counterfactual reasoning in imagination space
- Dynamic temporal abstraction for long-horizon planning
- Epistemic uncertainty quantification in imagination
- Scalable coordination-space exploration without combinatorial explosion



> Finally, just for searchability, a supplementary paper-title index is also available: [titles.md](./titles.md).



---
<br>


<div align=center><img src="./fig/logobeihang.png" width="60%">
</div> 



<p align="center">
  <i>This repository is actively maintained. If you find any errors or have new papers to suggest, please open an issue or submit a pull request!</i>
</p>


