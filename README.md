
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

> 🔥 This is a curated paper list for the survey **"Agent Exploration Toward Artificial General Intelligence"**, covering exploration mechanisms across reasoning, embodied AI, world models, and multi-agent systems.

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




## 1. Overview

It is not enough for AI systems to learn only what they are expected to learn. To move toward AGI, agents must also know what they do not know—and actively explore to acquire new information, capabilities, and experiences.  

We present a unified framework for exploration, named "Epistemic Exploration", connect it to insights from natural intelligence, reinforcement learning, and modern AI agents, and discuss how exploration may serve as a key mechanism driving the progression toward AGI. 

### 1.1 What is Epistemic Exploration?

> **Epistemic exploration** is the agent's capacity to actively acquire information that reduces its uncertainty about the world, convert that reduction into durable policy improvement, and keep future acquisition possible.

Unlike undirected exploration (e.g., ε-greedy), epistemic exploration is *intentional*, *belief-driven*, and *multi-scale*: the agent reasons about which actions are most informative and plans multi-step information-gathering strategies across reasoning trajectories, tool-use policies, embodied sensorimotor loops, world-model rollouts, and multi-agent coordination protocols.



## 📑 Table of Contents

- [📣 Notices](#-notices)
- [Citation](#citation)
- [1. Overview](#1-overview)
  - [1.1 What is Epistemic Exploration?](#11-what-is-epistemic-exploration)
- [📑 Table of Contents](#-table-of-contents)
  - [1.2 Three Criteria](#12-three-criteria)
  - [1.3 Unified Epistemic Exploration Objective](#13-unified-epistemic-exploration-objective)
  - [1.4 Five-Level Trajectory Toward AGI](#14-five-level-trajectory-toward-agi)
  - [1.5 3×5 Taxonomy](#15-35-taxonomy)
- [2. Levels 1–2: Responder → Reasoner — Reasoning-Space Exploration](#2-levels-12-responder--reasoner--reasoning-space-exploration)
  - [2.1 Token-Level Exploration: Local Branching via High-Entropy Tokens](#21-token-level-exploration-local-branching-via-high-entropy-tokens)
  - [2.2 Trajectory-Level Exploration: Diverse Solution Rollouts](#22-trajectory-level-exploration-diverse-solution-rollouts)
  - [2.3 Latent-Space Exploration: Searching Before Tokenization](#23-latent-space-exploration-searching-before-tokenization)
- [3. Level 3: Agent — Perception- \& Action-Space Exploration](#3-level-3-agent--perception---action-space-exploration)
  - [3.1 Digital Agents](#31-digital-agents)
    - [3.1.1 Uncertainty-Driven Exploration](#311-uncertainty-driven-exploration)
    - [3.1.2 Competence-Driven Exploration](#312-competence-driven-exploration)
    - [3.1.3 Reachability-Driven Exploration](#313-reachability-driven-exploration)
  - [3.2 Embodied Agents](#32-embodied-agents)
    - [3.2.1 Perceptual & Semantic-Spatial Spaces](#321-perceptual--semantic-spatial-spaces)
    - [3.2.2 Action & Skill Spaces](#322-action--skill-spaces)
    - [3.2.3 Safety & Reachable Spaces](#323-safety--reachable-spaces)
- [4. Level 4: Prospector -- Imagination-Space Exploration](#4-level-4-prospector----imagination-space-exploration)
  - [4.1 Imagined Space: Active \& Optimistic Planning](#41-imagined-space-active--optimistic-planning)
  - [4.2 Risk Frontier: Safety-Critical Boundary Exploration](#42-risk-frontier-safety-critical-boundary-exploration)
  - [4.3 Value Landscape: Intrinsic Motivation \& Semantic Exploration](#43-value-landscape-intrinsic-motivation--semantic-exploration)
  - [4.4 Latent Manifold: Structured \& Self-Supervised Exploration](#44-latent-manifold-structured--self-supervised-exploration)
  - [Infrastructure Papers (6 papers, discussed in body text)](#infrastructure-papers-6-papers-discussed-in-body-text)
- [5. Level 5: Ecosystem — Coordination-Space Exploration](#5-level-5-ecosystem--coordination-space-exploration)
  - [5.1 Behavior Pattern Exploration](#51-behavior-pattern-exploration)
  - [5.2 Role Dynamics Exploration](#52-role-dynamics-exploration)
  - [5.3 Organization Topology Exploration](#53-organization-topology-exploration)
- [6. Exploration Evaluation](#6-exploration-evaluation)
  - [6.1 Principles \& Infrastructure](#61-principles--infrastructure)
  - [6.2 Reasoning-Space Evaluation](#62-reasoning-space-evaluation)
  - [6.3 Interaction-Space Evaluation](#63-interaction-space-evaluation)
    - [6.3.1 Digital Agents](#631-digital-agents)
    - [6.3.2 Embodied Agents](#632-embodied-agents)
  - [6.4 Imagination-Space Evaluation](#64-imagination-space-evaluation)
  - [6.5 Coordination-Space Evaluation](#65-coordination-space-evaluation)
  - [Biological Exploration Parallels](#biological-exploration-parallels)
  - [Open Challenges](#open-challenges)

---
<br>




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

<p align="center"><img src="fig/level1_2_image.png" width="850"/></p>
<p align="center"><i>Figure: Levels 1–2 Reasoning-Space Exploration — Why (entropy escalation & reward stagnation), Where (tokens → turns → latent trajectories), and How (uncertainty / competence / reachability-driven).</i></p>

<br>

### 2.1 Token-Level Exploration: Local Branching via High-Entropy Tokens

Token-level exploration focuses on local uncertain decision points in the next-token distribution, since a few decisive tokens can redirect the subsequent proof, program, or explanation. Existing methods identify high-entropy tokens as reasoning forks and branch from these positions.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-06 | **TreeRL** | Explores reasoning via on-policy tree search from uncertain intermediate states | [TreeRL: LLM Reinforcement Learning with On-Policy Tree Search](https://arxiv.org/abs/2506.11902) | [![GitHub Stars](https://img.shields.io/github/stars/THUDM/TreeRL?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/THUDM/TreeRL) |
| 2025-06 | **Beyond-80/20** | Identifies high-entropy tokens as key reasoning forks | [Beyond the 80/20 Rule: High-Entropy Minority Tokens Drive Effective Reinforcement Learning for LLM Reasoning](https://arxiv.org/abs/2506.01939) | [![GitHub Stars](https://img.shields.io/github/stars/Shenzhi-Wang/Beyond-the-80-20-Rule-RLVR?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Shenzhi-Wang/Beyond-the-80-20-Rule-RLVR) |
| 2025-10 | **AEPO** | Breaks the exploration bottleneck by directly controlling policy entropy through temperature-guided REINFORCE | [Arbitrary Entropy Policy Optimization Breaks The Exploration Bottleneck of Reinforcement Learning](https://arxiv.org/pdf/2510.08141) | [![GitHub Stars](https://img.shields.io/github/stars/597358816/AEPO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/597358816/AEPO) |
<br>

### 2.2 Trajectory-Level Exploration: Diverse Solution Rollouts

Trajectory-level exploration treats the complete chain-of-thought or solution rollout as the basic unit of search and reward, making it especially suitable for verifiable-reward training. 

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-10 | **LATR** | Improves RLVR by explicitly enforcing trajectory-level diversity during group rollouts | [Lookahead Tree-Based Rollouts for Enhanced Trajectory-Level Exploration in Reinforcement Learning with Verifiable Rewards](https://arxiv.org/abs/2510.24302) | [![GitHub Stars](https://img.shields.io/github/stars/starreeze/latr&logo=github&label=GitHub&color=black)](https://github.com/starreeze/latr) |
| 2025-10 | **UCAS** | Promotes exploration by boosting uncertain-but-correct reasoning paths | [Unlocking Exploration in RLVR: Uncertainty-aware Advantage Shaping for Deeper Reasoning](https://arxiv.org/abs/2510.10649) | [![GitHub Stars](https://img.shields.io/github/stars/xvolcano02/UCAS&logo=github&label=GitHub&color=black)](https://github.com/xvolcano02/UCAS) |
| 2025-11 | **ICPO** | Promotes exploration by combining verifiable rewards with confidence-based preference advantages | [ICPO: Intrinsic Confidence-Driven Group Relative Preference Optimization for Efficient Reinforcement Learning](https://arxiv.org/abs/2511.21005) | - |
| 2025-06 | **E2H** | Guides exploration through an easy-to-hard curriculum | [Curriculum Reinforcement Learning from Easy to Hard Tasks Improves LLM Reasoning](https://arxiv.org/abs/2506.06632) | [![GitHub Stars](https://img.shields.io/github/stars/divelab/E2H-Reasoning?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/divelab/E2H-Reasoning) |
| 2026-01 | **HA-DW** | Reduces exploration imbalance by debiasing group-relative advantages across prompt difficulty | [Your Group-Relative Advantage Is Biased](https://arxiv.org/abs/2601.08521) | - |
| 2025-08 | **SvS** | Sustains exploration by self-synthesizing diverse but answer-equivalent problems during RLVR | [Beyond Pass@1: Self-play with Variational Problem Synthesis Sustains RLVR](https://arxiv.org/pdf/2508.14029) | [![GitHub Stars](https://img.shields.io/github/stars/MasterVito/SvS?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/MasterVito/SvS) |
| 2026-01 | **RLVRR** | Turns sparse end rewards into a verifiable reward chain that supports broader open-ended exploration | [From Verifiable Dot to Reward Chain: Harnessing Verifiable Reference-based Rewards for Reinforcement Learning of Open-ended Generation](https://arxiv.org/abs/2601.18533) | [![GitHub Stars](https://img.shields.io/github/stars/YJiangcm/RLVRR?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/YJiangcm/RLVRR) |

<br>

### 2.3 Latent-Space Exploration: Searching Before Tokenization

Latent-space exploration searches over hidden states or compact latent actions before committing to natural-language tokens, allowing the model to represent multiple possible continuations internally.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-12 | **ReLaX** | Promotes exploration by regulating latent hidden-state dynamics beyond token-level entropy | [ReLaX: Reasoning with Latent Exploration for Large Reasoning Models](https://arxiv.org/abs/2512.07558) | [![GitHub Stars](https://img.shields.io/github/stars/ZhangShimin1/ReLaX?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ZhangShimin1/ReLaX) |

---

<br>





## 3. Level 3: Agent — Perception- & Action-Space Exploration

At Level 3, the agent crosses a qualitative boundary: it moves from purely internal reasoning into situated interaction with external environments. The "Reasoner" of Levels 1–2 generates hypotheses within its own token space; the "Agent" must act on those hypotheses—querying databases, invoking APIs, reorienting sensors, or manipulating physical objects—and update its beliefs from the consequences. Exploration can no longer be confined to branching over reasoning trajectories; it now unfolds in perception and action space, where every exploratory step incurs real cost (latency, API calls, energy, or irreversible physical change).

### 3.1 Digital Agents

Digital agents operate in software-mediated environments—web browsers, code interpreters, file systems, and tool APIs. Their action space is discrete and combinatorial (which tool to call, with what arguments, in what order), feedback is fast but often sparse, and the primary exploration challenge is discovering effective tool-invocation policies across a vast combinatorial manifold.

#### 3.1.1 Uncertainty-Driven Exploration

Beyond maintaining diversity, a digital agent must actively seek information to resolve the epistemic uncertainty that arises when static pre-trained priors prove insufficient in "environmentally-open" scenarios. Uncertainty-priority exploration leverages uncertainty signals to prioritize informative interactions and mitigate overconfident failures under partial observability. Methods typically fall into explicit uncertainty estimation (using UCB or count-based bonuses) and implicit self-perceived uncertainty (triggering reflection or knowledge seeking at capability boundaries):

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

To master the vast and high-dimensional action space inherent in agentic interaction, systems must transcend naive trial-and-error. Strategic exploration prunes the action manifold and prioritizes high-utility trajectories through curricula (staged complexity), prior-based credit assignment (objective-aligned process signals), and self-play (autonomously generating targeted action distributions):

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

A digital agent's policy can rapidly collapse onto a narrow set of favoured tool-invocation patterns, foreclosing alternative interaction strategies before they can be evaluated. Reachability-driven methods explicitly optimise for sustained trajectory diversity through entropy control (regulating policy entropy) and external experience injection (exposing the agent to useful off-policy behaviours):

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-08 | **EGPO** | Adds entropy bonuses to encourage exploration in function-call reasoning | [Reasoning through Exploration: A Reinforcement Learning Framework for Robust Function Calling](https://arxiv.org/abs/2508.05118) | [![GitHub Stars](https://img.shields.io/github/stars/BingguangHao/RLFC?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/BingguangHao/RLFC) |
| 2025-09 | **EPO** | Regularizes entropy to sustain exploration in multi-turn agent RL | [EPO: Entropy-regularized Policy Optimization for LLM Agents Reinforcement Learning](https://arxiv.org/abs/2509.22576) | [![GitHub Stars](https://img.shields.io/github/stars/WujiangXu/EPO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/WujiangXu/EPO) |
| 2025-09 | **ENTROPO** | Uses entropy-enhanced preferences to diversify coding-agent exploration | [Building Coding Agents via Entropy-Enhanced Multi-Turn Preference Optimization](https://arxiv.org/abs/2509.12434) | - |
| 2026-03 | **RAPO** | Expands policy exploration with retrieval-augmented experience | [RAPO: Expanding Exploration for LLM Agents via Retrieval-Augmented Policy Optimization](https://arxiv.org/abs/2603.03078) | - |
| 2026-04 | **E³-TIR** | Branches from high-entropy prefixes to exploit exploratory experience | [E3-TIR: Enhanced Experience Exploitation for Tool-Integrated Reasoning](https://arxiv.org/abs/2604.09455) | [![GitHub Stars](https://img.shields.io/github/stars/yuki-younai/E3-TIR?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/yuki-younai/E3-TIR) |

<br>

### 3.2 Embodied Agents

<p align="center"><img src="fig/Level3Embodied.png" width="850"/></p>
<p align="center"><i>Figure: Level 3 Embodied Agent Exploration — Exploration distributed across perceptual/semantic-spatial spaces, action/skill spaces, and safety spaces.</i></p>

Embodied agents—robotic manipulators, autonomous vehicles, navigation systems—explore in a continuous, high-dimensional action space defined by physical effectors and multimodal sensors. The cost of exploration is fundamentally different from the digital setting: every physical interaction consumes time, energy, and mechanical wear. To systematically navigate these constraints, embodied exploration operates across three distinct spaces:

#### 3.2.1 Perceptual & Semantic-Spatial Spaces

Before an agent can execute complex plans, it must actively control its sensors and navigate the environment to eliminate cognitive blind spots and reach task-relevant states. Exploration here focuses on reconstructing geometry, resolving semantic ambiguity, and pruning the spatial search manifold.

| Date | Method | Space / Focus | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-10 | **Active Semantic Perception** | **Semantic Inference:** Entropy-driven exploration over LLM-sampled scene graph hypotheses | [Active Semantic Perception](https://arxiv.org/abs/2510.05430) | [![GitHub Stars](https://img.shields.io/github/stars/grasp-lyrl/active_semantic_perception?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/grasp-lyrl/active_semantic_perception) |
| 2024-10 | **Fisher-Info Planning** | **Navigation:** MLLM-guided exploration balancing information gain vs. localisation risk | [Multimodal LLM Guided Exploration and Active Mapping using Fisher Information](https://arxiv.org/abs/2410.17422) | [![GitHub Stars](https://img.shields.io/github/stars/JiangWenPL/multimodal-active?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/JiangWenPL/multimodal-active) |
| 2024-10 | **ActiveSplat** | **Reconstruction:** Gaussian-splat viewpoint exploration maximises reconstruction fidelity | [ActiveSplat: High-Fidelity Scene Reconstruction through Active Gaussian Splatting](https://arxiv.org/abs/2410.21955) | [![GitHub Stars](https://img.shields.io/github/stars/Li-Yuetao/ActiveSplat?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Li-Yuetao/ActiveSplat) |
| 2024-04 | **ActiveRIR** | **Multi-modal Inference:** Cross-modal audio-visual exploration for acoustic scene mapping | [ActiveRIR: Active Audio-Visual Exploration for Building Room Impulse Responses](https://arxiv.org/abs/2404.16216) | - |
| 2023-11 | **Conan** | **Semantic Inference:** Active exploration as Bayesian query to disambiguate latent scene state | [Active Reasoning in an Open-World Environment](https://arxiv.org/abs/2311.02018) | [![GitHub Stars](https://img.shields.io/github/stars/ariesssxu/Conan-Active-Reasoning?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/ariesssxu/Conan-Active-Reasoning) |
| 2023-10 | **LFG** | **Navigation:** LLM semantic-priors prune frontier exploration toward goal-relevant regions | [Language Frontier Guide: LLM-Based Semantic Priors for Exploration](https://arxiv.org/abs/2310.10103) | [![GitHub Stars](https://img.shields.io/github/stars/Michael-Equi/lfg-nav?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/Michael-Equi/lfg-nav) |

#### 3.2.2 Action & Skill Spaces

Competence-driven exploration targets the fine-grained manipulation manifold, pushing beyond pre-trained priors. Recent advances shift from pure offline imitation to online policy exploration (RL-VLA) and inference-time deliberation (Test-Time Compute).

**Online RL and VLA Policy Exploration.** Safely expanding manipulation boundaries via PPO/GRPO and hybrid offline-to-online fine-tuning.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2026-04 | **π₀.₇** | Steerable flow VLA trained with diverse multimodal context for out-of-the-box generalist skills | [π₀.₇: a Steerable Generalist Robotic Foundation Model with Emergent Capabilities](https://arxiv.org/abs/2604.15483) | - |
| 2026-02 | **GigaBrain-0.5M** | Foundation VLA learned directly from world-model-based RL at fleet scale | [GigaBrain-0.5M*: A VLA That Learns From World Model-Based RL](https://arxiv.org/abs/2602.12099) | - |
| 2026-01 | **SOP** | Scalable online post-training infrastructure for fleet-scale VLA exploration | [SOP: Scalable Online Post-training for Generalist VLA Models](https://arxiv.org/abs/2601.03044) | - |
| 2025-11 | **WMPO** | Pure world-model PPO enables safe online action-space exploration for VLA | [WMPO: World Model-Based Policy Optimization for VLA](https://arxiv.org/abs/2511.09515) | - |
| 2025-11 | **π*₀.₆** | Flow-matching VLA that learns from online experience via offline RL | [π*₀.₆: A VLA That Learns From Experience](https://arxiv.org/abs/2511.14759) | - |
| 2025-11 | **SRPO** | Self-refined exploration bridging static data and online rollouts | [SRPO: Self-Refined Policy Optimization for VLA](https://arxiv.org/abs/2511.15605) | [![GitHub Stars](https://img.shields.io/github/stars/SUSTechBruce/SRPO_MLLMs?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/SUSTechBruce/SRPO_MLLMs) |
| 2025-10 | **π_RL** | First online PPO/GRPO RL fine-tuning for flow-matching VLA | [πRL: Online RL Fine-Tuning for Flow-Based Vision-Language-Action Models](https://arxiv.org/abs/2510.25889) | - |
| 2025-09 | **Dual-Actor FT** | Dual-actor decoupling of exploration vs. exploitation for stable offline-to-online RL | [Dual-Actor Fine-Tuning of VLA Models](https://arxiv.org/abs/2509.13774) | - |
| 2025-09 | **SimpleVLA-RL** | GRPO group-relative exploration scales VLA skill acquisition | [SimpleVLA-RL: Scaling VLA Training via Reinforcement Learning](https://arxiv.org/abs/2509.09674) | [![GitHub Stars](https://img.shields.io/github/stars/PRIME-RL/SimpleVLA-RL?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/PRIME-RL/SimpleVLA-RL) |
| 2025-05 | **VLA-RL** | Scalable PPO-based online action-space exploration for VLA policies | [VLA-RL: Towards Masterful and General Robotic Manipulation with Scalable RL](https://arxiv.org/abs/2505.18719) | [![GitHub Stars](https://img.shields.io/github/stars/GuanxingLu/vlarl?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/GuanxingLu/vlarl) |
| 2025-02 | **ConRFT** | Consistency-regularised offline-to-online exploration for diffusion VLA | [ConRFT: A Reinforced Fine-tuning Method for VLA Models via Consistency Policy](https://arxiv.org/abs/2502.05450) | [![GitHub Stars](https://img.shields.io/github/stars/cccedric/conrft?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/cccedric/conrft) |
| 2024-11 | **GRAPE** | Preference-aligned exploration generalises VLA policies to novel scenarios | [GRAPE: Generalizing Robot Policy via Preference Alignment](https://arxiv.org/abs/2411.19309) | - |
| 2024-10 | **HIL-SERL** | Sample-efficient on-robot RL with human-in-the-loop interventions for dexterous tasks | [Precise and Dexterous Robotic Manipulation via Human-in-the-Loop RL](https://arxiv.org/abs/2410.21845) | [![GitHub Stars](https://img.shields.io/github/stars/rail-berkeley/hil-serl?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/rail-berkeley/hil-serl) |

**Test-Time Compute & Cognitive Search.** Moving the exploration burden from training to deployment via inference-time deliberation.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2026-02 | **Recurrent-Depth VLA** | Implicit test-time compute scaling via latent iterative reasoning (no explicit tokens) | [Recurrent-Depth VLA: Implicit Test-Time Compute Scaling of VLA via Latent Iterative Reasoning](https://arxiv.org/abs/2602.07845) | - |
| 2026-01 | **TT-VLA** | Value-free on-the-fly test-time RL adapts VLA policies per-episode | [Test-Time VLA: On-the-Fly Adaptation for Embodied Policies](https://arxiv.org/abs/2601.06748) | - |
| 2025-12 | **TACO** | Anti-exploration test-time steering via continuous normalising flows | [TACO: Steering VLA Models at Test-Time via Anti-Exploration](https://arxiv.org/abs/2512.02834) | [![GitHub Stars](https://img.shields.io/github/stars/breez3young/TACO?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/breez3young/TACO) |
| 2025-11 | **DeepThinkVLA** | Slow-thinking test-time exploration through deliberate chain-of-action reasoning | [DeepThink-VLA: From Language Reasoning to Action Reasoning](https://arxiv.org/abs/2511.15669) | [![GitHub Stars](https://img.shields.io/github/stars/OpenBMB/DeepThinkVLA?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/OpenBMB/DeepThinkVLA) |
| 2025-09 | **VLA-Reasoner** | MCTS imagination-time exploration over autoregressive action trajectories | [VLA-Reasoner: Empowering VLA Models via Test-Time Monte Carlo Tree Search](https://arxiv.org/abs/2509.22643) | - |
| 2025-08 | **MB-Search VLA** | Model-based MCTS over AR / Diffusion VLA imagines trajectories before acting | [Improving Pre-Trained VLA Policies with Model-Based Search](https://arxiv.org/abs/2508.12211) | - |
| 2025-05 | **Hume** | System-2 deliberative exploration via continuous flow value guidance | [Hume: Introducing System-2 Thinking in Visual-Language-Action Model](https://arxiv.org/abs/2505.21432) | [![GitHub Stars](https://img.shields.io/github/stars/hume-vla/hume?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/hume-vla/hume) |
| 2024-10 | **V-GPS** | Offline value guidance steers generalist AR / diffusion VLA decoding at test time | [Steering Your Generalists: Improving Robotic Foundation Models via Value Guidance](https://arxiv.org/abs/2410.13816) | - |

#### 3.2.3 Safety & Reachable Spaces

To prevent irreversible physical damage while preserving the ability to learn, embodied agents must explore within constrained, dynamically shaped boundaries driven by synthesized rewards and hard safety shields.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025-05 | **TeViR** | **Reward:** Text-to-video diffusion rewards enable efficient sparse-task exploration | [TeViR: Text-to-Video Reward with Diffusion Models for Efficient RL](https://arxiv.org/abs/2505.19769) | - |
| 2025-03 | **SafeVLA** | **Safety:** Constrained policy exploration under hard safety guarantees for VLA | [SafeVLA: Towards Safety Alignment of VLA Model via Constrained Learning](https://arxiv.org/abs/2503.03480) | [![GitHub Stars](https://img.shields.io/github/stars/PKU-Alignment/SafeVLA?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/PKU-Alignment/SafeVLA) |
| 2024-09 | **CurricuLLM** | **Reward:** LLM-designed curricula for progressive exploration of hard manipulation skills | [CurricuLLM: Automatic Task Curricula Design for Learning Complex Robot Skills using LLMs](https://arxiv.org/abs/2409.18382) | [![GitHub Stars](https://img.shields.io/github/stars/labicon/CurricuLLM?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/labicon/CurricuLLM) |
| 2024-04 | **RECOVER** | **Safety:** Neuro-symbolic failure detection bounds exploratory trajectories in manipulation | [RECOVER: Neuro-Symbolic Failure Recovery for Robotic Manipulation](https://arxiv.org/abs/2404.00756) | - |
| 2023-10 | **Eureka** | **Reward:** LLM-synthesised executable reward code evolves the explorable task manifold | [Eureka: Human-Level Reward Design via Coding Large Language Models](https://arxiv.org/abs/2310.12931) | [![GitHub Stars](https://img.shields.io/github/stars/eureka-research/eureka?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/eureka-research/eureka) |

---

<br>

## 4. Level 4: Prospector -- Imagination-Space Exploration

At Levels 1--3, exploration operates within spaces the agent directly inhabits. Level 4 introduces a qualitatively different regime: exploration within **learned world models**---internal simulators that approximate environment dynamics and enable imagination-driven planning. This shift transforms exploration from costly physical trial-and-error to efficient mental simulation, where agents evaluate counterfactual futures and discover strategies without real-world consequences.

The world model serves as a cognitive sandbox where the agent navigates latent manifolds, generates simulated rollouts, and probes epistemic boundaries. This dual exploration regime introduces unique challenges: prediction errors compound over imagined horizons, uncertainty must be disentangled from irreducible noise, and safety-critical details risk being lost in latent compression. The exploration objective shifts from ``which action to take'' to ``which latent configurations are worth visiting, which imagined trajectories are physically plausible, and how can intrinsic signals guide exploration when external feedback is absent.''

<p align="center"><img src="fig/level4_worldmodel.png" width="850"/></p>
<p align="center"><i>Figure: Level 4 Imagination-Space Exploration -- Why (dual exploration problem: reality drift, noise hijacking, detail loss), Where (imagined space, risk frontier, value landscape, latent manifold), and How (model-based RL, video generation, autonomous driving, social dynamics).</i></p>

<br>

### 4.1 Imagined Space: Active & Optimistic Planning

Imagined-space exploration operates within the internal simulation of the world model, where agents generate trajectories thousands of times faster than physical experiments. Methods here focus on planning to explore---maximizing expected novelty in imagined states through ensemble disagreement, optimistic dynamics, or state archiving.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2019-06 | **MAX** | Maximizes Bayesian novelty via forward-model ensembles to plan observation of novel events | [Model-Based Active Exploration](https://arxiv.org/abs/1810.12162) | - |
| 2020-05 | **Plan2Explore** | First ``plan to explore'' method: decouples exploration from task reward via latent ensemble disagreement in imagined space | [Planning to Explore via Self-Supervised World Models](https://arxiv.org/abs/2005.05960) | - |
| 2021-02 | **Go-Explore** | ``Return-then-explore'' paradigm with explicit state archive and goal-conditioned return policies | [First return, then explore](https://doi.org/10.1038/s41586-020-03157-9) | - |
| 2026-02 | **Optimistic WM** | RBMLE-based optimism directly into world model learning; gradient-based optimistic dynamics without ensemble estimation | [Optimistic World Models](https://arxiv.org/abs/2602.10044) | - |

<br>

### 4.2 Risk Frontier: Safety-Critical Boundary Exploration

Risk-frontier exploration requires probing operational boundaries to identify failure modes. In safety-critical domains, agents must deliberately seek out regions of high epistemic uncertainty at the edge of their competence, resolving model uncertainty through risk-seeking trajectory optimization.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2019-04 | **Curious iLQR** | Bayesian dynamics + risk-seeking iLQR to resolve model uncertainty at operational boundaries | [Curious iLQR: Resolving Uncertainty in Model-based RL](https://arxiv.org/abs/1904.06786) | - |

<br>

### 4.3 Value Landscape: Intrinsic Motivation & Semantic Exploration

Value-landscape exploration constructs internal value surfaces through intrinsic motivation when dense external rewards are absent. Methods here span from classical prediction-error curiosity to foundation-model-guided semantic exploration, covering the full spectrum of self-generated reward signals.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 1991 | **Schmidhuber** | Foundational theory: curiosity as intrinsic reward proportional to world-model learning progress | [A Possibility for Implementing Curiosity and Boredom](https://direct.mit.edu/books/edited-volume/3865/chapter/162771/A-Possibility-for-Implementing-Curiosity-and) | - |
| 2016 | **VIME** | Variational information maximization: Bayesian neural network provides information-gain intrinsic rewards | [VIME: Variational Information Maximizing Exploration](https://arxiv.org/abs/1605.09674) | [![GitHub Stars](https://img.shields.io/github/stars/matthewlujp/VIME?style=flat&logo=github&label=GitHub&color=black)](https://github.com/matthewlujp/VIME) |
| 2021 | **SelMo** | Pure curiosity optimization within world model generates diverse manipulation and locomotion behaviors | [Is Curiosity All You Need?](https://deepmind.google/discover/blog/is-curiosity-all-you-need-on-the-utility-of-emergent-behaviours-from-curious-exploration/) | - |
| 2023 | **Hindsight Curiosity** | Retrospective curiosity: asks ``should I have predicted this?'' to avoid noise-hijacking in stochastic environments | [Curiosity in Hindsight](https://arxiv.org/abs/2211.10515) | - |
| 2025 | **Mantiuk** | Curiosity and competence co-evolve with world model learning in a feedback loop | [From Curiosity to Competence](https://arxiv.org/abs/2507.08210) | - |
| 2025 | **SENSEI** | Foundation models guide semantic exploration toward meaningful behaviors | [SENSEI: Semantic Exploration Guided by Foundation Models](https://arxiv.org/abs/2503.01584) | - |

<br>

### 4.4 Latent Manifold: Structured & Self-Supervised Exploration

Latent-manifold exploration operates on the compressed representation spaces learned by world models, where semantically similar states cluster. Methods here inject structure (object-centric, relational, geometric) into exploration or achieve exploration purely through self-supervised predictive learning.

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2020 | **LWM** | Self-supervised temporal representations for novelty detection in hard-exploration Atari games | [Latent World Models for Intrinsically Motivated Exploration](https://proceedings.neurips.cc/paper/2020/hash/3c09bb10e2189124fdd8f467cc8b55a7-Abstract.html) | - |
| 2023 | **Sergeant-Perthuis** | Geometry of WM (Euclidean vs.~projective) fundamentally impacts epistemic value and curiosity | [Influence of the Geometry of the World Model on Curiosity Based Exploration](https://arxiv.org/abs/2304.00188) | - |
| 2022 | **Sancaktar** | Relational inductive biases for compositional multi-object exploration with structured world models | [Curious Exploration via Structured World Models](https://arxiv.org/abs/2206.11403) | - |
| 2025 | **GX-Chen** | Object-centric abstraction with discriminative WM for efficient count-based exploration planning | [Efficient Exploration with Object-Centric Abstraction](https://arxiv.org/abs/2408.11816) | - |
| 2025 | **Santana** | Exploration policies learned entirely from self-supervised predictive WM training without external reward | [Learning To Explore With Predictive World Model](https://arxiv.org/abs/2502.13200) | - |
| 2026 | **One Life** | Infer symbolic programmatic world models from minimal unguided exploration in stochastic environments | [One Life to Learn](https://openreview.net/forum?id=UQ36IrVCw2) | [![GitHub Stars](https://img.shields.io/github/stars/codezakh/onelife?style=flat&logo=github&label=GitHub&color=black)](https://github.com/codezakh/onelife) |
| 2024 | **SeeX** | Separated world model extracts endogenous/exogenous info for robust exploration in visual distractor environments | [Leveraging Separated World Model for Exploration](https://proceedings.neurips.cc/paper_files/paper/2024/hash/96189e90e599ccc43f00434ff3ed0312-Abstract-Conference.html) | - |
| 2025 | **InDRiVE** | Ensemble-disagreement curiosity extended to autonomous driving via Dreamer-style world models | [InDRiVE: Intrinsic Disagreement-based Reinforcement for Vehicle Exploration](https://arxiv.org/abs/2503.05573) | - |

<br>

---

### Infrastructure Papers (6 papers, discussed in body text)

The following six papers provide the world model architecture and algorithmic foundation for the exploration methods above:

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2018 | **World Models** | V-M-C architecture: VAE compresses observations, RNN predicts latent dynamics, controller evolves in imagination | [Recurrent World Models Facilitate Policy Evolution](https://arxiv.org/abs/1809.01999) | [![GitHub Stars](https://img.shields.io/github/stars/danijar/dreamerv3?style=flat&logo=github&label=GitHub&color=black)](https://github.com/danijar/dreamerv3) |
| 2019 | **PlaNet** | RSSM for latent-space planning; decomposes latent states into deterministic and stochastic components | [Learning Latent Dynamics for Planning from Pixels](https://arxiv.org/abs/1811.04551) | - |
| 2020 | **Dreamer** | Actor-critic training within imagined latent space of RSSM world model | [Dream to Control](https://arxiv.org/abs/1912.01603) | - |
| 2023 | **DreamerV3** | Single WM algorithm masters diverse domains without hyperparameter tuning | [Mastering Diverse Domains through World Models](https://arxiv.org/abs/2301.04104) | [![GitHub Stars](https://img.shields.io/github/stars/danijar/dreamerv3?style=flat&logo=github&label=GitHub&color=black)](https://github.com/danijar/dreamerv3) |
| 2022 | **DayDreamer** | Dreamer transferred from simulation to physical robots | [DayDreamer: World Models for Physical Robot Learning](https://arxiv.org/abs/2206.14176) | [![GitHub Stars](https://img.shields.io/github/stars/danijar/daydreamer?style=flat&logo=github&label=GitHub&color=black)](https://github.com/danijar/daydreamer) |
| 2026 | **R2-Dreamer** | Eliminates decoders and augmentation; redundancy reduction improves exploration | [R2-Dreamer](https://arxiv.org/abs/2603.18202) | - |

<br>

**Summary Statistics:** 25 papers total (19 core exploration + 6 infrastructure), spanning 1991--2026. Methods are distributed across 4 exploration spaces (Imagined Space, Risk Frontier, Value Landscape, Latent Manifold) and 4 application domains (Model-Based RL, Video Generation, Autonomous Driving, Social Dynamics).

---

<br>



## 5. Level 5: Ecosystem — Coordination-Space Exploration

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



### 5.1 Behavior Pattern Exploration

This subsection cites works in multi-agent reinforcement learning on joint trajectory diversity, collaborative novelty, peer incentivization, and behavioral novelty. Corresponding in-text citations: [76, 78, 79, 80].

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025 | **TEM** | Trajectory entropy maximization for efficient multi-agent exploration, emphasizing trajectory-level diversity | [Toward Efficient Multi-Agent Exploration with Trajectory Entropy Maximization](https://arxiv.org/abs/2502.08365v1) | - |
| 2023 | **EMAX** | Uses multiple value functions to estimate where agents are still uncertain, then guides them to explore those unclear but potentially useful joint behaviors | [Ensemble Value Functions for Efficient Exploration in Multi-Agent Reinforcement Learning](https://arxiv.org/abs/2302.03439) | - |
| 2024 | **JIM** | Joint intrinsic motivation enabling coordinated exploration in multi-agent deep RL | [Joint Intrinsic Motivation for Coordinated Exploration in Multi-Agent Deep Reinforcement Learning](https://dl.acm.org/doi/10.5555/3677260.3677261) | - |
| 2025 | **PIMAEX** | Multi-agent exploration through peer incentivization, modeling inter-agent influence | [PIMAEX: Multi-Agent Exploration through Peer Incentivization](https://doi.org/10.5220/0013260000003890) | - |
| 2025 | **CERMIC** | Curiosity-driven exploration via multi-agent contextual calibration for behavioural novelty | [Wonder Wins Ways: Curiosity-Driven Exploration through Multi-Agent Contextual Calibration](https://arxiv.org/abs/2509.20648) | [![GitHub Stars](https://img.shields.io/github/stars/PyyWill/CERMIC?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/PyyWill/CERMIC) |
| 2025 | **CMAT** | Keeps a fixed multi-agent collaboration structure, then uses feedback to make each role better at doing its part in the team | [CMAT: A Multi-Agent Collaboration Tuning Framework for Enhancing Small Language Models](https://arxiv.org/abs/2404.01663) | - |
| 2025 | **W4S** | Lets a weak meta-agent learn how to organize stronger agents, so the system explores better workflows instead of relying on a hand-written pipeline | [Weak-for-Strong: Training Weak Meta-Agent to Harness Strong Executors](https://arxiv.org/abs/2504.04785) | - |

---

### 5.2 Role Dynamics Exploration

This subsection cites works on fixed-role collaboration, role competence enhancement, dynamic team construction, and weak-to-strong model cascading. Corresponding in-text citations: [89, 81, 86, 87].

| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025 | **Orchestrator** | Uses active inference to decide which agent should act next, helping the team adjust its roles and actions when the task is uncertain | [Orchestrator: Active Inference for Multi-Agent Systems in Long-Horizon Tasks](https://arxiv.org/abs/2509.05651) | - |
| 2024 | **AgentVerse** | Facilitates multi-agent collaboration and explores emergent behaviors via dynamic role adjustment and agent recruitment | [AgentVerse: Facilitating Multi-Agent Collaboration and Exploring Emergent Behaviors](https://openreview.net/forum?id=EHg5GDnyq1) | [![GitHub Stars](https://img.shields.io/github/stars/OpenBMB/AgentVerse?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/OpenBMB/AgentVerse) |
| 2025 | **CMAT** | Multi-agent collaboration tuning framework enhancing small language models through role competence and feedback-driven tuning | [CMAT: A Multi-Agent Collaboration Tuning Framework for Enhancing Small Language Models](https://arxiv.org/abs/2404.01663) | - |
| 2024 | **AgentVerse** | Lets the team change which agents participate and what roles they play, so collaboration can adapt when the current team structure is not enough | [AgentVerse: Facilitating Multi-Agent Collaboration and Exploring Emergent Behaviors](https://openreview.net/forum?id=EHg5GDnyq1) | [![GitHub Stars](https://img.shields.io/github/stars/OpenBMB/AgentVerse?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/OpenBMB/AgentVerse) |
| 2023 | **AutoMix** | Starts from cheaper or weaker models and calls stronger models only when needed, exploring when to stop or escalate during problem solving | [AutoMix: Automatically Mixing Language Models](https://arxiv.org/abs/2310.12963) | - |
| 2024 | **Cascade Routing** | Unified approach to routing and cascading for LLMs, enabling weak-to-strong model cascades with cost-quality trade-offs | [A Unified Approach to Routing and Cascading for LLMs](https://arxiv.org/abs/2410.10347) | [![GitHub Stars](https://img.shields.io/github/stars/eth-sri/cascade-routing?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/eth-sri/cascade-routing) |
| 2023 | **CAMEL** | Communicative agents for "mind" exploration of large language model society via role-playing | [CAMEL: Communicative Agents for "Mind" Exploration of Large Language Model Society](https://arxiv.org/abs/2303.17760) | [![GitHub Stars](https://img.shields.io/github/stars/camel-ai/camel?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/camel-ai/camel) |
| 2024 | **MetaGPT** | Uses software-company-style roles such as product manager, architect, engineer, and reviewer to make collaboration more structured and stable | [MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework](https://arxiv.org/abs/2308.00352) | [![GitHub Stars](https://img.shields.io/github/stars/FoundationAgents/MetaGPT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/FoundationAgents/MetaGPT) |




### 5.3 Organization Topology Exploration

This subsection cites the work discussing how multi-agent collaboration structures evolve from fixed workflows into learnable, evolvable organizational processes. Corresponding in-text citation: [90].


| Date | Method | Key Idea | Paper | Github |
|:---:|:-------:|:---------|:------|:---:|
| 2025 | **Orchestrator** | Adjusts the interaction structure during a task by deciding when to continue, replan, backtrack, or call another agent | [Orchestrator: Active Inference for Multi-Agent Systems in Long-Horizon Tasks](https://arxiv.org/abs/2509.05651) | - |
| 2025 | **CMAT** | Learns better collaboration patterns among agents through feedback, instead of relying only on a manually fixed team structure | [CMAT: A Multi-Agent Collaboration Tuning Framework for Enhancing Small Language Models](https://arxiv.org/abs/2404.01663) | - |
| 2025 | **W4S** | Optimizes the overall workflow by learning which stronger agents to use and in what order | [Weak-for-Strong: Training Weak Meta-Agent to Harness Strong Executors](https://arxiv.org/abs/2504.04785) | - |
| 2024 | **MetaGPT** | Defines a structured collaboration graph through fixed roles, ordered procedures, and shared documents | [MetaGPT: Meta Programming for A Multi-Agent Collaborative Framework](https://arxiv.org/abs/2308.00352) | [![GitHub Stars](https://img.shields.io/github/stars/FoundationAgents/MetaGPT?style=for-the-badge&logo=github&label=GitHub&color=black)](https://github.com/FoundationAgents/MetaGPT) |
| 2025 | **MACNET** | Organizes many agents into a clear collaboration network, so information can flow through the team without every agent talking to everyone | [Scaling Large Language Model-based Multi-Agent Collaboration](https://arxiv.org/abs/2406.07155) | - |
| 2026 | **MA-EO** | Multi-agent collaboration via evolving orchestration, enabling dynamic scheduling and learnable organization topology | [Multi-Agent Collaboration via Evolving Orchestration](https://arxiv.org/abs/2505.19591) | - |


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

