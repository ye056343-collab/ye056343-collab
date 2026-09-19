[← 中文主页](../README.zh-CN.md) · [English](#english)

# 智服小车：基于 ROS 的室内自主搬运服务机器人

**项目实践 · 浙江工业大学 · 2026.01 — 2026.08**  
🏆 中国高校智能机器人创意大赛一等奖 · 2026

## 任务目标

面向室内物块搬运，让机器人完成从环境感知、目标识别到抓取、放置和返回终点的完整流程。

## 系统组成

| 模块 | 实现内容 |
| :--- | :--- |
| 建图与定位 | 激光雷达建图、室内定位 |
| 目标识别 | AprilTag 标签识别，确定抓取顺序与放置区域 |
| 导航与到位 | 全局导航与局部速度精调，配合 DWA 和代价地图参数整定 |
| 抓取与放置 | 机械臂吸附抓取、回零校准、放置动作顺序修正 |
| 流程协调 | 任务状态机串联导航、识别、搬运放置和返回终点 |

## 工程实践重点

- **到位精度**：针对目标点附近停位不稳，结合局部速度精调以及 DWA、代价地图参数整定改善流程。
- **抓取放置**：针对机械臂放置偏差，开展回零校准并调整放置动作顺序。
- **模块协同**：通过任务状态机衔接导航、标签识别与机械臂动作。

## 材料状态

此页为项目经历与方法介绍，目前未提供公开源码、实机演示视频或量化测试记录。

---

## English

[← Back to the English profile](../README.md)

### ROS indoor autonomous transport robot

**Engineering project · Zhejiang University of Technology · January — August 2026**  
First Prize, 中国高校智能机器人创意大赛 · 2026

The project integrates LiDAR mapping and localization, AprilTag recognition, and suction-based robotic-arm manipulation. A task state machine coordinates navigation, recognition, pick-and-place, and return-to-goal.

Engineering work addresses stopping instability and placement offsets through DWA and costmap tuning, local velocity adjustments, arm homing calibration, and placement-sequence changes.

This is a project overview. Source code, robot demonstration videos, and quantitative test records are not currently provided.
