# Chip-Learning 🔧

> **芯片技术知识库（AI产品经理辅助版）**
>
> **定位**：AI产品经理的芯片知识补充库，辅助技术判断和供应商谈判
> **核心理念**：AI为主，芯片为辅；够用就好，不求精通
> **目标**：能与芯片研发、供应商进行有效对话，做出正确选型决策

---

## 🎯 为什么芯片知识对AI PM重要

作为AI系统产品经理，你不需要设计芯片，但需要：

```
❌ 不需要：设计晶体管、写Verilog、跑EDA
✅ 需要：理解芯片如何影响AI产品性能、成本、功耗
✅ 需要：能评估不同芯片方案的优劣
✅ 需要：能与芯片供应商进行技术谈判
✅ 需要：理解芯片供应链风险和交付周期
```

**特别是你的背景（新能源三电）**：
- 车规级要求（功能安全、AEC-Q100）你有天然优势
- 功率电子经验帮助你理解芯片功耗和散热
- 供应商管理经验可直接复用到芯片供应商

---

## 📂 知识库结构

```
Chip-Learning/
├── 00-芯片速成（1周上手）/           ← 先看这个！
│   ├── README.md                     ← 芯片核心概念速览
│   └── AI芯片选型速查.md
│
├── 01-半导体物理基础/                ← 理解芯片为什么是这样
├── 02-数字电路设计/                  ← 理解芯片怎么工作
├── 03-计算机体系结构/                ← 理解CPU/GPU/NPU架构
├── 04-VLSI设计与EDA/                 ← 理解芯片怎么制造
├── 05-芯片制造工艺/                  ← 理解先进制程
├── 06-存储器与接口/                  ← 理解HBM/DDR/PCIe
├── 07-AI芯片架构/                    ← 理解NPU/TPU设计
├── 08-先进封装与Chiplet/             ← 理解CoWoS/UCIe
├── 09-芯片产业生态/                  ← 理解产业链和供应链
├── 10-产品经理实战/                  ← 芯片选型与谈判
│
├── papers/                           ← 论文与报告索引
│   ├── A级必读（10篇）/              ← 里程碑论文
│   ├── B级推荐（20篇）/              ← 重要论文
│   └── C级参考（70篇）/              ← 延伸阅读
│
├── roadmap/
│   └── 学习计划.md                    ← 按需学习路径
│
└── resources/                        ← 外部资源
```

---

## 🚀 快速开始

### 如果你时间紧迫（1周速成）

👉 **打开 `00-芯片速成（1周上手）/README.md`**

覆盖：
- Day 1: 芯片全景图（10分钟建立全局观）
- Day 2: AI芯片类型与对比
- Day 3: 算力评估与选型逻辑
- Day 4: 车规级芯片特别要求
- Day 5: 芯片供应链与产业格局
- Day 6-7: 实战演练（模拟选型+谈判）

### 如果你有更多时间（按需深入）

| 你的需求 | 推荐阅读 |
|----------|----------|
| 理解芯片架构 | 03-计算机体系结构 |
| 理解AI芯片设计 | 07-AI芯片架构 |
| 做芯片选型 | 10-产品经理实战 + AI-learning/tools/芯片选型矩阵 |
| 理解供应链 | 09-芯片产业生态 |
| 理解制造工艺 | 05-芯片制造工艺 |

---

## 🎯 与AI-learning的衔接

```
AI-learning（主战场）
    ├── 08-AI芯片与硬件（30%芯片知识）
    │       └── 链接到 Chip-Learning 深入
    │
    └── tools/芯片选型矩阵.md（快速参考）
            └── 链接到 Chip-Learning 详细分析

Chip-Learning（辅助库）
    ├── 00-芯片速成（1周上手）
    ├── 07-AI芯片架构（深入理解）
    └── 10-产品经理实战（选型方法论）
```

**使用建议**：
- 日常工作中用 AI-learning/tools/芯片选型矩阵.md 快速查询
- 需要深入理解时来 Chip-Learning 阅读对应章节
- 车规级要求是你的优势领域，可以重点看 10-产品经理实战

---

## 📚 核心论文速览

### A级必读（10篇）

| 编号 | 论文 | 为什么必读 | 阅读时间 |
|------|------|------------|----------|
| A-01 | [A New Golden Age for Computer Architecture](https://www.cs.utexas.edu/users/mckinley/talks/Berkeley-2018-Computer-Architecture-Golden-Age.pdf) | 理解后摩尔时代架构创新 | 30分钟 |
| A-02 | [The Case for RISC](https://people.eecs.berkeley.edu/~pattrsn/papers/RISC_1982.pdf) | 理解指令集设计哲学 | 20分钟 |
| A-03 | [In-Datacenter Performance Analysis of a Tensor Processing Unit](https://arxiv.org/abs/1704.04760) | AI专用芯片开山之作 | 40分钟 |
| A-04 | [High Performance DVFS](https://ieeexplore.ieee.org/document/4690956) | 理解功耗管理 | 20分钟 |
| A-05 | [Dennard Scaling](https://ieeexplore.ieee.org/document/4781214) | 理解摩尔定律物理基础 | 15分钟 |
| A-06 | [Dark Silicon and the End of Multicore Scaling](https://ieeexplore.ieee.org/document/5958025) | 理解能效墙 | 25分钟 |
| A-07 | [Eyeriss: Energy-Efficient CNN Accelerator](https://arxiv.org/abs/1602.01528) | 边缘AI芯片设计范式 | 35分钟 |
| A-08 | [China's Semiconductor Industry](https://carnegieendowment.org/research/2023/04/the-semiconductor-industry-and-ai-chip-development-in-china) | 地缘政治与产业格局 | 30分钟 |
| A-09 | [ITRS Roadmap](https://www.semiconductors.org/resources/2015-international-technology-roadmap-for-semiconductors-itrs/) | 产业技术标准 | 浏览 |
| A-10 | [Computer Architecture: A Quantitative Approach](https://www.elsevier.com/books/computer-architecture/hennessy/978-0-12-820109-1) | 体系结构圣经 | 按需 |

### 快速阅读策略

```
你不是研究员，不需要逐行推导。

阅读方法：
1. 先看摘要和结论（5分钟）
2. 再看图表（5分钟）
3. 最后看核心贡献（10分钟）
4. 记下3个关键takeaway

总时间：每篇20-30分钟
```

---

## 🛠️ 实用工具

### 芯片选型快速评估表

```
□ 应用场景
  □ 云端训练 / 云端推理 / 边缘 / 车载
  
□ 算力需求
  □ 模型参数量？
  □ 推理延迟要求？
  □ 吞吐量要求？
  
□ 功耗限制
  □ 设备功耗预算？
  □ 散热方式？
  
□ 环境要求
  □ 车规级？（ASIL等级？）
  □ 工业级？（温度范围？）
  □ 消费级？
  
□ 供应链
  □ 供货周期？
  □ 国产替代要求？
  □ 第二供应商？
  
□ 成本
  □ 单颗芯片预算？
  □ 总体拥有成本（TCO）？
  
□ 生态
  □ 支持框架？
  □ 开发工具成熟度？
  □ 技术支持？
```

---

## 💡 核心认知（牢记这10条）

1. **算力≠性能**：峰值算力只是理论值，实际利用率通常30-70%
2. **Memory Wall**：AI推理往往是内存带宽瓶颈，不是算力瓶颈
3. **精度与效率**：INT8量化通常只损失1-2%精度，但速度提升2-4x
4. **功耗是硬约束**：边缘/车载场景功耗决定一切
5. **软件生态>硬件性能**：CUDA生态是NVIDIA最大的护城河
6. **车规级=贵+慢**：AEC-Q100认证通常需要1-2年
7. **芯片供应链脆弱**：从设计到量产通常2-3年，缺芯时更久
8. **先进制程≠好选择**：7nm足够多数AI芯片，5nm/3nm成本太高
9. **Chiplet是趋势**：通过封装提升性能，降低对先进制程依赖
10. **国产替代是战略需求**：地缘政治下，供应链安全越来越重要

---

## 🔗 知识三角

```
        AI-learning（主战场）
              │
    ┌─────────┴─────────┐
    │                   │
    ▼                   ▼
LinuxHermes          Chip-Learning
(具身智能)            (芯片辅助)
```

| 仓库 | 你的使用场景 |
|------|-------------|
| **AI-learning** | 主知识库，80%时间在这里 |
| **Chip-Learning** | 辅助库，需要芯片选型时查阅 |
| **LinuxHermes** | 具身智能项目参考 |
| **Idea-Paperworks** | 快速记录和灵感 |

---

> 📝 **维护说明**: 本知识库是AI-learning的辅助库，面向AI产品经理的芯片知识补充。
>
> **核心理念**：够用就好，不求精通。你的价值在于连接技术与产品，而不是成为芯片工程师。
>
> 最后更新: 2026-06-30
