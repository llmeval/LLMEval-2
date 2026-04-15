<p align="center">
  <img src="llmeval-logo.png" width="200">
</p>

<h2 align="center">LLMEval-2: 中文大语言模型评测第二期 — 专业领域评测</h2>

<p align="center">
  <a href="https://arxiv.org/abs/2312.07398"><img src="https://img.shields.io/badge/论文-Arxiv-blue.svg?style=for-the-badge" alt="论文"></a>
  <a href="https://doi.org/10.1609/aaai.v38i17.29934"><img src="https://img.shields.io/badge/会议-AAAI%202024-orange.svg?style=for-the-badge" alt="AAAI 2024"></a>
  <a href="https://github.com/llmeval"><img src="https://img.shields.io/badge/组织-LLMEval-green.svg?style=for-the-badge" alt="LLMEval"></a>
</p>

> **注意：** 英文版 README 请参阅 [README.md](README.md)。

## 🔔 最新消息

- 🏆 **[2024-03-24]** 论文 "LLMEval: A Preliminary Study on How to Evaluate Large Language Models" 被 **AAAI 2024** 录用。
- 📊 **[2023-07]** LLMEval-2 评测结果发布，涵盖 12 个学科领域的 20 个大语言模型评测。

## 📚 项目简介

LLMEval-2 是 [LLMEval](https://arxiv.org/abs/2312.07398)（AAAI 2024）论文的**第二期评测数据集**。与聚焦通用能力的第一期不同，LLMEval-2 以**专业领域评测**为核心，涵盖 **12 个学科领域**，共约 **480 题**（含客观题和主观题）。

### 核心特点

- **12 个学科领域** — 由学科专家基于外部数据库构造领域知识测试集
- **双题型设计** — 每学科约 25–30 道客观题 + 10–15 道主观题
- **实用导向** — 基于本科生和研究生在学习中希望借助大模型解决的真实任务
- **20 个模型** — 全面比较，同时提供人工评测与 GPT-4 自动评测结果

## 📋 评分标准

| 题目类型 | 评价维度 | 分值 | 评价标准描述 |
|:---------|:---------|:-----|:------------|
| 客观题 | 答案准确性 | 3 分 | 回答内容是否正确 |
| 客观题 | 解释正确性 | 2 分 | 解释是否生成错误内容 |
| 主观题 | 准确性 | 5 分 | 回答内容是否有错 |
| 主观题 | 信息量 | 3 分 | 回答信息是否充足 |
| 主观题 | 流畅性 | 3 分 | 回答格式语法是否正确 |
| 主观题 | 逻辑性 | 3 分 | 回答逻辑是否严谨 |

## 🏆 排行榜

| 模型名称 | 客观·准确 | 客观·解释 | 流畅性 | 准确率 | 逻辑性 | 信息量 | 排名 | 总分 |
|:---------|:---------|:---------|:-------|:-------|:-------|:-------|:-----|:-----|
| GPT-4 | 2.378 (2.395) | 1.670 (1.595) | 2.895 (2.989) | 4.260 (4.545) | 2.779 (2.903) | 2.691 (2.886) | 1 (1) | 86.72 (89.54) |
| GPT-3.5 | 2.160 (2.138) | 1.542 (1.503) | 2.861 (3.000) | 3.822 (4.295) | 2.694 (2.818) | 2.489 (2.750) | 2 (2) | 80.71 (84.69) |
| 讯飞星火 | 2.114 (2.243) | 1.557 (1.632) | 2.815 (2.977) | 3.750 (4.193) | 2.560 (2.739) | 2.196 (2.716) | 3 (5) | 78.05 (82.26) |
| Baichuan-13B-Chat | 2.003 (2.013) | 1.428 (1.441) | 2.847 (2.949) | 3.727 (4.102) | 2.631 (2.778) | 2.472 (2.756) | 4 (6) | 77.51 (81.82) |
| MiniMax-Abab5 | 1.922 (1.928) | 1.443 (1.493) | 2.878 (2.989) | 3.800 (3.977) | 2.656 (2.722) | 2.478 (2.699) | 5 (7) | 77.47 (80.64) |
| NewBing | 2.197 (2.211) | 1.583 (1.615) | 2.796 (2.989) | 3.608 (3.875) | 2.558 (2.773) | 2.061 (2.511) | 6 (4) | 77.28 (82.63) |
| Claude | 1.923 (2.066) | 1.463 (1.576) | 2.680 (2.977) | 3.597 (4.125) | 2.613 (2.801) | 2.414 (2.710) | 7 (3) | 75.57 (83.49) |
| MOSS-Mars | 1.961 (1.967) | 1.465 (1.470) | 2.737 (3.000) | 3.480 (3.807) | 2.508 (2.648) | 2.229 (2.534) | 8 (9) | 74.41 (79.21) |
| 天工 | 1.933 (1.961) | 1.354 (1.500) | 2.774 (2.983) | 3.520 (3.807) | 2.576 (2.682) | 2.339 (2.523) | 9 (8) | 74.36 (79.31) |
| Ziya-LLaMA-13B | 1.681 (1.592) | 1.306 (1.201) | 2.804 (3.000) | 3.207 (3.364) | 2.473 (2.585) | 2.120 (2.278) | 10 (13) | 69.48 (70.92) |

*注：括号内数值为 GPT-4 自动评测的打分及排名。全部 20 个模型结果详见 [LLMEVAL-2.pdf](LLMEVAL-2.pdf)。*

## 📄 完整报告

完整评测报告：[LLMEVAL-2.pdf](LLMEVAL-2.pdf)

## 🔗 相关项目

| 项目 | 说明 | 链接 |
|------|------|------|
| **LLMEval**（AAAI 2024） | 主论文，包含方法论与分析 | [arXiv](https://arxiv.org/abs/2312.07398) |
| **LLMEval-1** | 第一期：通用能力评测 | [GitHub](https://github.com/llmeval/LLMEval-1) |
| **LLMEval-Fair**（ACL 2026） | 鲁棒公平评测，20 万+题 | [GitHub](https://github.com/llmeval/LLMEval-Fair) |
| **LLMEval-Med**（EMNLP 2025） | 医学大模型基准 | [GitHub](https://github.com/llmeval/LLMEval-Med) |
| **官方网站** | 全部项目与排行榜 | [llmeval.com](http://llmeval.com/) |

## 📝 引用

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

## 📞 联系我们

本项目已经向公众开放，欢迎参与我们的评测。

- **网站**：[http://llmeval.com/](http://llmeval.com/)
- **邮箱**：mingzhang23@m.fudan.edu.cn
- **微信**：zanyingluan

---

<p align="center">
  <b>LLMEval</b> | 复旦大学 NLP 实验室
</p>
