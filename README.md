<p align="center">
  <img src="llmeval-logo.png" width="200">
</p>

<h2 align="center">LLMEval-2: Professional Domain Evaluation of Chinese LLMs (Phase II)</h2>

<p align="center">
  <a href="https://arxiv.org/abs/2312.07398"><img src="https://img.shields.io/badge/Paper-Arxiv-blue.svg?style=for-the-badge" alt="Paper"></a>
  <a href="https://doi.org/10.1609/aaai.v38i17.29934"><img src="https://img.shields.io/badge/Venue-AAAI%202024-orange.svg?style=for-the-badge" alt="AAAI 2024"></a>
  <a href="https://github.com/llmeval"><img src="https://img.shields.io/badge/Org-LLMEval-green.svg?style=for-the-badge" alt="LLMEval"></a>
</p>

> **Note:** For the Chinese version of this README, please refer to [README_zh.md](README_zh.md).

## 🔔 News

- 🏆 **[2024-03-24]** Our paper "LLMEval: A Preliminary Study on How to Evaluate Large Language Models" has been accepted at **AAAI 2024**.
- 📊 **[2023-07]** LLMEval-2 evaluation results released, covering 20 LLMs across 12 academic disciplines.

## 📚 Overview

LLMEval-2 is the **Phase II dataset** of the [LLMEval](https://arxiv.org/abs/2312.07398) paper (AAAI 2024). While LLMEval-1 focused on general capabilities, LLMEval-2 targets **professional domain evaluation** across **12 academic disciplines** with approximately **480 questions** (both objective and subjective).

### Key Features

- **12 academic disciplines** — domain-specific knowledge test sets constructed by subject experts from external databases
- **Dual question types** — ~25–30 objective (multiple-choice) + ~10–15 subjective (open-ended) questions per discipline
- **Practical focus** — questions based on real tasks undergraduate and graduate students seek LLM assistance with
- **20 LLMs evaluated** — comprehensive comparison with both human and GPT-4 scoring

## 📋 Evaluation Criteria

| Question Type | Dimension | Max Score | Description |
|:-------------|:----------|:----------|:------------|
| Objective | Answer Accuracy | 3 | Is the answer correct? |
| Objective | Explanation Quality | 2 | Does the explanation contain errors? |
| Subjective | Accuracy | 5 | Is the answer content correct? |
| Subjective | Informativeness | 3 | Is sufficient information provided? |
| Subjective | Fluency | 3 | Are grammar and format correct? |
| Subjective | Logic | 3 | Is the reasoning sound? |

## 🏆 Leaderboard

| Model | Obj. Accuracy | Obj. Explanation | Fluency | Accuracy | Logic | Info. | Rank | Total |
|:------|:-------------|:-----------------|:--------|:---------|:------|:------|:-----|:------|
| GPT-4 | 2.378 (2.395) | 1.670 (1.595) | 2.895 (2.989) | 4.260 (4.545) | 2.779 (2.903) | 2.691 (2.886) | 1 (1) | 86.72 (89.54) |
| GPT-3.5 | 2.160 (2.138) | 1.542 (1.503) | 2.861 (3.000) | 3.822 (4.295) | 2.694 (2.818) | 2.489 (2.750) | 2 (2) | 80.71 (84.69) |
| Xunfei-Spark | 2.114 (2.243) | 1.557 (1.632) | 2.815 (2.977) | 3.750 (4.193) | 2.560 (2.739) | 2.196 (2.716) | 3 (5) | 78.05 (82.26) |
| Baichuan-13B-Chat | 2.003 (2.013) | 1.428 (1.441) | 2.847 (2.949) | 3.727 (4.102) | 2.631 (2.778) | 2.472 (2.756) | 4 (6) | 77.51 (81.82) |
| MiniMax-Abab5 | 1.922 (1.928) | 1.443 (1.493) | 2.878 (2.989) | 3.800 (3.977) | 2.656 (2.722) | 2.478 (2.699) | 5 (7) | 77.47 (80.64) |
| NewBing | 2.197 (2.211) | 1.583 (1.615) | 2.796 (2.989) | 3.608 (3.875) | 2.558 (2.773) | 2.061 (2.511) | 6 (4) | 77.28 (82.63) |
| Claude | 1.923 (2.066) | 1.463 (1.576) | 2.680 (2.977) | 3.597 (4.125) | 2.613 (2.801) | 2.414 (2.710) | 7 (3) | 75.57 (83.49) |
| MOSS-Mars | 1.961 (1.967) | 1.465 (1.470) | 2.737 (3.000) | 3.480 (3.807) | 2.508 (2.648) | 2.229 (2.534) | 8 (9) | 74.41 (79.21) |
| Tiangong | 1.933 (1.961) | 1.354 (1.500) | 2.774 (2.983) | 3.520 (3.807) | 2.576 (2.682) | 2.339 (2.523) | 9 (8) | 74.36 (79.31) |
| Ziya-LLaMA-13B | 1.681 (1.592) | 1.306 (1.201) | 2.804 (3.000) | 3.207 (3.364) | 2.473 (2.585) | 2.120 (2.278) | 10 (13) | 69.48 (70.92) |

*Values in parentheses are GPT-4 automated evaluation scores and rankings. Full results for all 20 models available in [LLMEVAL-2.pdf](LLMEVAL-2.pdf).*

## 📄 Full Report

The complete evaluation report is available: [LLMEVAL-2.pdf](LLMEVAL-2.pdf)

## 🔗 Related Projects

| Project | Description | Link |
|---------|-------------|------|
| **LLMEval** (AAAI 2024) | Main paper with methodology and analysis | [arXiv](https://arxiv.org/abs/2312.07398) |
| **LLMEval-1** | Phase I: General capability evaluation | [GitHub](https://github.com/llmeval/LLMEval-1) |
| **LLMEval-Fair** (ACL 2026) | Robust & fair evaluation, 200K+ questions | [GitHub](https://github.com/llmeval/LLMEval-Fair) |
| **LLMEval-Med** (EMNLP 2025) | Medical LLM benchmark | [GitHub](https://github.com/llmeval/LLMEval-Med) |
| **Official Website** | All projects & leaderboard | [llmeval.com](http://llmeval.com/) |

## 📝 Citation

```bibtex
@inproceedings{zhang2024llmeval,
  title     = {LLMEval: A Preliminary Study on How to Evaluate Large Language Models},
  author    = {Yue Zhang and Ming Zhang and Haipeng Yuan and Shichun Liu and Yongyao Shi and Tao Gui and Qi Zhang and Xuanjing Huang},
  booktitle = {Proceedings of the AAAI Conference on Artificial Intelligence},
  volume    = {38},
  number    = {17},
  pages     = {19615--19622},
  year      = {2024},
  doi       = {10.1609/aaai.v38i17.29934}
}
```

## 📞 Contact Us

This project is open to the public, and we welcome you to participate in our evaluation.

- **Website**: [http://llmeval.com/](http://llmeval.com/)
- **Email**: mingzhang23@m.fudan.edu.cn
- **WeChat**: zanyingluan

---

<p align="center">
  <b>LLMEval</b> | Fudan University NLP Lab
</p>
