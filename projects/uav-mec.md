[← 中文主页](../README.zh-CN.md) · [English](#english)

# 流态天线赋能的无人机辅助移动边缘计算安全传输

**独立项目负责人 · 浙江工业大学 · 2025.05 — 至今**

## 研究问题

无人机的位置影响通信链路，端口选择、功率、卸载与时隙分配又共同影响任务处理和安全传输。本项目将这些决策放在同一系统模型中，探索离散资源决策与连续轨迹决策的联合优化。

## 我的工作

| 环节 | 内容 |
| :--- | :--- |
| 系统建模 | 融合流态天线端口、任务卸载、功率控制、时隙资源分配和安全传输约束 |
| 算法设计 | DDQN 负责离散资源与端口选择，PPO 负责连续无人机轨迹优化 |
| 仿真分析 | 结合通信链路、安全速率和任务计算模型开展性能分析与可视化 |

## 方法结构

```text
通信与计算系统状态
        │
        ├── DDQN → 离散资源分配 / 天线端口选择
        └── PPO  → 连续无人机轨迹决策
                         │
                  系统仿真与指标分析
```

上图是研究框架示意，不代表训练结果。

## 已公开材料

[ye056343-collab/yep](https://github.com/ye056343-collab/yep) 中的 `main.py` 是仿真与绘图脚本片段，使用手工资源和轨迹策略检查环境。脚本涉及奖励、信息年龄（AoI）、任务积压、安全速率、服务量、能耗和轨迹等输出。

该公开仓库尚缺少脚本导入的 `action_space.py`、`config.py` 和 `uav_mec_env.py`，也未提供 DDQN/PPO 训练实现，因此目前不能仅凭仓库文件复现完整研究。本页不报告未经公开实验支持的性能提升比例。

---

## English

[← Back to the English profile](../README.md)

### Secure UAV-assisted MEC with fluid antenna systems

**Independent project lead · Zhejiang University of Technology · May 2025 — Present**

I model the coupling between UAV trajectories, antenna-port selection, task offloading, power control, time allocation, and secure transmission. The proposed joint framework assigns discrete resource and antenna decisions to DDQN and continuous UAV trajectory decisions to PPO.

My work covers system modeling, reinforcement-learning algorithm design, simulation analysis, and visualization.

The [public repository](https://github.com/ye056343-collab/yep) contains a simulation and plotting excerpt using hand-crafted policies. It does not include the imported environment modules or DDQN/PPO training implementation, so it is not a complete reproduction package. No quantitative improvement claims are made here.
