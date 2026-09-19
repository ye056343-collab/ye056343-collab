[← 返回主页](../README.md) · [English](#english)

# 基于分层与混合整数线性规划的 NIPT 检测时点优化

**核心成员 · 浙江工业大学 · 2025.09 — 2025.11**  
🏆 全国大学生数学建模竞赛国家二等奖 · 2025

## 建模问题

围绕 BMI、孕周与检测指标之间的关系，研究如何在分组和样本量等约束下选择检测时点，并开展女胎异常判定的分类建模。

## 方法路线

| 阶段 | 方法与用途 |
| :--- | :--- |
| 关系分析 | Spearman 相关性分析，考察变量关联 |
| 分层与拟合 | BMI 分层与二次回归，刻画 Y 染色体浓度、孕周、BMI 之间的非线性关系 |
| 分组与时点优化 | 混合整数线性规划，约束包含连续分组、最小样本量和检测时点范围 |
| 异常判定 | 使用染色体 Z 值、测序质量与母体特征建立逻辑回归和随机森林分类模型 |
| 模型评估 | 使用 AUC、Recall、F1 等指标评估分类效果 |

## 项目价值

这段实践将统计分析、约束优化与分类评估串联起来：先理解变量关系，再把分组与时点选择表达为可求解的优化问题，最后针对异常判定使用多指标评估。

## 材料状态

此页为数学建模竞赛经历介绍，目前未提供论文、代码、数据或具体评估数值。项目是竞赛建模研究，不作为临床检测建议。

---

## English

### NIPT testing-time optimization with stratification and MILP

**Core team member · Zhejiang University of Technology · September — November 2025**  
National Second Prize, China Undergraduate Mathematical Contest in Modeling · 2025

The project combines Spearman correlation, BMI stratification, and quadratic regression to study relationships between fetal Y-chromosome concentration, gestational age, and BMI.

A mixed-integer linear program selects contiguous BMI groups and testing times under minimum sample-size and timing constraints. Logistic regression and random forests address female-fetus abnormality classification using chromosome Z-scores, sequencing-quality measures, and maternal features, with AUC, recall, and F1 as evaluation metrics.

This is a competition-project overview, not clinical guidance. Papers, source code, datasets, and numerical evaluation results are not currently provided.
