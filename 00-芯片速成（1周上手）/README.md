# 00 - 芯片速成（1周上手）

> **目标**：1周内建立芯片核心概念，能与芯片研发/供应商有效对话
> **适用**：时间紧迫，需要快速建立芯片判断力的AI产品经理
> **投入**：每天1-2小时，共7天

---

## Day 1：芯片全景图（10分钟建立全局观）

**学习目标**：建立芯片产业的全局认知——从晶体管到底层架构再到产业生态

### 芯片分类速览

```
芯片世界
├── 处理器（计算）
│   ├── CPU（通用计算）→ Intel/AMD/ARM
│   ├── GPU（并行计算）→ NVIDIA/AMD
│   ├── NPU（AI专用）→ 高通/华为/地平线
│   ├── TPU（Google专用）→ Google
│   └── FPGA（可编程）→ Xilinx/Intel
├── 存储器
│   ├── SRAM（高速缓存）→ 片上
│   ├── DRAM（内存）→ 三星/SK海力士/美光
│   ├── Flash（存储）→ 三星/铠侠
│   └── HBM（高带宽内存）→ 海力士/三星
├── 接口/互联
│   ├── PCIe（扩展接口）
│   ├── UCIe（芯粒互联）
│   └── NVLink（NVIDIA专用）
└── 传感器/模拟
    ├── 图像传感器（CIS）→ 索尼/三星
    └── 射频芯片（RF）→ 高通/Qorvo
```

### 一句话理解各类芯片

| 芯片 | 一句话理解 | 类比 |
|------|-----------|------|
| CPU | 通用大脑，什么都能做但什么都不精 | 瑞士军刀 |
| GPU | 并行计算专家，适合矩阵运算 | 流水线工厂 |
| NPU | AI专用加速器，针对神经网络优化 | 专用机床 |
| TPU | Google定制的AI芯片 | 特斯拉超级工厂 |
| FPGA | 可编程硬件，灵活但开发难 | 乐高积木 |

### 学习资源

📖 **必读**：
1. [SIA 2025 Factbook](https://www.semiconductors.org/wp-content/uploads/2025/05/2025-SIA-Factbook-FINAL-1.pdf) — 全球半导体行业全景数据，2024年全球销售额$6305亿
2. [McKinsey: Semiconductor Industry Outlook 2026](https://www.mckinsey.com/industries/semiconductors/our-insights/hiding-in-plain-sight-the-underestimated-size-of-the-semiconductor-industry) — 行业估值$6300-6800亿，2030年预计$1万亿+
3. [Gartner: Semiconductor Revenue >$1.3T in 2026](https://www.gartner.com/en/newsroom/press-releases/2026-04-08-gartner-forecasts-worldwide-semiconductor-revenue-to-exceed-us-dollars-one-point-3-trillion-in-2026) — 2026全球半导体营收预测
4. [Hennessy & Patterson: 体系结构第6版](https://shop.elsevier.com/books/computer-architecture/hennessy/978-0-12-8119051) — 体系结构圣经，2017图灵奖

🎬 **课程**：
1. [MIT 6.004 Computation Structures](https://6004.mit.edu/) — 从MOS晶体管到完整计算机系统，芯片入门黄金课程
2. [UC Berkeley CS61C](https://cs61c.org/) — CPU设计、内存层次、RISC-V指令集
3. [Stanford EE282](https://online.stanford.edu/courses/ee282-computer-systems-architecture) — 现代计算系统架构设计

🛠️ **案例**：
1. [RISC-V 官方规范](https://riscv.org/specifications/ratified/) — 开源ISA官方规范
2. [复旦 Chiplet课程](https://cihlab.github.io/course/chiplet25.html) — Chiplet与异构集成封装

---

## Day 2：AI芯片类型与对比

### AI芯片全景

| 类型 | 代表产品 | 算力 | 功耗 | 优势 | 劣势 |
|------|----------|------|------|------|------|
| **GPU** | NVIDIA H100 | 989 TFLOPS | 700W | 生态最强，通用 | 贵，功耗高 |
| **NPU** | 高通骁龙8 Gen3 | 45 TOPS | 5W | 低功耗，集成 | 灵活性差 |
| **TPU** | Google TPU v5 | ~1 PFLOPS | 200W | Transformer优化 | 仅Google |
| **FPGA** | Xilinx Versal | 可编程 | 50W | 灵活，低延迟 | 开发难 |
| **DSA** | 地平线征程5 | 128 TOPS | 30W | 专用高效 | 生态小 |

### 学习资源

📖 **必读**：
1. [精读A03_TPU_彻底掌握手册.md](https://github.com/ly1992921/Chip-Learning/blob/main/精读文章/A级精读/精读A03_TPU_彻底掌握手册.md) — TPU架构深度精读
2. [精读A06_Eyeriss_彻底掌握手册.md](https://github.com/ly1992921/Chip-Learning/blob/main/精读文章/A级精读/精读A06_Eyeriss_彻底掌握手册.md) — 边缘AI芯片设计
3. [NVIDIA Blackwell Architecture](https://resources.nvidia.com/en-us-blackwell-architecture) — NVIDIA官方Blackwell白皮书
4. [Google TPU v5e](https://docs.cloud.google.com/tpu/docs/v5e) — Google TPU v5e技术文档

🎬 **课程**：
1. [UC Berkeley CS152/252](https://hkn.eecs.berkeley.edu/courseguides/CS/152) — 体系结构进阶：指令集设计、流水线、多处理器
2. [Harvard CS141](https://hackway.org/docs/cs/senior/architecture/cs141/) — 从逻辑设计到机器组织

🛠️ **基准**：
1. [MLPerf Inference v5.1](https://mlcommons.org/2025/09/mlperf-inference-v5-1-results/) — 行业标准AI芯片推理基准
2. [Epoch AI Benchmarks](https://epoch.ai/benchmarks) — AI模型和硬件基准测试追踪

---

## Day 3：算力评估与选型逻辑

### 算力指标解读

| 指标 | 全称 | 含义 | 注意 |
|------|------|------|------|
| FLOPS | Floating Point OPS | 每秒浮点运算 | 分FP64/FP32/FP16/INT8 |
| TOPS | Tera OPS | 每秒万亿次操作 | 通常指INT8 |
| TFLOPS | Tera FLOPS | 每秒万亿次浮点运算 | 10^12 |
| PFLOPS | Peta FLOPS | 每秒千万亿次浮点运算 | 10^15 |

### 关键认知：峰值算力 ≠ 实际性能

实际性能 = 峰值算力 × 利用率。利用率通常只有30-70%。

**Roofline模型**：如果 计算强度 > 内存带宽/算力 → Compute Bound；反之 → Memory Bound。大多数AI推理是Memory Bound。

### 学习资源

📖 **必读**：
1. [精读A07_DVFS_彻底掌握手册.md](https://github.com/ly1992921/Chip-Learning/blob/main/精读文章/A级精读/精读A07_DVFS_彻底掌握手册.md) — 功耗管理核心技术
2. [MLPerf Inference Datacenter](https://mlcommons.org/benchmarks/inference-datacenter/) — 行业标准评估方法论
3. [McKinsey on Semiconductors 2024](https://www.mckinsey.com/industries/semiconductors/our-insights) — 算力需求场景深度分析
4. [Computer Architecture: A Quantitative Approach](https://shop.elsevier.com/books/computer-architecture/hennessy/978-0-12-8119051) — 量化分析经典教材

🎬 **课程**：
1. [UC Berkeley CS61C](https://cs61c.org/) — 性能评估方法论、Amdahl定律
2. [Stanford EE282](https://online.stanford.edu/courses/ee282-computer-systems-architecture) — 高级系统评估

🛠️ **工具**：
1. [NVIDIA GPU Compute Capability](https://developer.nvidia.com/cuda/gpus) — GPU计算能力对照表

---

## Day 4：车规级芯片特别要求

### 功能安全等级（ISO 26262）

| ASIL等级 | 风险程度 | 典型应用 |
|----------|----------|----------|
| ASIL-D | 最高 | 自动驾驶主控 |
| ASIL-B | 高 | ADAS |
| QM | 质量管理 | 信息娱乐 |

### 学习资源

📖 **必读**：
1. [AEC-Q100 Rev J](http://www.aecouncil.com/Documents/AEC_Q100_Rev_J_Base_Document.pdf) — 车规芯片可靠性认证标准
2. [ISO 26262 功能安全标准](https://www.iso26262.net.cn/) — ASIL-A/B/C/D等级全面解读
3. [Yole Automotive Semiconductor 2025](https://www.yolegroup.com/press-release/infineon-technologies-nxp-and-stmicroelectronics-face-rising-competition-in-132-billion-automotive-semiconductor-race/) — 汽车半导体$1320亿市场格局

🎬 **课程**：
1. [ISO 26262功能安全工程师知识库](https://x-gen-lab.github.io/knowledge-os/02-technologies/embedded/10-cross-cutting-concerns/03-security-reliability/intermediate/06-iso26262-automotive-safety/) — 嵌入式视角的实操教程

🛠️ **案例**：
1. [地平线征程6系列](https://www.horizon.auto/solutions/horizon-journey/horizon-journey6) — 10-560TOPS车规AI芯片
2. [NVIDIA DRIVE AGX Orin](https://www.eefocus.com/article/1967440.html) — 车规级自动驾驶计算平台

---

## Day 5：芯片供应链与产业格局

### 产业链分工

```
芯片设计（Fabless）     → NVIDIA/高通/华为/地平线
    ↓
晶圆制造（Foundry）     → 台积电/三星/中芯国际
    ↓
封装测试（OSAT）        → 日月光/安靠/长电
    ↓
终端应用               → 车企/手机厂商/数据中心
```

### 学习资源

📖 **必读**：
1. [BCG/SIA: Supply Chain Resilience (2024)](https://www.bcg.com/publications/2024/emerging-resilience-in-semiconductor-supply-chain) — 全球供应链韧性和地缘风险
2. [Omdia: The Great Decoupling](https://omdia.tech.informa.com/blogs/2025/sep/the-great-decoupling-how-geopolitics-is-reshaping-semiconductor-supply-chains) — 中美科技脱钩重塑供应链
3. [ASML 2025 Annual Report](https://ourbrand.asml.com/m/8ab959d4926657b/original/asml-2025-annual-report-strategic-report-section.pdf) — EUV光刻战略分析

🛠️ **案例**：
1. [TrendForce: ASML's EUV Edge](https://www.trendforce.com/news/2025/11/10/news-asmls-magic-uncovered-tech-and-partners-behind-its-euv-edge-china-cant-replicate/) — ASML EUV技术护城河
2. [华为AI芯片路线图 2025-2028](https://www.caixinglobal.com/2025-09-19/huawei-unveils-three-year-ai-chip-roadmap-as-nvidia-faces-setbacks-in-china-102363891.html) — 中美博弈下的芯片发展

---

## Day 6-7：实战演练

### 模拟选型场景

**场景1：车载智驾芯片选型**
```
需求：L2+自动驾驶，8路摄像头
约束：车规级，功耗<50W，成本敏感
候选：NVIDIA Orin / 地平线J5 / 高通Snapdragon Ride
```

**场景2：边缘AI盒子选型**
```
需求：工厂质检，延迟<100ms，成本<5000元
候选：Jetson AGX Orin / 寒武纪MLU220 / 华为Atlas 200
```

### 学习资源

📖 **必读**：
1. [ChipMate: AI驱动的芯片选型推荐系统](https://www.sciencedirect.com/science/article/pii/S1879239126002122) — 学术界选型方法论
2. [AI Factory TCO白皮书](https://cdn.prod.website-files.com/667211036fda1fadbea6530d/6850b08cd7329429dac944aa_White%20Paper%20TCO%20Final%20June%202025.pdf) — AI总拥有成本建模
3. [百度大模型一体机TCO](https://cloud.baidu.com/article/3826301) — GPU集群和单机方案成本对比

🛠️ **工具**：
1. [ChipNav](https://chipnav.com/) — GPU/NPU/ASIC性能参数和价格对比
2. [EY半导体采购策略](https://www.ey.com/en_jp/insights/supply-chain/the-future-of-semiconductor-procurement-in-response-of-changing-semiconductor-supply-chain) — 芯片采购策略重构

---

## ✅ 1周验收标准

完成本周学习后，你应该能：
- [ ] **说出5种AI芯片类型**，并说明各自优缺点
- [ ] **解释TOPS和FLOPS的区别**，以及为什么利用率不高
- [ ] **理解车规级要求**（ASIL等级、AEC-Q100）
- [ ] **完成一个芯片选型分析**（给定场景，选出合适芯片并说明理由）
- [ ] **列出芯片供应商谈判的5个关键问题**
