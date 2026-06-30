# 07 - AI芯片架构

> AI芯片是专门为AI计算设计的处理器。理解AI芯片架构，是AI芯片PM的核心能力。
>
> **与AI-learning的衔接**: AI-learning从AI算法角度介绍芯片，本章从芯片设计角度深入。

## 📚 本章节学习目标

- [ ] 理解AI工作负载的计算特点
- [ ] 掌握NPU/TPU/ASIC的架构设计
- [ ] 理解脉动阵列和存算一体
- [ ] 能分析AI芯片的PPA指标

## 🎯 核心知识点

### 7.1 AI工作负载分析
- 矩阵乘法是核心操作
- 计算密度与内存带宽
- 数据复用模式
- **PM视角**: AI芯片设计围绕矩阵运算优化

### 7.2 GPU架构
- CUDA Core与Tensor Core
- 共享内存与缓存设计
- NVLink与互联
- **PM视角**: GPU是通用AI计算的首选

### 7.3 TPU架构
- Matrix Multiply Unit (MXU)
- 脉动阵列 (Systolic Array)
- HBM高带宽内存
- **PM视角**: TPU展示了专用架构的效率优势

### 7.4 NPU/ASIC设计
- 神经网络加速器设计
- 数据流架构（Weight Stationary / Output Stationary / Row Stationary）
- 稀疏性支持
- **PM视角**: 专用芯片的效率 vs 灵活性权衡

### 7.5 存算一体 (PIM/CIM)
- 近存计算与存内计算
- 模拟计算
- ReRAM/PCM/Flash存算
- **PM视角**: 存算一体可能突破内存墙

### 7.6 边缘AI芯片
- 低功耗设计
- 量化支持
- 多模态处理
- **PM视角**: 边缘场景对产品定义的独特要求

## 🔗 推荐资源

| 资源类型 | 名称 | 链接 | 难度 |
|----------|------|------|------|
| 论文 | TPU Architecture (ISCA'17) | [arXiv](https://arxiv.org/abs/1704.04760) | ⭐⭐⭐ |
| 论文 | Eyeriss (ISSCC'16) | [arXiv](https://arxiv.org/abs/1602.01528) | ⭐⭐⭐ |
| 论文 | Systolic Arrays Survey | [IEEE](https://ieeexplore.ieee.org) | ⭐⭐⭐ |
| 报告 | AI Chip Landscape | [AnandTech](https://www.anandtech.com) | ⭐⭐ |
| 报告 | 中国AI芯片产业分析 | [Carnegie](https://carnegieendowment.org) | ⭐⭐ |

## ✅ 检查清单

- [ ] 理解AI工作负载的计算特点
- [ ] 理解GPU/TPU/NPU架构差异
- [ ] 理解脉动阵列工作原理
- [ ] 理解存算一体的概念
- [ ] 能对比3种以上边缘AI芯片
