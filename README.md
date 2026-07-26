[![Awesome Logo](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![arXiv](https://img.shields.io/badge/arXiv-2605.18661-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.18661)
[![Project Page](https://img.shields.io/badge/Project-Page-orange?style=flat-square&logo=gitbook)](https://worldbench.github.io/awesome-ai-auto-research)
![Visitors](https://komarev.com/ghpvc/?username=worldbench&repo=awesome-ai-auto-research&label=Hello,%20Visitor%20&color=yellow&style=social)
[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-red.svg?style=flat)](https://github.com/worldbench/awesome-ai-auto-research/pulls)

# :sunglasses: Awesome AI Auto-Research

| <img width="100%" src="docs/assets/teaser_paper.png"> |
|:-:|

This repository accompanies the survey paper **"[AI for Auto-Research: Roadmap & User Guide](https://worldbench.github.io/awesome-ai-auto-research)"** and tracks papers on AI-assisted and automated scientific research, covering the **full research lifecycle**.

### :robot: AI Auto-Research

We organize the academic research lifecycle as eight interconnected stages grouped into four epistemological phases. Each phase serves a distinct function in producing, scrutinizing, and communicating scientific knowledge.

| | |
|:-:|:-|
| <img width="360px" src="docs/assets/s1.png"> | **Phase 1: Creation**<br>Generating novel research ideas, searching and synthesizing literature, running coding experiments, and creating publication-quality tables and figures. This phase spans **Idea Generation**, **Literature Review**, **Coding & Experiments**, and **Tables & Figures**. |
| <img width="360px" src="docs/assets/s5.png"> | **Phase 2: Writing**<br>Drafting, editing, and polishing academic manuscripts. AI assistance ranges from semi-automated grammar and citation tools to fully automated paper generation — the most commercially mature yet ethically contested stage. |
| <img width="360px" src="docs/assets/s6.png"> | **Phase 3: Validation**<br>Automated peer review generation, reviewer-paper matching, review quality assessment, and AI-assisted author rebuttals. This phase covers **Peer Review** and **Rebuttal & Revision**. |
| <img width="360px" src="docs/assets/s8.png"> | **Phase 4: Dissemination**<br>Converting papers into slides, posters, videos, websites, and social media content. Each output format targets a different audience and demands its own design logic and AI tool chain. |
| | |

For additional details, kindly refer to our :books: [**Paper**](https://worldbench.github.io/assets_common/papers/survey-ai-auto-research.pdf) and :earth_asia: [**Project Page**](https://worldbench.github.io/awesome-ai-auto-research).

### :books: Citation
If you find this work helpful for your research, please kindly consider citing our paper:
```bibtex
@article{survey-ai-auto-research,
  title   = {{AI} for {Auto-Research}: Roadmap \& User Guide},
  author  = {Kong, Lingdong and Sun, Xian and Chow, Wei and Li, Linfeng and Lin, Kevin Qinghong and Zhang, Xuan Billy
             and Wang, Song and Li, Rong and Wu, Qing and Gao, Wei and Wang, Yingshuo and Xie, Shaoyuan
             and Liu, Jiachen and Qu, Leigang and Li, Shijie and Ng, Lai Xing and Cottereau, Benoit R.
             and Liu, Ziwei and Chua, Tat-Seng and Ooi, Wei Tsang},
  journal = {arXiv preprint arXiv:2605.18661},
  year    = {2026}
}
```



## Table of Contents
- [**0. Background**](#background)
<!--
    - [What Is AI Auto-Research?](#what-is-ai-auto-research)
    - [Five Central Findings](#five-central-findings)
- [**Exhibition: AI-Generated Artifacts**](#exhibition-ai-generated-research-artifacts)
    - [Slide Decks](#ai-generated-slide-decks)
    - [Research Posters](#ai-generated-research-posters)
-->
- [**1. Idea Generation**](#1-idea-generation)
    - [LLM Internal Knowledge-Based Generation](#llm-internal-knowledge-based-generation)
    - [External Signal-Driven Generation](#external-signal-driven-generation)
    - [Multi-Agent Collaborative Generation](#multi-agent-collaborative-generation)
    - [Novelty and Feasibility Assessment](#novelty-and-feasibility-assessment)
- [**2. Literature Review & Paper Search**](#2-literature-review-paper-search)
    - [Literature Retrieval](#literature-retrieval)
    - [Survey & Related Work Generation](#survey-related-work-generation)
    - [Deep Research Agents](#deep-research-agents)
    - [Retrieval and Synthesis Quality Assessment](#retrieval-and-synthesis-quality-assessment)
- [**3. Coding & Experimentation**](#3-coding-experimentation)
    - [Code Generation](#code-generation)
    - [Paper-to-Code](#paper-to-code)
    - [Experiment Execution & Orchestration](#experiment-execution-orchestration)
    - [Code Correctness and Reproducibility Assessment](#code-correctness-and-reproducibility-assessment)
- [**4. Tables & Figures**](#4-tables-figures)
    - [Scientific Figure Generation](#scientific-figure-generation)
    - [Table Understanding & Generation](#table-understanding-generation)
    - [Mathematical Formulas & TikZ](#mathematical-formulas-tikz)
    - [Visual Fidelity and Scientific Accuracy Assessment](#visual-fidelity-and-scientific-accuracy-assessment)
- [**5. Paper Writing**](#5-paper-writing)
    - [Semi-Automated Writing Assistance](#semi-automated-writing-assistance)
    - [Fully Automated Paper Generation](#fully-automated-paper-generation)
    - [Societal Analysis](#societal-analysis)
    - [Writing Quality and AI Detection Assessment](#writing-quality-and-ai-detection-assessment)
- [**6. Peer Review**](#6-peer-review)
    - [Automated Review Generation](#automated-review-generation)
    - [Meta-Review & Reviewer Matching](#meta-review-reviewer-matching)
    - [Review Quality Assessment](#review-quality-assessment)
    - [Adversarial Attacks & Bias Analysis](#adversarial-attacks-bias-analysis)
    - [Detection & Policy](#detection-policy)
    - [Review Consistency and Bias Assessment](#review-consistency-and-bias-assessment)
- [**7. Rebuttal**](#7-rebuttal)
    - [Reviewer Comment Analysis](#reviewer-comment-analysis)
    - [Automated Rebuttal Generation](#automated-rebuttal-generation)
    - [Rebuttal Effectiveness Assessment](#rebuttal-effectiveness-assessment)
- [**8. Dissemination (Paper2X)**](#8-dissemination-paper2x)
    - [Slides & Presentations](#slides--presentations)
    - [Posters](#posters)
    - [Video & Web](#video--web)
    - [Fidelity and Adoption Assessment](#fidelity-and-adoption-assessment)
- [**9. End-to-End Systems**](#9-end-to-end-systems)
    - [Fully Automated Research Systems](#fully-automated-research-systems)
    - [Domain-Specific Systems](#domain-specific-systems)
    - [Evolutionary & Self-Improving Systems](#evolutionary-self-improving-systems)
    - [Research Platforms & Infrastructure](#research-platforms-infrastructure)
- [**10. Societal & Critical Perspectives**](#10-societal-critical-perspectives)
- [**11. Surveys & Curated Lists**](#11-surveys-curated-lists)
- [**12. Tools & GitHub Repos**](#12-tools-github-repos)




| <img width="100%" src="docs/assets/phase1.png"> |
|:-:|


<!--
# Background

| | |
|:-:|:-|
| <img width="260px" src="docs/assets/teaser.png"> | AI-assisted research is crossing a threshold. Fully automated systems can now generate research papers for as little as **$15**, while long-horizon agents execute experiments, draft manuscripts, and simulate critique with minimal human input. Yet this productivity frontier exposes a deeper integrity problem: under scientific pressure, even frontier LLMs still **fabricate results**, miss hidden errors, and fail to judge novelty reliably. |
| | |


## What Is AI Auto-Research?

"AI auto-research" refers to the use of AI systems to automate, assist, or accelerate stages of the **complete academic research lifecycle** -- from hypothesis formation to public dissemination. We organize the lifecycle into **eight interconnected stages** across **four phases**:

| Phase | Stages | Function |
|:-|:-|:-|
| **Phase 1: Creation** | Idea Generation · Literature Review · Coding & Experiments · Tables & Figures | Materially producing a research contribution |
| **Phase 2: Writing** | Paper Writing | Organizing outputs into a formal manuscript |
| **Phase 3: Validation** | Peer Review · Rebuttal & Revision | External scrutiny and iterative refinement |
| **Phase 4: Dissemination** | Paper2X (posters, slides, videos, agents) | Communicating findings to broader audiences |


## What Is the Capability-Integrity Challenge?

The central challenge is not whether AI can produce the *forms* of research, but whether it can preserve the *substance* -- evidence, judgment, provenance, and accountability:

- **Artifact generation outpaces verification.** Generated ideas can appear novel yet weaken after implementation; generated code may run but implement the wrong algorithm; fluent prose can conceal unsupported claims.
- **Capability boundaries emerge on open-ended tasks.** Performance drops sharply for genuinely novel ideas, long-horizon experiments, and scientific judgment.
- **Human-governed collaboration is most credible.** AI should reduce mechanical friction while researchers retain responsibility for interpretation, experimental design, and accountability.


## Five Central Findings

| # | Finding |
|:-:|:-|
| 1 | **Structured tasks benefit most.** AI excels at grounded, externally checkable tasks; capability drops for novel, underspecified, or long-horizon work. |
| 2 | **Artifact generation outpaces verification.** AI can produce plausible outputs faster than it can prove those outputs are correct, faithful, or meaningful. |
| 3 | **Human-governed collaboration is most reliable.** The strongest deployment pattern across all stages is not full autonomy but human-AI collaboration. |
| 4 | **Effective systems converge on layered architectures.** Exploration + execution + verification; orchestration and feedback design matter as much as model scale. |
| 5 | **AI use is a governance problem, not a detection problem.** The key questions are disclosure, attribution, and whether scientific integrity is preserved. |

| <img width="100%" src="docs/assets/teaser_paper.png"> |
|:-:|
| **AI auto-research across the complete lifecycle.** Four phases, eight stages. |



# Exhibition: AI-Generated Research Artifacts

> AI-generated outputs produced from this survey paper using state-of-the-art Paper2X tools. Click any thumbnail to visit the project page gallery.


## AI-Generated Slide Decks

Four automatically-generated presentation decks, each using a different AI tool.

| | |
|:-:|:-:|
| [![GPT-5.5 Slides](https://worldbench.github.io/assets/auto-research/slides/slides-teaser-GPT5.5.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) | [![NotebookLM Slides](https://worldbench.github.io/assets/auto-research/slides/slides-teaser-NotebookLM.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) |
| **GPT-5.5** (28 slides) &nbsp; [Download](https://worldbench.github.io/assets/auto-research/slides/slides-GPT5.5.pptx) | **NotebookLM** (11 slides) &nbsp; [Download](https://worldbench.github.io/assets/auto-research/slides/slides-NotebookLM.pptx) |
| [![Claude Opus 4.7 Slides](https://worldbench.github.io/assets/auto-research/slides/slides-teaser-Opus4.7.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) | [![Manus 1.6 Slides](https://worldbench.github.io/assets/auto-research/slides/slides-teaser-Manus-1.6.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) |
| **Claude Opus 4.7** (27 slides) &nbsp; [Download](https://worldbench.github.io/assets/auto-research/slides/slides-Opus4.7.pptx) | **Manus 1.6** (12 slides) &nbsp; [Download](https://worldbench.github.io/assets/auto-research/slides/slides-Manus-1.6.pptx) |


## AI-Generated Research Posters

Nine AI-generated posters -- six portrait and three landscape -- produced from the survey paper.

**Portrait Format**

| | | |
|:-:|:-:|:-:|
| [![01](https://worldbench.github.io/assets/auto-research/posters/Gemini-Pro.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) | [![02](https://worldbench.github.io/assets/auto-research/posters/Qwen-Image-2.0.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) | [![03](https://worldbench.github.io/assets/auto-research/posters/Claude-Opus4.7.jpg)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) |
| **01 Gemini Pro** | **02 Qwen-Image-2.0** | **03 Claude Opus 4.7** |
| [![04](https://worldbench.github.io/assets/auto-research/posters/SenseNova-U1-8B-MoT.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) | [![05](https://worldbench.github.io/assets/auto-research/posters/GPT-5.5.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) | [![06](https://worldbench.github.io/assets/auto-research/posters/Seedream-4.0.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) |
| **04 SenseNova-U1** | **05 GPT-5.5** | **06 Seedream 4.0** |

**Landscape Format**

| | |
|:-:|:-:|
| [![07](https://worldbench.github.io/assets/auto-research/posters/Gemini-Pro-Landscape.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) | [![08](https://worldbench.github.io/assets/auto-research/posters/Qwen-Image-2.0-Landscape.png)](https://worldbench.github.io/awesome-ai-auto-research#exhibition) |
| **07 Gemini Pro** | **08 Qwen-Image-2.0** |

| [![09]( https://worldbench.github.io/assets/auto-research/posters/Claude-Opus4.7-Landscape.jpg)]( https://worldbench.github.io/awesome-ai-auto-research#exhibition) |
|:-:|
| **09 Claude Opus 4.7** |
-->
# 1. Idea Generation

### LLM Internal Knowledge-Based Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Chain of Ideas` | [![arXiv](https://img.shields.io/badge/arXiv-2410.13185-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.13185)<br>Chain of Ideas: Revolutionizing Research Via Novel Idea Development with LLM Agents | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/DAMO-NLP-SG/CoI-Agent)](https://github.com/DAMO-NLP-SG/CoI-Agent) |
| `ResearchAgent` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.naacl-long.342/)<br>ResearchAgent: Iterative Research Idea Generation over Scientific Literature with Large Language Models | NAACL '25 | - | [![GitHub](https://img.shields.io/github/stars/JinheonBaek/ResearchAgent)](https://github.com/JinheonBaek/ResearchAgent) |
| `SciMON` | [![arXiv](https://img.shields.io/badge/arXiv-2305.14259-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2305.14259)<br>SciMON: Scientific Inspiration Machines Optimized for Novelty | ACL '24 | - | [![GitHub](https://img.shields.io/github/stars/EagleW/CLBD)](https://github.com/EagleW/CLBD) |
| `Idea Gen Agent` | [![arXiv](https://img.shields.io/badge/arXiv-2409.04109-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2409.04109)<br>Can LLMs Generate Novel Research Ideas? A Large Scale Human Study with 100+ NLP Researchers | arXiv '24 | - | - |
| `IRIS` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.acl-demo.57/)<br>IRIS: Interactive Research Ideation System for Accelerating Scientific Discovery | ACL '25 | - | [![GitHub](https://img.shields.io/github/stars/Anikethh/IRIS-Interactive-Research-Ideation-System)](https://github.com/Anikethh/IRIS-Interactive-Research-Ideation-System) |
| `Spark` | [![arXiv](https://img.shields.io/badge/arXiv-2504.20090-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.20090)<br>Spark: A System for Scientifically Creative Idea Generation | ICCC '25 | - | - |
| `Diverse Hypo. Search` | [![arXiv](https://img.shields.io/badge/arXiv-2606.10587-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.10587)<br>Towards Diverse Scientific Hypothesis Search with Large Language Models | arXiv '26 | - | - |
||

### External Signal-Driven Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `MOOSE-Chem` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openreview.net/forum?id=X9OfMNNepI)<br>MOOSE-Chem: Large Language Models for Rediscovering Unseen Chemistry Scientific Hypotheses | ICLR '25 | - | - |
| `Nova` | [![arXiv](https://img.shields.io/badge/arXiv-2410.14255-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.14255)<br>Nova: An Iterative Planning and Search Approach to Enhance Novelty and Diversity of LLM Generated Ideas | arXiv '24 | - | - |
| `SciAgents` | [![arXiv](https://img.shields.io/badge/arXiv-2409.05556-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2409.05556)<br>SciAgents: Automating Scientific Discovery through Multi-Agent Intelligent Graph Reasoning | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/lamm-mit/SciAgentsDiscovery)](https://github.com/lamm-mit/SciAgentsDiscovery) |
| `SciPIP` | [![arXiv](https://img.shields.io/badge/arXiv-2410.23166-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.23166)<br>SciPIP: An LLM-based Scientific Paper Idea Proposer | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/cheerss/SciPIP)](https://github.com/cheerss/SciPIP) |
| `IdeaSynth` | [![arXiv](https://img.shields.io/badge/arXiv-2410.04025-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.04025)<br>IdeaSynth: Iterative Research Idea Development Through Evolving and Composing Idea Facets with Literature-Grounded Feedback | CHI '25 | - | - |
| `MOOSE-Chem2` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://nips.cc/virtual/2025/poster/118171)<br>MOOSE-Chem2: Exploring LLM Limits in Fine-Grained Scientific Hypothesis Discovery via Hierarchical Search | NeurIPS '25 | - | - |
||

### Multi-Agent Collaborative Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Combi. Creativity` | [![arXiv](https://img.shields.io/badge/arXiv-2412.14141-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.14141)<br>Combi. Creativity | arXiv '24 | - | - |
| `Deep Ideation` | [![arXiv](https://img.shields.io/badge/arXiv-2511.02238-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.02238)<br>Deep Ideation: Designing LLM Agents to Generate Novel Research Ideas on Scientific Concept Network | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/kyZhao-1/Deep-Ideation)](https://github.com/kyZhao-1/Deep-Ideation) |
| `VirSci` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.acl-long.1368/)<br>Many Heads Are Better Than One: Improved Scientific Idea Generation by A LLM-Based Multi-Agent System | ACL '25 | - | [![GitHub](https://img.shields.io/github/stars/open-sciencelab/Virtual-Scientists)](https://github.com/open-sciencelab/Virtual-Scientists) |
| `Multi-Agent Dial.` | [![arXiv](https://img.shields.io/badge/arXiv-2507.08350-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2507.08350)<br>Multi-Agent Dial. | SIGDIAL '25 | - | - |
| `Artificial Hivemind` | [![arXiv](https://img.shields.io/badge/arXiv-2510.22954-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.22954)<br>Artificial Hivemind: The Open-Ended Homogeneity of Language Models (and Beyond) | NeurIPS '25 | - | - |
| `Auditable AI Sci.` | [![arXiv](https://img.shields.io/badge/arXiv-2607.09195-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2607.09195)<br>Toward Auditable AI Scientists: A Hypothesis Evolution Protocol for LLM Agents | arXiv '26 | - | - |
||

### Novelty and Feasibility Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `IdeaBench` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://doi.org/10.1145/3711896.3737419)<br>LiveIdeaBench: Evaluating LLMs' Scientific Creativity and Idea Generation with Minimal Context | KDD '25 | - | - |
| `LiveIdeaBench` | [![arXiv](https://img.shields.io/badge/arXiv-2412.17596-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.17596)<br>LiveIdeaBench: Evaluating LLMs' Scientific Creativity and Idea Generation with Minimal Context | arXiv '24 | - | - |
| `AI Idea Bench 2025` | [![arXiv](https://img.shields.io/badge/arXiv-2504.14191-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.14191)<br>AI Idea Bench 2025: AI Research Idea Generation Benchmark | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/yansheng-qiu/AI_Idea_Bench_2025)](https://github.com/yansheng-qiu/AI_Idea_Bench_2025) |
| `HeurekaBench` | [![arXiv](https://img.shields.io/badge/arXiv-2601.01678-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.01678)<br>HeurekaBench: A Benchmarking Framework for AI Co-scientist | ICLR '26 | - | [![GitHub](https://img.shields.io/github/stars/mlbio-epfl/HeurekaBench)](https://github.com/mlbio-epfl/HeurekaBench) |
| `ResearchBench` | [![arXiv](https://img.shields.io/badge/arXiv-2503.21248-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.21248)<br>ResearchBench: Benchmarking LLMs in Scientific Discovery via Inspiration-Based Task Decomposition | ACL '26 | - | - |
| `HindSight` | [![arXiv](https://img.shields.io/badge/arXiv-2603.15164-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.15164)<br>HindSight: Evaluating LLM-Generated Research Ideas via Future Impact | arXiv '26 | - | - |
| `Rubric Rewards` | [![arXiv](https://img.shields.io/badge/arXiv-2512.23707-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.23707)<br>Training AI Co-Scientists Using Rubric Rewards | arXiv '25 | - | - |
| `DeepInnovator` | [![arXiv](https://img.shields.io/badge/arXiv-2602.18920-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.18920)<br>DeepInnovator: Triggering the Innovative Capabilities of LLMs | arXiv '26 | - | [![GitHub](https://img.shields.io/github/stars/HKUDS/DeepInnovator)](https://github.com/HKUDS/DeepInnovator) |
| `FlowPIE` | [![arXiv](https://img.shields.io/badge/arXiv-2603.29557-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.29557)<br>FlowPIE: Test-Time Scientific Idea Evolution with Flow-Guided Literature Exploration | arXiv '26 | - | - |
| `SoundnessBench` | [![arXiv](https://img.shields.io/badge/arXiv-2605.30329-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.30329)<br>SoundnessBench: Can Your AI Scientist Really Tell Good Research Ideas from Bad Ones? | arXiv '26 | - | - |
| `LLM-Judge Novelty` | [![arXiv](https://img.shields.io/badge/arXiv-2606.12071-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.12071)<br>On the Limits of LLM-as-Judge for Scientific Novelty Assessment | arXiv '26 | - | - |
||



# 2. Literature Review & Paper Search

### Literature Retrieval

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `CiteME` | [![arXiv](https://img.shields.io/badge/arXiv-2407.12861-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.12861)<br>CiteME: Can Language Models Accurately Cite Scientific Claims? | arXiv '24 | - | - |
| `LitLLM` | [![arXiv](https://img.shields.io/badge/arXiv-2402.01788-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.01788)<br>LitLLM: A Toolkit for Literature Review with Large Language Models | arXiv '24 | - | - |
| `LitSearch` | [![arXiv](https://img.shields.io/badge/arXiv-2407.18940-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.18940)<br>LitSearch: A Retrieval Benchmark for Scientific Literature Search | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/princeton-nlp/LitSearch)](https://github.com/princeton-nlp/LitSearch) |
| `PaperQA2` | [![arXiv](https://img.shields.io/badge/arXiv-2409.13740-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2409.13740)<br>Language Agents Achieve Superhuman Synthesis of Scientific Knowledge | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/Future-House/paper-qa)](https://github.com/Future-House/paper-qa) |
| `OpenResearcher` | [![arXiv](https://img.shields.io/badge/arXiv-2408.09578-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2408.09578)<br>OpenResearcher: Unleashing AI for Accelerated Scientific Research | EMNLP '24 | - | - |
| `PaSa` | [![arXiv](https://img.shields.io/badge/arXiv-2501.10120-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.10120)<br>PaSa: An LLM Agent for Comprehensive Academic Paper Search | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/bytedance/pasa)](https://github.com/bytedance/pasa) |
| `Self-Evolving Retrieval` | [![arXiv](https://img.shields.io/badge/arXiv-2605.14306-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.14306)<br>Towards Self-Evolving Agentic Literature Retrieval | arXiv '26 | - | - |
| `MasterSet` | [![arXiv](https://img.shields.io/badge/arXiv-2604.17680-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.17680)<br>MasterSet: A Large-Scale Benchmark for Must-Cite Citation Recommendation in the AI/ML Literature | arXiv '26 | - | - |
||

### Survey & Related Work Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ChatPaper` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://github.com/kaixindelele/ChatPaper)<br>ChatPaper: Use LLM to summarize papers | GitHub '23 | - | [![GitHub](https://img.shields.io/github/stars/kaixindelele/ChatPaper)](https://github.com/kaixindelele/ChatPaper) |
| `PaperQA` | [![arXiv](https://img.shields.io/badge/arXiv-2312.07559-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.07559)<br>PaperQA: Retrieval-Augmented Generative Agent for Scientific Research | arXiv '23 | - | [![GitHub](https://img.shields.io/github/stars/Future-House/paper-qa)](https://github.com/Future-House/paper-qa) |
| `AutoSurvey` | [![arXiv](https://img.shields.io/badge/arXiv-2406.10252-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2406.10252)<br>AutoSurvey: Large Language Models Can Automatically Write Surveys | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/AutoSurveys/AutoSurvey)](https://github.com/AutoSurveys/AutoSurvey) |
| `GPT Researcher` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://github.com/assafelovic/gpt-researcher)<br>GPT Researcher: Autonomous Agent for Comprehensive Online Research | GitHub '24 | - | [![GitHub](https://img.shields.io/github/stars/assafelovic/gpt-researcher)](https://github.com/assafelovic/gpt-researcher) |
| `LLMs for Lit. Review` | [![arXiv](https://img.shields.io/badge/arXiv-2412.13612-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.13612)<br>LLMs for Lit. Review | arXiv '24 | - | - |
| `STORM` | [![arXiv](https://img.shields.io/badge/arXiv-2402.14207-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.14207)<br>Assisting in Writing Wikipedia-like Articles From Scratch with Large Language Models | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/stanford-oval/storm)](https://github.com/stanford-oval/storm) |
| `Agentic AutoSurvey` | [![arXiv](https://img.shields.io/badge/arXiv-2509.18661-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.18661)<br>Agentic AutoSurvey: Let LLMs Survey LLMs | arXiv '25 | - | - |
| `Citegeist` | [![arXiv](https://img.shields.io/badge/arXiv-2503.23229-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.23229)<br>Citegeist: Automated Generation of Related Work Analysis on the arXiv Corpus | arXiv '25 | - | - |
| `IterSurvey` | [![arXiv](https://img.shields.io/badge/arXiv-2510.21900-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.21900)<br>IterSurvey: Deep Literature Survey Automation with an Iterative Workflow | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/HancCui/IterSurvey_Autosurveyv2)](https://github.com/HancCui/IterSurvey_Autosurveyv2) |
| `LiRA` | [![arXiv](https://img.shields.io/badge/arXiv-2510.05138-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.05138)<br>LiRA: A Multi-Agent Framework for Reliable and Readable Literature Review Generation | arXiv '25 | - | - |
| `SurveyForge` | [![arXiv](https://img.shields.io/badge/arXiv-2503.04629-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.04629)<br>SurveyForge: On the Outline Heuristics, Memory-Driven Generation, and Multi-dimensional Evaluation for Automated Survey Writing | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/Alpha-Innovator/SurveyForge)](https://github.com/Alpha-Innovator/SurveyForge) |
| `SurveyG` | [![arXiv](https://img.shields.io/badge/arXiv-2510.07733-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.07733)<br>SurveyG: A Multi-Agent LLM Framework with Hierarchical Citation Graph for Automated Survey Generation | arXiv '25 | - | - |
| `SurveyX` | [![arXiv](https://img.shields.io/badge/arXiv-2502.14776-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.14776)<br>SurveyX: Academic Survey Automation via Large Language Models | arXiv '25 | - | - |
| `InteractiveSurvey` | [![arXiv](https://img.shields.io/badge/arXiv-2504.08762-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.08762)<br>InteractiveSurvey: An LLM-based Personalized and Interactive Survey Paper Generation System | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/TechnicolorGUO/InteractiveSurvey)](https://github.com/TechnicolorGUO/InteractiveSurvey) |
| `CiteLLM` | [![arXiv](https://img.shields.io/badge/arXiv-2602.23075-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.23075)<br>CiteLLM: An Agentic Platform for Trustworthy Scientific Reference Discovery | arXiv '26 | - | - |
| `DeepSurvey` | [![arXiv](https://img.shields.io/badge/arXiv-2605.29522-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.29522)<br>DeepSurvey: Enhancing Analytical Depth and Citation Reliability in Automated Survey Generation | arXiv '26 | - | - |
| `STRUCTSURVEY` | [![arXiv](https://img.shields.io/badge/arXiv-2607.01243-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2607.01243)<br>STRUCTSURVEY: Structured Agentic Retrieval for Automated Survey Paper Generation | arXiv '26 | - | - |
||

### Deep Research Agents

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ASReview` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s42256-020-00287-7)<br>An Open Source Machine Learning Framework for Efficient and Transparent Systematic Reviews | Nature MI '21 | - | [![GitHub](https://img.shields.io/github/stars/asreview/asreview)](https://github.com/asreview/asreview) |
| `CHIME` | [![arXiv](https://img.shields.io/badge/arXiv-2407.16148-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.16148)<br>CHIME: LLM-Assisted Hierarchical Organization of Scientific Studies for Literature Review Support | arXiv '24 | - | - |
| `DeepResearch-Agent` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://github.com/SkyworkAI/DeepResearchAgent)<br>DeepResearchAgent: A Hierarchical Multi-Agent System for Deep Research | GitHub '25 | - | [![GitHub](https://img.shields.io/github/stars/SkyworkAI/DeepResearchAgent)](https://github.com/SkyworkAI/DeepResearchAgent) |
| `DeerFlow` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://github.com/bytedance/deer-flow)<br>DeerFlow: A Deep Research Framework Orchestrating Sub-Agents, Memory, and Sandboxes | GitHub '25 | - | [![GitHub](https://img.shields.io/github/stars/bytedance/deer-flow)](https://github.com/bytedance/deer-flow) |
| `OpenScholar` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://doi.org/10.1038/s41586-025-10072-4)<br>OpenScholar: Synthesizing Scientific Literature with Retrieval-Augmented LMs | Nature '26 | - | - |
| `AutoAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2502.05957-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.05957)<br>AutoAgent | arXiv '25 | - | - |
| `Tongyi DeepResearch` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://github.com/Alibaba-NLP/DeepResearch)<br>Tongyi DeepResearch | GitHub '25 | - | [![GitHub](https://img.shields.io/github/stars/Alibaba-NLP/DeepResearch)](https://github.com/Alibaba-NLP/DeepResearch) |
| `O-Researcher` | [![arXiv](https://img.shields.io/badge/arXiv-2601.03743-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.03743)<br>O-Researcher: An Open Ended Deep Research Model via Multi-Agent Distillation and Agentic RL | arXiv '26 | - | - |
| `OpenResearcher` | [![arXiv](https://img.shields.io/badge/arXiv-2603.20278-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.20278)<br>OpenResearcher: Unleashing AI for Accelerated Scientific Research | arXiv '26 | - | [![GitHub](https://img.shields.io/github/stars/TIGER-AI-Lab/OpenResearcher)](https://github.com/TIGER-AI-Lab/OpenResearcher) |
||

### Retrieval and Synthesis Quality Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `DeepScholar-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2508.20033-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.20033)<br>DeepScholar-Bench: A Live Benchmark and Automated Evaluation for Generative Research Synthesis | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/guestrin-lab/deepscholar-bench)](https://github.com/guestrin-lab/deepscholar-bench) |
| `ReportBench` | [![arXiv](https://img.shields.io/badge/arXiv-2508.15804-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.15804)<br>ReportBench: Evaluating Deep Research Agents via Academic Survey Tasks | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/ByteDance-BandAI/ReportBench)](https://github.com/ByteDance-BandAI/ReportBench) |
| `IDRBench` | [![arXiv](https://img.shields.io/badge/arXiv-2601.06676-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.06676)<br>IDRBench: Interactive Deep Research Benchmark | arXiv '26 | - | - |
| `ScholarGym` | [![arXiv](https://img.shields.io/badge/arXiv-2601.21654-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.21654)<br>ScholarGym: Benchmarking Large Language Model Capabilities in the Information-Gathering Stage of Deep Research | arXiv '26 | - | - |
| `SciNetBench` | [![arXiv](https://img.shields.io/badge/arXiv-2601.03260-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.03260)<br>SciNetBench: A Relation-Aware Benchmark for Scientific Literature Retrieval Agents | arXiv '26 | - | - |
| `AutoResearchBench` | [![arXiv](https://img.shields.io/badge/arXiv-2604.25256-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.25256)<br>AutoResearchBench: Benchmarking AI Agents on Complex Scientific Literature Discovery | arXiv '26 | - | - |
| `PaperMind` | [![arXiv](https://img.shields.io/badge/arXiv-2604.21304-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.21304)<br>PaperMind: Benchmarking Agentic Reasoning and Critique over Scientific Papers in Multimodal LLMs | arXiv '26 | - | - |
||



# 3. Coding & Experimentation

### Code Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `SWE-bench` | [![arXiv](https://img.shields.io/badge/arXiv-2310.06770-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.06770)<br>SWE-bench: Can Language Models Resolve Real-World GitHub Issues? | ICLR '24 | - | [![GitHub](https://img.shields.io/github/stars/princeton-nlp/SWE-bench)](https://github.com/princeton-nlp/SWE-bench) |
| `SWE-agent` | [![arXiv](https://img.shields.io/badge/arXiv-2405.15793-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2405.15793)<br>SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/princeton-nlp/SWE-agent)](https://github.com/princeton-nlp/SWE-agent) |
| `OpenHands` | [![arXiv](https://img.shields.io/badge/arXiv-2407.16741-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.16741)<br>OpenHands: An Open Platform for AI Software Developers as Generalist Agents | ICLR '25 | - | [![GitHub](https://img.shields.io/github/stars/All-Hands-AI/OpenHands)](https://github.com/All-Hands-AI/OpenHands) |
| `SWE-bench Pro` | [![arXiv](https://img.shields.io/badge/arXiv-2509.16941-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.16941)<br>SWE-Bench Pro: Can AI Agents Solve Long-Horizon Software Engineering Tasks? | arXiv '25 | - | - |
| `SWE-EVO` | [![arXiv](https://img.shields.io/badge/arXiv-2512.18470-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.18470)<br>SWE-EVO: Benchmarking Coding Agents in Long-Horizon Software Evolution Scenarios | arXiv '25 | - | - |
||

### Paper-to-Code

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `FunSearch` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s41586-023-06924-6)<br>Mathematical Discoveries from Program Search with Large Language Models | Nature '24 | - | [![GitHub](https://img.shields.io/github/stars/google-deepmind/funsearch)](https://github.com/google-deepmind/funsearch) |
| `SciCode` | [![arXiv](https://img.shields.io/badge/arXiv-2407.13168-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.13168)<br>SciCode: A Research Coding Benchmark Curated by Scientists | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/scicode-bench/SciCode)](https://github.com/scicode-bench/SciCode) |
| `PaperBench` | [![arXiv](https://img.shields.io/badge/arXiv-2504.01848-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.01848)<br>PaperBench: Evaluating AI's Ability to Replicate AI Research | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/openai/preparedness)](https://github.com/openai/preparedness) |
| `PaperCoder` | [![arXiv](https://img.shields.io/badge/arXiv-2504.17192-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.17192)<br>Paper2Code: Automating Code Generation from Scientific Papers in Machine Learning | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/going-doer/Paper2Code)](https://github.com/going-doer/Paper2Code) |
| `ResearchCodeBench` | [![arXiv](https://img.shields.io/badge/arXiv-2506.02314-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.02314)<br>ResearchCodeBench: Benchmarking LLMs on Implementing Novel ML Research Code | arXiv '25 | - | - |
| `SciReplicate-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2504.00255-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.00255)<br>SciReplicate-Bench: Benchmarking LLMs in Agent-driven Algorithmic Reproduction from Research Papers | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/xyzCS/SciReplicate-Bench)](https://github.com/xyzCS/SciReplicate-Bench) |
||

### Experiment Execution & Orchestration

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `BioPlanner` | [![arXiv](https://img.shields.io/badge/arXiv-2310.10632-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.10632)<br>BioPlanner: Automatic Evaluation of LLMs on Protocol Planning | arXiv '23 | - | [![GitHub](https://img.shields.io/github/stars/bioplanner/bioplanner)](https://github.com/bioplanner/bioplanner) |
| `CRISPR-GPT` | [![arXiv](https://img.shields.io/badge/arXiv-2404.18021-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2404.18021)<br>CRISPR-GPT for Agentic Automation of Gene-Editing Experiments | arXiv '24 | - | - |
| `DS-Agent` | [![arXiv](https://img.shields.io/badge/arXiv-2402.17453-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.17453)<br>DS-Agent: Automated Data Science by Empowering Large Language Models with Case-Based Reasoning | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/guosyjlu/DS-Agent)](https://github.com/guosyjlu/DS-Agent) |
| `MLE-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2410.07095-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.07095)<br>MLE-Bench: Evaluating Machine Learning Agents on Machine Learning Engineering | arXiv '24 | - | - |
| `MLAgentBench` | [![arXiv](https://img.shields.io/badge/arXiv-2310.03302-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.03302)<br>MLAgentBench: Evaluating Language Agents on Machine Learning Experimentation | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/snap-stanford/MLAgentBench)](https://github.com/snap-stanford/MLAgentBench) |
| `MLR-Copilot` | [![arXiv](https://img.shields.io/badge/arXiv-2408.14033-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2408.14033)<br>MLR-Copilot: Autonomous Machine Learning Research based on Large Language Models Agents | arXiv '24 | - | - |
| `AIDE` | [![arXiv](https://img.shields.io/badge/arXiv-2502.13138-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.13138)<br>AIDE: AI-Driven Exploration in the Space of Code | arXiv '25 | - | - |
| `AlphaEvolve` | [![arXiv](https://img.shields.io/badge/arXiv-2506.13131-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.13131)<br>AlphaEvolve: A Coding Agent for Scientific and Algorithmic Discovery | arXiv '25 | - | - |
| `AutoReproduce` | [![arXiv](https://img.shields.io/badge/arXiv-2505.20662-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.20662)<br>AutoReproduce: Automatic AI Experiment Reproduction with Paper Lineage | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/AI9Stars/AutoReproduce)](https://github.com/AI9Stars/AutoReproduce) |
| `CURIE` | [![arXiv](https://img.shields.io/badge/arXiv-2502.16069-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.16069)<br>Curie: Toward Rigorous and Automated Scientific Experimentation with AI Agents | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/Just-Curieous/Curie)](https://github.com/Just-Curieous/Curie) |
| `MLGym` | [![arXiv](https://img.shields.io/badge/arXiv-2502.14499-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.14499)<br>MLGym: A New Framework and Benchmark for Advancing AI Research Agents | arXiv '25 | - | - |
| `MLR-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2505.19955-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.19955)<br>MLR-Bench: Evaluating AI Agents on Open-Ended Machine Learning Research | arXiv '25 | - | - |
| `Execution-Grounded` | [![arXiv](https://img.shields.io/badge/arXiv-2601.14525-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.14525)<br>Towards Execution-Grounded Automated AI Research | arXiv '26 | - | - |
| `Learn to Discover` | [![arXiv](https://img.shields.io/badge/arXiv-2601.16175-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.16175)<br>Learning to Discover at Test Time | arXiv '26 | - | - |
| `AutoNumerics` | [![arXiv](https://img.shields.io/badge/arXiv-2602.17607-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.17607)<br>AutoNumerics: An Autonomous, PDE-Agnostic Multi-Agent Pipeline for Scientific Computing | arXiv '26 | - | [![GitHub](https://img.shields.io/github/stars/Daviddjddu/Autonumerics)](https://github.com/Daviddjddu/Autonumerics) |
| `SciNav` | [![arXiv](https://img.shields.io/badge/arXiv-2603.20256-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.20256)<br>SciNav: A General Agent Framework for Scientific Coding Tasks | arXiv '26 | - | - |
| `FrontierScience` | [![arXiv](https://img.shields.io/badge/arXiv-2601.21165-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.21165)<br>FrontierScience: Evaluating AI's Ability to Perform Expert-Level Scientific Tasks | arXiv '26 | - | - |
| `EvoDS` | [![arXiv](https://img.shields.io/badge/arXiv-2606.03841-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.03841)<br>EvoDS: Self-Evolving Autonomous Data Science Agent with Skill Learning and Context Management | arXiv '26 | - | - |
| `AutoTTS` | [![arXiv](https://img.shields.io/badge/arXiv-2605.08083-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.08083)<br>LLMs Improving LLMs: Agentic Discovery for Test-Time Scaling | arXiv '26 | - | [![GitHub](https://img.shields.io/github/stars/zhengkid/AutoTTS)](https://github.com/zhengkid/AutoTTS) |
| `AutoScientists` | [![arXiv](https://img.shields.io/badge/arXiv-2605.28655-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.28655)<br>AutoScientists: Self-Organizing Agent Teams for Long-Running Scientific Experimentation | arXiv '26 | - | - |
| `EurekAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2606.13662-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.13662)<br>EurekAgent: Agent Environment Engineering is All You Need For Autonomous Scientific Discovery | arXiv '26 | - | - |
||

### Code Correctness and Reproducibility Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `DiscoveryBench` | [![arXiv](https://img.shields.io/badge/arXiv-2407.01725-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.01725)<br>DiscoveryBench: Towards Data-Driven Discovery with Large Language Models | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/allenai/discoverybench)](https://github.com/allenai/discoverybench) |
| `DiscoveryWorld` | [![arXiv](https://img.shields.io/badge/arXiv-2406.06769-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2406.06769)<br>DiscoveryWorld: A Virtual Environment for Developing and Evaluating Automated Scientific Discovery Agents | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/allenai/discoveryworld)](https://github.com/allenai/discoveryworld) |
| `InfiAgent-DABench` | [![arXiv](https://img.shields.io/badge/arXiv-2401.05507-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2401.05507)<br>InfiAgent-DABench: Evaluating Agents on Data Analysis Tasks | arXiv '24 | - | - |
| `ScienceAgentBench` | [![arXiv](https://img.shields.io/badge/arXiv-2410.05080-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.05080)<br>ScienceAgentBench: Toward Rigorous Assessment of Language Agents for Data-Driven Scientific Discovery | arXiv '24 | - | - |
| `LAB-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2407.10362-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.10362)<br>Lab-Bench: Measuring Capabilities of Language Models for Biology Research | arXiv '24 | - | [![GitHub](https://img.shields.io/github/stars/Future-House/LAB-Bench)](https://github.com/Future-House/LAB-Bench) |
| `KernelBench` | [![arXiv](https://img.shields.io/badge/arXiv-2502.10517-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.10517)<br>KernelBench: Can LLMs Write Efficient GPU Kernels? | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/ScalingIntelligence/KernelBench)](https://github.com/ScalingIntelligence/KernelBench) |
| `TritonBench` | [![arXiv](https://img.shields.io/badge/arXiv-2502.14752-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.14752)<br>TritonBench: Benchmarking Large Language Model Capabilities for Generating Triton Operators | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/thunlp/TritonBench)](https://github.com/thunlp/TritonBench) |
| `AstaBench` | [![arXiv](https://img.shields.io/badge/arXiv-2510.21652-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.21652)<br>AstaBench: Rigorous Benchmarking of AI Agents with a Scientific Research Suite | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/allenai/asta-bench)](https://github.com/allenai/asta-bench) |
| `ResearchClawBench` | [![arXiv](https://img.shields.io/badge/arXiv-2512.16969-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.16969)<br>Probing Scientific General Intelligence of LLMs with Scientist-Aligned Workflows | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/InternScience/ResearchClawBench)](https://github.com/InternScience/ResearchClawBench) |
| `EXP-Bench` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openreview.net/forum?id=KjgyAm383Z)<br>EXP-Bench: Can AI Conduct AI Research Experiments? | ICLR '26 | - | [![GitHub](https://img.shields.io/github/stars/Just-Curieous/Curie)](https://github.com/Just-Curieous/Curie/tree/main/benchmark/exp_bench) |
| `PostTrainBench` | [![arXiv](https://img.shields.io/badge/arXiv-2603.08640-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.08640)<br>PostTrainBench: Can LLM Agents Automate LLM Post-Training? | arXiv '26 | - | [![GitHub](https://img.shields.io/github/stars/aisa-group/PostTrainBench)](https://github.com/aisa-group/PostTrainBench) |
| `MLReplicate` | [![arXiv](https://img.shields.io/badge/arXiv-2605.16616-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.16616)<br>MLReplicate: Benchmarking Autonomous Research Systems for Machine Learning Reproducibility | arXiv '26 | - | - |
| `BeyondSWE` | [![arXiv](https://img.shields.io/badge/arXiv-2603.03194-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.03194)<br>BeyondSWE: Can Current Code Agent Survive Beyond Single-Repo Bug Fixing? | arXiv '26 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aweai-team.github.io/BeyondSWE/) | [![GitHub](https://img.shields.io/github/stars/AweAI-Team/BeyondSWE)](https://github.com/AweAI-Team/BeyondSWE) |
| `NatureBench` | [![arXiv](https://img.shields.io/badge/arXiv-2606.24530-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.24530)<br>NatureBench: Can Coding Agents Match the Published SOTA of Nature-Family Papers? | arXiv '26 | - | - |
||



# 4. Tables & Figures

### Scientific Figure Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ChartGPT` | [![arXiv](https://img.shields.io/badge/arXiv-2311.01920-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2311.01920)<br>ChartGPT: Leveraging LLMs to Generate Charts from Abstract Natural Language | arXiv '23 | - | - |
| `MatPlotAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2402.11453-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.11453)<br>MatPlotAgent: Method and Evaluation for LLM-Based Agentic Scientific Data Visualization | arXiv '24 | - | - |
| `CoDA` | [![arXiv](https://img.shields.io/badge/arXiv-2510.03194-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.03194)<br>CoDA: Agentic Systems for Collaborative Data Visualization | arXiv '25 | - | - |
| `PlotGen` | [![arXiv](https://img.shields.io/badge/arXiv-2502.00988-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.00988)<br>PlotGen: Multi-Agent LLM-based Scientific Data Visualization via Multimodal Feedback | arXiv '25 | - | - |
| `VIS-Shepherd` | [![arXiv](https://img.shields.io/badge/arXiv-2506.13326-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.13326)<br>VIS-Shepherd: Constructing Critic for LLM-based Data Visualization Generation | arXiv '25 | - | - |
| `DiagramAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2411.11916-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.11916)<br>From Words to Structured Visuals: A Benchmark and Framework for Text-to-Diagram Generation and Editing | CVPR '25 | - | - |
| `StarVector` | [![arXiv](https://img.shields.io/badge/arXiv-2312.11556-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.11556)<br>StarVector: Generating Scalable Vector Graphics Code from Images and Text | CVPR '25 | - | - |
| `VisCoder` | [![arXiv](https://img.shields.io/badge/arXiv-2506.03930-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.03930)<br>VisCoder: Fine-Tuning LLMs for Executable Python Visualization Code Generation | EMNLP '25 | - | - |
| `AI-Generated Figures` | [![arXiv](https://img.shields.io/badge/arXiv-2603.16159-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.16159)<br>AI-Generated Figures | arXiv '26 | - | - |
| `AutoFigure-Edit` | [![arXiv](https://img.shields.io/badge/arXiv-2603.06674-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.06674)<br>AutoFigure-Edit: Generating Editable Scientific Illustration | arXiv '26 | - | [![GitHub](https://img.shields.io/github/stars/ResearAI/AutoFigure-Edit)](https://github.com/ResearAI/AutoFigure-Edit) |
| `AutoFigure` | [![arXiv](https://img.shields.io/badge/arXiv-2602.03828-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.03828)<br>AutoFigure-Edit: Generating Editable Scientific Illustration | ICLR '26 | - | [![GitHub](https://img.shields.io/github/stars/ResearAI/AutoFigure)](https://github.com/ResearAI/AutoFigure) |
| `PaperBanana` | [![arXiv](https://img.shields.io/badge/arXiv-2601.23265-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.23265)<br>PaperBanana: Automating Academic Illustration for AI Scientists | arXiv '26 | - | - |
| `SAIL` | [![arXiv](https://img.shields.io/badge/arXiv-2603.18145-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.18145)<br>Setting SAIL: Leveraging Scientist-AI-Loops for Rigorous Visualization Tools | arXiv '26 | - | - |
| `Crafter` | [![arXiv](https://img.shields.io/badge/arXiv-2605.30611-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.30611)<br>Crafter: A Multi-Agent Harness for Editable Scientific Figure Generation from Diverse Inputs | arXiv '26 | - | - |
| `DiagramRAG` | [![arXiv](https://img.shields.io/badge/arXiv-2605.27931-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.27931)<br>DiagramRAG: A Lightweight Framework to Retrieve Scientific Diagram for Figure Generation | arXiv '26 | - | - |
| `GeoSVG-RL` | [![arXiv](https://img.shields.io/badge/arXiv-2605.25447-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.25447)<br>GeoSVG-RL: Geometry-Aware Reinforcement Learning for Layout-Constrained Text-to-SVG Diagram Generation | arXiv '26 | - | - |
| `Can AI Draw Sci.` | [![arXiv](https://img.shields.io/badge/arXiv-2606.28406-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.28406)<br>Can AI Draw Science? A Benchmark for Evaluating Scientific Figure Generation by Text-to-Image and Multimodal Models | arXiv '26 | - | - |
||

### Table Understanding & Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ArxivDIGESTables` | [![arXiv](https://img.shields.io/badge/arXiv-2410.22360-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.22360)<br>ArxivDIGESTables: Synthesizing Scientific Literature into Tables using Language Models | EMNLP '24 | - | - |
| `Chain-of-Table` | [![arXiv](https://img.shields.io/badge/arXiv-2401.04398-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2401.04398)<br>Chain-of-Table: Evolving Tables in Reasoning Chain for Table Understanding | ICLR '24 | - | - |
| `ShowTable` | [![arXiv](https://img.shields.io/badge/arXiv-2512.13303-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.13303)<br>ShowTable: Unlocking Creative Table Visualization with Collaborative Reflection and Refinement | CVPR '26 | - | - |
| `Table2LaTeX-RL` | [![arXiv](https://img.shields.io/badge/arXiv-2509.17589-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.17589)<br>Table2LaTeX-RL: Converting Table Images to High-Fidelity LaTeX Code Using Reinforced Multimodal Language Models | arXiv '25 | - | - |
| `CSPO` | [![arXiv](https://img.shields.io/badge/arXiv-2604.10918-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.10918)<br>CSPO: Alleviating Reward Ambiguity for Structured Table-to-LaTeX Generation | arXiv '26 | - | - |
||

### Mathematical Formulas & TikZ

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `AutomaTikZ` | [![arXiv](https://img.shields.io/badge/arXiv-2310.00367-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.00367)<br>AutomaTikZ: Text-Guided Synthesis of Scientific Vector Graphics with TikZ | ICLR '24 | - | - |
| `DeTikZify` | [![arXiv](https://img.shields.io/badge/arXiv-2405.15306-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2405.15306)<br>DeTikZify: Synthesizing Graphics Programs for Scientific Figures and Sketches with TikZ | NeurIPS '24 | - | - |
| `TikZilla` | [![arXiv](https://img.shields.io/badge/arXiv-2603.03072-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.03072)<br>TikZilla: Scaling Text-to-TikZ with High-Quality Data and Reinforcement Learning | arXiv '26 | - | - |
||

### Visual Fidelity and Scientific Accuracy Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `StructEval` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openreview.net/forum?id=buDwV7LUA7)<br>StructEval: Benchmarking LLMs' Capabilities to Generate Structural Outputs | TMLR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://tiger-ai-lab.github.io/StructEval/) | [![GitHub](https://img.shields.io/github/stars/TIGER-AI-Lab/StructEval)](https://github.com/TIGER-AI-Lab/StructEval) |
| `PlotCraft` | [![arXiv](https://img.shields.io/badge/arXiv-2511.00010-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.00010)<br>PlotCraft: Pushing the Limits of LLMs for Complex and Interactive Data Visualization | arXiv '25 | - | - |
| `TeXpert` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.sdp-1.2/)<br>TeXpert: Multi-Level Benchmark for LaTeX Code Generation | SDP '25 | - | - |
| `AbGen` | [![arXiv](https://img.shields.io/badge/arXiv-2507.13300-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2507.13300)<br>AbGen: Evaluating Large Language Models in Ablation Study Design and Evaluation for Scientific Research | ACL '25 | - | - |
| `SciFig` | [![arXiv](https://img.shields.io/badge/arXiv-2601.04390-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.04390)<br>SciFig: Towards Automating Scientific Figure Generation | arXiv '26 | - | - |
| `SciFlow-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2602.09809-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.09809)<br>SciFlow-Bench: Evaluating Structure-Aware Scientific Diagram Generation via Inverse Parsing | arXiv '26 | - | - |
| `FigureBench` | [![arXiv](https://img.shields.io/badge/arXiv-2602.03828-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.03828)<br>AutoFigure: Generating and Refining Publication-Ready Scientific Illustrations | ICLR '26 | - | [![GitHub](https://img.shields.io/github/stars/ResearAI/AutoFigure)](https://github.com/ResearAI/AutoFigure) |
||



# 5. Paper Writing

### Semi-Automated Writing Assistance

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `CoAuthor` | [![arXiv](https://img.shields.io/badge/arXiv-2201.06796-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2201.06796)<br>CoAuthor: Human-AI Collaborative Writing with Language Models | arXiv '22 | - | - |
| `AI Writing Study` | [![arXiv](https://img.shields.io/badge/arXiv-2506.20595-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.20595)<br>AI Writing Study | AIED '25 | - | - |
| `DraftMarks` | [![arXiv](https://img.shields.io/badge/arXiv-2509.23505-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.23505)<br>DraftMarks: Enhancing Transparency in Human-AI Co-Writing Through Interactive Skeuomorphic Process Traces | arXiv '25 | - | - |
| `PaperDebugger` | [![arXiv](https://img.shields.io/badge/arXiv-2512.02589-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.02589)<br>PaperDebugger: A Plugin-Based Multi-Agent System for In-Editor Academic Writing, Review, and Editing | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/PaperDebugger/PaperDebugger)](https://github.com/PaperDebugger/PaperDebugger) |
| `ScholarCopilot` | [![arXiv](https://img.shields.io/badge/arXiv-2504.00824-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.00824)<br>ScholarCopilot: Training LLMs for Academic Writing with Integrated Citation | arXiv '25 | - | - |
| `XtraGPT` | [![arXiv](https://img.shields.io/badge/arXiv-2505.11336-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.11336)<br>XtraGPT: Context-Aware and Controllable Academic Paper Revision | arXiv '25 | - | - |
| `LimAgents` | [![arXiv](https://img.shields.io/badge/arXiv-2601.11578-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.11578)<br>Multi-Agent LLMs for Generating Research Limitations | arXiv '26 | - | - |
| `PaperMentor` | [![arXiv](https://img.shields.io/badge/arXiv-2606.08857-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.08857)<br>PaperMentor: A Human-Centered Multi-Agent Writing Tutor for AI Research Papers on Overleaf | arXiv '26 | - | - |
||

### Fully Automated Paper Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `CycleResearcher` | [![arXiv](https://img.shields.io/badge/arXiv-2411.00816-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.00816)<br>CycleResearcher: Improving Automated Research via Automated Review | ICLR '25 | - | - |
| `Agent Laboratory` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.findings-emnlp.320/)<br>Agent Laboratory: Using LLM Agents as Research Assistants | EMNLP '25 | - | - |
| `FutureGen` | [![arXiv](https://img.shields.io/badge/arXiv-2503.16561-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.16561)<br>FutureGen: A RAG-based Approach to Generate the Future Work of Scientific Article | arXiv '25 | - | - |
| `AI Scientist` | [![arXiv](https://img.shields.io/badge/arXiv-2408.06292-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2408.06292)<br>The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery | Nature '26 | - | [![GitHub](https://img.shields.io/github/stars/SakanaAI/AI-Scientist)](https://github.com/SakanaAI/AI-Scientist) |
| `APRES` | [![arXiv](https://img.shields.io/badge/arXiv-2603.03142-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.03142)<br>APRES: An Agentic Paper Revision and Evaluation System | arXiv '26 | - | - |
| `LECTOR` | [![arXiv](https://img.shields.io/badge/arXiv-2605.25964-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.25964)<br>LECTOR: Joint Optimization of Scientific Reasoning Graphs and Introduction Generation | arXiv '26 | - | - |
| `RWGBench` | [![arXiv](https://img.shields.io/badge/arXiv-2606.24894-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.24894)<br>RWGBench: Evaluating Scholarly Positioning in Related Work Generation | arXiv '26 | - | - |
||

### Societal Analysis

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `AI Writing Adoption` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s41586-025-08681-8)<br>AI Writing Adoption | Nature '26 | - | - |
| `Nature AI Survey` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/d41586-025-04066-5)<br>More than Half of Researchers Now Use AI for Peer Review | Nature '26 | - | - |
| `Denial of Science` | [![arXiv](https://img.shields.io/badge/arXiv-2607.10712-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2607.10712)<br>Distributed Denial of Science: How Indirect Data Poisoning of AI Systems Can Industrialize Scientific Fraud | arXiv '26 | - | - |
| `AI Slop OSS` | [![arXiv](https://img.shields.io/badge/arXiv-2607.04003-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2607.04003)<br>"AI Slop is DDoSing Open Source": Understanding the Impact of AI-Generated Contributions on Open Source Sustainability | arXiv '26 | - | - |
||

### Writing Quality and AI Detection Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Mapping LLM Use` | [![arXiv](https://img.shields.io/badge/arXiv-2404.01268-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2404.01268)<br>Mapping the Increasing Use of LLMs in Scientific Papers | arXiv '24 | - | - |
| `CycleReviewer` | [![arXiv](https://img.shields.io/badge/arXiv-2411.00816-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.00816)<br>CycleResearcher: Improving Automated Research via Automated Review | ICLR '25 | - | - |
| `Stanford Agentic` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://paperreview.ai/tech-overview)<br>Stanford Agentic | Web '25 | - | - |
| `SciIG` | [![arXiv](https://img.shields.io/badge/arXiv-2508.14273-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.14273)<br>Let's Use ChatGPT To Write Our Paper! Benchmarking LLMs To Write the Introduction of a Research Paper | arXiv '25 | - | - |
| `Watermarking` | [![arXiv](https://img.shields.io/badge/arXiv-2503.15772-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.15772)<br>Detecting LLM-Generated Peer Reviews | arXiv '25 | - | - |
| `PaperWritingBench` | [![arXiv](https://img.shields.io/badge/arXiv-2604.05018-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.05018)<br>PaperOrchestra: A Multi-Agent Framework for Automated AI Research Paper Writing | arXiv '26 | - | - |
| `CiteTracer` | [![arXiv](https://img.shields.io/badge/arXiv-2605.08583-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.08583)<br>Source or It Didn't Happen: A Multi-Agent Framework for Citation Hallucination Detection | arXiv '26 | - | - |
| `Process Eval` | [![arXiv](https://img.shields.io/badge/arXiv-2606.15583-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.15583)<br>Process-Oriented Evaluation of AI-Assisted Scientific Writing | arXiv '26 | - | - |
||



# 6. Peer Review

### Automated Review Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ChatReviewer` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://github.com/nishiwen1214/ChatReviewer)<br>ChatReviewer: ChatGPT-based Paper Reviewing and Response Generation | GitHub '23 | - | [![GitHub](https://img.shields.io/github/stars/nishiwen1214/ChatReviewer)](https://github.com/nishiwen1214/ChatReviewer) |
| `AI-Peer-Review` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://github.com/poldrack/ai-peer-review)<br>AI-Peer-Review | GitHub '24 | - | [![GitHub](https://img.shields.io/github/stars/poldrack/ai-peer-review)](https://github.com/poldrack/ai-peer-review) |
| `MARG` | [![arXiv](https://img.shields.io/badge/arXiv-2401.04259-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2401.04259)<br>MARG: Multi-Agent Review Generation for Scientific Papers | arXiv '24 | - | - |
| `Reviewer2` | [![arXiv](https://img.shields.io/badge/arXiv-2402.10886-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.10886)<br>Reviewer2: Optimizing Review Generation Through Prompt Generation | arXiv '24 | - | - |
| `ReviewRL` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.emnlp-main.857/)<br>ReviewRL: Towards Automated Scientific Review with RL | EMNLP '25 | - | - |
| `DeepReviewer` | [![arXiv](https://img.shields.io/badge/arXiv-2503.08569-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.08569)<br>DeepReview: Improving LLM-based Paper Review with Human-like Deep Thinking Process | arXiv '25 | - | - |
| `OpenReviewer` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.naacl-demo.44/)<br>OpenReviewer: A Specialized Large Language Model for Generating Critical Scientific Paper Reviews | NAACL '25 | - | - |
| `REMOR` | [![arXiv](https://img.shields.io/badge/arXiv-2505.11718-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.11718)<br>REMOR: Automated Peer Review Generation with LLM Reasoning and Multi-Objective Reinforcement Learning | arXiv '25 | - | - |
| `ScholarPeer` | [![arXiv](https://img.shields.io/badge/arXiv-2601.22638-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.22638)<br>ScholarPeer: A Context-Aware Multi-Agent Framework for Automated Peer Review | arXiv '26 | - | - |
| `ProReviewer` | [![arXiv](https://img.shields.io/badge/arXiv-2606.13349-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.13349)<br>From Passive Generation to Investigation: A Proactive Scientific Peer Review Agent | arXiv '26 | - | - |
| `PeerCheck` | [![arXiv](https://img.shields.io/badge/arXiv-2606.20897-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.20897)<br>PeerCheck: Enhancing LLM-Generated Academic Reviews Towards Human-Level Quality | arXiv '26 | - | - |
||

### Meta-Review & Reviewer Matching

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `AgentReview` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2024.emnlp-main.70/)<br>AgentReview: Exploring Peer Review Dynamics with LLM Agents | EMNLP '24 | - | - |
| `Meta-Review LLMs` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.naacl-long.395/)<br>Meta-Review LLMs | NAACL '25 | - | - |
| `RATE` | [![arXiv](https://img.shields.io/badge/arXiv-2601.19637-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.19637)<br>RATE: Reviewer Profiling and Annotation-free Training for Expertise Ranking in Peer Review Systems | arXiv '26 | - | - |
| `MERIT` | [![arXiv](https://img.shields.io/badge/arXiv-2605.27865-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.27865)<br>MERIT: Matching Expertise via Rubric-Informed Training for Reviewer Assignment | arXiv '26 | - | - |
||

### Adversarial Attacks & Bias Analysis

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Raina etal` | [![arXiv](https://img.shields.io/badge/arXiv-2402.14016-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.14016)<br>Raina etal | EMNLP '24 | - | - |
| `AI Review Lottery` | [![arXiv](https://img.shields.io/badge/arXiv-2405.02150-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2405.02150)<br>The AI Review Lottery: Widespread AI-Assisted Peer Reviews Boost Paper Scores and Acceptance Rates | arXiv '24 | - | - |
| `Ye etal` | [![arXiv](https://img.shields.io/badge/arXiv-2412.01708-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.01708)<br>Ye etal | arXiv '24 | - | - |
| `Breaking the Reviewer` | [![arXiv](https://img.shields.io/badge/arXiv-2506.11113-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.11113)<br>Breaking the Reviewer: Assessing the Vulnerability of Large Language Models in Automated Peer Review Under Textual Adversarial Attacks | arXiv '25 | - | - |
| `LLM Reviewer Bias` | [![arXiv](https://img.shields.io/badge/arXiv-2509.09912-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.09912)<br>LLM Reviewer Bias | arXiv '25 | - | - |
| `Prompt Injection` | [![arXiv](https://img.shields.io/badge/arXiv-2509.10248-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.10248)<br>Prompt Injection Attacks on LLM Generated Reviews of Scientific Publications | arXiv '25 | - | - |
| `Sahoo etal` | [![arXiv](https://img.shields.io/badge/arXiv-2512.10449-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.10449)<br>Sahoo etal | arXiv '25 | - | - |
| `Zhou etal` | [![arXiv](https://img.shields.io/badge/arXiv-2511.01287-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.01287)<br>Zhou etal | arXiv '25 | - | - |
| `Presentation Gaming` | [![arXiv](https://img.shields.io/badge/arXiv-2606.13044-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.13044)<br>No Hidden Prompts Needed! You Can Game AI Peer Review with Presentation-Only Revisions | arXiv '26 | - | - |
| `LLMs Favor LLMs?` | [![arXiv](https://img.shields.io/badge/arXiv-2601.20920-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.20920)<br>Do LLMs Favor LLMs? Quantifying Interaction Effects in Peer Review | arXiv '26 | - | - |
| `Gaming AI Reviews` | [![arXiv](https://img.shields.io/badge/arXiv-2606.10159-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.10159)<br>Gaming AI-Assisted Peer Reviews Poses New Risks to the Scientific Community | arXiv '26 | - | - |
| `Phantom Refs` | [![arXiv](https://img.shields.io/badge/arXiv-2607.00738-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2607.00738)<br>Phantom References: Hallucinated Citations That Survive Peer Review at Top-Tier Conferences | arXiv '26 | - | - |
||

### Detection & Policy

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `AI Detection` | [![arXiv](https://img.shields.io/badge/arXiv-2502.19614-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.19614)<br>Is Your Paper Being Reviewed by an LLM? Benchmarking AI Text Detection in Peer Review | arXiv '25 | - | - |
| `AI Use Rejects` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/d41586-026-00893-2)<br>Major Conference Catches Illicit AI Use — and Rejects Hundreds of Papers | Nature '26 | - | - |
| `Nature AI Survey` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/d41586-025-04066-5)<br>More than Half of Researchers Now Use AI for Peer Review | Nature '26 | - | - |
| `Policy Enforcement` | [![arXiv](https://img.shields.io/badge/arXiv-2603.20450-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.20450)<br>Policy Enforcement | arXiv '26 | - | - |
| `Reviewer Feedback` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://doi.org/10.1145/3772318.3791431)<br>What Happens When Reviewers Receive AI Feedback in Their Reviews? | CHI '26 | - | - |
| `AAAI-26 Pilot` | [![arXiv](https://img.shields.io/badge/arXiv-2604.13940-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.13940)<br>AI-Assisted Peer Review at Scale: The AAAI-26 AI Review Pilot | arXiv '26 | - | - |
||

### Review Consistency and Bias Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Review Survey` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.sciencedirect.com/science/article/pii/S1566253525004051)<br>More than Half of Researchers Now Use AI for Peer Review — often Against Guidance | IF '25 | - | - |
| `Stanford Agentic` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://paperreview.ai/tech-overview)<br>Stanford Agentic | Web '25 | - | - |
| `ClaimCheck` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.findings-emnlp.1185/)<br>ClaimCheck: How Grounded are LLM Critiques of Scientific Papers? | EMNLP '25 | - | - |
| `REFUTE` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://huggingface.co/datasets/BGPT-OFFICIAL/refute/blob/main/TECHNICAL_REPORT.md)<br>REFUTE: A Benchmark for Scientific Critique and Epistemic Calibration in Language Models | HF '26 | [Website](https://huggingface.co/datasets/BGPT-OFFICIAL/refute) | - |
| `ReViewGraph` | [![arXiv](https://img.shields.io/badge/arXiv-2511.08317-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.08317)<br>Automatic Paper Reviewing with Heterogeneous Graph Reasoning over LLM-Simulated Reviewer-Author Debates | AAAI '26 | - | - |
| `ReviewAgents` | [![arXiv](https://img.shields.io/badge/arXiv-2503.08506-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.08506)<br>ReviewAgents: Bridging the Gap Between Human and AI-Generated Paper Reviews | arXiv '25 | - | - |
| `ICLR 2025 Study` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s42256-026-01188-x)<br>ICLR 2025 Study | NMI '26 | - | - |
| `AI Reviewer Limits` | [![arXiv](https://img.shields.io/badge/arXiv-2605.20668-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.20668)<br>On the limits and opportunities of AI reviewers: Reviewing the reviews of Nature-family papers with 45 expert scientists | arXiv '26 | - | - |
| `PRISM` | [![arXiv](https://img.shields.io/badge/arXiv-2605.26730-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.26730)<br>PRISM: A Multi-Dimensional Benchmark for Evaluating LLM Peer Reviewers | arXiv '26 | - | - |
||



# 7. Rebuttal

### Reviewer Comment Analysis

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ReviewMT` | [![arXiv](https://img.shields.io/badge/arXiv-2406.05688-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2406.05688)<br>Peer Review as A Multi-Turn and Long-Context Dialogue with Role-Based Interactions | arXiv '24 | - | - |
| `ICLR Rebuttal Study` | [![arXiv](https://img.shields.io/badge/arXiv-2511.15462-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.15462)<br>ICLR Rebuttal Study | arXiv '25 | - | - |
| `RbtAct` | [![arXiv](https://img.shields.io/badge/arXiv-2603.09723-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.09723)<br>RbtAct: Rebuttal as Supervision for Actionable Review Feedback Generation | arXiv '26 | - | - |
| `GoodPoint` | [![arXiv](https://img.shields.io/badge/arXiv-2604.11924-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.11924)<br>GoodPoint: Learning Constructive Scientific Paper Feedback from Author Responses | arXiv '26 | - | - |
||

### Automated Rebuttal Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ReviewerToo` | [![arXiv](https://img.shields.io/badge/arXiv-2510.08867-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.08867)<br>ReviewerToo: Should AI Join The Program Committee? A Look At The Future of Peer Review | arXiv '25 | - | - |
| `RebuttalAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2601.15715-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.15715)<br>RebuttalAgent: Strategic Persuasion in Academic Rebuttal via Theory of Mind | ICLR '26 | - | [![GitHub](https://img.shields.io/github/stars/Zhitao-He/RebuttalAgent)](https://github.com/Zhitao-He/RebuttalAgent) |
| `Author-in-the-Loop` | [![arXiv](https://img.shields.io/badge/arXiv-2602.11173-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.11173)<br>Author-in-the-Loop Response Generation and Evaluation: Integrating Author Expertise and Intent in Responses to Peer Review | ACL '26 | - | - |
| `DRPG` | [![arXiv](https://img.shields.io/badge/arXiv-2601.18081-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.18081)<br>DRPG: An Agentic Framework for Academic Rebuttal | arXiv '26 | - | [![GitHub](https://img.shields.io/github/stars/ulab-uiuc/DRPG-RebuttalAgent)](https://github.com/ulab-uiuc/DRPG-RebuttalAgent) |
| `Paper2Rebuttal` | [![arXiv](https://img.shields.io/badge/arXiv-2601.14171-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.14171)<br>Paper2Rebuttal: A Multi-Agent Framework for Transparent Author Response Assistance | arXiv '26 | - | - |
| `Defend` | [![arXiv](https://img.shields.io/badge/arXiv-2603.27360-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.27360)<br>Defend: Automated Rebuttals for Peer Review with Minimal Author Guidance | arXiv '26 | - | - |
||

### Rebuttal Effectiveness Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Re$^2$` | [![arXiv](https://img.shields.io/badge/arXiv-2505.07920-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.07920)<br>Re$^2$ | arXiv '25 | - | - |
| `Commitment Checklist` | [![arXiv](https://img.shields.io/badge/arXiv-2603.00003-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.00003)<br>Commitment Checklist: Auditing Author Commitments in Peer Review | arXiv '26 | - | - |
| `Re$^3$Align` | [![arXiv](https://img.shields.io/badge/arXiv-2602.11173-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.11173)<br>Re$^3$Align | ACL '26 | - | - |
| `Rebuttals Move` | [![arXiv](https://img.shields.io/badge/arXiv-2606.22166-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.22166)<br>Rebuttals Move Peer-Review Scores, but Initial-Review Structure Bounds the Movement | arXiv '26 | - | - |
| `Trust AI Reviews` | [![arXiv](https://img.shields.io/badge/arXiv-2605.16623-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.16623)<br>To Trust or Not to Trust: Authors' Response to AI-based Reviews | arXiv '26 | - | - |
||



# 8. Dissemination (Paper2X)

### Paper2Poster

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `P2P` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openreview.net/forum?id=JojyT9niJL)<br>P2P: Automated Paper-to-Poster Generation and Fine-Grained Benchmark | ICLR '26 | - | - |
| `Paper2Poster` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openreview.net/forum?id=p0E74lpRBD)<br>Paper2Poster: Towards Multimodal Poster Automation from Scientific Papers | NeurIPS '25 | - | [![GitHub](https://img.shields.io/github/stars/Paper2Poster/Paper2Poster)](https://github.com/Paper2Poster/Paper2Poster) |
| `PosterForest` | [![arXiv](https://img.shields.io/badge/arXiv-2508.21720-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.21720)<br>PosterForest: Hierarchical Multi-Agent Collaboration for Scientific Poster Generation | arXiv '25 | - | - |
| `PosterGen` | [![arXiv](https://img.shields.io/badge/arXiv-2508.17188-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.17188)<br>PosterGen: Aesthetic-Aware Paper-to-Poster Generation via Multi-Agent LLMs | arXiv '25 | - | - |
| `APEX` | [![arXiv](https://img.shields.io/badge/arXiv-2601.04794-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.04794)<br>APEX: Academic Poster Editing Agentic Expert | arXiv '26 | - | [![GitHub](https://img.shields.io/github/stars/Breesiu/APEX)](https://github.com/Breesiu/APEX) |
| `PosterOmni` | [![arXiv](https://img.shields.io/badge/arXiv-2602.12127-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.12127)<br>PosterOmni: Generalized Artistic Poster Creation via Task Distillation and Unified Reward Feedback | arXiv '26 | - | - |
| `Any2Poster` | [![arXiv](https://img.shields.io/badge/arXiv-2606.02915-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.02915)<br>Any2Poster: Any-Source Poster Generation Across Modalities and Domains | arXiv '26 | - | - |
||

### Paper2Slides

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `DOC2PPT` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://ojs.aaai.org/index.php/AAAI/article/view/19943)<br>DOC2PPT: Automatic Presentation Slides Generation from Scientific Documents | AAAI '22 | - | - |
| `PPTAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2501.03936-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.03936)<br>PPTAgent: Generating and Evaluating Presentations Beyond Text-to-Slides | EMNLP '25 | - | [![GitHub](https://img.shields.io/github/stars/icip-cas/PPTAgent)](https://github.com/icip-cas/PPTAgent) |
| `AutoPresent` | [![arXiv](https://img.shields.io/badge/arXiv-2501.00912-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.00912)<br>AutoPresent: Designing Structured Visuals from Scratch | CVPR '25 | - | - |
| `Paper2Slides` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://github.com/HKUDS/Paper2Slides)<br>Paper2Slides: From Paper to Presentation in One Click | GitHub '25 | - | [![GitHub](https://img.shields.io/github/stars/HKUDS/Paper2Slides)](https://github.com/HKUDS/Paper2Slides) |
| `Auto-Slides` | [![arXiv](https://img.shields.io/badge/arXiv-2509.11062-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.11062)<br>Auto-Slides: An Interactive Multi-Agent System for Creating and Customizing Research Presentations | arXiv '25 | - | - |
| `PASS` | [![arXiv](https://img.shields.io/badge/arXiv-2501.06497-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.06497)<br>PASS: Presentation Automation for Slide Generation and Speech | arXiv '25 | - | - |
| `SlideGen` | [![arXiv](https://img.shields.io/badge/arXiv-2512.04529-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.04529)<br>SlideGen: Collaborative Multimodal Agents for Scientific Slide Generation | arXiv '25 | - | - |
| `Talk to Your Slides` | [![arXiv](https://img.shields.io/badge/arXiv-2505.11604-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.11604)<br>Talk to Your Slides: Efficient Slide Editing Agent | arXiv '25 | - | - |
| `SlideTailor` | [![arXiv](https://img.shields.io/badge/arXiv-2512.20292-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.20292)<br>SlideTailor: Personalized Presentation Slide Generation for Scientific Papers | AAAI '26 | - | [![GitHub](https://img.shields.io/github/stars/nusnlp/SlideTailor)](https://github.com/nusnlp/SlideTailor) |
| `DeepPresenter` | [![arXiv](https://img.shields.io/badge/arXiv-2602.22839-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.22839)<br>DeepPresenter: Environment-Grounded Reflection for Agentic Presentation Generation | arXiv '26 | - | [![GitHub](https://img.shields.io/github/stars/icip-cas/PPTAgent)](https://github.com/icip-cas/PPTAgent) |
| `Office Raccoon` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.sensetime.com/en/news-detail/51170569)<br>Office Raccoon | Web '26 | - | - |
| `X+Slides` | [![arXiv](https://img.shields.io/badge/arXiv-2606.19256-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.19256)<br>X+Slides: Benchmarking Audience-Conditioned Slide Generation | arXiv '26 | - | - |
||

### Paper2Video

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Preacher` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://github.com/Gen-Verse/Paper2Video)<br>Preacher: Paper-to-Video Agentic System | ICCV '25 | - | [![GitHub](https://img.shields.io/github/stars/Gen-Verse/Paper2Video)](https://github.com/Gen-Verse/Paper2Video) |
| `Paper2Video` | [![arXiv](https://img.shields.io/badge/arXiv-2510.05096-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.05096)<br>Paper2Video: Automatic Video Generation from Scientific Papers | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/showlab/Paper2Video)](https://github.com/showlab/Paper2Video) |
| `PresentAgent` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.emnlp-demos.58/)<br>PresentAgent: Multimodal Agent for Presentation Video Generation | EMNLP '25 | - | [![GitHub](https://img.shields.io/github/stars/AIGeeksGroup/PresentAgent)](https://github.com/AIGeeksGroup/PresentAgent) |
| `PresentAgent-2` | [![arXiv](https://img.shields.io/badge/arXiv-2605.11363-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.11363)<br>PresentAgent-2: Towards Generalist Multimodal Presentation Agents | arXiv '26 | - | - |
| `Paper2Video Talks` | [![arXiv](https://img.shields.io/badge/arXiv-2606.28531-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.28531)<br>A Good Talk Does not Look Like a Summary, It Teaches You! Measuring Takeaways from Paper-to-Video Talks | arXiv '26 | - | - |
||

### Paper2Web & Social Media

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Paper2Web` | [![arXiv](https://img.shields.io/badge/arXiv-2510.15842-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.15842)<br>Paper2Web: Let's Make Your Paper Alive! | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/YuhangChen1/Paper2All)](https://github.com/YuhangChen1/Paper2All) |
| `ResearchStudio-Reel` | [![arXiv](https://img.shields.io/badge/arXiv-2607.04438-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2607.04438)<br>ResearchStudio-Reel: Automate the Last Mile of Research from Paper to Poster, Video, and Blog | arXiv '26 | - | - |
| `I-WebGenBench` | [![arXiv](https://img.shields.io/badge/arXiv-2606.00750-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.00750)<br>I-WebGenBench: Evaluating Interactivity in LLM-Generated Scientific Web Applications | arXiv '26 | - | - |
||

### Fidelity and Adoption Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `PPTEval` | [![arXiv](https://img.shields.io/badge/arXiv-2501.03936-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.03936)<br>PPTAgent: Generating and Evaluating Presentations Beyond Text-to-Slides | EMNLP '25 | - | [![GitHub](https://img.shields.io/github/stars/icip-cas/PPTAgent)](https://github.com/icip-cas/PPTAgent) |
| `PresentQuiz` | [![arXiv](https://img.shields.io/badge/arXiv-2510.05096-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.05096)<br>Paper2Video: Automatic Video Generation from Scientific Papers | arXiv '25 | - | [![GitHub](https://img.shields.io/github/stars/showlab/Paper2Video)](https://github.com/showlab/Paper2Video) |
| `PresentEval` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.emnlp-demos.58/)<br>PresentAgent: Multimodal Agent for Presentation Video Generation | EMNLP '25 | - | [![GitHub](https://img.shields.io/github/stars/AIGeeksGroup/PresentAgent)](https://github.com/AIGeeksGroup/PresentAgent) |
| `Sci. Comm. Correspondence` | [![arXiv](https://img.shields.io/badge/arXiv-2605.05831-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.05831)<br>Unifying Scientific Communication: Fine-Grained Correspondence Across Scientific Media | arXiv '26 | - | - |
||





# 9. End-to-End Systems

### Fully Automated Research Systems

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ResearchTown` | [![arXiv](https://img.shields.io/badge/arXiv-2500.00000-b31b1b?style=flat-square&logo=arxiv)](https://proceedings.mlr.press/v267/yu25a.html)<br>ResearchTown: Simulator of Human Research Community | ICML 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://proceedings.mlr.press/v267/yu25a.html) | [![GitHub](https://img.shields.io/github/stars/ulab-uiuc/research-town)](https://github.com/ulab-uiuc/research-town) |
| `Agent Laboratory` | [![arXiv](https://img.shields.io/badge/arXiv-2501.04227-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.04227)<br>Agent Laboratory: Using LLM Agents as Research Assistants | arXiv 2025 | - | - |
| `AgentRxiv` | [![arXiv](https://img.shields.io/badge/arXiv-2503.18102-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.18102)<br>AgentRxiv: Towards Collaborative Autonomous Research | arXiv 2025 | - | - |
| `ARIS` | - | GitHub 2025 | - | [![GitHub](https://img.shields.io/github/stars/wanshuiyin/Auto-claude-code-research-in-sleep)](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep) |
| `freephdlabor` | [![arXiv](https://img.shields.io/badge/arXiv-2510.15624-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.15624)<br>Build Your Personalized Research Group: A Multiagent Framework for Continual and Interactive Science Automation | arXiv 2025 | - | - |
| `SciMaster` | [![arXiv](https://img.shields.io/badge/arXiv-2507.05241-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2507.05241)<br>SciMaster: Towards General-Purpose Scientific AI Agents | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/sjtu-sai-agents/X-Master)](https://github.com/sjtu-sai-agents/X-Master) |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s41586-026-08420-7)<br>Towards End-to-End Automation of AI Research | Nature 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s41586-026-08420-7) | [![GitHub](https://img.shields.io/github/stars/SakanaAI/AI-Scientist)](https://github.com/SakanaAI/AI-Scientist) |
| `Idea2Story` | [![arXiv](https://img.shields.io/badge/arXiv-2601.20833-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.20833)<br>Idea2Story: An Automated Pipeline for Transforming Research Concepts into Complete Scientific Narratives | arXiv 2026 | - | - |
| `UniScientist` | - | Web 2026 | - | - |
| `ASI-Evolve` | - | GitHub 2026 | - | [![GitHub](https://img.shields.io/github/stars/GAIR-NLP/ASI-Evolve)](https://github.com/GAIR-NLP/ASI-Evolve) |
| `FARS` | - | Web 2026 | - | - |
| `AutoResearchClaw` | - | GitHub 2026 | - | [![GitHub](https://img.shields.io/github/stars/aiming-lab/AutoResearchClaw)](https://github.com/aiming-lab/AutoResearchClaw) |
| `CORAL` | [![arXiv](https://img.shields.io/badge/arXiv-2604.01658-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.01658)<br>CORAL: Towards Autonomous Multi-Agent Evolution for Open-Ended Discovery | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/Human-Agent-Society/CORAL)](https://github.com/Human-Agent-Society/CORAL) |
| `AutoSOTA` | [![arXiv](https://img.shields.io/badge/arXiv-2604.05550-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.05550)<br>AutoSOTA: An End-to-End Automated Research System for State-of-the-Art AI Model Discovery | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/tsinghua-fib-lab/AutoSOTA)](https://github.com/tsinghua-fib-lab/AutoSOTA) |
| `AiScientist-LH` | [![arXiv](https://img.shields.io/badge/arXiv-2604.13018-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.13018)<br>Toward Autonomous Long-Horizon Engineering for ML Research | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/AweAI-Team/AiScientist)](https://github.com/AweAI-Team/AiScientist) |
| `OpenResearcher (2026)` | [![arXiv](https://img.shields.io/badge/arXiv-2603.20278-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.20278)<br>OpenResearcher: A Fully Open Pipeline for Long-Horizon Deep Research Trajectory Synthesis | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/TIGER-AI-Lab/OpenResearcher)](https://github.com/TIGER-AI-Lab/OpenResearcher) |
| `Aletheia` | [![arXiv](https://img.shields.io/badge/arXiv-2602.10177-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.10177)<br>Towards Autonomous Mathematics Research | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/google-deepmind/superhuman)](https://github.com/google-deepmind/superhuman) |
| `AutoSci` | [![arXiv](https://img.shields.io/badge/arXiv-2605.31468-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.31468)<br>AutoSci: A Memory-Centric Agentic System for the Full Scientific Research Lifecycle | arXiv 2026 | - | - |
| `ScientistOne` | [![arXiv](https://img.shields.io/badge/arXiv-2605.26340-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.26340)<br>ScientistOne: Towards Human-Level Autonomous Research via Chain-of-Evidence | arXiv 2026 | - | - |
| `Arbor` | [![arXiv](https://img.shields.io/badge/arXiv-2606.11926-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.11926)<br>Toward Generalist Autonomous Research via Hypothesis-Tree Refinement | arXiv 2026 | - | - |
| `Agon` | [![arXiv](https://img.shields.io/badge/arXiv-2606.24177-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.24177)<br>Agon: An Autonomous Large-Scale Omnidisciplinary Research System Built on Prompt Economy | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/AutoResearch-Factory/Agon)](https://github.com/AutoResearch-Factory/Agon) |
| `ResearchClawBench` | [![arXiv](https://img.shields.io/badge/arXiv-2606.07591-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.07591)<br>ResearchClawBench: A Benchmark for End-to-End Autonomous Scientific Research | arXiv 2026 | - | - |
| `Act as Real Researcher` | [![arXiv](https://img.shields.io/badge/arXiv-2606.07462-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.07462)<br>Act As a Real Researcher: A Suite of Benchmarks Evaluating Frontier LLMs and Agentic Harnesses in Research Lifecycle | arXiv 2026 | - | - |
| `ResearchArena` | [![arXiv](https://img.shields.io/badge/arXiv-2605.19156-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.19156)<br>How Far Are We From True Auto-Research? | arXiv 2026 | - | - |
| `NVAITC AI Sci.` | [![arXiv](https://img.shields.io/badge/arXiv-2607.11084-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2607.11084)<br>NVAITC AI Scientist: A Governed End-to-End Research System -- A Hypertension GWAS Case Study | arXiv '26 | - | - |
||

### Domain-Specific Systems

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `AlphaFold 3` | [![arXiv](https://img.shields.io/badge/arXiv-2400.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s41586-024-07487-w)<br>Accurate Structure Prediction of Biomolecular Interactions with AlphaFold 3 | Nature 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s41586-024-07487-w) | - |
| `Medical AI Scientist` | [![arXiv](https://img.shields.io/badge/arXiv-2603.28589-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.28589)<br>Towards a Medical AI Scientist | arXiv 2026 | - | - |
| `Cognitive Scientist` | [![arXiv](https://img.shields.io/badge/arXiv-2606.26448-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.26448)<br>Closing the Loop to Discover Psychological Theories with an Automated Cognitive Scientist | arXiv '26 | - | - |
| `Molecular Closed-Loop` | [![arXiv](https://img.shields.io/badge/arXiv-2606.22731-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.22731)<br>Closed-loop Auto Research for Molecular Property Prediction: Discovering and Certifying Generalizable Improvements | arXiv '26 | - | - |
||

### Evolutionary & Self-Improving Systems

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ShinkaEvolve` | [![arXiv](https://img.shields.io/badge/arXiv-2509.19349-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.19349)<br>ShinkaEvolve: Towards Open-Ended and Sample-Efficient Program Evolution | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/SakanaAI/ShinkaEvolve)](https://github.com/SakanaAI/ShinkaEvolve) |
| `Darwin Godel Machine` | [![arXiv](https://img.shields.io/badge/arXiv-2505.22954-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.22954)<br>Darwin Godel Machine: Open-Ended Evolution of Self-Improving Agents | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/jennyzzt/dgm)](https://github.com/jennyzzt/dgm) |
| `EvoMaster` | [![arXiv](https://img.shields.io/badge/arXiv-2604.17406-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.17406)<br>EvoMaster: A Foundational Evolving Agent Framework for Agentic Science at Scale | arXiv 2026 | - | - |
| `Self-Driving Lab` | [![arXiv](https://img.shields.io/badge/arXiv-2607.04508-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2607.04508)<br>Compressing the Validation Bottleneck: An Agentic Self-Driving Lab for Scientific Discovery | arXiv '26 | - | - |
| `Meta-Reflection` | [![arXiv](https://img.shields.io/badge/arXiv-2607.01131-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2607.01131)<br>Autonomous Scientific Discovery via Iterative Meta-Reflection | arXiv '26 | - | - |
||

### Research Platforms & Infrastructure

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Towards an AI co-scientist` | [![arXiv](https://img.shields.io/badge/arXiv-2502.18864-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.18864)<br>Towards an AI co-scientist | arXiv 2025 | - | - |
| `PiFlow` | [![arXiv](https://img.shields.io/badge/arXiv-2505.15047-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.15047)<br>PiFlow: Principle-aware Scientific Discovery with Multi-Agent Collaboration | arXiv 2025 | - | - |
| `LabClaw` | - | Web 2026 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.technologyreview.com/2026/03/20/1134438/openai-is-throwing-everything-into-building-a-fully-automated-researcher)<br>OpenAI Is Throwing Everything into Building a Fully Automated Researcher | MIT TR 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.technologyreview.com/2026/03/20/1134438/openai-is-throwing-everything-into-building-a-fully-automated-researcher) | - |
||


# 10. Societal & Critical Perspectives

> :timer_clock: In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| - | [![arXiv](https://img.shields.io/badge/arXiv-2500.00000-b31b1b?style=flat-square&logo=arxiv)](https://pubsonline.informs.org/doi/10.1287/orsc.2023.1745)<br>Navigating the Jagged Technological Frontier | Org. Sci. 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://pubsonline.informs.org/doi/10.1287/orsc.2023.1745) | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2500.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.sciencedirect.com/science/article/pii/S2590291124003139)<br>Reassessing Academic Integrity in the Age of AI | SSH Open 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.sciencedirect.com/science/article/pii/S2590291124003139) | - |
| `The AI Deskilling Paradox` | [![arXiv](https://img.shields.io/badge/arXiv-2500.00000-b31b1b?style=flat-square&logo=arxiv)](https://cacm.acm.org/opinion/the-ai-deskilling-paradox/)<br>The AI Deskilling Paradox | CACM 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://cacm.acm.org/opinion/the-ai-deskilling-paradox/) | - |
| `Hidden Pitfalls of AI Scientist Systems` | [![arXiv](https://img.shields.io/badge/arXiv-2509.08713-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.08713)<br>The More You Automate, the Less You See: Hidden Pitfalls of AI Scientist Systems | arXiv 2025 | - | - |
| `Rethinking Science in the Age of AI` | [![arXiv](https://img.shields.io/badge/arXiv-2511.10524-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.10524)<br>Rethinking Science in the Age of Artificial Intelligence | arXiv 2025 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2500.00000-b31b1b?style=flat-square&logo=arxiv)](https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks/)<br>Measuring AI Ability to Complete Long Tasks | METR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks/) | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2512.08296-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.08296)<br>Towards a Science of Scaling Agent Systems | arXiv 2025 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s41586-025-08681-8)<br>Artificial Intelligence Tools Expand Scientists' Impact but Contract Science's Focus | Nature 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s41586-025-08681-8) | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.cell.com/patterns/fulltext/S2666-3899(25)<br>AI for Scientific Discovery is a Social Problem | Patterns 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.cell.com/patterns/fulltext/S2666-3899(25) | - |
| `Research Integrity in the Age of AI` | [![arXiv](https://img.shields.io/badge/arXiv-2601.05574-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.05574)<br>Research Integrity and Academic Authority in the Age of Artificial Intelligence: From Discovery to Curation? | arXiv 2026 | - | - |
| `SciSciGPT` | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s43588-026-00784-z)<br>SciSciGPT: Advancing Human-AI Collaboration in the Science of Science | Nature CS 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s43588-026-00784-z) | - |
| `SimStep` | [![arXiv](https://img.shields.io/badge/arXiv-2507.09664-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2507.09664)<br>SimStep: Chain-of-Abstractions for Incremental Specification and Debugging of AI-Generated Interactive Simulations | arXiv 2025 | - | - |
| `ConvoLearn` | [![arXiv](https://img.shields.io/badge/arXiv-2601.08950-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.08950)<br>ConvoLearn: A Learning Sciences Grounded Dataset for Fine-Tuning Dialogic AI Tutors | arXiv 2026 | - | - |
| `AFIM: Academic Fraud Inclination Metric` | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.alexalemi.com/arxiv-metric/docs.html)<br>AFIM: Academic Fraud Inclination Metric | Web 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.alexalemi.com/arxiv-metric/docs.html) | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2603.03338-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.03338)<br>AI Researchers' Views on Automating AI R\&D and Intelligence Explosions | arXiv 2026 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/d41586-026-01551-x)<br>AI Scientists Are Changing Research | Nature 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/d41586-026-01551-x) | - |
| `Learning by Creating (Talk)` | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.youtube.com/watch?v=iOyaj5u0-DY)<br>Learning by Creating: A Human-Centered Vision for AI in Education | Talk 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.youtube.com/watch?v=iOyaj5u0-DY) | - |
| `AI Sci. No Reasoning` | [![arXiv](https://img.shields.io/badge/arXiv-2604.18805-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.18805)<br>AI scientists produce results without reasoning scientifically | arXiv 2026 | - | - |
| `Not Built for Autonomy` | [![arXiv](https://img.shields.io/badge/arXiv-2605.08956-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.08956)<br>Agentic AI Scientists Are Not Built For Autonomous Scientific Discovery | arXiv 2026 | - | - |
| `Workflow != Closure` | [![arXiv](https://img.shields.io/badge/arXiv-2605.26200-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.26200)<br>Workflow Closure Is Not Scientific Closure in Auto-Research Systems | arXiv 2026 | - | - |
| `PseudoBench` | [![arXiv](https://img.shields.io/badge/arXiv-2606.18060-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2606.18060)<br>PseudoBench: Measuring How Agentic Auto-Research Fuels Pseudoscience | arXiv 2026 | - | - |
| `SciIntegrity-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2605.10246-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2605.10246)<br>SciIntegrity-Bench: A Benchmark for Evaluating Academic Integrity in AI Scientist Systems | arXiv 2026 | - | - |
||



# 11. Surveys & Curated Lists

> :timer_clock: In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `LLM4SR` | [![arXiv](https://img.shields.io/badge/arXiv-2501.04306-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.04306)<br>LLM4SR: A Survey on Large Language Models for Scientific Research | arXiv 2025 | - | - |
| `From Automation to Autonomy` | [![arXiv](https://img.shields.io/badge/arXiv-2505.13259-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.13259)<br>From Automation to Autonomy: A Survey on Large Language Models for Scientific Discovery | arXiv 2025 | - | - |
| `AI4Research` | [![arXiv](https://img.shields.io/badge/arXiv-2507.01903-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2507.01903)<br>AI4Research: A Survey of Artificial Intelligence for Scientific Research | arXiv 2025 | - | - |
| `A Survey of AI Scientists` | [![arXiv](https://img.shields.io/badge/arXiv-2510.23045-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.23045)<br>A Survey of AI Scientists | arXiv 2025 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2511.07448-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.07448)<br>Large Language Models for Scientific Idea Generation: A Creativity-Centered Survey | arXiv 2025 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2500.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.sciencedirect.com/science/article/pii/S1566253524005803)<br>Large Language Models for Automated Scholarly Paper Review: A Survey | Inf. Fusion 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.sciencedirect.com/science/article/pii/S1566253524005803) | - |
| `AutoResearch Survey` | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://haizhaoyang.github.io/research/autoresearch-survey.html)<br>What's Missing in Autonomous Research? A Systematization of Systems, Benchmarks, and Verification | Web 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://haizhaoyang.github.io/research/autoresearch-survey.html) | - |
||



# 12. Tools & GitHub Repos

> Open-source tools, frameworks, and curated resource lists for AI-assisted research (not directly tied to a single paper).


### Curated Lists

| Repository | Stars | Description |
|-----------|-------|-------------|
| [Awesome-Deep-Research](https://github.com/DavidZWZ/Awesome-Deep-Research) | [![GitHub](https://img.shields.io/github/stars/DavidZWZ/Awesome-Deep-Research)](https://github.com/DavidZWZ/Awesome-Deep-Research) | Up-to-date collection of agentic deep research resources |
| [Awesome-Scientific-Language-Models](https://github.com/yuzhimanhua/Awesome-Scientific-Language-Models) | [![GitHub](https://img.shields.io/github/stars/yuzhimanhua/Awesome-Scientific-Language-Models)](https://github.com/yuzhimanhua/Awesome-Scientific-Language-Models) | Survey of scientific LLMs (EMNLP'24) |
| [Awesome-LLM-Scientific-Discovery](https://github.com/HKUST-KnowComp/Awesome-LLM-Scientific-Discovery) | [![GitHub](https://img.shields.io/github/stars/HKUST-KnowComp/Awesome-LLM-Scientific-Discovery)](https://github.com/HKUST-KnowComp/Awesome-LLM-Scientific-Discovery) | Three-level autonomy framework (EMNLP'25) |
| [Awesome-AI-Scientist-Papers](https://github.com/openags/Awesome-AI-Scientist-Papers) | [![GitHub](https://img.shields.io/github/stars/openags/Awesome-AI-Scientist-Papers)](https://github.com/openags/Awesome-AI-Scientist-Papers) | Resources on AI Scientist systems |
| [Awesome-Auto-Research-Tools](https://github.com/handsome-rich/Awesome-Auto-Research-Tools) | [![GitHub](https://img.shields.io/github/stars/handsome-rich/Awesome-Auto-Research-Tools)](https://github.com/handsome-rich/Awesome-Auto-Research-Tools) | Automated research tools catalog |
| [awesome-autoresearch](https://github.com/alvinunreal/awesome-autoresearch) | [![GitHub](https://img.shields.io/github/stars/alvinunreal/awesome-autoresearch)](https://github.com/alvinunreal/awesome-autoresearch) | Autonomous improvement loops and research agents |
| [awesome-ai-research-writing](https://github.com/Leey21/awesome-ai-research-writing) | [![GitHub](https://img.shields.io/github/stars/Leey21/awesome-ai-research-writing)](https://github.com/Leey21/awesome-ai-research-writing) | Prompt templates and agent skills for AI-assisted writing |


### Idea Generation

| Repository | Stars | Description |
|-----------|-------|-------------|
| [Virtual-Scientists](https://github.com/RenqiChen/Virtual-Scientists) | [![GitHub](https://img.shields.io/github/stars/RenqiChen/Virtual-Scientists)](https://github.com/RenqiChen/Virtual-Scientists) | VirSci: multi-agent collaborative idea generation (ACL'25) |
| [ResearchAgent](https://github.com/JinheonBaek/ResearchAgent) | [![GitHub](https://img.shields.io/github/stars/JinheonBaek/ResearchAgent)](https://github.com/JinheonBaek/ResearchAgent) | Iterative idea proposal with reviewing agents |


### Literature Review

| Repository | Stars | Description |
|-----------|-------|-------------|
| [paper-qa](https://github.com/Future-House/paper-qa) | [![GitHub](https://img.shields.io/github/stars/Future-House/paper-qa)](https://github.com/Future-House/paper-qa) | PaperQA2: superhuman RAG for scientific Q&A |
| [local-deep-research](https://github.com/LearningCircuit/local-deep-research) | [![GitHub](https://img.shields.io/github/stars/LearningCircuit/local-deep-research)](https://github.com/LearningCircuit/local-deep-research) | Fully local deep research |
| [researchgpt](https://github.com/mukulpatnaik/researchgpt) | [![GitHub](https://img.shields.io/github/stars/mukulpatnaik/researchgpt)](https://github.com/mukulpatnaik/researchgpt) | Conversational interaction with research papers |
| [gpt-researcher](https://github.com/assafelovic/gpt-researcher) | [![GitHub](https://img.shields.io/github/stars/assafelovic/gpt-researcher)](https://github.com/assafelovic/gpt-researcher) | Autonomous agent for comprehensive online research |
| [AutoSurvey](https://github.com/AutoSurveys/AutoSurvey) | [![GitHub](https://img.shields.io/github/stars/AutoSurveys/AutoSurvey)](https://github.com/AutoSurveys/AutoSurvey) | Automated comprehensive literature surveys |
| [storm](https://github.com/stanford-oval/storm) | [![GitHub](https://img.shields.io/github/stars/stanford-oval/storm)](https://github.com/stanford-oval/storm) | Wikipedia-style article generation (STORM) |


### Coding & Experiments

| Repository | Stars | Description |
|-----------|-------|-------------|
| [autoresearch (Karpathy)](https://github.com/karpathy/autoresearch) | [![GitHub](https://img.shields.io/github/stars/karpathy/autoresearch)](https://github.com/karpathy/autoresearch) | Autonomous ML experiments, ~12 exp/hour overnight |
| [Paper2Code](https://github.com/going-doer/Paper2Code) | [![GitHub](https://img.shields.io/github/stars/going-doer/Paper2Code)](https://github.com/going-doer/Paper2Code) | Multi-agent ML paper to code transformation |
| [RD-Agent](https://github.com/microsoft/RD-Agent) | [![GitHub](https://img.shields.io/github/stars/microsoft/RD-Agent)](https://github.com/microsoft/RD-Agent) | Microsoft's LLM framework for autonomous data science |
| [MLAgentBench](https://github.com/snap-stanford/MLAgentBench) | [![GitHub](https://img.shields.io/github/stars/snap-stanford/MLAgentBench)](https://github.com/snap-stanford/MLAgentBench) | 13 end-to-end ML experimentation tasks |
| [SWE-bench](https://github.com/princeton-nlp/SWE-bench) | [![GitHub](https://img.shields.io/github/stars/princeton-nlp/SWE-bench)](https://github.com/princeton-nlp/SWE-bench) | Real-world GitHub issue resolution benchmark |
| [Thoth](https://github.com/SeeleAI/Thoth) | [![GitHub](https://img.shields.io/github/stars/SeeleAI/Thoth)](https://github.com/SeeleAI/Thoth) | Dashboard-first Claude Code and Codex runtime for durable autoresearch runs, work-item locks, ledgers, and reviewable verdicts |


### Peer Review

| Repository | Stars | Description |
|-----------|-------|-------------|
| [paper-reviewer](https://github.com/deep-diver/paper-reviewer) | [![GitHub](https://img.shields.io/github/stars/deep-diver/paper-reviewer)](https://github.com/deep-diver/paper-reviewer) | arXiv paper reviews + blog posts |
| [ai-peer-review](https://github.com/poldrack/ai-peer-review) | [![GitHub](https://img.shields.io/github/stars/poldrack/ai-peer-review)](https://github.com/poldrack/ai-peer-review) | Multi-LLM reviews + meta-review synthesis |
| [openreviewer](https://github.com/maxidl/openreviewer) | [![GitHub](https://img.shields.io/github/stars/maxidl/openreviewer)](https://github.com/maxidl/openreviewer) | Llama-8B fine-tuned on 79K expert reviews |

<div align="center">

**[⬆ Back to Top](#awesome-ai-auto-research)**

*Last updated: 2026-06-21 · Maintained by [WorldBench](https://github.com/worldbench)*

</div>
