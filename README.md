[![Awesome Logo](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![arXiv](https://img.shields.io/badge/arXiv-YOUR_ARXIV_ID-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/YOUR_ARXIV_ID)
![Visitors](https://komarev.com/ghpvc/?username=worldbench&repo=awesome-ai-auto-research&label=Hello,%20Visitor%20&color=yellow&style=social)
[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-red.svg?style=flat)](https://github.com/worldbench/awesome-ai-auto-research/pulls)

# :sunglasses: Awesome AI Auto-Research

This repository accompanies the survey paper **"[AI for Auto-Research: Roadmap & User Guide]()"** and tracks papers on AI-assisted and automated scientific research, covering the full research lifecycle.


<!-- ### :books: Citation

If you find this work helpful for your research, please kindly consider citing our paper:
```bibtex
@article{ai-auto-research,
  title   = {{AI} for {Auto-Research}: Roadmap \& User Guide},
  author  = {},
  journal = {arXiv preprint arXiv:},
  year    = {2026}
}
``` -->


# Background

| | |
|:-:|:-|
| **Phase 1: Creation** | Generating novel research ideas, searching and synthesizing literature, running coding experiments, and creating publication-quality tables and figures. This phase spans **Idea Generation**, **Literature Review**, **Coding & Experiments**, and **Tables & Figures**. |
| **Phase 2: Writing** | Drafting, editing, and polishing academic manuscripts. AI assistance ranges from semi-automated grammar and citation tools to fully automated paper generation — the most commercially mature yet ethically contested stage. |
| **Phase 3: Validation** | Automated peer review generation, reviewer-paper matching, review quality assessment, and AI-assisted author rebuttals. This phase covers **Peer Review** and **Rebuttal & Revision**. |
| **Phase 4: Dissemination** | Converting papers into slides, posters, videos, websites, and social media content. Each output format targets a different audience and demands its own design logic and AI tool chain. |
| | |


### Table of Contents
- [**0. Background**](#background)
- [**1. Idea Generation**](#1.-idea-generation)
    - [LLM Internal Knowledge-Based Generation](#llm-internal-knowledge-based-generation)
    - [External Signal-Driven Generation](#external-signal-driven-generation)
    - [Multi-Agent Collaborative Generation](#multi-agent-collaborative-generation)
    - [Novelty and Feasibility Assessment](#novelty-and-feasibility-assessment)
- [**2. Literature Review & Paper Search**](#2.-literature-review-paper-search)
    - [Literature Retrieval](#literature-retrieval)
    - [Survey & Related Work Generation](#survey-related-work-generation)
    - [Deep Research Agents](#deep-research-agents)
    - [Retrieval and Synthesis Quality Assessment](#retrieval-and-synthesis-quality-assessment)
- [**3. Coding & Experimentation**](#3.-coding-experimentation)
    - [Code Generation](#code-generation)
    - [Paper-to-Code](#paper-to-code)
    - [Experiment Execution & Orchestration](#experiment-execution-orchestration)
    - [Code Correctness and Reproducibility Assessment](#code-correctness-and-reproducibility-assessment)
- [**4. Tables & Figures**](#4.-tables-figures)
    - [Scientific Figure Generation](#scientific-figure-generation)
    - [Table Understanding & Generation](#table-understanding-generation)
    - [Mathematical Formulas & TikZ](#mathematical-formulas-tikz)
    - [Visual Fidelity and Scientific Accuracy Assessment](#visual-fidelity-and-scientific-accuracy-assessment)
- [**5. Peer Review**](#5.-peer-review)
    - [Automated Review Generation](#automated-review-generation)
    - [Meta-Review & Reviewer Matching](#meta-review-reviewer-matching)
    - [Review Quality Assessment](#review-quality-assessment)
    - [Adversarial Attacks & Bias Analysis](#adversarial-attacks-bias-analysis)
    - [Detection & Policy](#detection-policy)
- [**6. Rebuttal**](#6.-rebuttal)
    - [Reviewer Comment Analysis](#reviewer-comment-analysis)
    - [Automated Rebuttal Generation](#automated-rebuttal-generation)
    - [Rebuttal Effectiveness Assessment](#rebuttal-effectiveness-assessment)
- [**7. Paper Writing**](#7.-paper-writing)
    - [Semi-Automated Writing Assistance](#semi-automated-writing-assistance)
    - [Fully Automated Paper Generation](#fully-automated-paper-generation)
    - [Societal Analysis](#societal-analysis)
    - [Writing Quality and AI Detection Assessment](#writing-quality-and-ai-detection-assessment)
- [**8. Dissemination (Paper2X)**](#8.-dissemination-paper2x)
    - [Slides & Presentations](#slides--presentations)
    - [Posters](#posters)
    - [Video & Web](#video--web)
    - [Fidelity and Adoption Assessment](#fidelity-and-adoption-assessment)
- [**9. End-to-End Systems**](#9.-end-to-end-systems)
    - [Fully Automated Research Systems](#fully-automated-research-systems)
    - [Domain-Specific Systems](#domain-specific-systems)
    - [Evolutionary & Self-Improving Systems](#evolutionary-self-improving-systems)
    - [Research Platforms & Infrastructure](#research-platforms-infrastructure)
- [**10. Societal & Critical Perspectives**](#10.-societal-critical-perspectives)
- [**11. Surveys & Curated Lists**](#11.-surveys-curated-lists)
- [**12. Tools & GitHub Repos**](#12.-tools-github-repos)
# 1. Idea Generation

### LLM Internal Knowledge-Based Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `SciMON` | [![arXiv](https://img.shields.io/badge/arXiv-2305.14259-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2305.14259)<br>SciMON: Scientific Inspiration Machines Optimized for Novelty | ACL 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2024.acl-long.17/) | [![GitHub](https://img.shields.io/github/stars/EagleW/CLBD)](https://github.com/EagleW/CLBD) |
| `ResearchAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2404.07738-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2404.07738)<br>ResearchAgent: Iterative Research Idea Generation over Scientific Literature with Large Language Models | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/JinheonBaek/ResearchAgent)](https://github.com/JinheonBaek/ResearchAgent) |
| `AI Scientist` | [![arXiv](https://img.shields.io/badge/arXiv-2408.06292-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2408.06292)<br>The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/SakanaAI/AI-Scientist)](https://github.com/SakanaAI/AI-Scientist) |
| `Idea Gen Agent` | [![arXiv](https://img.shields.io/badge/arXiv-2409.04109-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2409.04109)<br>Can LLMs Generate Novel Research Ideas? A Large Scale Human Study with 100+ NLP Researchers | arXiv 2024 | - | - |
| `Chain of Ideas` | [![arXiv](https://img.shields.io/badge/arXiv-2410.13185-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.13185)<br>Chain of Ideas: Revolutionizing Research Via Novel Idea Development with LLM Agents | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/DAMO-NLP-SG/CoI-Agent)](https://github.com/DAMO-NLP-SG/CoI-Agent) |
| `Spark` | [![arXiv](https://img.shields.io/badge/arXiv-2504.20090-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.20090)<br>Spark: A System for Scientifically Creative Idea Generation | ICCC 2025 | - | - |
| `AI Scientist v2` | [![arXiv](https://img.shields.io/badge/arXiv-2504.08066-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.08066)<br>The AI Scientist v2: Workshop-Level Automated Scientific Discovery via Agentic Tree Search | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/SakanaAI/AI-Scientist-v2)](https://github.com/SakanaAI/AI-Scientist-v2) |
| `AI-Researcher` | [![arXiv](https://img.shields.io/badge/arXiv-2505.18705-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.18705)<br>AI-Researcher: Autonomous Scientific Innovation | arXiv 2025 | - | - |
| `EvoIdeator` | [![arXiv](https://img.shields.io/badge/arXiv-2603.21728-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.21728)<br>EvoIdeator: Evolving Scientific Ideas through Checklist-Grounded Reinforcement Learning | arXiv 2026 | - | - |
| `Rubric Rewards` | [![arXiv](https://img.shields.io/badge/arXiv-2512.23707-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.23707)<br>Training AI Co-Scientists Using Rubric Rewards | arXiv 2025 | - | - |
||

### External Signal-Driven Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `SciAgents` | [![arXiv](https://img.shields.io/badge/arXiv-2409.05556-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2409.05556)<br>SciAgents: Automating Scientific Discovery through Multi-Agent Intelligent Graph Reasoning | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/lamm-mit/SciAgentsDiscovery)](https://github.com/lamm-mit/SciAgentsDiscovery) |
| `MOOSE-Chem` | [![arXiv](https://img.shields.io/badge/arXiv-2410.07076-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.07076)<br>MOOSE-Chem: Large Language Models for Rediscovering Unseen Chemistry Scientific Hypotheses | arXiv 2024 | - | - |
| `Nova` | [![arXiv](https://img.shields.io/badge/arXiv-2410.14255-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.14255)<br>Nova: An Iterative Planning and Search Approach to Enhance Novelty and Diversity of LLM Generated Ideas | arXiv 2024 | - | - |
| `SciPIP` | [![arXiv](https://img.shields.io/badge/arXiv-2410.23166-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.23166)<br>SciPIP: An LLM-based Scientific Paper Idea Proposer | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/cheerss/SciPIP)](https://github.com/cheerss/SciPIP) |
| `IdeaSynth` | [![arXiv](https://img.shields.io/badge/arXiv-2410.04025-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.04025)<br>IdeaSynth: Iterative Research Idea Development Through Evolving and Composing Idea Facets with Literature-Grounded Feedback | CHI 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://dl.acm.org/doi/10.1145/3706598.3713851) | - |
| `MOOSE-Chem2` | [![arXiv](https://img.shields.io/badge/arXiv-2505.19209-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.19209)<br>MOOSE-Chem2: Exploring LLM Limits in Fine-Grained Scientific Hypothesis Discovery via Hierarchical Search | arXiv 2025 | - | - |
| `Kosmos` | [![arXiv](https://img.shields.io/badge/arXiv-2511.02824-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.02824)<br>Kosmos: An AI Scientist for Autonomous Discovery | arXiv 2025 | - | - |
| `Literature-Driven Scientific Theories` | [![arXiv](https://img.shields.io/badge/arXiv-2601.16282-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.16282)<br>Generating Literature-Driven Scientific Theories at Scale | arXiv 2026 | - | - |
| `FlowPIE` | [![arXiv](https://img.shields.io/badge/arXiv-2603.29557-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.29557)<br>FlowPIE: Test-Time Scientific Idea Evolution with Flow-Guided Literature Exploration | arXiv 2026 | - | - |
||

### Multi-Agent Collaborative Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `VirSci (Many Heads)` | [![arXiv](https://img.shields.io/badge/arXiv-2410.09403-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.09403)<br>Many Heads Are Better Than One: Improved Scientific Idea Generation by an LLM-Based Multi-Agent System | ACL 2025 | - | [![GitHub](https://img.shields.io/github/stars/open-sciencelab/Virtual-Scientists)](https://github.com/open-sciencelab/Virtual-Scientists) |
| `LLMs for Combinatorial Creativity` | [![arXiv](https://img.shields.io/badge/arXiv-2412.14141-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.14141)<br>LLMs can Realize Combinatorial Creativity: Generating Creative Ideas via LLMs for Scientific Research | arXiv 2024 | - | - |
| `Multi-Agent Dial.` | [![arXiv](https://img.shields.io/badge/arXiv-2411.12422-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.12422) | SIGDIAL 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.sigdial-1.24/) | - |
| `Deep Ideation` | [![arXiv](https://img.shields.io/badge/arXiv-2511.02238-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.02238)<br>Deep Ideation: Designing LLM Agents to Generate Novel Research Ideas on Scientific Concept Network | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/kyZhao-1/Deep-Ideation)](https://github.com/kyZhao-1/Deep-Ideation) |
| `Artificial Hivemind` | [![arXiv](https://img.shields.io/badge/arXiv-2510.22954-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.22954)<br>Artificial Hivemind: The Open-Ended Homogeneity of Language Models (and Beyond) | NeurIPS 2025 | - | - |
||

### Novelty and Feasibility Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `IdeaBench` | [![arXiv](https://img.shields.io/badge/arXiv-2411.02429-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.02429) | arXiv 2024 | - | - |
| `LiveIdeaBench` | [![arXiv](https://img.shields.io/badge/arXiv-2412.17596-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.17596)<br>LiveIdeaBench: Evaluating LLMs' Scientific Creativity and Idea Generation with Minimal Context | arXiv 2024 | - | - |
| `ResearchBench` | [![arXiv](https://img.shields.io/badge/arXiv-2503.21248-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.21248)<br>ResearchBench: Benchmarking LLMs in Scientific Discovery via Inspiration-Based Task Decomposition | ACL 2026 | - | - |
| `AI Idea Bench 2025` | [![arXiv](https://img.shields.io/badge/arXiv-2504.14191-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.14191)<br>AI Idea Bench 2025: AI Research Idea Generation Benchmark | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/yansheng-qiu/AI_Idea_Bench_2025)](https://github.com/yansheng-qiu/AI_Idea_Bench_2025) |
| `The Ideation-Execution Gap` | [![arXiv](https://img.shields.io/badge/arXiv-2506.20803-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.20803)<br>The Ideation-Execution Gap: Execution Outcomes of LLM-Generated versus Human Research Ideas | arXiv 2025 | - | - |
| `HeurekaBench` | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://openreview.net/forum?id=YOUR_ID)<br>HeurekaBench: A Benchmarking Framework for AI Co-scientist | ICLR 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://brbiclab.epfl.ch/projects/heurekabench/) | [![GitHub](https://img.shields.io/github/stars/mlbio-epfl/HeurekaBench)](https://github.com/mlbio-epfl/HeurekaBench) |
| `Why LLMs Aren't Scientists Yet` | [![arXiv](https://img.shields.io/badge/arXiv-2601.03315-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.03315)<br>Why LLMs Aren't Scientists Yet | arXiv 2026 | - | - |
| `AI Can Learn Scientific Taste` | [![arXiv](https://img.shields.io/badge/arXiv-2603.14473-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.14473)<br>AI Can Learn Scientific Taste | arXiv 2026 | - | - |
| `HindSight` | [![arXiv](https://img.shields.io/badge/arXiv-2603.15164-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.15164)<br>HindSight: Evaluating LLM-Generated Research Ideas via Future Impact | arXiv 2026 | - | - |
| `DeepInnovator` | [![arXiv](https://img.shields.io/badge/arXiv-2602.18920-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.18920)<br>DeepInnovator: Triggering the Innovative Capabilities of LLMs | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/HKUDS/DeepInnovator)](https://github.com/HKUDS/DeepInnovator) |
||


# 2. Literature Review & Paper Search

### Literature Retrieval

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `LitLLM` | [![arXiv](https://img.shields.io/badge/arXiv-2402.01788-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.01788)<br>LitLLM: A Toolkit for Literature Review with Large Language Models | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://litllm.github.io) | - |
| `OpenResearcher` | [![arXiv](https://img.shields.io/badge/arXiv-2408.09578-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2408.09578) | EMNLP 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2024.emnlp-demo.24/) | - |
| `CiteME` | [![arXiv](https://img.shields.io/badge/arXiv-2407.12861-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.12861)<br>CiteME: Can Language Models Accurately Cite Scientific Claims? | arXiv 2024 | - | - |
| `LitSearch` | [![arXiv](https://img.shields.io/badge/arXiv-2407.18940-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.18940)<br>LitSearch: A Retrieval Benchmark for Scientific Literature Search | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/princeton-nlp/LitSearch)](https://github.com/princeton-nlp/LitSearch) |
| `PaperQA2` | [![arXiv](https://img.shields.io/badge/arXiv-2409.13740-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2409.13740)<br>Language Agents Achieve Superhuman Synthesis of Scientific Knowledge | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/Future-House/paper-qa)](https://github.com/Future-House/paper-qa) |
| `PaSa` | [![arXiv](https://img.shields.io/badge/arXiv-2501.10120-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.10120)<br>PaSa: An LLM Agent for Comprehensive Academic Paper Search | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/bytedance/pasa)](https://github.com/bytedance/pasa) |
||

### Survey & Related Work Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ChatPaper` | - | GitHub 2023 | - | [![GitHub](https://img.shields.io/github/stars/kaixindelele/ChatPaper)](https://github.com/kaixindelele/ChatPaper) |
| `PaperQA` | [![arXiv](https://img.shields.io/badge/arXiv-2312.07559-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.07559)<br>PaperQA: Retrieval-Augmented Generative Agent for Scientific Research | arXiv 2023 | - | [![GitHub](https://img.shields.io/github/stars/Future-House/paper-qa)](https://github.com/Future-House/paper-qa) |
| `STORM` | [![arXiv](https://img.shields.io/badge/arXiv-2402.14207-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.14207)<br>Assisting in Writing Wikipedia-like Articles From Scratch with Large Language Models | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/stanford-oval/storm)](https://github.com/stanford-oval/storm) |
| `AutoSurvey` | [![arXiv](https://img.shields.io/badge/arXiv-2406.10252-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2406.10252)<br>AutoSurvey: Large Language Models Can Automatically Write Surveys | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/AutoSurveys/AutoSurvey)](https://github.com/AutoSurveys/AutoSurvey) |
| `GPT Researcher` | - | GitHub 2024 | - | [![GitHub](https://img.shields.io/github/stars/assafelovic/gpt-researcher)](https://github.com/assafelovic/gpt-researcher) |
| `LLMs for Automated Literature Review` | [![arXiv](https://img.shields.io/badge/arXiv-2412.13612-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.13612)<br>Large Language Models for Automated Literature Review | arXiv 2024 | - | - |
| `SurveyX` | [![arXiv](https://img.shields.io/badge/arXiv-2502.14776-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.14776)<br>SurveyX: Academic Survey Automation via Large Language Models | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](http://www.surveyx.cn) | - |
| `SurveyForge` | [![arXiv](https://img.shields.io/badge/arXiv-2503.04629-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.04629)<br>SurveyForge: On the Outline Heuristics, Memory-Driven Generation, and Multi-dimensional Evaluation for Automated Survey Writing | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/Alpha-Innovator/SurveyForge)](https://github.com/Alpha-Innovator/SurveyForge) |
| `CiteGeist` | [![arXiv](https://img.shields.io/badge/arXiv-2503.23229-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.23229)<br>Citegeist: Automated Generation of Related Work Analysis on the arXiv Corpus | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://citegeist.org) | - |
| `InteractiveSurvey` | [![arXiv](https://img.shields.io/badge/arXiv-2504.08762-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.08762)<br>InteractiveSurvey: An LLM-based Personalized and Interactive Survey Paper Generation System | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/TechnicolorGUO/InteractiveSurvey)](https://github.com/TechnicolorGUO/InteractiveSurvey) |
| `Agentic AutoSurvey` | [![arXiv](https://img.shields.io/badge/arXiv-2509.18661-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.18661)<br>Agentic AutoSurvey: Let LLMs Survey LLMs | arXiv 2025 | - | - |
| `LiRA` | [![arXiv](https://img.shields.io/badge/arXiv-2510.05138-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.05138)<br>LiRA: A Multi-Agent Framework for Reliable and Readable Literature Review Generation | arXiv 2025 | - | - |
| `SurveyG` | [![arXiv](https://img.shields.io/badge/arXiv-2510.07733-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.07733)<br>SurveyG: A Multi-Agent LLM Framework with Hierarchical Citation Graph for Automated Survey Generation | arXiv 2025 | - | - |
| `IterSurvey` | [![arXiv](https://img.shields.io/badge/arXiv-2510.21900-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.21900)<br>IterSurvey: Deep Literature Survey Automation with an Iterative Workflow | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/HancCui/IterSurvey_Autosurveyv2)](https://github.com/HancCui/IterSurvey_Autosurveyv2) |
| `CiteLLM` | [![arXiv](https://img.shields.io/badge/arXiv-2602.23075-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.23075)<br>CiteLLM: An Agentic Platform for Trustworthy Scientific Reference Discovery | arXiv 2026 | - | - |
||

### Deep Research Agents

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ASReview` | [![arXiv](https://img.shields.io/badge/arXiv-2100.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s42256-020-00287-7)<br>An Open Source Machine Learning Framework for Efficient and Transparent Systematic Reviews | Nature MI 2021 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://asreview.nl) | [![GitHub](https://img.shields.io/github/stars/asreview/asreview)](https://github.com/asreview/asreview) |
| `CHIME` | [![arXiv](https://img.shields.io/badge/arXiv-2407.16148-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.16148)<br>CHIME: LLM-Assisted Hierarchical Organization of Scientific Studies for Literature Review Support | arXiv 2024 | - | - |
| `OpenScholar` | [![arXiv](https://img.shields.io/badge/arXiv-2411.14199-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.14199)<br>OpenScholar: Synthesizing Scientific Literature with Retrieval-Augmented LMs | Nature 2025 | - | - |
| `DeepResearchAgent` | - | GitHub 2025 | - | [![GitHub](https://img.shields.io/github/stars/SkyworkAI/DeepResearchAgent)](https://github.com/SkyworkAI/DeepResearchAgent) |
| `DeerFlow` | - | GitHub 2025 | - | [![GitHub](https://img.shields.io/github/stars/bytedance/deer-flow)](https://github.com/bytedance/deer-flow) |
| `Tongyi DeepResearch` | - | GitHub 2025 | - | [![GitHub](https://img.shields.io/github/stars/Alibaba-NLP/DeepResearch)](https://github.com/Alibaba-NLP/DeepResearch) |
| `Auto-Deep-Research` | [![arXiv](https://img.shields.io/badge/arXiv-2502.05957-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.05957)<br>AutoAgent: A Fully-Automated and Zero-Code Framework for LLM Agents | arXiv 2025 | - | - |
| `O-Researcher` | [![arXiv](https://img.shields.io/badge/arXiv-2601.03743-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.03743)<br>O-Researcher: An Open Ended Deep Research Model via Multi-Agent Distillation and Agentic RL | arXiv 2026 | - | - |
||

### Retrieval and Synthesis Quality Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ReportBench` | [![arXiv](https://img.shields.io/badge/arXiv-2508.15804-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.15804)<br>ReportBench: Evaluating Deep Research Agents via Academic Survey Tasks | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/ByteDance-BandAI/ReportBench)](https://github.com/ByteDance-BandAI/ReportBench) |
| `DeepScholar-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2508.20033-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.20033)<br>DeepScholar-Bench: A Live Benchmark and Automated Evaluation for Generative Research Synthesis | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/guestrin-lab/deepscholar-bench)](https://github.com/guestrin-lab/deepscholar-bench) |
| `IDRBench` | [![arXiv](https://img.shields.io/badge/arXiv-2601.06676-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.06676)<br>IDRBench: Interactive Deep Research Benchmark | arXiv 2026 | - | - |
| `ScholarGym` | [![arXiv](https://img.shields.io/badge/arXiv-2601.21654-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.21654)<br>ScholarGym: Benchmarking Large Language Model Capabilities in the Information-Gathering Stage of Deep Research | arXiv 2026 | - | - |
| `SciNetBench` | [![arXiv](https://img.shields.io/badge/arXiv-2601.03260-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.03260)<br>SciNetBench: A Relation-Aware Benchmark for Scientific Literature Retrieval Agents | arXiv 2026 | - | - |
||


# 3. Coding & Experimentation

### Code Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `SWE-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2400.00000-b31b1b?style=flat-square&logo=arxiv)](https://openreview.net/forum?id=VTF8yNQM66)<br>SWE-bench: Can Language Models Resolve Real-World GitHub Issues? | ICLR 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openreview.net/forum?id=VTF8yNQM66) | [![GitHub](https://img.shields.io/github/stars/princeton-nlp/SWE-bench)](https://github.com/princeton-nlp/SWE-bench) |
| `SWE-agent` | [![arXiv](https://img.shields.io/badge/arXiv-2405.15793-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2405.15793) | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/princeton-nlp/SWE-agent)](https://github.com/princeton-nlp/SWE-agent) |
| `OpenHands` | [![arXiv](https://img.shields.io/badge/arXiv-2407.16741-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.16741)<br>OpenHands: An Open Platform for AI Software Developers as Generalist Agents | ICLR 2025 | - | [![GitHub](https://img.shields.io/github/stars/All-Hands-AI/OpenHands)](https://github.com/All-Hands-AI/OpenHands) |
| `SWE-Bench Pro` | [![arXiv](https://img.shields.io/badge/arXiv-2509.16941-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.16941)<br>SWE-Bench Pro: Can AI Agents Solve Long-Horizon Software Engineering Tasks? | arXiv 2025 | - | - |
| `SWE-EVO` | [![arXiv](https://img.shields.io/badge/arXiv-2512.18470-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.18470)<br>SWE-EVO: Benchmarking Coding Agents in Long-Horizon Software Evolution Scenarios | arXiv 2025 | - | - |
||

### Paper-to-Code

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `FunSearch` | [![arXiv](https://img.shields.io/badge/arXiv-2400.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s41586-023-06924-6)<br>Mathematical Discoveries from Program Search with Large Language Models | Nature 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s41586-023-06924-6) | [![GitHub](https://img.shields.io/github/stars/google-deepmind/funsearch)](https://github.com/google-deepmind/funsearch) |
| `SciCode` | [![arXiv](https://img.shields.io/badge/arXiv-2407.13168-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.13168)<br>SciCode: A Research Coding Benchmark Curated by Scientists | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://scicode-bench.github.io) | [![GitHub](https://img.shields.io/github/stars/scicode-bench/SciCode)](https://github.com/scicode-bench/SciCode) |
| `SciReplicate-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2504.00255-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.00255)<br>SciReplicate-Bench: Benchmarking LLMs in Agent-driven Algorithmic Reproduction from Research Papers | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://xyzcs.github.io/scireplicate.github.io/) | [![GitHub](https://img.shields.io/github/stars/xyzCS/SciReplicate-Bench)](https://github.com/xyzCS/SciReplicate-Bench) |
| `PaperBench` | [![arXiv](https://img.shields.io/badge/arXiv-2504.01848-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.01848)<br>PaperBench: Evaluating AI's Ability to Replicate AI Research | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/openai/preparedness)](https://github.com/openai/preparedness) |
| `PaperCoder` | [![arXiv](https://img.shields.io/badge/arXiv-2504.17192-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.17192)<br>Paper2Code: Automating Code Generation from Scientific Papers in Machine Learning | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/going-doer/Paper2Code)](https://github.com/going-doer/Paper2Code) |
| `ResearchCodeBench` | [![arXiv](https://img.shields.io/badge/arXiv-2506.02314-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.02314)<br>ResearchCodeBench: Benchmarking LLMs on Implementing Novel ML Research Code | arXiv 2025 | - | - |
||

### Experiment Execution & Orchestration

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `BioPlanner` | [![arXiv](https://img.shields.io/badge/arXiv-2310.10632-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.10632)<br>BioPlanner: Automatic Evaluation of LLMs on Protocol Planning | arXiv 2023 | - | [![GitHub](https://img.shields.io/github/stars/bioplanner/bioplanner)](https://github.com/bioplanner/bioplanner) |
| `Coscientist` | [![arXiv](https://img.shields.io/badge/arXiv-2300.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s41586-023-06792-0)<br>Autonomous Chemical Research with Large Language Models | Nature 2023 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s41586-023-06792-0) | - |
| `MLAgentBench` | [![arXiv](https://img.shields.io/badge/arXiv-2310.03302-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.03302)<br>MLAgentBench: Evaluating Language Agents on Machine Learning Experimentation | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/snap-stanford/MLAgentBench)](https://github.com/snap-stanford/MLAgentBench) |
| `DS-Agent` | [![arXiv](https://img.shields.io/badge/arXiv-2402.17453-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.17453)<br>DS-Agent: Automated Data Science by Empowering Large Language Models with Case-Based Reasoning | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/guosyjlu/DS-Agent)](https://github.com/guosyjlu/DS-Agent) |
| `ChemCrow` | [![arXiv](https://img.shields.io/badge/arXiv-2400.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s42256-024-00832-8)<br>ChemCrow: Augmenting Large Language Models with Chemistry Tools | Nature MI 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s42256-024-00832-8) | - |
| `CRISPR-GPT` | [![arXiv](https://img.shields.io/badge/arXiv-2404.18021-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2404.18021)<br>CRISPR-GPT for Agentic Automation of Gene-Editing Experiments | arXiv 2024 | - | - |
| `MLR-Copilot` | [![arXiv](https://img.shields.io/badge/arXiv-2408.14033-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2408.14033)<br>MLR-Copilot: Autonomous Machine Learning Research based on Large Language Models Agents | arXiv 2024 | - | - |
| `MLE-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2410.07095-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.07095)<br>MLE-Bench: Evaluating Machine Learning Agents on Machine Learning Engineering | arXiv 2024 | - | - |
| `autoresearch (Karpathy)` | - | GitHub 2025 | - | [![GitHub](https://img.shields.io/github/stars/karpathy/autoresearch)](https://github.com/karpathy/autoresearch) |
| `Dolphin` | [![arXiv](https://img.shields.io/badge/arXiv-2501.03916-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.03916)<br>Dolphin: Moving Towards Closed-loop Auto-research through Thinking, Practice, and Feedback | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://alpha-innovator.github.io/Dolphin-project-page) | - |
| `AIDE` | [![arXiv](https://img.shields.io/badge/arXiv-2502.13138-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.13138)<br>AIDE: AI-Driven Exploration in the Space of Code | arXiv 2025 | - | - |
| `Curie` | [![arXiv](https://img.shields.io/badge/arXiv-2502.16069-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.16069)<br>Curie: Toward Rigorous and Automated Scientific Experimentation with AI Agents | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/Just-Curieous/Curie)](https://github.com/Just-Curieous/Curie) |
| `MLGym` | [![arXiv](https://img.shields.io/badge/arXiv-2502.14499-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.14499)<br>MLGym: A New Framework and Benchmark for Advancing AI Research Agents | arXiv 2025 | - | - |
| `CodeScientist` | [![arXiv](https://img.shields.io/badge/arXiv-2503.22708-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.22708)<br>CodeScientist: End-to-End Semi-Automated Scientific Discovery with Code-based Experimentation | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/allenai/codescientist)](https://github.com/allenai/codescientist) |
| `AutoReproduce` | [![arXiv](https://img.shields.io/badge/arXiv-2505.20662-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.20662)<br>AutoReproduce: Automatic AI Experiment Reproduction with Paper Lineage | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/AI9Stars/AutoReproduce)](https://github.com/AI9Stars/AutoReproduce) |
| `R&D-Agent` | [![arXiv](https://img.shields.io/badge/arXiv-2505.14738-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.14738)<br>R\&D-Agent: An LLM-Agent Framework Towards Autonomous Data Science | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/microsoft/RD-Agent)](https://github.com/microsoft/RD-Agent) |
| `InternAgent / NovelSeek` | [![arXiv](https://img.shields.io/badge/arXiv-2505.16938-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.16938)<br>InternAgent: When Agent Becomes the Scientist -- Building Closed-Loop System from Hypothesis to Verification | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://alpha-innovator.github.io/InternAgent-project-page) | [![GitHub](https://img.shields.io/github/stars/Alpha-Innovor/InternAgent)](https://github.com/Alpha-Innovor/InternAgent) |
| `AlphaEvolve` | [![arXiv](https://img.shields.io/badge/arXiv-2506.13131-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.13131)<br>AlphaEvolve: A Coding Agent for Scientific and Algorithmic Discovery | arXiv 2025 | - | - |
| `MLR-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2505.19955-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.19955)<br>MLR-Bench: Evaluating AI Agents on Open-Ended Machine Learning Research | arXiv 2025 | - | - |
| `Execution-Grounded AI Research` | [![arXiv](https://img.shields.io/badge/arXiv-2601.14525-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.14525)<br>Towards Execution-Grounded Automated AI Research | arXiv 2026 | - | - |
| `SciNav` | [![arXiv](https://img.shields.io/badge/arXiv-2603.20256-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.20256)<br>SciNav: A General Agent Framework for Scientific Coding Tasks | arXiv 2026 | - | - |
| `Learn to Discover` | [![arXiv](https://img.shields.io/badge/arXiv-2601.16175-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.16175)<br>Learning to Discover at Test Time | arXiv 2026 | - | - |
| `FrontierScience` | [![arXiv](https://img.shields.io/badge/arXiv-2601.21165-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.21165)<br>FrontierScience: Evaluating AI's Ability to Perform Expert-Level Scientific Tasks | arXiv 2026 | - | - |
| `EvoScientist` | [![arXiv](https://img.shields.io/badge/arXiv-2603.08127-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.08127)<br>EvoScientist: Towards Multi-Agent Evolving AI Scientists for End-to-End Scientific Discovery | arXiv 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://evoscientist.ai) | [![GitHub](https://img.shields.io/github/stars/evoscientist/evoscientist)](https://github.com/evoscientist/evoscientist) |
||

### Code Correctness and Reproducibility Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `DiscoveryWorld` | [![arXiv](https://img.shields.io/badge/arXiv-2406.06769-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2406.06769)<br>DiscoveryWorld: A Virtual Environment for Developing and Evaluating Automated Scientific Discovery Agents | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/allenai/discoveryworld)](https://github.com/allenai/discoveryworld) |
| `DiscoveryBench` | [![arXiv](https://img.shields.io/badge/arXiv-2407.01725-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.01725)<br>DiscoveryBench: Towards Data-Driven Discovery with Large Language Models | arXiv 2024 | - | [![GitHub](https://img.shields.io/github/stars/allenai/discoverybench)](https://github.com/allenai/discoverybench) |
| `Lab-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2407.10362-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.10362)<br>Lab-Bench: Measuring Capabilities of Language Models for Biology Research | arXiv 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://huggingface.co/datasets/futurehouse/lab-bench) | [![GitHub](https://img.shields.io/github/stars/Future-House/LAB-Bench)](https://github.com/Future-House/LAB-Bench) |
| `InfiAgent-DABench` | [![arXiv](https://img.shields.io/badge/arXiv-2401.05507-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2401.05507)<br>InfiAgent-DABench: Evaluating Agents on Data Analysis Tasks | arXiv 2024 | - | - |
| `ScienceAgentBench` | [![arXiv](https://img.shields.io/badge/arXiv-2410.05080-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2410.05080)<br>ScienceAgentBench: Toward Rigorous Assessment of Language Agents for Data-Driven Scientific Discovery | arXiv 2024 | - | - |
| `RE-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2411.15114-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.15114)<br>RE-Bench: Evaluating Frontier AI R\&D Capabilities of Language Model Agents Against Human Experts | arXiv 2024 | - | - |
| `KernelBench` | [![arXiv](https://img.shields.io/badge/arXiv-2502.10517-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.10517)<br>KernelBench: Can LLMs Write Efficient GPU Kernels? | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/ScalingIntelligence/KernelBench)](https://github.com/ScalingIntelligence/KernelBench) |
| `TritonBench` | [![arXiv](https://img.shields.io/badge/arXiv-2502.14752-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.14752)<br>TritonBench: Benchmarking Large Language Model Capabilities for Generating Triton Operators | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/thunlp/TritonBench)](https://github.com/thunlp/TritonBench) |
| `AstaBench` | [![arXiv](https://img.shields.io/badge/arXiv-2510.21652-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.21652)<br>AstaBench: Rigorous Benchmarking of AI Agents with a Scientific Research Suite | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/allenai/asta-bench)](https://github.com/allenai/asta-bench) |
| `EXP-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2505.24785-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.24785)<br>EXP-Bench: Can AI Conduct AI Research Experiments? | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/EvolvingLMMs-Lab/EXP-Bench)](https://github.com/EvolvingLMMs-Lab/EXP-Bench) |
| `ResearchClawBench` | [![arXiv](https://img.shields.io/badge/arXiv-2512.16969-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.16969)<br>Probing Scientific General Intelligence of LLMs with Scientist-Aligned Workflows | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/InternScience/ResearchClawBench)](https://github.com/InternScience/ResearchClawBench) |
| `PostTrainBench` | [![arXiv](https://img.shields.io/badge/arXiv-2603.08640-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.08640)<br>PostTrainBench: Can LLM Agents Automate LLM Post-Training? | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/aisa-group/PostTrainBench)](https://github.com/aisa-group/PostTrainBench) |
||


# 4. Tables & Figures

### Scientific Figure Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ChartGPT` | [![arXiv](https://img.shields.io/badge/arXiv-2311.01920-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2311.01920)<br>ChartGPT: Leveraging LLMs to Generate Charts from Abstract Natural Language | arXiv 2023 | - | - |
| `MatPlotAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2402.11453-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.11453)<br>MatPlotAgent: Method and Evaluation for LLM-Based Agentic Scientific Data Visualization | arXiv 2024 | - | - |
| `DiagramAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2401.17464-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2401.17464) | CVPR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openaccess.thecvf.com/content/CVPR2025/papers/Wei_From_Words_to_Structured_Visuals_A_Benchmark_and_Framework_for_CVPR_2025_paper.pdf) | - |
| `StarVector` | [![arXiv](https://img.shields.io/badge/arXiv-2312.11556-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2312.11556) | CVPR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openaccess.thecvf.com/content/CVPR2025/papers/Rodriguez_StarVector_Generating_Scalable_Vector_Graphics_Code_from_Images_CVPR_2025_paper.pdf) | - |
| `VisCoder` | [![arXiv](https://img.shields.io/badge/arXiv-2407.04793-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2407.04793) | EMNLP Findings 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.findings-emnlp.167/) | - |
| `PlotGen` | [![arXiv](https://img.shields.io/badge/arXiv-2502.00988-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.00988)<br>PlotGen: Multi-Agent LLM-based Scientific Data Visualization via Multimodal Feedback | arXiv 2025 | - | - |
| `CoDA` | [![arXiv](https://img.shields.io/badge/arXiv-2510.03194-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.03194)<br>CoDA: Agentic Systems for Collaborative Data Visualization | arXiv 2025 | - | - |
| `VIS-Shepherd` | [![arXiv](https://img.shields.io/badge/arXiv-2506.13326-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.13326)<br>VIS-Shepherd: Constructing Critic for LLM-based Data Visualization Generation | arXiv 2025 | - | - |
| `PaperBanana` | [![arXiv](https://img.shields.io/badge/arXiv-2601.23265-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.23265)<br>PaperBanana: Automating Academic Illustration for AI Scientists | arXiv 2026 | - | - |
| `AutoFigure-Edit` | [![arXiv](https://img.shields.io/badge/arXiv-2603.06674-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.06674)<br>AutoFigure-Edit: Generating Editable Scientific Illustration | arXiv 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://deepscientist.cc) | [![GitHub](https://img.shields.io/github/stars/ResearAI/AutoFigure-Edit)](https://github.com/ResearAI/AutoFigure-Edit) |
| `AutoFigure` | [![arXiv](https://img.shields.io/badge/arXiv-2602.03828-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.03828) | ICLR 2026 | - | [![GitHub](https://img.shields.io/github/stars/ResearAI/AutoFigure)](https://github.com/ResearAI/AutoFigure) |
| `SAIL` | [![arXiv](https://img.shields.io/badge/arXiv-2603.18145-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.18145)<br>Setting SAIL: Leveraging Scientist-AI-Loops for Rigorous Visualization Tools | arXiv 2026 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2603.16159-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.16159)<br>AI-Generated Figures in Academic Publishing: Policies, Tools, and Practical Guidelines | arXiv 2026 | - | - |
||

### Table Understanding & Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Chain-of-Table` | [![arXiv](https://img.shields.io/badge/arXiv-2401.04398-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2401.04398)<br>Chain-of-Table: Evolving Tables in Reasoning Chain for Table Understanding | arXiv 2024 | - | - |
| `ArxivDIGESTables` | [![arXiv](https://img.shields.io/badge/arXiv-2310.14324-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.14324) | EMNLP 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2024.emnlp-main.542/) | - |
| `ShowTable` | [![arXiv](https://img.shields.io/badge/arXiv-2512.13303-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.13303)<br>ShowTable: Unlocking Creative Table Visualization with Collaborative Reflection and Refinement | arXiv 2025 | - | - |
| `Table2LaTeX-RL` | [![arXiv](https://img.shields.io/badge/arXiv-2509.17589-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.17589)<br>Table2LaTeX-RL: Converting Table Images to High-Fidelity LaTeX Code Using Reinforced Multimodal Language Models | arXiv 2025 | - | - |
||

### Mathematical Formulas & TikZ

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `AutomaTikZ` | [![arXiv](https://img.shields.io/badge/arXiv-2310.00367-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2310.00367) | ICLR 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openreview.net/forum?id=v3K5TVP8kZ) | - |
| `DeTikZify` | [![arXiv](https://img.shields.io/badge/arXiv-2405.15306-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2405.15306) | NeurIPS 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://papers.nips.cc/paper_files/paper/2024/hash/a5ace289f4e2c70b48b31ba15ac82ecd-Abstract-Conference.html) | - |
| `TikZilla` | [![arXiv](https://img.shields.io/badge/arXiv-2603.03072-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.03072)<br>TikZilla: Scaling Text-to-TikZ with High-Quality Data and Reinforcement Learning | arXiv 2026 | - | - |
||

### Visual Fidelity and Scientific Accuracy Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `AbGen` | [![arXiv](https://img.shields.io/badge/arXiv-2406.06357-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2406.06357) | ACL 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.acl-long.670/) | - |
| `PlotCraft` | [![arXiv](https://img.shields.io/badge/arXiv-2511.00010-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.00010)<br>PlotCraft: Pushing the Limits of LLMs for Complex and Interactive Data Visualization | arXiv 2025 | - | - |
| `TeXpert` | [![arXiv](https://img.shields.io/badge/arXiv-2506.16990-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.16990)<br>TeXpert: Multi-Level Benchmark for LaTeX Code Generation | arXiv 2025 | - | - |
| `SciFig` | [![arXiv](https://img.shields.io/badge/arXiv-2601.04390-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.04390)<br>SciFig: Towards Automating Scientific Figure Generation | arXiv 2026 | - | - |
| `SciFlow-Bench` | [![arXiv](https://img.shields.io/badge/arXiv-2602.09809-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.09809)<br>SciFlow-Bench: Evaluating Structure-Aware Scientific Diagram Generation via Inverse Parsing | arXiv 2026 | - | - |
| `FigureBench` | [![arXiv](https://img.shields.io/badge/arXiv-2602.03828-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.03828)<br>AutoFigure: Generating and Refining Publication-Ready Scientific Illustrations | ICLR 2026 | - | [![GitHub](https://img.shields.io/github/stars/ResearAI/AutoFigure)](https://github.com/ResearAI/AutoFigure) |
||


# 5. Peer Review

### Automated Review Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ChatReviewer` | - | GitHub 2023 | - | [![GitHub](https://img.shields.io/github/stars/nishiwen1214/ChatReviewer)](https://github.com/nishiwen1214/ChatReviewer) |
| `MARG` | [![arXiv](https://img.shields.io/badge/arXiv-2401.04259-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2401.04259)<br>MARG: Multi-Agent Review Generation for Scientific Papers | arXiv 2024 | - | - |
| `Reviewer2` | [![arXiv](https://img.shields.io/badge/arXiv-2402.10886-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.10886)<br>Reviewer2: Optimizing Review Generation Through Prompt Generation | arXiv 2024 | - | - |
| `AI-Peer-Review` | - | GitHub 2024 | - | [![GitHub](https://img.shields.io/github/stars/poldrack/ai-peer-review)](https://github.com/poldrack/ai-peer-review) |
| `DeepReviewer` | [![arXiv](https://img.shields.io/badge/arXiv-2503.08569-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.08569)<br>DeepReview: Improving LLM-based Paper Review with Human-like Deep Thinking Process | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://ai-researcher.net) | - |
| `OpenReviewer` | [![arXiv](https://img.shields.io/badge/arXiv-2412.11948-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.11948)<br>OpenReviewer: A Specialized Large Language Model for Generating Critical Scientific Paper Reviews | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://huggingface.co/spaces/idahl/OpenReviewer) | - |
| `REMOR` | [![arXiv](https://img.shields.io/badge/arXiv-2505.11718-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.11718)<br>REMOR: Automated Peer Review Generation with LLM Reasoning and Multi-Objective Reinforcement Learning | arXiv 2025 | - | - |
| `ReviewRL` | [![arXiv](https://img.shields.io/badge/arXiv-2504.13690-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.13690) | EMNLP 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.emnlp-main.949/) | - |
| `ScholarPeer` | [![arXiv](https://img.shields.io/badge/arXiv-2601.22638-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.22638)<br>ScholarPeer: A Context-Aware Multi-Agent Framework for Automated Peer Review | arXiv 2026 | - | - |
||

### Meta-Review & Reviewer Matching

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `AgentReview` | [![arXiv](https://img.shields.io/badge/arXiv-2406.12708-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2406.12708) | EMNLP 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2024.emnlp-main.70/) | - |
| `LLMs as Meta-Reviewers' Assistants` | [![arXiv](https://img.shields.io/badge/arXiv-2402.15589-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.15589) | NAACL 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.naacl-long.455/) | - |
| `RATE` | [![arXiv](https://img.shields.io/badge/arXiv-2601.19637-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.19637)<br>RATE: Reviewer Profiling and Annotation-free Training for Expertise Ranking in Peer Review Systems | arXiv 2026 | - | - |
||

### Review Quality Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ReviewMT` | [![arXiv](https://img.shields.io/badge/arXiv-2406.05688-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2406.05688)<br>Peer Review as A Multi-Turn and Long-Context Dialogue with Role-Based Interactions | arXiv 2024 | - | - |
| `ClaimCheck` | [![arXiv](https://img.shields.io/badge/arXiv-2503.21717-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.21717)<br>ClaimCheck: How Grounded are LLM Critiques of Scientific Papers? | arXiv 2025 | - | - |
| `ReviewAgents` | [![arXiv](https://img.shields.io/badge/arXiv-2503.08506-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.08506)<br>ReviewAgents: Bridging the Gap Between Human and AI-Generated Paper Reviews | arXiv 2025 | - | - |
| `Stanford Agentic` | - | Web 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://paperreview.ai/tech-overview) | - |
| `CycleResearcher` | [![arXiv](https://img.shields.io/badge/arXiv-2411.00816-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.00816)<br>CycleResearcher: Improving Automated Research via Automated Review | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://wengsyx.github.io/Researcher/) | - |
| `ReViewGraph` | [![arXiv](https://img.shields.io/badge/arXiv-2511.08317-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.08317)<br>Automatic Paper Reviewing with Heterogeneous Graph Reasoning over LLM-Simulated Reviewer-Author Debates | arXiv 2025 | - | - |
| `ReviewerToo` | [![arXiv](https://img.shields.io/badge/arXiv-2510.08867-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.08867)<br>ReviewerToo: Should AI Join The Program Committee? A Look At The Future of Peer Review | arXiv 2025 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s42256-025-01004-5)<br>A Large-Scale Randomized Study of Large Language Model Feedback in Peer Review | Nature MI 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s42256-025-01004-5) | - |
||

### Adversarial Attacks & Bias Analysis

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `AI Review Lottery` | [![arXiv](https://img.shields.io/badge/arXiv-2405.02150-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2405.02150)<br>The AI Review Lottery: Widespread AI-Assisted Peer Reviews Boost Paper Scores and Acceptance Rates | arXiv 2024 | - | - |
| `Raina et al.` | [![arXiv](https://img.shields.io/badge/arXiv-2402.14016-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2402.14016) | EMNLP 2024 | - | - |
| `Ye et al.` | [![arXiv](https://img.shields.io/badge/arXiv-2412.01708-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2412.01708)<br>Are We There Yet? Revealing the Risks of Utilizing Large Language Models in Scholarly Peer Review | arXiv 2024 | - | - |
| `Breaking the Reviewer` | [![arXiv](https://img.shields.io/badge/arXiv-2506.11113-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2506.11113)<br>Breaking the Reviewer: Assessing the Vulnerability of Large Language Models in Automated Peer Review Under Textual Adversarial Attacks | arXiv 2025 | - | - |
| `Sahoo et al.` | [![arXiv](https://img.shields.io/badge/arXiv-2512.10449-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.10449)<br>When Reject Turns into Accept: Quantifying the Vulnerability of LLM-Based Scientific Reviewers to Indirect Prompt Injection | arXiv 2025 | - | - |
| `Zhou et al.` | [![arXiv](https://img.shields.io/badge/arXiv-2511.01287-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.01287)<br>``Give a Positive Review Only'': An Early Investigation Into In-Paper Prompt Injection Attacks and Defenses for AI Reviewers | arXiv 2025 | - | - |
| `Prompt Injection Attacks on Peer Review` | [![arXiv](https://img.shields.io/badge/arXiv-2509.10248-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.10248)<br>Prompt Injection Attacks on LLM Generated Reviews of Scientific Publications | arXiv 2025 | - | - |
| `When Your Reviewer is an LLM` | [![arXiv](https://img.shields.io/badge/arXiv-2509.09912-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.09912)<br>When Your Reviewer is an LLM: Biases, Divergence, and Prompt Injection Risks in Peer Review | arXiv 2025 | - | - |
||

### Detection & Policy

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Monitoring AI-Modified Content` | [![arXiv](https://img.shields.io/badge/arXiv-2403.07183-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2403.07183)<br>Monitoring AI-Modified Content at Scale: A Case Study on the Impact of ChatGPT on AI Conference Peer Reviews | arXiv 2024 | - | - |
| `AI Text Detection in Peer Review` | [![arXiv](https://img.shields.io/badge/arXiv-2502.19614-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.19614)<br>Is Your Paper Being Reviewed by an LLM? Benchmarking AI Text Detection in Peer Review | arXiv 2025 | - | - |
| `Detecting LLM-Generated Peer Reviews` | [![arXiv](https://img.shields.io/badge/arXiv-2503.15772-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.15772)<br>Detecting LLM-Generated Peer Reviews | arXiv 2025 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2602.13817-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.13817)<br>What Happens When Reviewers Receive AI Feedback in Their Reviews? | arXiv 2026 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2603.20450-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.20450)<br>Policies Permitting LLM Use for Polishing Peer Reviews Are Currently Not Enforceable | arXiv 2026 | - | - |
| - | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/d41586-026-00159-z)<br>More than Half of Researchers Now Use AI for Peer Review | Nature News 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/d41586-026-00159-z) | - |
| `Major Conference Catches Illicit AI Use` | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/d41586-026-00866-7)<br>Major Conference Catches Illicit AI Use -- and Rejects Hundreds of Papers | Nature News 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/d41586-026-00866-7) | - |
||


# 6. Rebuttal

### Reviewer Comment Analysis

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Insights from ICLR Rebuttal Process` | [![arXiv](https://img.shields.io/badge/arXiv-2511.15462-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2511.15462)<br>Insights from ICLR Peer Review and Rebuttal Process | arXiv 2025 | - | - |
||

### Automated Rebuttal Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `DRPG` | [![arXiv](https://img.shields.io/badge/arXiv-2601.18081-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.18081)<br>DRPG: An Agentic Framework for Academic Rebuttal | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/ulab-uiuc/DRPG-RebuttalAgent)](https://github.com/ulab-uiuc/DRPG-RebuttalAgent) |
| `Paper2Rebuttal` | [![arXiv](https://img.shields.io/badge/arXiv-2601.14171-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.14171)<br>Paper2Rebuttal: A Multi-Agent Framework for Transparent Author Response Assistance | arXiv 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://mqleet.github.io/Paper2Rebuttal_ProjectPage/) | - |
| `RebuttalAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2601.15715-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.15715)<br>RebuttalAgent: Strategic Persuasion in Academic Rebuttal via Theory of Mind | ICLR 2026 | - | - |
| `Author-in-the-Loop` | [![arXiv](https://img.shields.io/badge/arXiv-2602.11173-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.11173)<br>Author-in-the-Loop Response Generation and Evaluation: Integrating Author Expertise and Intent in Responses to Peer Review | arXiv 2026 | - | - |
||

### Rebuttal Effectiveness Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Re2 Dataset` | [![arXiv](https://img.shields.io/badge/arXiv-2505.07920-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.07920)<br>Re2: A Consistency-Ensured Dataset for Full-stage Peer Review and Multi-Turn Rebuttal Discussions | arXiv 2025 | - | - |
| `Commitment Checklist` | [![arXiv](https://img.shields.io/badge/arXiv-2603.00003-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.00003)<br>Commitment Checklist: Auditing Author Commitments in Peer Review | arXiv 2026 | - | - |
||


# 7. Paper Writing

### Semi-Automated Writing Assistance

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `CoAuthor` | [![arXiv](https://img.shields.io/badge/arXiv-2201.06796-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2201.06796)<br>CoAuthor: Human-AI Collaborative Writing with Language Models | arXiv 2022 | - | - |
| `Script&Shift` | [![arXiv](https://img.shields.io/badge/arXiv-2502.07440-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.07440) | CHI 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://dl.acm.org/doi/10.1145/3706598.3713882) | - |
| `AI in the Writing Process` | [![arXiv](https://img.shields.io/badge/arXiv-2503.10000-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.10000) | AIED 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://link.springer.com/chapter/10.1007/978-3-031-64315-6_14) | - |
| `ScholarCopilot` | [![arXiv](https://img.shields.io/badge/arXiv-2504.00824-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2504.00824)<br>ScholarCopilot: Training LLMs for Academic Writing with Integrated Citation | arXiv 2025 | - | - |
| `OpenDraft` | - | GitHub 2025 | - | [![GitHub](https://img.shields.io/github/stars/federicodeponte/opendraft)](https://github.com/federicodeponte/opendraft) |
| `DraftMarks` | [![arXiv](https://img.shields.io/badge/arXiv-2509.23505-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.23505)<br>DraftMarks: Enhancing Transparency in Human-AI Co-Writing Through Interactive Skeuomorphic Process Traces | arXiv 2025 | - | - |
| `XtraGPT` | [![arXiv](https://img.shields.io/badge/arXiv-2505.11336-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.11336)<br>XtraGPT: Context-Aware and Controllable Academic Paper Revision | arXiv 2025 | - | - |
| `PaperDebugger` | [![arXiv](https://img.shields.io/badge/arXiv-2512.02589-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.02589)<br>PaperDebugger: A Plugin-Based Multi-Agent System for In-Editor Academic Writing, Review, and Editing | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/PaperDebugger/PaperDebugger)](https://github.com/PaperDebugger/PaperDebugger) |
| `LimAgents` | [![arXiv](https://img.shields.io/badge/arXiv-2601.11578-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.11578)<br>Multi-Agent LLMs for Generating Research Limitations | arXiv 2026 | - | - |
||

### Fully Automated Paper Generation

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `CycleResearcher` | [![arXiv](https://img.shields.io/badge/arXiv-2411.00816-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.00816)<br>CycleResearcher: Improving Automated Research via Automated Review | ICLR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://wengsyx.github.io/Researcher/) | - |
| `FutureGen` | [![arXiv](https://img.shields.io/badge/arXiv-2503.16561-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.16561)<br>FutureGen: A RAG-based Approach to Generate the Future Work of Scientific Article | arXiv 2025 | - | - |
| `APRES` | [![arXiv](https://img.shields.io/badge/arXiv-2603.03142-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.03142)<br>APRES: An Agentic Paper Revision and Evaluation System | arXiv 2026 | - | - |
||

### Societal Analysis

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| - | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s41586-025-08681-8)<br>Artificial Intelligence Tools Expand Scientists' Impact but Contract Science's Focus | Nature 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s41586-025-08681-8) | - |
| `Nature AI Survey` | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/d41586-026-00159-z)<br>More than Half of Researchers Now Use AI for Peer Review | Nature 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/d41586-026-00159-z) | - |
||

### Writing Quality and AI Detection Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Mapping LLM Use` | [![arXiv](https://img.shields.io/badge/arXiv-2404.01268-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2404.01268)<br>Mapping the Increasing Use of LLMs in Scientific Papers | arXiv 2024 | - | - |
| `CycleReviewer` | [![arXiv](https://img.shields.io/badge/arXiv-2411.00816-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2411.00816)<br>CycleResearcher: Improving Automated Research via Automated Review | ICLR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://wengsyx.github.io/Researcher/) | - |
| `Stanford Agentic` | - | Web 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://paperreview.ai/tech-overview) | - |
| `SciIG` | [![arXiv](https://img.shields.io/badge/arXiv-2508.14273-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.14273)<br>Let's Use ChatGPT To Write Our Paper! Benchmarking LLMs To Write the Introduction of a Research Paper | arXiv 2025 | - | - |
| `Watermarking` | [![arXiv](https://img.shields.io/badge/arXiv-2503.15772-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2503.15772)<br>Detecting LLM-Generated Peer Reviews | arXiv 2025 | - | - |
| `PaperWritingBench` | [![arXiv](https://img.shields.io/badge/arXiv-2604.05018-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.05018)<br>PaperOrchestra: A Multi-Agent Framework for Automated AI Research Paper Writing | arXiv 2026 | - | - |
||


# 8. Dissemination (Paper2X)

> :timer_clock: In chronological order, from the earliest to the latest.


### Slides & Presentations

> :timer_clock: In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `DOC2PPT` | [![arXiv](https://img.shields.io/badge/arXiv-2101.11796-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2101.11796) | AAAI 2022 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://ojs.aaai.org/index.php/AAAI/article/view/20049) | - |
| `AutoPresent` | [![arXiv](https://img.shields.io/badge/arXiv-2501.03722-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.03722) | CVPR 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openaccess.thecvf.com/content/CVPR2025/papers/Ge_AutoPresent_Designing_Structured_Visuals_from_Scratch_CVPR_2025_paper.pdf) | - |
| `PASS` | [![arXiv](https://img.shields.io/badge/arXiv-2501.06497-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.06497)<br>PASS: Presentation Automation for Slide Generation and Speech | arXiv 2025 | - | - |
| `Talk to Your Slides` | [![arXiv](https://img.shields.io/badge/arXiv-2505.11604-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.11604)<br>Talk to Your Slides: Efficient Slide Editing Agent | arXiv 2025 | - | - |
| `PPTAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2500.00000-b31b1b?style=flat-square&logo=arxiv)](https://aclanthology.org/2025.emnlp-main.832/)<br>PPTAgent: Generating and Evaluating Presentations Beyond Text-to-Slides | EMNLP 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://aclanthology.org/2025.emnlp-main.832/) | [![GitHub](https://img.shields.io/github/stars/icip-cas/PPTAgent)](https://github.com/icip-cas/PPTAgent) |
| `Auto-Slides` | [![arXiv](https://img.shields.io/badge/arXiv-2509.11062-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.11062)<br>Auto-Slides: An Interactive Multi-Agent System for Creating and Customizing Research Presentations | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://auto-slides.github.io) | - |
| `SlideGen` | [![arXiv](https://img.shields.io/badge/arXiv-2512.04529-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2512.04529)<br>SlideGen: Collaborative Multimodal Agents for Scientific Slide Generation | arXiv 2025 | - | - |
| `Paper2Slides` | - | GitHub 2025 | - | [![GitHub](https://img.shields.io/github/stars/HKUDS/Paper2Slides)](https://github.com/HKUDS/Paper2Slides) |
| `SlideTailor` | [![arXiv](https://img.shields.io/badge/arXiv-2600.00000-b31b1b?style=flat-square&logo=arxiv)](https://ojs.aaai.org/index.php/AAAI/article/view/35030)<br>SlideTailor: Personalized Presentation Slide Generation for Scientific Papers | AAAI 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://ojs.aaai.org/index.php/AAAI/article/view/35030) | [![GitHub](https://img.shields.io/github/stars/nusnlp/SlideTailor)](https://github.com/nusnlp/SlideTailor) |
| `DeepPresenter` | [![arXiv](https://img.shields.io/badge/arXiv-2602.22839-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.22839)<br>DeepPresenter: Environment-Grounded Reflection for Agentic Presentation Generation | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/icip-cas/PPTAgent)](https://github.com/icip-cas/PPTAgent) |
| `Office Raccoon (SenseTime)` | - | Web 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.sensetime.com/en/news-detail/51170569) | - |

### Posters

> :timer_clock: In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `P2P (Paper-to-Poster)` | [![arXiv](https://img.shields.io/badge/arXiv-2505.17104-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.17104)<br>P2P: Automated Paper-to-Poster Generation and Fine-Grained Benchmark | arXiv 2025 | - | - |
| `Paper2Poster` | [![arXiv](https://img.shields.io/badge/arXiv-2505.21497-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.21497)<br>Paper2Poster: Towards Multimodal Poster Automation from Scientific Papers | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/Paper2Poster/Paper2Poster)](https://github.com/Paper2Poster/Paper2Poster) |
| `PosterGen` | [![arXiv](https://img.shields.io/badge/arXiv-2508.17188-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.17188)<br>PosterGen: Aesthetic-Aware Paper-to-Poster Generation via Multi-Agent LLMs | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://Y-Research-SBU.github.io/PosterGen) | - |
| `PosterForest` | [![arXiv](https://img.shields.io/badge/arXiv-2508.21720-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2508.21720)<br>PosterForest: Hierarchical Multi-Agent Collaboration for Scientific Poster Generation | arXiv 2025 | - | - |
| `APEX` | [![arXiv](https://img.shields.io/badge/arXiv-2601.04794-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2601.04794)<br>APEX: Academic Poster Editing Agentic Expert | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/Breesiu/APEX)](https://github.com/Breesiu/APEX) |
| `PosterOmni` | [![arXiv](https://img.shields.io/badge/arXiv-2602.12127-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.12127)<br>PosterOmni: Generalized Artistic Poster Creation via Task Distillation and Unified Reward Feedback | arXiv 2026 | - | - |

### Video & Web

> :timer_clock: In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Preacher` | [![arXiv](https://img.shields.io/badge/arXiv-2500.00000-b31b1b?style=flat-square&logo=arxiv)](https://openaccess.thecvf.com/content/ICCV2025/papers/Liu_Preacher_Paper-to-Video_Agentic_System_ICCV_2025_paper.pdf)<br>Preacher: Paper-to-Video Agentic System | ICCV 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://openaccess.thecvf.com/content/ICCV2025/papers/Liu_Preacher_Paper-to-Video_Agentic_System_ICCV_2025_paper.pdf) | [![GitHub](https://img.shields.io/github/stars/Gen-Verse/Paper2Video)](https://github.com/Gen-Verse/Paper2Video) |
| `Paper2Video` | [![arXiv](https://img.shields.io/badge/arXiv-2510.05096-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.05096)<br>Paper2Video: Automatic Video Generation from Scientific Papers | arXiv 2025 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://showlab.github.io/Paper2Video/) | [![GitHub](https://img.shields.io/github/stars/showlab/Paper2Video)](https://github.com/showlab/Paper2Video) |
| `PresentAgent` | [![arXiv](https://img.shields.io/badge/arXiv-2507.04036-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2507.04036)<br>PresentAgent: Multimodal Agent for Presentation Video Generation | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/AIGeeksGroup/PresentAgent)](https://github.com/AIGeeksGroup/PresentAgent) |
| `Paper2Web` | [![arXiv](https://img.shields.io/badge/arXiv-2510.15842-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.15842)<br>Paper2Web: Let's Make Your Paper Alive! | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/YuhangChen1/Paper2All)](https://github.com/YuhangChen1/Paper2All) |
||

### Fidelity and Adoption Assessment

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `PPTEval` | [![arXiv](https://img.shields.io/badge/arXiv-2501.03936-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2501.03936)<br>PPTAgent: Generating and Evaluating Presentations Beyond Text-to-Slides | EMNLP 2025 | - | [![GitHub](https://img.shields.io/github/stars/icip-cas/PPTAgent)](https://github.com/icip-cas/PPTAgent) |
| `PresentQuiz` | [![arXiv](https://img.shields.io/badge/arXiv-2510.05096-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2510.05096)<br>Paper2Video: Automatic Video Generation from Scientific Papers | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/showlab/Paper2Video)](https://github.com/showlab/Paper2Video) |
| `PresentEval` | [![arXiv](https://img.shields.io/badge/arXiv-2507.04036-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2507.04036)<br>PresentAgent: Multimodal Agent for Presentation Video Generation | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/AIGeeksGroup/PresentAgent)](https://github.com/AIGeeksGroup/PresentAgent) |
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
| `UniScientist` | - | Web 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://unipat.ai/blog/UniScientist) | - |
| `ASI-Evolve` | - | GitHub 2026 | - | [![GitHub](https://img.shields.io/github/stars/GAIR-NLP/ASI-Evolve)](https://github.com/GAIR-NLP/ASI-Evolve) |
| `FARS` | - | Web 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://analemma.ai/blog/introducing-fars) | - |
| `AutoResearchClaw` | - | GitHub 2026 | - | [![GitHub](https://img.shields.io/github/stars/aiming-lab/AutoResearchClaw)](https://github.com/aiming-lab/AutoResearchClaw) |
| `CORAL` | [![arXiv](https://img.shields.io/badge/arXiv-2604.01658-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.01658)<br>CORAL: Towards Autonomous Multi-Agent Evolution for Open-Ended Discovery | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/Human-Agent-Society/CORAL)](https://github.com/Human-Agent-Society/CORAL) |
| `AutoSOTA` | [![arXiv](https://img.shields.io/badge/arXiv-2604.05550-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.05550)<br>AutoSOTA: An End-to-End Automated Research System for State-of-the-Art AI Model Discovery | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/tsinghua-fib-lab/AutoSOTA)](https://github.com/tsinghua-fib-lab/AutoSOTA) |
| `AiScientist-LH` | [![arXiv](https://img.shields.io/badge/arXiv-2604.13018-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2604.13018)<br>Toward Autonomous Long-Horizon Engineering for ML Research | arXiv 2026 | - | - |
| `OpenResearcher (2026)` | [![arXiv](https://img.shields.io/badge/arXiv-2603.20278-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.20278)<br>OpenResearcher: A Fully Open Pipeline for Long-Horizon Deep Research Trajectory Synthesis | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/TIGER-AI-Lab/OpenResearcher)](https://github.com/TIGER-AI-Lab/OpenResearcher) |
| `Aletheia` | [![arXiv](https://img.shields.io/badge/arXiv-2602.10177-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2602.10177)<br>Towards Autonomous Mathematics Research | arXiv 2026 | - | [![GitHub](https://img.shields.io/github/stars/google-deepmind/superhuman)](https://github.com/google-deepmind/superhuman) |
||

### Domain-Specific Systems

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `AlphaFold 3` | [![arXiv](https://img.shields.io/badge/arXiv-2400.00000-b31b1b?style=flat-square&logo=arxiv)](https://www.nature.com/articles/s41586-024-07487-w)<br>Accurate Structure Prediction of Biomolecular Interactions with AlphaFold 3 | Nature 2024 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://www.nature.com/articles/s41586-024-07487-w) | - |
| `Medical AI Scientist` | [![arXiv](https://img.shields.io/badge/arXiv-2603.28589-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2603.28589)<br>Towards a Medical AI Scientist | arXiv 2026 | - | - |
||

### Evolutionary & Self-Improving Systems

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `ShinkaEvolve` | [![arXiv](https://img.shields.io/badge/arXiv-2509.19349-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2509.19349)<br>ShinkaEvolve: Towards Open-Ended and Sample-Efficient Program Evolution | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/SakanaAI/ShinkaEvolve)](https://github.com/SakanaAI/ShinkaEvolve) |
| `Darwin Godel Machine` | [![arXiv](https://img.shields.io/badge/arXiv-2505.22954-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.22954)<br>Darwin Godel Machine: Open-Ended Evolution of Self-Improving Agents | arXiv 2025 | - | [![GitHub](https://img.shields.io/github/stars/jennyzzt/dgm)](https://github.com/jennyzzt/dgm) |
||

### Research Platforms & Infrastructure

> In chronological order, from the earliest to the latest.

| Model | Paper | Venue | Website | GitHub |
|:-:|:-|:-:|:-:|:-:|
||
| `Towards an AI co-scientist` | [![arXiv](https://img.shields.io/badge/arXiv-2502.18864-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2502.18864)<br>Towards an AI co-scientist | arXiv 2025 | - | - |
| `PiFlow` | [![arXiv](https://img.shields.io/badge/arXiv-2505.15047-b31b1b?style=flat-square&logo=arxiv)](https://arxiv.org/abs/2505.15047)<br>PiFlow: Principle-aware Scientific Discovery with Multi-Agent Collaboration | arXiv 2025 | - | - |
| `LabClaw` | - | Web 2026 | [![Website](https://img.shields.io/badge/Link-yellow?style=flat-square&logo=gitbook)](https://labclaw-ai.github.io) | - |
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


### Peer Review

| Repository | Stars | Description |
|-----------|-------|-------------|
| [paper-reviewer](https://github.com/deep-diver/paper-reviewer) | [![GitHub](https://img.shields.io/github/stars/deep-diver/paper-reviewer)](https://github.com/deep-diver/paper-reviewer) | arXiv paper reviews + blog posts |
| [ai-peer-review](https://github.com/poldrack/ai-peer-review) | [![GitHub](https://img.shields.io/github/stars/poldrack/ai-peer-review)](https://github.com/poldrack/ai-peer-review) | Multi-LLM reviews + meta-review synthesis |
| [openreviewer](https://github.com/maxidl/openreviewer) | [![GitHub](https://img.shields.io/github/stars/maxidl/openreviewer)](https://github.com/maxidl/openreviewer) | Llama-8B fine-tuned on 79K expert reviews |

<div align="center">

**[⬆ Back to Top](#awesome-ai-auto-research)**

*Last updated: 2026-04-26 · Maintained by [WorldBench](https://github.com/worldbench)*

</div>