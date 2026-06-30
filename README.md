# Chip-Learning 🔧

> **芯片产品经理技术知识库**
>
> 本知识库面向希望深入理解芯片底层原理的产品经理、技术管理者和行业研究者。
> 涵盖半导体物理、数字电路、计算机体系结构、VLSI设计、制造工艺、AI芯片架构、先进封装等核心技术知识。

---

## 📋 目录

- [学习路径总览](#学习路径总览)
- [知识库结构](#知识库结构)
- [100篇必读论文/报告清单](#100篇必读论文报告清单)
- [与AI-learning的衔接](#与ai-learning的衔接)
- [与具身智能的衔接](#与具身智能的衔接)
- [学习进度追踪](#学习进度追踪)
- [资源索引](#资源索引)

---

## 🗺️ 学习路径总览

```
Phase 1 (0-2月): 半导体物理与器件基础
Phase 2 (2-4月): 数字电路与计算机体系结构
Phase 3 (4-6月): VLSI设计与EDA工具
Phase 4 (6-8月): 芯片制造工艺与良率
Phase 5 (8-10月): AI芯片与先进封装
Phase 6 (持续): 产业生态与产品实战
```

### 阶段详细规划

#### Phase 1: 半导体物理与器件基础 (Week 1-8)

| 周次 | 主题 | 核心内容 | 目标产出 |
|------|------|----------|----------|
| W1-2 | 固体物理基础 | 晶格结构、能带理论、载流子 | 理解半导体物理本质 |
| W3-4 | PN结与MOS结构 | 二极管、晶体管工作原理 | 理解器件I-V特性 |
| W5-6 | CMOS技术 | CMOS反相器、逻辑门设计 | 理解数字电路基础 |
| W7-8 | 存储器基础 | SRAM、DRAM、Flash原理 | 理解存储器分类与特性 |

#### Phase 2: 数字电路与计算机体系结构 (Week 9-16)

| 周次 | 主题 | 核心内容 | 目标产出 |
|------|------|----------|----------|
| W9-10 | 数字逻辑设计 | 组合逻辑、时序逻辑、FSM | 能设计简单数字电路 |
| W11-12 | Verilog/SystemVerilog | HDL语法、RTL设计、验证 | 能读写RTL代码 |
| W13-14 | 计算机体系结构 | CPU流水线、缓存层次、分支预测 | 理解处理器设计原理 |
| W15-16 | RISC-V架构 | 指令集、微架构、生态 | 理解开源ISA设计 |

#### Phase 3: VLSI设计与EDA工具 (Week 17-24)

| 周次 | 主题 | 核心内容 | 目标产出 |
|------|------|----------|----------|
| W17-18 | VLSI设计流程 | 前端设计、综合、布局布线 | 理解芯片设计全流程 |
| W19-20 | EDA工具链 | Synopsys/Cadence/Mentor工具 | 了解主流EDA工具 |
| W21-22 | 时序分析与功耗 | Setup/Hold、静态时序分析、功耗优化 | 理解时序约束 |
| W23-24 | 物理设计 | Floorplan、Place&Route、DRC/LVS | 理解物理设计挑战 |

#### Phase 4: 芯片制造工艺与良率 (Week 25-32)

| 周次 | 主题 | 核心内容 | 目标产出 |
|------|------|----------|----------|
| W25-26 | 晶圆制造流程 | 光刻、刻蚀、沉积、离子注入 | 理解Fab制造步骤 |
| W27-28 | 先进制程 | FinFET、GAA、3nm/2nm技术 | 理解制程演进趋势 |
| W29-30 | 良率管理 | 缺陷分析、测试、可靠性 | 理解良率提升方法 |
| W31-32 | 封装技术 | 传统封装、BGA、SiP | 理解封装产业链 |

#### Phase 5: AI芯片与先进封装 (Week 33-40)

| 周次 | 主题 | 核心内容 | 目标产出 |
|------|------|----------|----------|
| W33-34 | AI加速器架构 | NPU/TPU/DPU设计、脉动阵列 | 理解AI芯片架构 |
| W35-36 | 存算一体 | PIM/CIM、模拟计算、存内计算 | 理解新兴架构 |
| W37-38 | Chiplet与先进封装 | UCIe、CoWoS、HBM | 理解先进封装技术 |
| W39-40 | 边缘AI芯片 | 低功耗设计、量化部署、NPU选型 | 理解边缘场景需求 |

#### Phase 6: 产业生态与产品实战 (持续)

| 主题 | 核心内容 | 目标产出 |
|------|----------|----------|
| 产业链分析 | IDM/Fabless/Foundry模式、供应链 | 形成产业认知 |
| 竞品分析 | NVIDIA/AMD/Intel/华为/寒武纪产品 | 形成竞品洞察 |
| 芯片产品定义 | 规格定义、PPA权衡、路线图规划 | 形成产品方法论 |
| 市场与投融资 | 芯片市场规模、投资逻辑、并购 | 形成商业洞察 |

---

## 📁 知识库结构

```
Chip-Learning/
├── 01-半导体物理基础/          # 固体物理、器件物理、能带理论
├── 02-数字电路设计/             # 组合逻辑、时序逻辑、Verilog、FPGA
├── 03-计算机体系结构/           # CPU/GPU架构、缓存、流水线、RISC-V
├── 04-VLSI设计与EDA/            # 设计流程、综合、P&R、验证
├── 05-芯片制造工艺/             # 光刻、刻蚀、FinFET、制程节点
├── 06-存储器与接口/             # SRAM/DRAM/Flash、DDR/PCIe/UCIe
├── 07-AI芯片架构/               # NPU/TPU、脉动阵列、存算一体
├── 08-先进封装与Chiplet/        # CoWoS、HBM、UCIe、3D封装
├── 09-芯片产业生态/             # 产业链、竞品、市场、投资
├── 10-产品经理实战/             # 规格定义、PPA分析、路线图
├── papers/                     # 论文/报告清单与索引
│   ├── A级必读 (10篇)          # 奠基性论文/报告
│   ├── B级推荐 (20篇)          # 重要论文/报告
│   └── C级参考 (70篇)          # 延伸阅读
├── roadmap/                    # 学习路径规划
├── resources/                  # 外部资源链接
└── notes/                      # 个人学习笔记
```

---

## 📚 100篇必读论文/报告清单

### 🏆 A级必读 (10篇) — 奠基性论文/报告，必须精读

> A级文献是芯片领域的"原典"，涵盖体系结构、半导体器件、VLSI设计的里程碑工作。

| 编号 | 论文/报告 | 作者/来源 | 年份 | 核心贡献 | 为什么必读 |
|------|-----------|-----------|------|----------|------------|
| A-01 | [A New Golden Age for Computer Architecture](https://www.cs.utexas.edu/users/mckinley/talks/Berkeley-2018-Computer-Architecture-Golden-Age.pdf) | Patterson & Hennessy | 2018 | 计算机体系结构新黄金时代宣言 | 理解后摩尔时代架构创新方向 |
| A-02 | [The Case for Reduced Instruction Set Computing](https://people.eecs.berkeley.edu/~pattrsn/papers/RISC_1982.pdf) | Patterson & Ditzel | 1982 | RISC架构的开创性论证 | 理解指令集设计哲学 |
| A-03 | [In-Datacenter Performance Analysis of a Tensor Processing Unit](https://arxiv.org/abs/1704.04760) | Jouppi et al. (Google) | 2017 | TPU架构与性能分析 | AI专用芯片的开山之作 |
| A-04 | [High Performance Dynamic Voltage Frequency Scaling](https://ieeexplore.ieee.org/document/4690956) | Nowka et al. | 2010 | DVFS技术 | 理解功耗管理核心 |
| A-05 | [Dennard Scaling and Its Implications](https://ieeexplore.ieee.org/document/4781214) | Dennard et al. | 1974/2007 | MOSFET缩放定律 | 理解摩尔定律物理基础 |
| A-06 | [Dark Silicon and the End of Multicore Scaling](https://ieeexplore.ieee.org/document/5958025) | Esmaeilzadeh et al. | 2011 | 暗硅问题分析 | 理解能效墙与架构约束 |
| A-07 | [Eyeriss: An Energy-Efficient Reconfigurable Accelerator for Deep CNNs](https://arxiv.org/abs/1602.01528) | Chen et al. (MIT) | 2016 | 稀疏化与数据流优化 | 边缘AI芯片设计范式 |
| A-08 | [The Semiconductor Industry and AI Chip Development in China](https://carnegieendowment.org/research/2023/04/the-semiconductor-industry-and-ai-chip-development-in-china) | Carnegie Endowment | 2023 | 中国半导体产业全景分析 | 地缘政治与产业格局 |
| A-09 | [International Technology Roadmap for Semiconductors (ITRS)](https://www.semiconductors.org/resources/2015-international-technology-roadmap-for-semiconductors-itrs/) | ITRS | 2015 | 半导体技术路线图 | 产业技术标准与发展方向 |
| A-10 | [Computer Architecture: A Quantitative Approach (6th Ed.)](https://www.elsevier.com/books/computer-architecture/hennessy/978-0-12-820109-1) | Hennessy & Patterson | 2019 | 计算机体系结构权威教材 | 体系结构PM必读圣经 |

---

### ⭐ B级推荐 (20篇) — 重要论文/报告，建议精读

#### B1-B5: 计算机体系结构与处理器

| 编号 | 论文 | 作者 | 年份 | 会议 | 核心贡献 |
|------|------|------|------|------|----------|
| B-01 | [RISC-V: An Open Standard for SoCs](https://riscv.org/about/) | Waterman et al. | 2014 | Hot Chips | 开源指令集架构 |
| B-02 | [A Survey of Techniques for Dynamic Branch Prediction](https://arxiv.org/abs/1502.07826) | Mittal | 2018 | arXiv | 分支预测技术综述 |
| B-03 | [Cache Replacement Policies](https://dl.acm.org/doi/10.1145/2797051) | Jaleel et al. | 2016 | ACM CSUR | 缓存替换策略 |
| B-04 | [GPU Computing: Past, Present, and Future](https://ieeexplore.ieee.org/document/6183597) | Owens et al. | 2012 | IEEE Micro | GPU发展历程 |
| B-05 | [Apple M1: A Chip with Heterogeneous CPU Clusters](https://www.anandtech.com/show/16252/mac-mini-apple-m1-tested) | Apple / AnandTech | 2020 | Hot Chips | 异构SoC设计典范 |

#### B6-B10: VLSI设计与EDA

| 编号 | 论文 | 作者 | 年份 | 会议 | 核心贡献 |
|------|------|------|------|------|----------|
| B-06 | [OpenROAD: Toward an Open-Source Digital Design Implementation Tool Chain](https://ieeexplore.ieee.org/document/8742145) | Ajayi et al. | 2019 | DAC | 开源EDA工具链 |
| B-07 | [Machine Learning for IC Physical Design](https://arxiv.org/abs/2012.00315) | Ren & Fojtik | 2021 | arXiv | ML辅助芯片设计 |
| B-08 | [Physical Design for 3D ICs: Challenges and Opportunities](https://ieeexplore.ieee.org/document/9209106) | Pavlidis & Savidis | 2020 | IEEE Design & Test | 3D IC物理设计 |
| B-09 | [Power Management Techniques for Integrated Circuits](https://ieeexplore.ieee.org/document/1678935) | Chandrakasan et al. | 2008 | Proceedings IEEE | 功耗管理综述 |
| B-10 | [Formal Verification in Hardware Design: A Survey](https://arxiv.org/abs/2203.01892) | Johannsen & Drechsler | 2022 | arXiv | 形式化验证综述 |

#### B11-B15: 半导体制造与先进制程

| 编号 | 论文 | 作者 | 年份 | 会议 | 核心贡献 |
|------|------|------|------|------|----------|
| B-11 | [FinFET and GAA Device Physics and Scaling](https://ieeexplore.ieee.org/document/9334012) | Loubet et al. | 2021 | VLSI Technology | FinFET与GAA器件物理 |
| B-12 | [EUV Lithography: Status and Challenges](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/11323/113230F/EUV-lithography-status-and-challenges/10.1117/12.2558813.short) | Bakshi | 2020 | SPIE | EUV光刻技术 |
| B-13 | [Advanced Packaging Technologies for HPC and AI](https://ieeexplore.ieee.org/document/9966745) | Lau | 2022 | IEEE TED | 先进封装技术 |
| B-14 | [HBM Memory: Architecture and Design](https://ieeexplore.ieee.org/document/8695712) | Kim et al. | 2019 | JSSC | HBM存储架构 |
| B-15 | [Chiplet Technology and Standardization](https://ieeexplore.ieee.org/document/10106296) | Topol et al. | 2023 | IEEE Micro | Chiplet技术与标准 |

#### B16-B20: AI芯片与存算一体

| 编号 | 论文 | 作者 | 年份 | 会议 | 核心贡献 |
|------|------|------|------|------|----------|
| B-16 | [Eyeriss v2: A Flexible Accelerator for Emerging DNNs](https://arxiv.org/abs/1807.07928) | Chen et al. | 2019 | JSSC | Eyeriss演进 |
| B-17 | [A Survey of ReRAM-based Neuromorphic Computing](https://ieeexplore.ieee.org/document/8781878) | Ielmini & Wong | 2018 | Proceedings IEEE | 存内计算综述 |
| B-18 | [DaDianNao: A Machine-Learning Supercomputer](https://ieeexplore.ieee.org/document/7011421) | Chen et al. | 2014 | MICRO | 大规模ML加速器 |
| B-19 | [FlexASR: A Flexible Accelerator for Speech Recognition](https://arxiv.org/abs/2009.00088) | - | 2020 | arXiv | 语音AI加速器 |
| B-20 | [NVIDIA Hopper Architecture In-Depth](https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/) | NVIDIA | 2022 | Hot Chips | Hopper架构详解 |

---

### 📖 C级参考 (70篇) — 延伸阅读，按需查阅

#### C1-C10: 半导体物理与器件

| 编号 | 论文/资料 | 来源 | 年份 | 核心主题 |
|------|-----------|------|------|----------|
| C-01 | [Semiconductor Device Physics (Sze & Ng)](https://www.wiley.com/en-us/Physics+of+Semiconductor+Devices%2C+4th+Edition-p-9780471143239) | Wiley | 2006 | 器件物理圣经 |
| C-02 | [MOS Capacitor and MOSFET Theory](https://www.springer.com/gp/book/9783540250071) | Springer | 2005 | MOS理论 |
| C-03 | [Short-Channel Effects in MOSFETs](https://ieeexplore.ieee.org/document/1050511) | IEEE | 1979 | 短沟道效应 |
| C-04 | [High-k/Metal Gate Technology](https://ieeexplore.ieee.org/document/4609177) | IEEE | 2007 | 高k介质技术 |
| C-05 | [Stress Engineering for CMOS Performance Enhancement](https://ieeexplore.ieee.org/document/1707641) | IEEE | 2006 | 应力工程 |
| C-06 | [TFET: Tunnel Field-Effect Transistor](https://ieeexplore.ieee.org/document/5547660) | IEEE | 2010 | 隧穿晶体管 |
| C-07 | [GaN and SiC Power Devices](https://ieeexplore.ieee.org/document/8752523) | IEEE | 2019 | 宽禁带半导体 |
| C-08 | [Spintronics for Memory and Logic](https://www.nature.com/articles/nature08960) | Nature | 2010 | 自旋电子学 |
| C-09 | [2D Materials for Future Electronics](https://www.nature.com/articles/nature12385) | Nature | 2014 | 二维材料 |
| C-10 | [Quantum Computing with Superconducting Qubits](https://www.nature.com/articles/nature08812) | Nature | 2011 | 超导量子计算 |

#### C11-C20: 数字电路与体系结构

| 编号 | 论文 | 作者 | 年份 | 核心主题 |
|------|------|------|------|----------|
| C-11 | [The Berkeley Out-of-Order Machine (BOOM)](https://ieeexplore.ieee.org/document/7746068) | Celio et al. | 2015 | 开源乱序处理器 |
| C-12 | [Arm Cortex-A78 Architecture](https://www.arm.com/products/silicon-ip-cpu/cortex-a/cortex-a78) | Arm | 2020 | 移动处理器架构 |
| C-13 | [Intel Alder Lake Hybrid Architecture](https://www.intel.com/content/www/us/en/products/details/processors/core.html) | Intel | 2021 | 混合架构设计 |
| C-14 | [AMD Zen 4 Microarchitecture](https://www.amd.com/en/technologies/zen-core-4) | AMD | 2022 | Zen微架构 |
| C-15 | [NVIDIA Ampere Architecture](https://www.nvidia.com/en-us/data-center/ampere-architecture/) | NVIDIA | 2020 | GPU架构 |
| C-16 | [Graph Processing on GPUs: A Survey](https://arxiv.org/abs/1905.05102) | Shi et al. | 2019 | GPU图计算 |
| C-17 | [Near-Memory Processing: Past, Present, and Future](https://ieeexplore.ieee.org/document/8668456) | Ghose et al. | 2019 | 近存计算 |
| C-18 | [Processing-in-Memory: A Survey](https://arxiv.org/abs/2012.03112) | Mutlu et al. | 2021 | 存内计算综述 |
| C-19 | [Data Movement is All You Need: A Case Study on CNNs](https://arxiv.org/abs/2007.00072) | Yang et al. | 2020 | 数据移动瓶颈 |
| C-20 | [A Survey of Hardware Accelerators for Deep Learning](https://arxiv.org/abs/2103.05831) | Deng et al. | 2021 | DL加速器综述 |

#### C21-C30: VLSI设计与EDA

| 编号 | 论文 | 作者 | 年份 | 核心主题 |
|------|------|------|------|----------|
| C-21 | [Logic Synthesis: A Survey](https://arxiv.org/abs/2206.11987) | - | 2022 | 逻辑综合 |
| C-22 | [Placement and Routing in VLSI Design](https://ieeexplore.ieee.org/document/677077) | IEEE | 1988 | 布局布线经典 |
| C-23 | [Static Timing Analysis: A Survey](https://arxiv.org/abs/2102.12478) | - | 2021 | 静态时序分析 |
| C-24 | [Clock Tree Synthesis: Algorithms and Challenges](https://ieeexplore.ieee.org/document/1648582) | IEEE | 2006 | 时钟树综合 |
| C-25 | [Low Power Design Techniques](https://ieeexplore.ieee.org/document/1678935) | Chandrakasan | 2008 | 低功耗设计 |
| C-26 | [Design for Testability (DFT)](https://ieeexplore.ieee.org/document/5386957) | IEEE | 2010 | 可测试性设计 |
| C-27 | [RTL to GDSII: The Complete Design Flow](https://www.springer.com/gp/book/9780792376006) | Springer | 2002 | 完整设计流程 |
| C-28 | [Machine Learning for EDA: A Survey](https://arxiv.org/abs/2102.03357) | - | 2021 | ML4EDA综述 |
| C-29 | [Reinforcement Learning for Chip Floorplanning](https://www.nature.com/articles/s41586-021-03544-w) | Google | 2021 | RL芯片布局(Nature) |
| C-30 | [OpenLANE: An Open-Source Digital ASIC Flow](https://ieeexplore.ieee.org/document/9492573) | Efabless | 2021 | 开源ASIC流程 |

#### C31-C40: 制造工艺与良率

| 编号 | 论文/报告 | 来源 | 年份 | 核心主题 |
|------|-----------|------|------|----------|
| C-31 | [Optical Lithography: Introduction and Fundamentals](https://spie.org/Publications/Book/525496) | SPIE | 2005 | 光刻基础 |
| C-32 | [Self-Aligned Double Patterning (SADP)](https://ieeexplore.ieee.org/document/6064627) | IEEE | 2012 | 自对准双图案 |
| C-33 | [Directed Self-Assembly for Lithography](https://www.nature.com/articles/nature06527) | Nature | 2008 | 定向自组装 |
| C-34 | [Atomic Layer Deposition (ALD) Technology](https://ieeexplore.ieee.org/document/5462196) | IEEE | 2010 | ALD技术 |
| C-35 | [Plasma Etching: Fundamentals and Applications](https://www.springer.com/gp/book/9783540631436) | Springer | 1999 | 等离子体刻蚀 |
| C-36 | [CMP: Chemical Mechanical Planarization](https://ieeexplore.ieee.org/document/4769659) | IEEE | 2008 | 化学机械抛光 |
| C-37 | [Wafer Bonding: A Key Technology for 3D ICs](https://ieeexplore.ieee.org/document/6699941) | IEEE | 2014 | 晶圆键合 |
| C-38 | [Yield Enhancement through Defect Analysis](https://ieeexplore.ieee.org/document/4781216) | IEEE | 2007 | 良率提升 |
| C-39 | [Reliability Challenges in Advanced CMOS](https://ieeexplore.ieee.org/document/9206712) | IEEE | 2022 | 可靠性挑战 |
| C-40 | [TCAD Simulation for Semiconductor Devices](https://ieeexplore.ieee.org/document/5701309) | IEEE | 2011 | TCAD仿真 |

#### C41-C50: 存储器技术

| 编号 | 论文 | 作者 | 年份 | 核心主题 |
|------|------|------|------|----------|
| C-41 | [SRAM Cell Design and Scaling Challenges](https://ieeexplore.ieee.org/document/5711258) | IEEE | 2011 | SRAM设计 |
| C-42 | [DRAM Technology and Scaling](https://ieeexplore.ieee.org/document/8752383) | IEEE | 2019 | DRAM技术 |
| C-43 | [3D NAND Flash Memory](https://ieeexplore.ieee.org/document/8752514) | IEEE | 2019 | 3D NAND |
| C-44 | [Emerging Memory Technologies: RRAM, MRAM, PCM](https://ieeexplore.ieee.org/document/8573774) | IEEE | 2019 | 新型存储器 |
| C-45 | [HBM2E and HBM3 Memory Architecture](https://ieeexplore.ieee.org/document/9361670) | IEEE | 2021 | HBM演进 |
| C-46 | [CXL: Compute Express Link for Memory Expansion](https://www.computeexpresslink.org/) | CXL Consortium | 2022 | CXL互联 |
| C-47 | [Processing Near Memory: A Survey](https://arxiv.org/abs/1905.04601) | Mutlu | 2019 | 近存处理 |
| C-48 | [Storage Class Memory: Technology and Systems](https://ieeexplore.ieee.org/document/8752382) | IEEE | 2019 | SCM技术 |
| C-49 | [DDR5 SDRAM: Architecture and Features](https://ieeexplore.ieee.org/document/9361670) | JEDEC | 2020 | DDR5标准 |
| C-50 | [GDDR and HBM for AI Workloads](https://ieeexplore.ieee.org/document/9334013) | IEEE | 2021 | AI存储带宽 |

#### C51-C60: AI芯片与加速器

| 编号 | 论文 | 作者 | 年份 | 核心主题 |
|------|------|------|------|----------|
| C-51 | [TPU v4: An Optically Reconfigurable Supercomputer](https://ieeexplore.ieee.org/document/9923713) | Google | 2022 | TPU v4架构 |
| C-52 | [NVIDIA Tensor Core Architecture](https://developer.nvidia.com/tensor-cores) | NVIDIA | 2017 | Tensor Core |
| C-53 | [Intel Nervana NNP Architecture](https://www.intel.com/content/www/us/en/artificial-intelligence/nervana.html) | Intel | 2019 | Nervana NNP |
| C-54 | [Graphcore IPU Architecture](https://www.graphcore.ai/products/ipu) | Graphcore | 2020 | IPU架构 |
| C-55 | [Cerebras Wafer Scale Engine](https://cerebras.net/product/) | Cerebras | 2019 | 晶圆级引擎 |
| C-56 | [Groq TSP Architecture](https://groq.com/wp-content/uploads/2020/06/Groq-White-Paper.pdf) | Groq | 2020 | TSP架构 |
| C-57 | [SambaNova RDU Architecture](https://sambanova.ai/technology/) | SambaNova | 2021 | RDU架构 |
| C-58 | [Tenstorrent Grayskull Architecture](https://tenstorrent.com/products/) | Tenstorrent | 2021 | Grayskull |
| C-59 | [ReRAM-based In-Memory Computing for AI](https://ieeexplore.ieee.org/document/8668347) | IEEE | 2019 | ReRAM存算 |
| C-60 | [Photonic AI Accelerators](https://www.nature.com/articles/s41586-021-04286-3) | Nature | 2022 | 光子AI芯片 |

#### C61-C70: 产业生态与市场

| 编号 | 报告/论文 | 来源 | 年份 | 核心主题 |
|------|-----------|------|------|----------|
| C-61 | [The CHIPS and Science Act: Implications for Semiconductors](https://www.whitehouse.gov/briefing-room/statements-releases/2022/08/09/fact-sheet-chips-and-science-act-will-lower-costs-create-jobs-strengthen-supply-chains-and-counter-china/) | US Gov | 2022 | 芯片法案分析 |
| C-62 | [China's Semiconductor Ecosystem](https://carnegieendowment.org/research/2023/04/the-semiconductor-industry-and-ai-chip-development-in-china) | Carnegie | 2023 | 中国半导体生态 |
| C-63 | [Semiconductor Market Outlook 2024](https://www.gartner.com/en/documents/4020767) | Gartner | 2024 | 市场展望 |
| C-64 | [AI Chip Market Analysis](https://www.mckinsey.com/industries/semiconductors/our-insights/the-role-of-ai-in-semiconductor-design) | McKinsey | 2023 | AI芯片市场 |
| C-65 | [Foundry Business Model and Competition](https://www.counterpointresearch.com/insights/global-foundry-market-share/) | Counterpoint | 2023 | 代工竞争格局 |
| C-66 | [Semiconductor Supply Chain Analysis](https://www.bcg.com/publications/2021/semiconductor-supply-chain) | BCG | 2021 | 供应链分析 |
| C-67 | [Investment Trends in AI Chips](https://pitchbook.com/news/articles/ai-chip-startup-funding-trends) | PitchBook | 2023 | 投融资趋势 |
| C-68 | [NVIDIA Data Center Revenue Analysis](https://investor.nvidia.com/) | NVIDIA IR | 2024 | 数据中心业务 |
| C-69 | [Apple Silicon Strategy](https://www.apple.com/newsroom/2020/11/apple-unleashes-m1/) | Apple | 2020 | 苹果芯片策略 |
| C-70 | [RISC-V Ecosystem and Commercialization](https://riscv.org/about/) | RISC-V Intl | 2024 | RISC-V商业化 |

---

## 🔗 与AI-learning的衔接

| 本仓库章节 | AI-learning对应内容 | 衔接说明 |
|-----------|-------------------|----------|
| 03-计算机体系结构 | 03-深度学习框架 | 理解模型在硬件上的运行 |
| 07-AI芯片架构 | 08-AI芯片与硬件 | AI芯片是AI系统的硬件基础 |
| 09-芯片产业生态 | 09-商业化与产品策略 | 从技术到商业的完整链路 |
| 06-存储器与接口 | 07-AI系统与工程 | 存储带宽是AI系统瓶颈 |
| 10-产品经理实战 | 09-商业化与产品策略 | PM方法论互通 |

---

## 🤖 与具身智能的衔接

| 本仓库章节 | LinuxHermes对应内容 | 衔接说明 |
|-----------|-------------------|----------|
| 07-AI芯片 | LearningRecording/硬件篇 | 机器人计算平台选型(NVIDIA Jetson/高通等) |
| 03-计算机体系结构 | 具身智能硬件 | 机器人控制器SoC架构 |
| 06-存储器 | 整机BOM拆解 | 机器人存储系统选型(HBM/LPDDR) |
| 10-产品经理实战 | PM学习配套册 | 芯片PM与机器人PM方法论 |
| 09-产业生态 | 人形机器人整机架构 | 供应链与产业链分析 |

---

## 📊 学习进度追踪

使用以下模板记录学习进度：

```markdown
### 学习记录模板

**日期**: YYYY-MM-DD
**章节**: 章节名
**论文**: 论文标题
**状态**: 未开始 / 进行中 / 已完成
**笔记链接**: ./notes/xxx.md
**核心收获**:
- 要点1
- 要点2
**疑问与待解决**:
- 问题1
```

---

## 🔗 资源索引

### 在线课程
- [MIT 6.004: Computation Structures](https://ocw.mit.edu/courses/6-004-computation-structures-spring-2017/) — 数字系统基础
- [Berkeley CS61C: Great Ideas in Computer Architecture](https://cs61c.org/) — 计算机体系结构
- [Stanford EE282: Computer Systems Architecture](https://web.stanford.edu/class/ee282/) — 系统架构
- [NTU VLSI Design](https://www.youtube.com/playlist?list=PLZgpos4wVnCYO1kI5ZG8f7I8j3) — VLSI设计
- [Coursera: VLSI CAD](https://www.coursera.org/learn/vlsi-cad-logic) — EDA工具

### 推荐书籍
- 《Computer Architecture: A Quantitative Approach》(Hennessy & Patterson) — 体系结构圣经
- 《Digital Design and Computer Architecture》(Harris & Harris) — 数字设计入门
- 《CMOS VLSI Design》(Weste & Harris) — VLSI设计经典
- 《Semiconductor Device Physics》(Sze & Ng) — 器件物理
- 《Chip War》(Chris Miller) — 芯片地缘政治必读

### 社区与资讯
- [SemiWiki](https://www.semiwiki.com/) — 半导体社区
- [EE Times](https://www.eetimes.com/) — 电子工程新闻
- [SemiEngineering](https://semiengineering.com/) — 半导体工程
- [AnandTech](https://www.anandtech.com/) — 硬件评测
- [WikiChip](https://en.wikichip.org/wiki/WikiChip) — 芯片架构百科

---

> 📝 **维护说明**: 本知识库由 `ly1992921` 维护，内容随学习进度持续更新。
> 
> 建议配合 Obsidian 或 VS Code 使用，将仓库 clone 到本地作为 vault/workspace。
>
> 最后更新: 2026-06-30
