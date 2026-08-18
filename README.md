# 🤖 DeepSeek模型系列 · 深度解析

> 📘 28章 深度解析 · 交互式 HTML 课程

> **English TL;DR:** An all-Chinese 28-chapter deep dive on the **DeepSeek model family** — the Chinese lab that redefined LLM cost-efficiency. Traces the full arc: the V1 dense base (67B, bilingual scaling law, 100K BPE vocab) → DeepSeekMoE (fine-grained experts) + MLA (low-rank KV compression, ~93% memory savings) → V2 (236B MoE + MLA) → FP8 first-100B+ training, Multi-Token Prediction, DualPipe, 128K context, the \$5.6M/671B training milestone → GRPO reasoning RL (R1-Zero → R1), Coder/Math, and the latest V3.1/V3.2 (DSA) / V4 (1.6T, hybrid attention, Muon). Includes local deployment, fine-tuning and API best practices.

## 📖 课程简介

本课程围绕 **DeepSeek 模型家族**的技术创新主线做深度解析：从 V1 稠密基座、10 万 BPE 词表与双语缩放，到开源分水岭——**DeepSeekMoE（细粒度专家）+ MLA（低秩 KV 压缩，节省 93% 显存）** 的 V2，再到 V3 的 FP8 千亿训练、多 Token 预测、DualPipe、以 **$5.6M 训练 671B** 的成本奇迹；随后剖析 R1 的 **GRPO 强化推理**与 R1-Zero→R1 路线，以及 Coder/Math 垂直模型，最后落到 128K 上下文、量化、本地部署、微调与 API 实践，展望 V3.1/V3.2/V4 与开源生态。

## 🚀 快速开始

```bash
open index.html   # macOS，纯静态即开即看
```

## 📂 项目结构

```text
deepseek-tutorial/
├── index.html / 01.html ~ 28.html / courses.json / theme.css
```

## 📖 章节目录

| # | 章节 | 核心 |
|---|------|------|
| 01–05 | 起点与对齐 | 效率困境、V1 基座、10 万 BPE、数据管线、SFT+DPO |
| 06–09 | MoE 与 MLA | MoE 入门、DeepSeekMoE、MLA 注意力、V2 融合 |
| 10–15 | 训练系统 | 无辅助损失负载均衡、FP8、MTP、DualPipe、128K、$5.6M/671B |
| 16–18 | 推理与评测 | 推理优化、量化压缩、评测体系 |
| 19–22 | R 系列与垂直 | GRPO、R1-Zero→R1、Coder、Math |
| 23–25 | 落地实践 | 本地部署、微调适配、API 最佳实践 |
| 26–28 | 演进与生态 | V3.1/3.2、V4、开源生态与愿景 |

## ✨ 值得关注的技术亮点

- **MLA**：低秩 KV 压缩，推理显存节省约 93%
- **DeepSeekMoE**：共享 + 细粒度专家，稀疏激活实现高性价比
- **无辅助损失负载均衡**：稳定稀疏训练
- **GRPO 强化推理**：无价值模型 + 规则奖励，R1 的核心
- **成本工程**：$5.6M 训练 671B 的成本/拓扑拆解

## 🎯 前置知识

- 适合：LLM 研究者 / 推理与训练工程师 / 关注开源大模型的开发者
- 建议具备：Transformer + MoE + 注意力机制基础概念

## ✨ 特色

- 完整追踪 DeepSeek 五代数成本/性能演进
- 从架构创新到成本奇迹到本地部署与 API 落地
- 即开即用纯静态 HTML

---
*本课程由 `deepseek-tutorial/` 项目维护。*