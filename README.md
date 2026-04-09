<div align="center">

# Awesome AI Auto-Research

**A Curated List of Papers on AI-Assisted and Automated Scientific Research**

[![Survey](https://img.shields.io/badge/Survey-arXiv-b31b1b.svg)](https://arxiv.org/abs/YOUR_ARXIV_ID)
[![Project Page](https://img.shields.io/badge/Project-Page-blue.svg)](https://worldbench.github.io/awesome-auto-research)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![GitHub Stars](https://img.shields.io/github/stars/worldbench/awesome-ai-auto-research?style=social)](https://github.com/worldbench/awesome-ai-auto-research)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

</div>

---

## About

This repository accompanies the survey paper **"A Survey on AI Auto-Research"** and tracks papers on AI-assisted and automated scientific research, covering the full research pipeline — from **idea generation** and **literature review** through **coding**, **writing**, **peer review**, **rebuttal**, and **dissemination**. We also include **end-to-end autonomous research systems** and work on **societal implications**.

If you find a missing paper or a broken link, please open an issue or pull request.

---

## Citation

If you find this repository useful, please consider citing our survey paper:

```bibtex
@article{kong2026aiautoresearch,
  title   = {A Survey on {AI} Auto-Research},
  author  = {Kong, Lingdong and Chow, Wei and Li, Linfeng and Wang, Song and Li, Rong and Sun, Xian and Qu, Leigang and Ng, Lai Xing and Cottereau, Beno\^{i}t R. and Zhu, Jianke and Hoi, Steven C. H. and Liu, Ziwei and Chua, Tat-Seng and Ooi, Wei Tsang},
  journal = {arXiv preprint arXiv:YOUR\_ARXIV\_ID},
  year    = {2026}
}
```

---

## Table of Contents

- [Idea Generation](#idea-generation)
- [Literature Review & Paper Search](#literature-review--paper-search)
- [Coding & Experimentation](#coding--experimentation)
- [Tables & Figures](#tables--figures)
- [Peer Review](#peer-review)
- [Rebuttal](#rebuttal)
- [Paper Writing](#paper-writing)
- [Dissemination (Paper2X)](#dissemination-paper2x)
- [End-to-End Systems](#end-to-end-systems)
- [Societal & Critical Perspectives](#societal--critical-perspectives)
- [Surveys & Curated Lists](#surveys--curated-lists)
- [Tools & GitHub Repos](#tools--github-repos)

---

## 💡 Idea Generation

> Systems and benchmarks for automated generation, evaluation, and refinement of scientific research ideas.

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [SciMON](https://arxiv.org/abs/2305.14259) | [Paper](https://aclanthology.org/2024.acl-long.17/) | ACL'24 | [GitHub](https://github.com/EagleW/CLBD) |
| [ResearchAgent](https://github.com/JinheonBaek/ResearchAgent) | [arXiv](https://arxiv.org/abs/2404.07738) | arXiv'24 | [GitHub](https://github.com/JinheonBaek/ResearchAgent) |
| [AI Scientist](https://github.com/SakanaAI/AI-Scientist) | [arXiv](https://arxiv.org/abs/2408.06292) | arXiv'24 | [GitHub](https://github.com/SakanaAI/AI-Scientist) |
| [SciAgents](https://github.com/lamm-mit/SciAgentsDiscovery) | [arXiv](https://arxiv.org/abs/2409.05556) | arXiv'24 | [GitHub](https://github.com/lamm-mit/SciAgentsDiscovery) |
| [Can LLMs Generate Novel Research Ideas?](https://arxiv.org/abs/2409.04109) | [arXiv](https://arxiv.org/abs/2409.04109) | arXiv'24 | — |
| [MOOSE-Chem](https://arxiv.org/abs/2410.07076) | [arXiv](https://arxiv.org/abs/2410.07076) | arXiv'24 | — |
| [VirSci (Many Heads)](https://github.com/open-sciencelab/Virtual-Scientists) | [arXiv](https://arxiv.org/abs/2410.09403) | arXiv'24 | [GitHub](https://github.com/open-sciencelab/Virtual-Scientists) |
| [Chain of Ideas](https://github.com/DAMO-NLP-SG/CoI-Agent) | [arXiv](https://arxiv.org/abs/2410.13185) | arXiv'24 | [GitHub](https://github.com/DAMO-NLP-SG/CoI-Agent) |
| [Nova](https://arxiv.org/abs/2410.14255) | [arXiv](https://arxiv.org/abs/2410.14255) | arXiv'24 | — |
| [SciPIP](https://github.com/cheerss/SciPIP) | [arXiv](https://arxiv.org/abs/2410.23166) | arXiv'24 | [GitHub](https://github.com/cheerss/SciPIP) |
| [IdeaBench](https://arxiv.org/abs/2411.02429) | [arXiv](https://arxiv.org/abs/2411.02429) | arXiv'24 | — |
| [LLMs for Combinatorial Creativity](https://arxiv.org/abs/2412.14141) | [arXiv](https://arxiv.org/abs/2412.14141) | arXiv'24 | — |
| [LiveIdeaBench](https://arxiv.org/abs/2412.17596) | [arXiv](https://arxiv.org/abs/2412.17596) | arXiv'24 | — |
| [IdeaSynth](https://arxiv.org/abs/2410.04025) | [Paper](https://dl.acm.org/doi/10.1145/3706598.3713851) | CHI'25 | — |
| [IRIS](https://github.com/Anikethh/IRIS-Interactive-Research-Ideation-System) | [Paper](https://aclanthology.org/2025.acl-demo.51/) | ACL'25 | [GitHub](https://github.com/Anikethh/IRIS-Interactive-Research-Ideation-System) |
| [Multi-Agent LLM Dialogues for Ideation](https://arxiv.org/abs/2411.12422) | [Paper](https://aclanthology.org/2025.sigdial-1.24/) | SIGDIAL'25 | — |
| [Spark](https://arxiv.org/abs/2504.20090) | [Paper](https://arxiv.org/abs/2504.20090) | ICCC'25 | — |
| [ResearchBench](https://arxiv.org/abs/2503.21248) | [arXiv](https://arxiv.org/abs/2503.21248) | arXiv'25 | — |
| [AI Idea Bench 2025](https://github.com/ai-idea-bench/ai-idea-bench.github.io) | [arXiv](https://arxiv.org/abs/2504.14191) | arXiv'25 | [GitHub](https://github.com/yansheng-qiu/AI_Idea_Bench_2025) |
| [AI Scientist v2](https://github.com/SakanaAI/AI-Scientist-v2) | [arXiv](https://arxiv.org/abs/2504.08066) | arXiv'25 | [GitHub](https://github.com/SakanaAI/AI-Scientist-v2) |
| [AI-Researcher](https://arxiv.org/abs/2505.18705) | [arXiv](https://arxiv.org/abs/2505.18705) | arXiv'25 | — |
| [MOOSE-Chem2](https://arxiv.org/abs/2505.19209) | [arXiv](https://arxiv.org/abs/2505.19209) | arXiv'25 | — |
| [The Ideation-Execution Gap](https://arxiv.org/abs/2506.20803) | [arXiv](https://arxiv.org/abs/2506.20803) | arXiv'25 | — |
| [Deep Ideation](https://github.com/kyZhao-1/Deep-Ideation) | [arXiv](https://arxiv.org/abs/2511.02238) | arXiv'25 | [GitHub](https://github.com/kyZhao-1/Deep-Ideation) |
| [Kosmos](https://arxiv.org/abs/2511.02824) | [arXiv](https://arxiv.org/abs/2511.02824) | arXiv'25 | — |
| [HeurekaBench](https://brbiclab.epfl.ch/projects/heurekabench/) | [Paper](https://openreview.net/forum?id=YOUR_ID) | ICLR'26 | [GitHub](https://github.com/mlbio-epfl/HeurekaBench) |
| [Why LLMs Aren't Scientists Yet](https://arxiv.org/abs/2601.03315) | [arXiv](https://arxiv.org/abs/2601.03315) | arXiv'26 | — |
| [Literature-Driven Scientific Theories](https://arxiv.org/abs/2601.16282) | [arXiv](https://arxiv.org/abs/2601.16282) | arXiv'26 | — |
| [AI Can Learn Scientific Taste](https://arxiv.org/abs/2603.14473) | [arXiv](https://arxiv.org/abs/2603.14473) | arXiv'26 | — |
| [EvoIdeator](https://arxiv.org/abs/2603.21728) | [arXiv](https://arxiv.org/abs/2603.21728) | arXiv'26 | — |
| [HindSight](https://arxiv.org/abs/2603.15164) | [arXiv](https://arxiv.org/abs/2603.15164) | arXiv'26 | — |

---

## 🔍 Literature Review & Paper Search

> Tools and benchmarks for automated literature search, synthesis, and survey generation.

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [ASReview](https://asreview.nl) | [Paper](https://www.nature.com/articles/s42256-020-00287-7) | Nature MI'21 | [GitHub](https://github.com/asreview/asreview) |
| [PaperQA](https://github.com/Future-House/paper-qa) | [arXiv](https://arxiv.org/abs/2312.07559) | arXiv'23 | [GitHub](https://github.com/Future-House/paper-qa) |
| [LitLLM](https://litllm.github.io) | [arXiv](https://arxiv.org/abs/2402.01788) | arXiv'24 | — |
| [STORM](https://github.com/stanford-oval/storm) | [arXiv](https://arxiv.org/abs/2402.14207) | arXiv'24 | [GitHub](https://github.com/stanford-oval/storm) |
| [OpenResearcher (2024)](https://arxiv.org/abs/2408.09578) | [Paper](https://aclanthology.org/2024.emnlp-demo.24/) | EMNLP'24 | — |
| [CHIME](https://arxiv.org/abs/2407.16148) | [arXiv](https://arxiv.org/abs/2407.16148) | arXiv'24 | — |
| [CiteME](https://arxiv.org/abs/2407.12861) | [arXiv](https://arxiv.org/abs/2407.12861) | arXiv'24 | — |
| [LitSearch](https://github.com/princeton-nlp/LitSearch) | [arXiv](https://arxiv.org/abs/2407.18940) | arXiv'24 | [GitHub](https://github.com/princeton-nlp/LitSearch) |
| [PaperQA2](https://arxiv.org/abs/2409.13740) | [arXiv](https://arxiv.org/abs/2409.13740) | arXiv'24 | [GitHub](https://github.com/Future-House/paper-qa) |
| [AutoSurvey](https://github.com/AutoSurveys/AutoSurvey) | [arXiv](https://arxiv.org/abs/2406.10252) | arXiv'24 | [GitHub](https://github.com/AutoSurveys/AutoSurvey) |
| [OpenScholar](https://arxiv.org/abs/2411.14199) | [arXiv](https://arxiv.org/abs/2411.14199) | arXiv'24 | — |
| [GPT Researcher](https://github.com/assafelovic/gpt-researcher) | — | GitHub'24 | [GitHub](https://github.com/assafelovic/gpt-researcher) |
| [LLMs for Automated Literature Review](https://arxiv.org/abs/2412.13612) | [arXiv](https://arxiv.org/abs/2412.13612) | arXiv'24 | — |
| [Elicit](https://elicit.com) | — | Web'24 | — |
| [Semantic Scholar](https://www.semanticscholar.org) | — | Web'24 | — |
| [PaSa](https://github.com/bytedance/pasa) | [arXiv](https://arxiv.org/abs/2501.10120) | arXiv'25 | [GitHub](https://github.com/bytedance/pasa) |
| [SurveyX](http://www.surveyx.cn) | [arXiv](https://arxiv.org/abs/2502.14776) | arXiv'25 | — |
| [SurveyForge](https://github.com/Alpha-Innovator/SurveyForge) | [arXiv](https://arxiv.org/abs/2503.04629) | arXiv'25 | [GitHub](https://github.com/Alpha-Innovator/SurveyForge) |
| [CiteGeist](https://citegeist.org) | [arXiv](https://arxiv.org/abs/2503.23229) | arXiv'25 | — |
| [DeepResearchAgent](https://github.com/SkyworkAI/DeepResearchAgent) | — | GitHub'25 | [GitHub](https://github.com/SkyworkAI/DeepResearchAgent) |
| [DeerFlow](https://github.com/bytedance/deer-flow) | — | GitHub'25 | [GitHub](https://github.com/bytedance/deer-flow) |
| [Tongyi DeepResearch](https://github.com/Alibaba-NLP/DeepResearch) | — | GitHub'25 | [GitHub](https://github.com/Alibaba-NLP/DeepResearch) |
| [Agentic AutoSurvey](https://arxiv.org/abs/2509.18661) | [arXiv](https://arxiv.org/abs/2509.18661) | arXiv'25 | — |
| [LiRA](https://arxiv.org/abs/2510.05138) | [arXiv](https://arxiv.org/abs/2510.05138) | arXiv'25 | — |
| [SurveyG](https://arxiv.org/abs/2510.07733) | [arXiv](https://arxiv.org/abs/2510.07733) | arXiv'25 | — |
| [IterSurvey](https://github.com/HancCui/IterSurvey_Autosurveyv2) | [arXiv](https://arxiv.org/abs/2510.21900) | arXiv'25 | [GitHub](https://github.com/HancCui/IterSurvey_Autosurveyv2) |
| [ReportBench](https://github.com/ByteDance-BandAI/ReportBench) | [arXiv](https://arxiv.org/abs/2508.15804) | arXiv'25 | [GitHub](https://github.com/ByteDance-BandAI/ReportBench) |
| [DeepScholar-Bench](https://github.com/guestrin-lab/deepscholar-bench) | [arXiv](https://arxiv.org/abs/2508.20033) | arXiv'25 | [GitHub](https://github.com/guestrin-lab/deepscholar-bench) |
| [IDRBench](https://arxiv.org/abs/2601.06676) | [arXiv](https://arxiv.org/abs/2601.06676) | arXiv'26 | — |
| [CiteLLM](https://arxiv.org/abs/2602.23075) | [arXiv](https://arxiv.org/abs/2602.23075) | arXiv'26 | — |
| [O-Researcher](https://arxiv.org/abs/2601.03743) | [arXiv](https://arxiv.org/abs/2601.03743) | arXiv'26 | — |
| [ScholarGym](https://arxiv.org/abs/2601.21654) | [arXiv](https://arxiv.org/abs/2601.21654) | arXiv'26 | — |
| [SciNetBench](https://arxiv.org/abs/2601.03260) | [arXiv](https://arxiv.org/abs/2601.03260) | arXiv'26 | — |

---

## 🧪 Coding & Experimentation

> Agents and benchmarks for AI-driven coding, experimentation, hypothesis testing, and scientific software engineering.

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [BioPlanner](https://github.com/bioplanner/bioplanner) | [arXiv](https://arxiv.org/abs/2310.10632) | arXiv'23 | [GitHub](https://github.com/bioplanner/bioplanner) |
| [Coscientist](https://www.nature.com/articles/s41586-023-06792-0) | [Paper](https://www.nature.com/articles/s41586-023-06792-0) | Nature'23 | — |
| [MLAgentBench](https://github.com/snap-stanford/MLAgentBench) | [arXiv](https://arxiv.org/abs/2310.03302) | arXiv'24 | [GitHub](https://github.com/snap-stanford/MLAgentBench) |
| [DS-Agent](https://github.com/guosyjlu/DS-Agent) | [arXiv](https://arxiv.org/abs/2402.17453) | arXiv'24 | [GitHub](https://github.com/guosyjlu/DS-Agent) |
| [ChemCrow](https://www.nature.com/articles/s42256-024-00832-8) | [Paper](https://www.nature.com/articles/s42256-024-00832-8) | Nature MI'24 | — |
| [CRISPR-GPT](https://arxiv.org/abs/2404.18021) | [arXiv](https://arxiv.org/abs/2404.18021) | arXiv'24 | — |
| [FunSearch](https://www.nature.com/articles/s41586-023-06924-6) | [Paper](https://www.nature.com/articles/s41586-023-06924-6) | Nature'24 | [GitHub](https://github.com/google-deepmind/funsearch) |
| [DiscoveryWorld](https://github.com/allenai/discoveryworld) | [arXiv](https://arxiv.org/abs/2406.06769) | arXiv'24 | [GitHub](https://github.com/allenai/discoveryworld) |
| [SciCode](https://scicode-bench.github.io) | [arXiv](https://arxiv.org/abs/2407.13168) | arXiv'24 | [GitHub](https://github.com/scicode-bench/SciCode) |
| [DiscoveryBench](https://github.com/allenai/discoverybench) | [arXiv](https://arxiv.org/abs/2407.01725) | arXiv'24 | [GitHub](https://github.com/allenai/discoverybench) |
| [Lab-Bench](https://huggingface.co/datasets/futurehouse/lab-bench) | [arXiv](https://arxiv.org/abs/2407.10362) | arXiv'24 | — |
| [InfiAgent-DABench](https://arxiv.org/abs/2401.05507) | [arXiv](https://arxiv.org/abs/2401.05507) | arXiv'24 | — |
| [MLR-Copilot](https://arxiv.org/abs/2408.14033) | [arXiv](https://arxiv.org/abs/2408.14033) | arXiv'24 | — |
| [SWE-Bench](https://github.com/princeton-nlp/SWE-bench) | [Paper](https://openreview.net/forum?id=VTF8yNQM66) | ICLR'24 | [GitHub](https://github.com/princeton-nlp/SWE-bench) |
| [ScienceAgentBench](https://arxiv.org/abs/2410.05080) | [arXiv](https://arxiv.org/abs/2410.05080) | arXiv'24 | — |
| [RE-Bench](https://arxiv.org/abs/2411.15114) | [arXiv](https://arxiv.org/abs/2411.15114) | arXiv'24 | — |
| [autoresearch (Karpathy)](https://github.com/karpathy/autoresearch) | — | GitHub'25 | [GitHub](https://github.com/karpathy/autoresearch) |
| [AI Scientist (code)](https://github.com/SakanaAI/AI-Scientist) | — | GitHub'24 | [GitHub](https://github.com/SakanaAI/AI-Scientist) |
| [Dolphin](https://alpha-innovator.github.io/Dolphin-project-page) | [arXiv](https://arxiv.org/abs/2501.03916) | arXiv'25 | — |
| [AIDE](https://arxiv.org/abs/2502.13138) | [arXiv](https://arxiv.org/abs/2502.13138) | arXiv'25 | — |
| [Curie](https://github.com/Just-Curieous/Curie) | [arXiv](https://arxiv.org/abs/2502.16069) | arXiv'25 | [GitHub](https://github.com/Just-Curieous/Curie) |
| [MLGym](https://arxiv.org/abs/2502.14499) | [arXiv](https://arxiv.org/abs/2502.14499) | arXiv'25 | — |
| [CodeScientist](https://github.com/allenai/codescientist) | [arXiv](https://arxiv.org/abs/2503.22708) | arXiv'25 | [GitHub](https://github.com/allenai/codescientist) |
| [SciReplicate-Bench](https://xyzcs.github.io/scireplicate.github.io/) | [arXiv](https://arxiv.org/abs/2504.00255) | arXiv'25 | [GitHub](https://github.com/xyzCS/SciReplicate-Bench) |
| [PaperBench](https://github.com/openai/preparedness) | [arXiv](https://arxiv.org/abs/2504.01848) | arXiv'25 | [GitHub](https://github.com/openai/preparedness) |
| [Paper2Code](https://github.com/going-doer/Paper2Code) | [arXiv](https://arxiv.org/abs/2504.17192) | arXiv'25 | [GitHub](https://github.com/going-doer/Paper2Code) |
| [AutoReproduce](https://github.com/AI9Stars/AutoReproduce) | [arXiv](https://arxiv.org/abs/2505.20662) | arXiv'25 | [GitHub](https://github.com/AI9Stars/AutoReproduce) |
| [R&D-Agent](https://github.com/microsoft/RD-Agent) | [arXiv](https://arxiv.org/abs/2505.14738) | arXiv'25 | [GitHub](https://github.com/microsoft/RD-Agent) |
| [InternAgent / NovelSeek](https://alpha-innovator.github.io/InternAgent-project-page) | [arXiv](https://arxiv.org/abs/2505.16938) | arXiv'25 | [GitHub](https://github.com/Alpha-Innovor/InternAgent) |
| [AlphaEvolve](https://arxiv.org/abs/2506.13131) | [arXiv](https://arxiv.org/abs/2506.13131) | arXiv'25 | — |
| [ResearchCodeBench](https://arxiv.org/abs/2506.02314) | [arXiv](https://arxiv.org/abs/2506.02314) | arXiv'25 | — |
| [SWE-Bench Pro](https://arxiv.org/abs/2509.16941) | [arXiv](https://arxiv.org/abs/2509.16941) | arXiv'25 | — |
| [MLR-Bench](https://arxiv.org/abs/2505.19955) | [arXiv](https://arxiv.org/abs/2505.19955) | arXiv'25 | — |
| [SWE-EVO](https://arxiv.org/abs/2512.18470) | [arXiv](https://arxiv.org/abs/2512.18470) | arXiv'25 | — |
| [Execution-Grounded AI Research](https://arxiv.org/abs/2601.14525) | [arXiv](https://arxiv.org/abs/2601.14525) | arXiv'26 | — |
| [SciNav](https://arxiv.org/abs/2603.20256) | [arXiv](https://arxiv.org/abs/2603.20256) | arXiv'26 | — |
| [EvoScientist](https://evoscientist.ai) | [arXiv](https://arxiv.org/abs/2603.08127) | arXiv'26 | [GitHub](https://github.com/evoscientist/evoscientist) |

---

## 📊 Tables & Figures

> Systems for automated generation of scientific tables, charts, figures, TikZ diagrams, and visualizations.

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [ChartGPT](https://arxiv.org/abs/2311.01920) | [arXiv](https://arxiv.org/abs/2311.01920) | arXiv'23 | — |
| [Chain-of-Table](https://arxiv.org/abs/2401.04398) | [arXiv](https://arxiv.org/abs/2401.04398) | arXiv'24 | — |
| [MatPlotAgent](https://arxiv.org/abs/2402.11453) | [arXiv](https://arxiv.org/abs/2402.11453) | arXiv'24 | — |
| [AutomaTikZ](https://arxiv.org/abs/2310.00367) | [Paper](https://openreview.net/forum?id=v3K5TVP8kZ) | ICLR'24 | — |
| [ArxivDIGESTables](https://arxiv.org/abs/2310.14324) | [Paper](https://aclanthology.org/2024.emnlp-main.542/) | EMNLP'24 | — |
| [DeTikZify](https://arxiv.org/abs/2405.15306) | [Paper](https://papers.nips.cc/paper_files/paper/2024/hash/a5ace289f4e2c70b48b31ba15ac82ecd-Abstract-Conference.html) | NeurIPS'24 | — |
| [DiagramAgent](https://arxiv.org/abs/2401.17464) | [Paper](https://openaccess.thecvf.com/content/CVPR2025/papers/Wei_From_Words_to_Structured_Visuals_A_Benchmark_and_Framework_for_CVPR_2025_paper.pdf) | CVPR'25 | — |
| [AbGen](https://arxiv.org/abs/2406.06357) | [Paper](https://aclanthology.org/2025.acl-long.670/) | ACL'25 | — |
| [StarVector](https://arxiv.org/abs/2312.11556) | [Paper](https://openaccess.thecvf.com/content/CVPR2025/papers/Rodriguez_StarVector_Generating_Scalable_Vector_Graphics_Code_from_Images_CVPR_2025_paper.pdf) | CVPR'25 | — |
| [VisCoder](https://arxiv.org/abs/2407.04793) | [Paper](https://aclanthology.org/2025.findings-emnlp.167/) | EMNLP Findings'25 | — |
| [PlotGen](https://arxiv.org/abs/2502.00988) | [arXiv](https://arxiv.org/abs/2502.00988) | arXiv'25 | — |
| [CoDA](https://arxiv.org/abs/2510.03194) | [arXiv](https://arxiv.org/abs/2510.03194) | arXiv'25 | — |
| [PlotCraft](https://arxiv.org/abs/2511.00010) | [arXiv](https://arxiv.org/abs/2511.00010) | arXiv'25 | — |
| [ShowTable](https://arxiv.org/abs/2512.13303) | [arXiv](https://arxiv.org/abs/2512.13303) | arXiv'25 | — |
| [Table2LaTeX-RL](https://arxiv.org/abs/2509.17589) | [arXiv](https://arxiv.org/abs/2509.17589) | arXiv'25 | — |
| [VIS-Shepherd](https://arxiv.org/abs/2506.13326) | [arXiv](https://arxiv.org/abs/2506.13326) | arXiv'25 | — |
| [TeXpert](https://arxiv.org/abs/2506.16990) | [arXiv](https://arxiv.org/abs/2506.16990) | arXiv'25 | — |
| [PaperBanana](https://arxiv.org/abs/2601.23265) | [arXiv](https://arxiv.org/abs/2601.23265) | arXiv'26 | — |
| [SciFig](https://arxiv.org/abs/2601.04390) | [arXiv](https://arxiv.org/abs/2601.04390) | arXiv'26 | — |
| [SciFlow-Bench](https://arxiv.org/abs/2602.09809) | [arXiv](https://arxiv.org/abs/2602.09809) | arXiv'26 | — |
| [AutoFigure-Edit](https://deepscientist.cc) | [arXiv](https://arxiv.org/abs/2603.06674) | arXiv'26 | [GitHub](https://github.com/ResearAI/AutoFigure-Edit) |
| [SAIL](https://arxiv.org/abs/2603.18145) | [arXiv](https://arxiv.org/abs/2603.18145) | arXiv'26 | — |
| [TikZilla](https://arxiv.org/abs/2603.03072) | [arXiv](https://arxiv.org/abs/2603.03072) | arXiv'26 | — |
| [AI-Generated Figures: Policies & Guidelines](https://arxiv.org/abs/2603.16159) | [arXiv](https://arxiv.org/abs/2603.16159) | arXiv'26 | — |

---

## 🔬 Peer Review

> Automated peer review generation, analysis of AI usage in review, and bias/robustness studies.

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [MARG](https://arxiv.org/abs/2401.04259) | [arXiv](https://arxiv.org/abs/2401.04259) | arXiv'24 | — |
| [AI Review Lottery](https://arxiv.org/abs/2405.02150) | [arXiv](https://arxiv.org/abs/2405.02150) | arXiv'24 | — |
| [Monitoring AI-Modified Content](https://arxiv.org/abs/2403.07183) | [arXiv](https://arxiv.org/abs/2403.07183) | arXiv'24 | — |
| [Peer Review as Multi-Turn Dialogue](https://arxiv.org/abs/2406.05688) | [arXiv](https://arxiv.org/abs/2406.05688) | arXiv'24 | — |
| [AI-Peer-Review](https://github.com/poldrack/ai-peer-review) | — | GitHub'24 | [GitHub](https://github.com/poldrack/ai-peer-review) |
| [AgentReview](https://arxiv.org/abs/2406.12708) | [Paper](https://aclanthology.org/2024.emnlp-main.70/) | EMNLP'24 | — |
| [LLMs as Meta-Reviewers' Assistants](https://arxiv.org/abs/2402.15589) | [Paper](https://aclanthology.org/2025.naacl-long.455/) | NAACL'25 | — |
| [AI Text Detection in Peer Review](https://arxiv.org/abs/2502.19614) | [arXiv](https://arxiv.org/abs/2502.19614) | arXiv'25 | — |
| [DeepReview](https://ai-researcher.net) | [arXiv](https://arxiv.org/abs/2503.08569) | arXiv'25 | — |
| [ClaimCheck](https://arxiv.org/abs/2503.21717) | [arXiv](https://arxiv.org/abs/2503.21717) | arXiv'25 | — |
| [ReviewAgents](https://arxiv.org/abs/2503.08506) | [arXiv](https://arxiv.org/abs/2503.08506) | arXiv'25 | — |
| [OpenReviewer](https://huggingface.co/spaces/idahl/OpenReviewer) | [arXiv](https://arxiv.org/abs/2412.11948) | arXiv'25 | — |
| [REMOR](https://arxiv.org/abs/2505.11718) | [arXiv](https://arxiv.org/abs/2505.11718) | arXiv'25 | — |
| [Detecting LLM-Generated Peer Reviews](https://arxiv.org/abs/2503.15772) | [arXiv](https://arxiv.org/abs/2503.15772) | arXiv'25 | — |
| [Automated Scientific Reviewing (Stanford)](https://paperreview.ai/tech-overview) | — | Web'25 | — |
| [Breaking the Reviewer](https://arxiv.org/abs/2506.11113) | [arXiv](https://arxiv.org/abs/2506.11113) | arXiv'25 | — |
| [Prompt Injection Attacks on Peer Review](https://arxiv.org/abs/2509.10248) | [arXiv](https://arxiv.org/abs/2509.10248) | arXiv'25 | — |
| [When Your Reviewer is an LLM](https://arxiv.org/abs/2509.09912) | [arXiv](https://arxiv.org/abs/2509.09912) | arXiv'25 | — |
| [CycleResearcher](https://wengsyx.github.io/Researcher/) | [arXiv](https://arxiv.org/abs/2411.00816) | arXiv'25 | — |
| [Automatic Paper Reviewing with Graph Reasoning](https://arxiv.org/abs/2511.08317) | [arXiv](https://arxiv.org/abs/2511.08317) | arXiv'25 | — |
| [ReviewerToo](https://arxiv.org/abs/2510.08867) | [arXiv](https://arxiv.org/abs/2510.08867) | arXiv'25 | — |
| [ReviewRL](https://arxiv.org/abs/2504.13690) | [Paper](https://aclanthology.org/2025.emnlp-main.949/) | EMNLP'25 | — |
| [Large-Scale Randomized Study of LLM Feedback](https://www.nature.com/articles/s42256-025-01004-5) | [Paper](https://www.nature.com/articles/s42256-025-01004-5) | Nature MI'26 | — |
| [RATE](https://arxiv.org/abs/2601.19637) | [arXiv](https://arxiv.org/abs/2601.19637) | arXiv'26 | — |
| [What Happens When Reviewers Receive AI Feedback](https://arxiv.org/abs/2602.13817) | [arXiv](https://arxiv.org/abs/2602.13817) | arXiv'26 | — |
| [Policies Permitting LLM Use Not Enforceable](https://arxiv.org/abs/2603.20450) | [arXiv](https://arxiv.org/abs/2603.20450) | arXiv'26 | — |
| [More than Half of Researchers Use AI for Peer Review](https://www.nature.com/articles/d41586-026-00159-z) | [Paper](https://www.nature.com/articles/d41586-026-00159-z) | Nature News'26 | — |
| [Major Conference Catches Illicit AI Use](https://www.nature.com/articles/d41586-026-00866-7) | [Paper](https://www.nature.com/articles/d41586-026-00866-7) | Nature News'26 | — |

---

## 💬 Rebuttal

> Systems and datasets for AI-assisted author rebuttals and response generation in the peer review process.

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [Re2 Dataset](https://arxiv.org/abs/2505.07920) | [arXiv](https://arxiv.org/abs/2505.07920) | arXiv'25 | — |
| [Insights from ICLR Rebuttal Process](https://arxiv.org/abs/2511.15462) | [arXiv](https://arxiv.org/abs/2511.15462) | arXiv'25 | — |
| [DRPG](https://github.com/ulab-uiuc/DRPG-RebuttalAgent) | [arXiv](https://arxiv.org/abs/2601.18081) | arXiv'26 | [GitHub](https://github.com/ulab-uiuc/DRPG-RebuttalAgent) |
| [Paper2Rebuttal](https://mqleet.github.io/Paper2Rebuttal_ProjectPage/) | [arXiv](https://arxiv.org/abs/2601.14171) | arXiv'26 | — |
| [RebuttalAgent](https://arxiv.org/abs/2601.15715) | [arXiv](https://arxiv.org/abs/2601.15715) | arXiv'26 | — |
| [Author-in-the-Loop](https://arxiv.org/abs/2602.11173) | [arXiv](https://arxiv.org/abs/2602.11173) | arXiv'26 | — |
| [Commitment Checklist](https://arxiv.org/abs/2603.00003) | [arXiv](https://arxiv.org/abs/2603.00003) | arXiv'26 | — |

---

## ✍️ Paper Writing

> Tools and studies on AI assistance for academic writing, revision, citation, and co-authorship.

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [CoAuthor](https://arxiv.org/abs/2201.06796) | [arXiv](https://arxiv.org/abs/2201.06796) | arXiv'22 | — |
| [CycleResearcher](https://wengsyx.github.io/Researcher/) | [arXiv](https://arxiv.org/abs/2411.00816) | arXiv'24 | — |
| [Script&Shift](https://arxiv.org/abs/2502.07440) | [Paper](https://dl.acm.org/doi/10.1145/3706598.3713882) | CHI'25 | — |
| [AI in the Writing Process](https://arxiv.org/abs/2503.10000) | [Paper](https://link.springer.com/chapter/10.1007/978-3-031-64315-6_14) | AIED'25 | — |
| [FutureGen](https://arxiv.org/abs/2503.16561) | [arXiv](https://arxiv.org/abs/2503.16561) | arXiv'25 | — |
| [ScholarCopilot](https://arxiv.org/abs/2504.00824) | [arXiv](https://arxiv.org/abs/2504.00824) | arXiv'25 | — |
| [OpenDraft](https://github.com/federicodeponte/opendraft) | — | GitHub'25 | [GitHub](https://github.com/federicodeponte/opendraft) |
| [DraftMarks](https://arxiv.org/abs/2509.23505) | [arXiv](https://arxiv.org/abs/2509.23505) | arXiv'25 | — |
| [XtraGPT](https://arxiv.org/abs/2505.11336) | [arXiv](https://arxiv.org/abs/2505.11336) | arXiv'25 | — |
| [Let's Use ChatGPT to Write Our Paper!](https://arxiv.org/abs/2508.14273) | [arXiv](https://arxiv.org/abs/2508.14273) | arXiv'25 | — |
| [PaperDebugger](https://github.com/PaperDebugger/PaperDebugger) | [arXiv](https://arxiv.org/abs/2512.02589) | arXiv'25 | [GitHub](https://github.com/PaperDebugger/PaperDebugger) |
| [AI Tools Expand Impact but Contract Focus](https://www.nature.com/articles/s41586-025-08681-8) | [Paper](https://www.nature.com/articles/s41586-025-08681-8) | Nature'26 | — |
| [APRES](https://arxiv.org/abs/2603.03142) | [arXiv](https://arxiv.org/abs/2603.03142) | arXiv'26 | — |
| [Multi-Agent LLMs for Research Limitations](https://arxiv.org/abs/2601.11578) | [arXiv](https://arxiv.org/abs/2601.11578) | arXiv'26 | — |

---

## 📢 Dissemination (Paper2X)

> Systems that transform research papers into slides, posters, videos, websites, and other presentation formats.

### 📑 Slides & Presentations

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [DOC2PPT](https://arxiv.org/abs/2101.11796) | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/20049) | AAAI'22 | — |
| [AutoPresent](https://arxiv.org/abs/2501.03722) | [Paper](https://openaccess.thecvf.com/content/CVPR2025/papers/Ge_AutoPresent_Designing_Structured_Visuals_from_Scratch_CVPR_2025_paper.pdf) | CVPR'25 | — |
| [PASS](https://arxiv.org/abs/2501.06497) | [arXiv](https://arxiv.org/abs/2501.06497) | arXiv'25 | — |
| [Talk to Your Slides](https://arxiv.org/abs/2505.11604) | [arXiv](https://arxiv.org/abs/2505.11604) | arXiv'25 | — |
| [PPTAgent](https://github.com/icip-cas/PPTAgent) | [Paper](https://aclanthology.org/2025.emnlp-main.832/) | EMNLP'25 | [GitHub](https://github.com/icip-cas/PPTAgent) |
| [PresentAgent](https://github.com/AIGeeksGroup/PresentAgent) | [arXiv](https://arxiv.org/abs/2507.04036) | arXiv'25 | [GitHub](https://github.com/AIGeeksGroup/PresentAgent) |
| [Auto-Slides](https://auto-slides.github.io) | [arXiv](https://arxiv.org/abs/2509.11062) | arXiv'25 | — |
| [SlideGen](https://arxiv.org/abs/2512.04529) | [arXiv](https://arxiv.org/abs/2512.04529) | arXiv'25 | — |
| [Paper2Slides](https://github.com/HKUDS/Paper2Slides) | — | GitHub'25 | [GitHub](https://github.com/HKUDS/Paper2Slides) |
| [SlideTailor](https://github.com/nusnlp/SlideTailor) | [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/35030) | AAAI'26 | [GitHub](https://github.com/nusnlp/SlideTailor) |
| [DeepPresenter](https://arxiv.org/abs/2602.22839) | [arXiv](https://arxiv.org/abs/2602.22839) | arXiv'26 | [GitHub](https://github.com/icip-cas/PPTAgent) |
| [Office Raccoon (SenseTime)](https://www.sensetime.com/en/news-detail/51170569) | — | Web'26 | — |

### 🗺️ Posters

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [P2P (Paper-to-Poster)](https://arxiv.org/abs/2505.17104) | [arXiv](https://arxiv.org/abs/2505.17104) | arXiv'25 | — |
| [Paper2Poster](https://github.com/Paper2Poster/Paper2Poster) | [arXiv](https://arxiv.org/abs/2505.21497) | arXiv'25 | [GitHub](https://github.com/Paper2Poster/Paper2Poster) |
| [PosterGen](https://Y-Research-SBU.github.io/PosterGen) | [arXiv](https://arxiv.org/abs/2508.17188) | arXiv'25 | — |
| [PosterForest](https://arxiv.org/abs/2508.21720) | [arXiv](https://arxiv.org/abs/2508.21720) | arXiv'25 | — |
| [APEX](https://github.com/Breesiu/APEX) | [arXiv](https://arxiv.org/abs/2601.04794) | arXiv'26 | [GitHub](https://github.com/Breesiu/APEX) |
| [PosterOmni](https://arxiv.org/abs/2602.12127) | [arXiv](https://arxiv.org/abs/2602.12127) | arXiv'26 | — |

### 🎬 Video & Web

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [Preacher](https://github.com/Gen-Verse/Paper2Video) | [Paper](https://openaccess.thecvf.com/content/ICCV2025/papers/Liu_Preacher_Paper-to-Video_Agentic_System_ICCV_2025_paper.pdf) | ICCV'25 | [GitHub](https://github.com/Gen-Verse/Paper2Video) |
| [Paper2Video](https://showlab.github.io/Paper2Video/) | [arXiv](https://arxiv.org/abs/2510.05096) | arXiv'25 | [GitHub](https://github.com/showlab/Paper2Video) |
| [Paper2Web](https://github.com/YuhangChen1/Paper2All) | [arXiv](https://arxiv.org/abs/2510.15842) | arXiv'25 | [GitHub](https://github.com/YuhangChen1/Paper2All) |

---

## 🤖 End-to-End Systems

> Fully integrated autonomous research pipelines that span multiple stages of the scientific process.

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [ResearchTown](https://github.com/ulab-uiuc/research-town) | [Paper](https://proceedings.mlr.press/v267/yu25a.html) | ICML'25 | [GitHub](https://github.com/ulab-uiuc/research-town) |
| [Agent Laboratory](https://arxiv.org/abs/2501.04227) | [arXiv](https://arxiv.org/abs/2501.04227) | arXiv'25 | — |
| [Towards an AI co-scientist](https://arxiv.org/abs/2502.18864) | [arXiv](https://arxiv.org/abs/2502.18864) | arXiv'25 | — |
| [OpenAI Deep Research](https://openai.com/index/deep-research) | — | Web'25 | — |
| [Google Deep Research](https://blog.google/products/gemini/google-gemini-deep-research) | — | Web'25 | — |
| [AgentRxiv](https://arxiv.org/abs/2503.18102) | [arXiv](https://arxiv.org/abs/2503.18102) | arXiv'25 | — |
| [AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs) | — | GitHub'25 | [GitHub](https://github.com/Orchestra-Research/AI-Research-SKILLs) |
| [Biomni](https://github.com/snap-stanford/Biomni) | — | GitHub'25 | [GitHub](https://github.com/snap-stanford/Biomni) |
| [Idea2Paper](https://github.com/AgentAlphaAGI/Idea2Paper) | — | GitHub'25 | [GitHub](https://github.com/AgentAlphaAGI/Idea2Paper) |
| [ResearchClaw](https://github.com/ymx10086/ResearchClaw) | — | GitHub'25 | [GitHub](https://github.com/ymx10086/ResearchClaw) |
| [ARIS](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep) | — | GitHub'25 | [GitHub](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep) |
| [PiFlow](https://arxiv.org/abs/2505.15047) | [arXiv](https://arxiv.org/abs/2505.15047) | arXiv'25 | — |
| [Towards End-to-End Automation of AI Research](https://www.nature.com/articles/s41586-026-08420-7) | [Paper](https://www.nature.com/articles/s41586-026-08420-7) | Nature'26 | [GitHub](https://github.com/SakanaAI/AI-Scientist) |
| [Idea2Story](https://arxiv.org/abs/2601.20833) | [arXiv](https://arxiv.org/abs/2601.20833) | arXiv'26 | — |
| [LabClaw](https://labclaw-ai.github.io) | — | Web'26 | — |
| [UniScientist](https://unipat.ai/blog/UniScientist) | — | Web'26 | — |
| [ASI-Evolve](https://github.com/GAIR-NLP/ASI-Evolve) | — | GitHub'26 | [GitHub](https://github.com/GAIR-NLP/ASI-Evolve) |
| [FARS](https://analemma.ai/blog/introducing-fars) | — | Web'26 | — |
| [AutoResearchClaw](https://github.com/aiming-lab/AutoResearchClaw) | — | GitHub'26 | [GitHub](https://github.com/aiming-lab/AutoResearchClaw) |
| [OpenResearcher (2026)](https://github.com/TIGER-AI-Lab/OpenResearcher) | [arXiv](https://arxiv.org/abs/2603.20278) | arXiv'26 | [GitHub](https://github.com/TIGER-AI-Lab/OpenResearcher) |
| [Aletheia](https://arxiv.org/abs/2602.10177) | [arXiv](https://arxiv.org/abs/2602.10177) | arXiv'26 | [GitHub](https://github.com/google-deepmind/superhuman/tree/main/aletheia) |
| [OpenAI Is Building a Fully Automated Researcher](https://www.technologyreview.com/2026/03/20/1134438/openai-is-throwing-everything-into-building-a-fully-automated-researcher) | [Article](https://www.technologyreview.com/2026/03/20/1134438/openai-is-throwing-everything-into-building-a-fully-automated-researcher) | MIT TR'26 | — |

---

## 🌐 Societal & Critical Perspectives

> Studies on the societal implications, risks, integrity concerns, and broader impacts of AI in scientific research.

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [Navigating the Jagged Technological Frontier](https://pubsonline.informs.org/doi/10.1287/orsc.2023.1745) | [Paper](https://pubsonline.informs.org/doi/10.1287/orsc.2023.1745) | Org. Sci.'25 | — |
| [Reassessing Academic Integrity in the Age of AI](https://www.sciencedirect.com/science/article/pii/S2590291124003139) | [Paper](https://www.sciencedirect.com/science/article/pii/S2590291124003139) | SSH Open'25 | — |
| [The AI Deskilling Paradox](https://cacm.acm.org/opinion/the-ai-deskilling-paradox/) | [Paper](https://cacm.acm.org/opinion/the-ai-deskilling-paradox/) | CACM'25 | — |
| [Hidden Pitfalls of AI Scientist Systems](https://arxiv.org/abs/2509.08713) | [arXiv](https://arxiv.org/abs/2509.08713) | arXiv'25 | — |
| [Rethinking Science in the Age of AI](https://arxiv.org/abs/2511.10524) | [arXiv](https://arxiv.org/abs/2511.10524) | arXiv'25 | — |
| [Measuring AI Ability to Complete Long Tasks](https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks/) | [Blog](https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks/) | METR'25 | — |
| [Towards a Science of Scaling Agent Systems](https://arxiv.org/abs/2512.08296) | [arXiv](https://arxiv.org/abs/2512.08296) | arXiv'25 | — |
| [AI Tools Expand Impact but Contract Focus](https://www.nature.com/articles/s41586-025-08681-8) | [Paper](https://www.nature.com/articles/s41586-025-08681-8) | Nature'26 | — |
| [AI for Scientific Discovery is a Social Problem](https://www.cell.com/patterns/fulltext/S2666-3899(25)00336-3) | [Paper](https://www.cell.com/patterns/fulltext/S2666-3899(25)00336-3) | Patterns'26 | — |
| [Research Integrity in the Age of AI](https://arxiv.org/abs/2601.05574) | [arXiv](https://arxiv.org/abs/2601.05574) | arXiv'26 | — |
| [SciSciGPT](https://www.nature.com/articles/s43588-026-00784-z) | [Paper](https://www.nature.com/articles/s43588-026-00784-z) | Nature CS'26 | — |
| [SimStep](https://arxiv.org/abs/2507.09664) | [arXiv](https://arxiv.org/abs/2507.09664) | arXiv'25 | — |
| [ConvoLearn](https://arxiv.org/abs/2601.08950) | [arXiv](https://arxiv.org/abs/2601.08950) | arXiv'26 | — |
| [AFIM: Academic Fraud Inclination Metric](https://www.alexalemi.com/arxiv-metric/docs.html) | [Web](https://www.alexalemi.com/arxiv-metric/docs.html) | Web'26 | — |
| [AI Researchers' Views on Automating AI R&D](https://arxiv.org/abs/2603.03338) | [arXiv](https://arxiv.org/abs/2603.03338) | arXiv'26 | — |
| [AI Scientists Are Changing Research (Editorial)](https://www.nature.com/articles/d41586-026-01551-x) | [Paper](https://www.nature.com/articles/d41586-026-01551-x) | Nature'26 | — |
| [Learning by Creating (Talk)](https://www.youtube.com/watch?v=iOyaj5u0-DY) | [Video](https://www.youtube.com/watch?v=iOyaj5u0-DY) | Talk'26 | — |

---

## 📚 Surveys & Curated Lists

> Survey papers and curated reading lists that provide an overview of AI for scientific research.

| Name | Paper | Venue | Code |
|------|-------|-------|------|
| [LLM4SR](https://arxiv.org/abs/2501.04306) | [arXiv](https://arxiv.org/abs/2501.04306) | arXiv'25 | — |
| [From Automation to Autonomy](https://arxiv.org/abs/2505.13259) | [arXiv](https://arxiv.org/abs/2505.13259) | arXiv'25 | — |
| [AI4Research](https://arxiv.org/abs/2507.01903) | [arXiv](https://arxiv.org/abs/2507.01903) | arXiv'25 | — |
| [A Survey of AI Scientists](https://arxiv.org/abs/2510.23045) | [arXiv](https://arxiv.org/abs/2510.23045) | arXiv'25 | — |
| [LLMs for Scientific Idea Generation: Survey](https://arxiv.org/abs/2511.07448) | [arXiv](https://arxiv.org/abs/2511.07448) | arXiv'25 | — |
| [LLMs for Automated Scholarly Paper Review: Survey](https://www.sciencedirect.com/science/article/pii/S1566253524005803) | [Paper](https://www.sciencedirect.com/science/article/pii/S1566253524005803) | Inf. Fusion'25 | — |
| [awesome-ai-research-writing](https://github.com/Leey21/awesome-ai-research-writing) | — | GitHub'24 | [GitHub](https://github.com/Leey21/awesome-ai-research-writing) |
| [Awesome-LLM-Scientific-Discovery](https://github.com/HKUST-KnowComp/Awesome-LLM-Scientific-Discovery) | — | GitHub'25 | [GitHub](https://github.com/HKUST-KnowComp/Awesome-LLM-Scientific-Discovery) |

---

## 🛠 Tools & GitHub Repos

> Open-source tools, frameworks, and curated resource lists for AI-assisted research (not directly tied to a single paper).

### Curated Lists

| Repository | Stars | Description |
|-----------|-------|-------------|
| [Awesome-Deep-Research](https://github.com/DavidZWZ/Awesome-Deep-Research) | ~684 | Up-to-date collection of agentic deep research resources |
| [Awesome-Scientific-Language-Models](https://github.com/yuzhimanhua/Awesome-Scientific-Language-Models) | ~647 | Survey of scientific LLMs (EMNLP'24) |
| [Awesome-LLM-Scientific-Discovery](https://github.com/HKUST-KnowComp/Awesome-LLM-Scientific-Discovery) | ~319 | Three-level autonomy framework (EMNLP'25) |
| [Awesome-AI-Scientist-Papers](https://github.com/openags/Awesome-AI-Scientist-Papers) | ~136 | Resources on AI Scientist systems |
| [Awesome-Auto-Research-Tools](https://github.com/handsome-rich/Awesome-Auto-Research-Tools) | ~129 | Automated research tools catalog |
| [awesome-autoresearch](https://github.com/alvinunreal/awesome-autoresearch) | — | Autonomous improvement loops and research agents |

### Idea Generation

| Repository | Stars | Description |
|-----------|-------|-------------|
| [Virtual-Scientists](https://github.com/RenqiChen/Virtual-Scientists) | ~66 | VirSci: multi-agent collaborative idea generation (ACL'25) |
| [ResearchAgent](https://github.com/JinheonBaek/ResearchAgent) | ~29 | Iterative idea proposal with reviewing agents |

### Literature Review

| Repository | Stars | Description |
|-----------|-------|-------------|
| [paper-qa](https://github.com/Future-House/paper-qa) | ~8,300 | PaperQA2: superhuman RAG for scientific Q&A |
| [local-deep-research](https://github.com/LearningCircuit/local-deep-research) | ~4,200 | Fully local deep research |
| [researchgpt](https://github.com/mukulpatnaik/researchgpt) | ~3,500 | Conversational interaction with research papers |
| [gpt-researcher](https://github.com/assafelovic/gpt-researcher) | — | Autonomous agent for comprehensive online research |
| [AutoSurvey](https://github.com/AutoSurveys/AutoSurvey) | ~462 | Automated comprehensive literature surveys |
| [storm](https://github.com/stanford-oval/storm) | — | Wikipedia-style article generation (STORM) |

### Coding & Experiments

| Repository | Stars | Description |
|-----------|-------|-------------|
| [autoresearch (Karpathy)](https://github.com/karpathy/autoresearch) | ~55,400 | Autonomous ML experiments, ~12 exp/hour overnight |
| [Paper2Code](https://github.com/going-doer/Paper2Code) | ~4,300 | Multi-agent ML paper to code transformation |
| [RD-Agent](https://github.com/microsoft/RD-Agent) | — | Microsoft's LLM framework for autonomous data science |
| [MLAgentBench](https://github.com/snap-stanford/MLAgentBench) | ~334 | 13 end-to-end ML experimentation tasks |
| [SWE-bench](https://github.com/princeton-nlp/SWE-bench) | — | Real-world GitHub issue resolution benchmark |

### Peer Review

| Repository | Stars | Description |
|-----------|-------|-------------|
| [paper-reviewer](https://github.com/deep-diver/paper-reviewer) | ~824 | arXiv paper reviews + blog posts |
| [ai-peer-review](https://github.com/poldrack/ai-peer-review) | ~123 | Multi-LLM reviews + meta-review synthesis |
| [openreviewer](https://github.com/maxidl/openreviewer) | ~9 | Llama-8B fine-tuned on 79K expert reviews |

---

<div align="center">

**[⬆ Back to Top](#awesome-ai-auto-research)**

*Last updated: 2026-04-08 · Maintained by [WorldBench](https://github.com/worldbench)*

</div>
