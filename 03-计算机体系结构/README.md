# 03 - 计算机体系结构

> 体系结构决定了芯片能做什么、做得多快、消耗多少能量。
> 这是芯片PM最需要深入理解的领域。

## 📚 本章节学习目标

- [ ] 理解CPU流水线、缓存层次、分支预测
- [ ] 理解GPU架构和并行计算
- [ ] 掌握RISC-V指令集基础
- [ ] 能分析不同处理器的PPA（性能/功耗/面积）

## 🎯 核心知识点

### 3.1 CPU微架构
- 指令流水线（5级/7级/超流水线）
- 超标量与乱序执行
- 分支预测（BHT、BTB、TAGE）
- 缓存层次（L1/L2/L3）
- **PM视角**: 理解CPU性能由什么决定

### 3.2 缓存与内存
- 缓存映射方式（直接/组相联/全相联）
- 替换策略（LRU、FIFO、随机）
- 一致性协议（MESI）
- 虚拟内存与TLB
- **PM视角**: 内存墙是AI性能的主要瓶颈

### 3.3 GPU架构
- SIMD/SPMD执行模型
- CUDA核心 vs Tensor Core
- 内存层次（Global/Shared/Local/Constant）
- **PM视角**: GPU为什么适合AI计算？

### 3.4 RISC-V
- 指令集设计理念
- 模块化扩展
- 主流实现（SiFive、Andes、平头哥）
- 生态与商业化
- **PM视角**: RISC-V的开放生态带来的机会

### 3.5 PPA分析
- 性能指标（IPC、频率、延迟）
- 功耗分析（动态/静态/泄漏）
- 面积估算
- **PM视角**: PPA权衡是芯片产品的核心决策

## 🔗 推荐资源

| 资源类型 | 名称 | 链接 | 难度 |
|----------|------|------|------|
| 教材 | 《计算机体系结构：量化研究方法》(Hennessy & Patterson) | [Elsevier](https://www.elsevier.com) | ⭐⭐⭐ |
| 教材 | 《超标量处理器设计》(张承义) | ⭐⭐⭐ |
| 课程 | Berkeley CS152 | [Berkeley](https://inst.eecs.berkeley.edu/~cs152/) | ⭐⭐⭐ |
| 课程 | RISC-V Online Course | [RISC-V](https://riscv.org/learn/) | ⭐⭐ |
| 报告 | Apple M系列芯片分析 | [AnandTech](https://www.anandtech.com/) | ⭐⭐ |

## ✅ 检查清单

- [ ] 理解CPU流水线工作原理
- [ ] 理解缓存层次结构
- [ ] 理解GPU与CPU架构差异
- [ ] 了解RISC-V基本指令
- [ ] 能进行基本的PPA分析
