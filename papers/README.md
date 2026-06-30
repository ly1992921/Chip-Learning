# Chip-Learning 论文与报告索引

> 100篇必读文献，按重要性分为A/B/C三级
> 面向AI系统产品经理的芯片知识补充
> 覆盖：计算机体系结构 | 半导体器件物理 | AI芯片架构 | VLSI与EDA | 芯片制造工艺 | 存储器与互联 | 先进封装 | 产业生态 | 车载/边缘AI芯片

---

## 🏆 A级必读（10篇）

| 编号 | 标题 | 作者/来源 | 年份 | 核心贡献 | 为什么必读 | 链接 |
|------|------|-----------|------|----------|-----------|------|
| A-01 | Cramming More Components onto Integrated Circuits | Gordon Moore, *Electronics* | 1965 | 提出集成电路上晶体管密度每18-24个月翻倍的规律（摩尔定律），为半导体产业发展提供了可预测的路线图 | 理解芯片行业节奏的根本所在——摩尔定律是整个半导体产业规划和投资的基础假设 | [Chip History](https://www.chiphistory.org/20-moore-s-law-original-draft-1965) |
| A-02 | Design of Ion-Implanted MOSFET's with Very Small Physical Dimensions | R.H. Dennard 等, *IEEE JSSC* | 1974 | 提出MOSFET按比例缩小的理论（Dennard Scaling），核心是器件尺寸缩小30%可使密度翻倍、功耗密度不变 | 解释了过去30年芯片性能提升的物理机制，以及为何2010年后Dennard Scaling失效导致了"暗硅"和多核转向 | [IEEE Xplore](https://ieeexplore.ieee.org/document/1050511) |
| A-03 | RISC I: A Reduced Instruction Set VLSI Computer | D.A. Patterson, C.H. Sequin, *ISCA* | 1981 | 提出精简指令集计算机（RISC）架构，证明简化指令集反而能提升整体性能，奠定了现代处理器设计哲学 | 现代绝大多数高性能芯片（ARM、RISC-V、Apple Silicon）都基于RISC理念，是理解CPU架构的起点 | [ACM DL](https://dl.acm.org/doi/10.5555/800052.801895) |
| A-04 | In-Datacenter Performance Analysis of a Tensor Processing Unit | N. Jouppi 等 (Google), *ISCA* | 2017 | 详细介绍Google TPU v1架构——专为神经网络推理设计的领域专用ASIC，性能功耗比是传统CPU/GPU的数十倍 | 首次证明领域专用架构（DSA）在AI场景的巨大优势，开启了AI芯片军备竞赛 | [arXiv](https://arxiv.org/abs/1704.04760) |
| A-05 | A New Golden Age for Computer Architecture | J. Hennessy, D. Patterson, *CACM* | 2019 | 图灵奖演讲整理，提出摩尔定律放缓后领域专用架构（DSA）、开放ISA（RISC-V）和软硬件协同设计是架构创新的新方向 | 系统性地说明为何AI时代是芯片架构的"新黄金十年"，产品经理战略必读 | [CACM](https://cacm.acm.org/research/a-new-golden-age-for-computer-architecture/) |
| A-06 | FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness | T. Dao 等 (Stanford), *NeurIPS* | 2022 | 提出IO感知的精确注意力算法，通过分块（tiling）将HBM访问量降低数倍，成为LLM训练和推理的核心优化 | 这是"算法-硬件协同设计"的完美案例，深刻影响了H100等GPU的内存子系统设计 | [arXiv](https://arxiv.org/abs/2205.14135) |
| A-07 | First Draft of a Report on the EDVAC | John von Neumann | 1945 | 提出存储程序概念（冯·诺依曼架构），定义了现代计算机的五大组成部分 | 所有计算机架构的"始祖"——理解冯·诺依曼瓶颈（存储墙）是理解AI芯片创新的关键线索 | [PDF (MIT)](https://people.csail.mit.edu/brooks/idocs/VvN.pdf) |
| A-08 | DianNao: A Small-Footprint High-Throughput Accelerator for Ubiquitous Machine Learning | T. Chen 等 (中科院计算所), *ASPLOS* | 2014 | 提出面向大规模CNN/DNN的专用加速器架构，在面积受限条件下实现了大幅超越通用处理器的能效 | 中国AI芯片（寒武纪系列）的奠基之作，也是理解神经网络加速器设计范式的经典案例 | [ACM DL](https://dl.acm.org/doi/10.1145/2654822.2541967) |
| A-09 | NVIDIA H100 Tensor Core GPU Architecture (Whitepaper) | NVIDIA | 2022 | 详细介绍Hopper架构H100 GPU，包括第四代Tensor Core、Transformer Engine（FP8）、DPX指令、NVLink Switch等创新 | 大模型时代的"算力引擎"，H100架构直接决定了GPT时代AI训练的效率和成本 | [NVIDIA Whitepaper](https://resources.nvidia.com/en-us-hopper-architecture/nvidia-h100-tensor-c) |
| A-10 | Strengthening the Global Semiconductor Supply Chain in an Uncertain Era | SIA / BCG | 2021 | 系统性分析全球半导体供应链的地理分布、脆弱性和风险，量化了不同区域的产能依赖关系 | 理解芯片产业"卡脖子"问题的必读报告——解释了为何芯片是地缘政治的核心 | [BCG报告](https://www.bcg.com/publications/2021/strengthening-the-global-semiconductor-supply-chain) |

---

## 📘 B级推荐（20篇）

### 计算机体系结构

| 编号 | 标题 | 作者/来源 | 年份 | 核心主题 | 链接 |
|------|------|-----------|------|----------|------|
| B-01 | Computer Architecture: A Quantitative Approach | J. Hennessy, D. Patterson (Morgan Kaufmann) | 1990（首版） | 计算机体系结构领域的"圣经"，系统化定量方法分析处理器设计、存储层次、并行计算 | [Book Site](https://www.elsevier.com/books/computer-architecture/hennessy/978-0-12-811905-1) |
| B-02 | The RISC-V Instruction Set Manual, Volume I: User-Level ISA, Version 2.0 | A. Waterman, Y. Lee, D. Patterson, K. Asanović (UC Berkeley) | 2014 | 定义RISC-V开放指令集架构，为芯片设计提供免费可扩展的ISA选择，打破x86/ARM的垄断 | [UC Berkeley EECS](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2014/EECS-2014-54.html) |
| B-03 | Dark Silicon and the End of Multicore Scaling | H. Esmaeilzadeh 等, *ISCA* | 2011 | 揭示Dennard Scaling失效后"暗硅"问题的严重性——未来芯片只能让一小部分晶体管同时工作 | [IEEE Xplore](https://ieeexplore.ieee.org/document/6307773) |

### 半导体器件物理

| 编号 | 标题 | 作者/来源 | 年份 | 核心主题 | 链接 |
|------|------|-----------|------|----------|------|
| B-04 | FinFET: A Self-Aligned Double-Gate MOSFET Scalable to 20 nm | X. Huang 等 (UC Berkeley), *IEEE TED* | 2001 | 提出FinFET（鳍式场效应晶体管）结构，用3D栅极包裹沟道解决短沟道效应，延续摩尔定律 | [IEEE Xplore](https://ieeexplore.ieee.org/document/905675) |
| B-05 | A 30 Year Retrospective on Dennard's MOSFET Scaling Paper | R.H. Dennard 等, *IEEE SSCS* | 2007 | 回顾MOSFET缩放理论的三十年历程，分析缩放理论为何失效及其后续影响 | [IEEE Xplore](https://ieeexplore.ieee.org/document/4785534) |
| B-06 | A Review of the Gate-All-Around Nanosheet FET Process Opportunities | N. Loubet 等 (IBM/CEA-Leti), *Electronics* | 2022 | 综述GAA（环绕栅极）纳米片FET工艺——FinFET之后的下一个晶体管结构 | [MDPI](https://www.mdpi.com/2079-9292/11/21/3589) |

### AI芯片架构

| 编号 | 标题 | 作者/来源 | 年份 | 核心主题 | 链接 |
|------|------|-----------|------|----------|------|
| B-07 | NVIDIA Tesla V100 GPU Architecture (Volta Whitepaper) | NVIDIA | 2017 | 首次引入Tensor Core，为深度学习矩阵运算提供专用硬件单元，改变AI训练硬件格局 | [NVIDIA Whitepaper](https://images.nvidia.com/content/volta-architecture/pdf/volta-architecture-whitepaper.pdf) |
| B-08 | Eyeriss: An Energy-Efficient Reconfigurable Accelerator for Deep CNNs | Y.H. Chen 等 (MIT), *JSSC* | 2016 | 提出以数据流为中心的可重构CNN加速器，通过减少数据搬移实现高能效 | [IEEE Xplore](https://ieeexplore.ieee.org/document/7738524) |
| B-09 | Tensor Core Programmability, Performance & Precision | NVIDIA / ArXiv | 2018 | 深入分析NVIDIA Tensor Core编程模型、混合精度训练的性能与准确度权衡 | [arXiv](https://arxiv.org/abs/1803.04014) |

### VLSI设计与EDA

| 编号 | 标题 | 作者/来源 | 年份 | 核心主题 | 链接 |
|------|------|-----------|------|----------|------|
| B-10 | The OpenROAD Project: An Open-Source RTL-to-GDS Flow for Chip Design | T. Ajayi 等 (UC San Diego), *DATE* | 2019 | 提出完整开源数字芯片设计流程（RTL→GDS），降低芯片设计门槛，推动硬件开源 | [OpenROAD Project](https://theopenroadproject.org/) |
| B-11 | Machine Learning for Electronic Design Automation: A Survey | G. Huang 等 (香港科大), *ACM TODAES* | 2021 | 全面综述机器学习在EDA各环节（逻辑综合、布局布线、时序分析等）的应用 | [ACM DL](https://dl.acm.org/doi/10.1145/3451179) |

### 芯片制造工艺

| 编号 | 标题 | 作者/来源 | 年份 | 核心主题 | 链接 |
|------|------|-----------|------|----------|------|
| B-12 | A 3nm CMOS FinFlex Platform Technology with Enhanced Power Efficiency | TSMC, *IEDM* | 2022 | 详细介绍台积电3nm（N3）FinFlex工艺——提供了标准、低功耗、高性能三种单元配置 | [IEEE Xplore](https://ieeexplore.ieee.org/document/10019498) |
| B-13 | High-NA EUV Lithography: Current Status and Outlook | H.J. Levinson, *JJAP* | 2022 | 综述高数值孔径（High-NA）EUV光刻技术的关键光学特性和未来挑战 | [IOP Science](https://iopscience.iop.org/article/10.35848/1347-4065/ac49fa) |
| B-14 | IRDS 2022 Lithography Chapter | IEEE IRDS | 2022 | 国际器件与系统路线图2022年光刻章节——半导体工艺路线图的权威预测 | [IEEE IRDS](https://irds.ieee.org/images/files/pdf/2022/2022IRDS_Litho.pdf) |

### 存储器与互联

| 编号 | 标题 | 作者/来源 | 年份 | 核心主题 | 链接 |
|------|------|-----------|------|----------|------|
| B-15 | JEDEC JESD235 — High Bandwidth Memory (HBM) DRAM Standard | JEDEC | 2013 | 定义HBM标准——通过硅中介层的宽接口（1024位）和3D堆叠实现超高带宽 | [JEDEC](https://www.jedec.org/standards-documents/docs/jesd235) |
| B-16 | Compute Express Link (CXL) Specification 1.0/2.0 | CXL Consortium / Intel | 2019/2022 | 定义基于PCIe的高缓存一致性互联协议，实现CPU、内存、加速器的共享一致性内存 | [CXL Consortium](https://computeexpresslink.org/) |
| B-17 | AMD Chiplet Architecture for High-Performance Server and Desktop Products | AMD, *ISSCC* | 2020 | 展示AMD基于Infinity Fabric的Chiplet架构（Rome/Matisse），将多个小芯片集成在同一封装 | [IEEE Xplore](https://ieeexplore.ieee.org/document/9063103) |

### 先进封装

| 编号 | 标题 | 作者/来源 | 年份 | 核心主题 | 链接 |
|------|------|-----------|------|----------|------|
| B-18 | UCIe Specification 1.0 — Universal Chiplet Interconnect Express | UCIe Consortium | 2022 | 定义开放的Die-to-Die互联标准，实现不同厂商Chiplet的互操作性 | [UCIe官网](https://www.uciexpress.org/specifications) |
| B-19 | SIA State of the U.S. Semiconductor Industry 2024 | Semiconductor Industry Association | 2024 | 全面报告美国半导体产业现状，涵盖CHIPS法案实施、供应链投资、劳动力等 | [SIA报告](https://www.semiconductors.org/wp-content/uploads/2024/09/SIA_State-of-Industry-Report_2024_final_091124.pdf) |

### 车载与边缘AI芯片

| 编号 | 标题 | 作者/来源 | 年份 | 核心主题 | 链接 |
|------|------|-----------|------|----------|------|
| B-20 | ISO 26262: Functional Safety Standard for Road Vehicles | ISO | 2018（第二版） | 道路车辆功能安全标准——车载芯片安全设计的核心规范，定义ASIL等级（A/B/C/D） | [ISO](https://www.iso.org/standard/68383.html) |

---

## 📖 C级参考（70篇）

### 计算机体系结构（C-01 ~ C-08）

| 编号 | 标题 | 核心主题 | 链接 |
|------|------|----------|------|
| C-01 | The gem5 Simulator (Binkert 等, *ISCA*, 2011) | 开源计算机体系结构模拟器的设计与架构 | [PDF](https://research.cs.wisc.edu/multifacet/papers/can11_gem5.pdf) |
| C-02 | The Landscape of Computer Architecture Research (ISCA 50th Retrospective) | 计算机体系结构50年研究全景回顾 | [ACM DL](https://dl.acm.org/doi/10.1145/3579371.3589119) |
| C-03 | IBM POWER10 Processor (Starke 等, *IEEE Micro*, 2021) | 第10代POWER企业级处理器架构设计 | [IEEE Xplore](https://ieeexplore.ieee.org/document/9352481) |
| C-04 | Apple M1 SoC Architecture Analysis (AnandTech, 2020) | Apple M1统一内存架构与Firestorm/Icestorm大小核设计 | [AnandTech](https://www.anandtech.com/show/16252/apple-silicon-m1-all-details) |
| C-05 | Arm AMBA 5 CHI Coherent Hub Interface | ARM AMBA5 CHI缓存一致性集线器接口架构标准 | [ARM](https://www.arm.com/architecture/system-architectures/amba/amba-5) |
| C-06 | A Survey of CMP Cache Coherence Protocols (Martin 等, *ACM CSUR*, 2012) | 多核处理器缓存一致性协议综述（MOESI/MESI） | [ACM DL](https://dl.acm.org/doi/10.1145/2331135.2331136) |
| C-07 | Micro-architecture Independent Processor Characterization | 独立于微架构的处理器性能特征分析方法 | [IEEE Xplore](https://ieeexplore.ieee.org/document/4359851) |
| C-08 | DARPA Electronics Resurgence Initiative (ERI, 2017) | DARPA电子复兴计划——美国半导体创新生态建设 | [DARPA](https://www.darpa.mil/news/2017/electronics-resurgence-initiative) |

### 半导体器件物理（C-09 ~ C-15）

| 编号 | 标题 | 核心主题 | 链接 |
|------|------|----------|------|
| C-09 | Short-Channel Effects in SOI MOSFETs (J.G. Fossum, *IEEE TED*) | SOI MOSFET中的短沟道效应理论分析 | [IEEE Xplore](https://ieeexplore.ieee.org/document/5575488) |
| C-10 | Sub-20nm FinFET: Overview and Perspectives (J.P. Colinge, 2014) | 20nm以下FinFET工艺的挑战与展望 | [Springer](https://link.springer.com/article/10.1007/s10825-014-0625-x) |
| C-11 | Comprehensive Review of FinFET Technology (MDPI, 2024) | FinFET技术完整综述：历史、结构、挑战和材料 | [MDPI](https://www.mdpi.com/2072-666X/15/10/1187) |
| C-12 | GaN Semiconductor Devices: A Review (F. Roccaforte 等) | GaN宽禁带半导体的器件物理与应用 | [Wiley](https://onlinelibrary.wiley.com/doi/10.1002/pssa.201700139) |
| C-13 | SiC Power Device Technology (J.A. Cooper, *IEEE TED*) | SiC功率器件的技术进步与应用前景 | [IEEE Xplore](https://ieeexplore.ieee.org/document/6233080) |
| C-14 | CMOS Device Technology Beyond Transistor Scaling (Ferain 等, *Nature*, 2011) | 后摩尔时代CMOS器件技术创新 | [Nature](https://www.nature.com/articles/nature10112) |
| C-15 | Impact of MOSFET Scaling on Analog Performance (Y. Tsividis) | MOSFET尺寸缩小对模拟电路性能的影响 | [IEEE Xplore](https://ieeexplore.ieee.org/document/1050691) |

### AI芯片架构（C-16 ~ C-32）

| 编号 | 标题 | 核心主题 | 链接 |
|------|------|----------|------|
| C-16 | FPGA Accelerators for Deep Neural Networks: Progress and Challenges (Mittal, 2020) | FPGA加速DNN的进展与挑战综述 | [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0743731520303121) |
| C-17 | Cerebras Wafer-Scale Engine Architecture (Hot Chips 2022) | 晶圆级集成计算引擎的架构设计与挑战 | [Hot Chips](http://www.hc34.hotchips.org/assets/program/conference/day2/Machine%20Learning/HC2022_Cerebras_Final_v02.pdf) |
| C-18 | Graphcore Colossus MK2 IPU (White Paper, 2021) | 面向图计算和稀疏模型的智能处理单元（IPU）架构 | [Graphcore](https://www.graphcore.ai/resources/white-papers) |
| C-19 | Groq LPU: Language Processing Unit Architecture (Hot Chips 2023) | 面向LLM推理的张量流处理器（LPU）架构设计 | [Groq](https://groq.com/our-technology/) |
| C-20 | Cambricon: ISA for Neural Network Accelerators (S. Liu, *ISCA*, 2016) | 寒武纪神经网络加速器指令集架构 | [ISCA 2016](http://novel.ict.ac.cn/diannao/) |
| C-21 | ShiDianNao: Near-Sensor Vision Processor (Z. Du, *ISCA*, 2015) | 面向视觉传感器的近传感器神经网络加速器 | [ACM DL](https://dl.acm.org/doi/10.1145/2749469.2750389) |
| C-22 | DaDianNao: A Machine-Learning Supercomputer (Y. Chen, *MICRO*, 2014) | 面向机器学习的大规模多核加速器架构 | [ACM DL](https://dl.acm.org/doi/10.1109/MICRO.2014.58) |
| C-23 | Sparse GPU Kernels for Transformers (NVIDIA, 2022) | 稀疏计算加速Transformer的GPU内核优化技术 | [NVIDIA Dev Blog](https://developer.nvidia.com/blog/accelerating-inference-with-sparsity-on-nvidia-gpus/) |
| C-24 | Efficient Hardware Accelerator for Sparse Transformer NNs (IEEE, 2022) | 稀疏Transformer神经网络的高效硬件加速器 | [IEEE Xplore](https://ieeexplore.ieee.org/document/9937659) |
| C-25 | Design of Analog-AI Accelerators for Transformer-based LMs (IBM, 2023) | 基于模拟AI的Transformer语言模型硬件加速器 | [IEEE Xplore](https://ieeexplore.ieee.org/document/10413767) |
| C-26 | Mixed-Precision Training (Micikevicius 等, *ICLR*, 2018) | 混合精度训练的数值精度分析与硬件需求 | [arXiv](https://arxiv.org/abs/1710.03740) |
| C-27 | NVIDIA Blackwell Architecture Overview (GTC 2024) | B200/B100 GPU架构创新与AI训练推理性能提升 | [NVIDIA Blog](https://developer.nvidia.com/blog/nvidia-blackwell-architecture-in-depth/) |
| C-28 | A Survey of Near-Data Processing Architectures (*ACM CSUR*, 2023) | 近数据处理架构综述——将计算搬到数据附近 | [ACM DL](https://dl.acm.org/doi/10.1145/3629578) |
| C-29 | In-Memory Computing for Neural Networks (Sebastian, *IEEE*, 2022) | 存内计算加速神经网络的器件、电路与架构 | [IEEE Xplore](https://ieeexplore.ieee.org/document/9756356) |
| C-30 | Hardware-Software Co-Design for LLM Inference (NVIDIA Megatron) | 大语言模型推理的软硬件协同设计 | [NVIDIA](https://developer.nvidia.com/megatron-lm) |
| C-31 | Chiplet Heterogeneous-Integration AI Processor (*IEEE ISSCC*, 2023) | 基于Chiplet的异构集成AI处理器设计 | [IEEE Xplore](https://ieeexplore.ieee.org/document/10049867) |
| C-32 | Google Edge TPU: ML Coprocessor for Edge Devices (2019) | 面向边缘设备的小型AI推理芯片架构 | [Google Coral](https://aiyprojects.withgoogle.com/edge-tpu) |

### VLSI设计与EDA（C-33 ~ C-42）

| 编号 | 标题 | 核心主题 | 链接 |
|------|------|----------|------|
| C-33 | An Introduction to VLSI Physical Design (M. Sarrafzadeh) | VLSI物理设计经典教程：布局布线、时序闭合 | [Book](https://www.amazon.com/Introduction-Physical-VLSI-Synthesis-ebook/dp/B01LZ53R00) |
| C-34 | A Graph Placement Methodology for Fast Chip Design (Mirhoseini, *Nature*, 2021) | 基于强化学习的芯片布局优化（谷歌芯片设计AI） | [Nature](https://www.nature.com/articles/s41586-021-03544-w) |
| C-35 | EDA 3.0: Automated Chip Design with ML (Google, 2020) | ML驱动的芯片设计自动化——EDA 3.0概念 | [Nature](https://www.nature.com/articles/s41586-021-03544-w) |
| C-36 | OpenROAD: Open-Source Autonomous RTL-GDSII Flow (DARPA) | DARPA资助的开源芯片设计完整流程工具链 | [GitHub](https://github.com/The-OpenROAD-Project/OpenROAD) |
| C-37 | Logic Synthesis in a Nutshell | 逻辑综合技术概述——从RTL到门级网表 | [Semantic Scholar](https://www.semanticscholar.org/paper/Logic-synthesis-in-a-nutshell-Ma) |
| C-38 | Clock Distribution Networks in VLSI Circuits (Friedman, 2001) | VLSI时钟分配网络与时钟树综合技术 | [IEEE Xplore](https://ieeexplore.ieee.org/document/927817) |
| C-39 | Formal Verification of Digital Circuits (R. Drechsler, 2022) | 数字电路形式化验证方法学 | [Springer](https://link.springer.com/book/10.1007/978-3-030-93828-8) |
| C-40 | High-Level Synthesis for FPGAs (J. Cong, *IEEE Access*, 2016) | FPGA高层次综合技术综述 | [IEEE Xplore](https://ieeexplore.ieee.org/document/7801076) |
| C-41 | Layout Design and Verification (DRC/LVS/Parasitic Extraction) | IC版图设计与验证技术概述 | [Semiconductor Engineering](https://semiengineering.com/) |
| C-42 | Power Distribution Networks in Modern VLSI (IR Drop & EM) | 现代VLSI供电网络、IR压降和电迁移问题 | [Semiconductor Engineering](https://semiengineering.com/) |

### 芯片制造工艺（C-43 ~ C-50）

| 编号 | 标题 | 核心主题 | 链接 |
|------|------|----------|------|
| C-43 | Semiconductor Manufacturing Technology (M. Quirk, 2001) | 半导体制造工艺教程：氧化、光刻、刻蚀、沉积、CMP | [Book](https://www.amazon.com/Semiconductor-Manufacturing-Technology-Michael-Quirk/dp/0130815209) |
| C-44 | EUV Lithography: Coming of Age (Banine 等, *SPIE*, 2022) | EUV光刻技术的成熟化历程与产业化 | [SPIE DL](https://www.spiedigitallibrary.org/) |
| C-45 | ASML High-NA EUV: The Road to Sub-2nm (2023) | ASML高数值孔径EUV光刻——通往2nm以下工艺之路 | [ASML](https://www.asml.com/en/products/euv-lithography-systems) |
| C-46 | Chemical Mechanical Planarization (CMP) for Advanced Nodes | 先进制程节点的化学机械平坦化技术 | [Semiconductor Engineering](https://semiengineering.com/knowledge_centers/manufacturing/process/cmp/) |
| C-47 | Atomic Layer Deposition (ALD) in Semiconductor Manufacturing | 原子层沉积技术在半导体制造中的应用 | [Semiconductor Engineering](https://semiengineering.com/) |
| C-48 | Yield Management in Advanced Semiconductor Manufacturing | 先进半导体制造中的良率管理方法 | [Semiconductor Engineering](https://semiengineering.com/) |
| C-49 | Semiconductor Process Variation and Design for Manufacturability (DFM) | 工艺偏差分析与可制造性设计 | [Semiconductor Engineering](https://semiengineering.com/) |
| C-50 | Samsung SF3 3nm GAA Technology (VLSI Symposium, 2023) | 三星GAA 3nm工艺（SF3）——世界首个环绕栅极量产工艺 | [IEEE Xplore](https://ieeexplore.ieee.org/document/10185353) |

### 存储器与互联（C-51 ~ C-57）

| 编号 | 标题 | 核心主题 | 链接 |
|------|------|----------|------|
| C-51 | HBM3 vs HBM2e vs GDDR6X: Memory Technology Comparison | HBM3/HBM2e/GDDR6X存储器技术对比分析 | [Semiconductor Engineering](https://semiengineering.com/) |
| C-52 | DDR5 SDRAM Standard (JEDEC JESD79-5) | DDR5 SDRAM标准规范 | [JEDEC](https://www.jedec.org/standards-documents/docs/jesd79-5) |
| C-53 | PCI Express 6.0 and CXL Interconnect Analysis | PCIe 6.0与CXL互联技术分析 | [PCI-SIG](https://pcisig.com/) |
| C-54 | Memory-Centric Computing: Near-Data Processing and PIM (2023) | 以内存为中心的计算：近数据处理和存算一体 | [arXiv](https://arxiv.org/abs/2305.01839) |
| C-55 | NVLink and NVSwitch: Multi-GPU Interconnection (NVIDIA) | NVIDIA高带宽多GPU互连技术 | [NVIDIA](https://www.nvidia.com/en-us/data-center/nvlink/) |
| C-56 | Interconnect Challenges in Scaling Beyond 2nm (Meindl, 2018) | 2nm以下工艺中互连的挑战：RC延迟、电迁移 | [IEEE Xplore](https://ieeexplore.ieee.org/document/8457361) |
| C-57 | Review of Chiplet-Based Design: System Architecture (SCIENCE CHINA, 2024) | 基于Chiplet的系统架构与互连技术综述 | [Springer](https://link.springer.com/article/10.1007/s11432-023-3926-8) |

### 先进封装（C-58 ~ C-62）

| 编号 | 标题 | 核心主题 | 链接 |
|------|------|----------|------|
| C-58 | TSMC CoWoS-S/R/L Technology Overview (TSMC, 2023) | 台积电CoWoS（Chip-on-Wafer-on-Substrate）先进封装技术 | [TSMC 3DFabric](https://3dfabric.tsmc.com/english/dedicatedFoundry/technology/cowos.htm) |
| C-59 | 3D IC Packaging: TSVs, Microbumps and Hybrid Bonding (K.N. Tu, 2011) | 3D IC封装关键技术：硅通孔（TSV）、微凸点、混合键合 | [Springer](https://link.springer.com/article/10.1007/s10854-011-0474-2) |
| C-60 | Wafer-to-Wafer Hybrid Bonding at 400nm Pitch (*Nature*, 2024) | 400nm间距晶圆混合键合——实现3D堆叠的关键突破 | [Nature](https://www.nature.com/articles/s44287-024-00019-8) |
| C-61 | Chiplet Heterogeneous Integration Technology: Status (MDPI, 2020) | Chiplet异构集成技术现状与挑战 | [MDPI](https://www.mdpi.com/2079-9292/9/4/670) |
| C-62 | GSA Heterogeneous Integration Chiplet White Paper (2023) | 全球半导体联盟（GSA）Chiplet异构集成白皮书 | [GSA](https://www.gsaglobal.org/wp-content/uploads/2023/02/2022-IPIG-Heterogenous-Integration-Chiplets-White-Paper-Final-v4.pdf) |

### 芯片产业生态（C-63 ~ C-70）

| 编号 | 标题 | 核心主题 | 链接 |
|------|------|----------|------|
| C-63 | CHIPS and Science Act of 2022 (Public Law 117-167) | 美国芯片与科学法案全文——520亿美元半导体产业激励计划 | [Congress.gov](https://www.congress.gov/117/plaws/publ167/PLAW-117publ167.pdf) |
| C-64 | Emerging Resilience in Global Semiconductor Supply Chain (SIA/BCG, 2024) | 2024年全球半导体供应链韧性分析报告 | [BCG](https://www.bcg.com/publications/2024/emerging-resilience-in-semiconductor-supply-chain) |
| C-65 | PCAST: Revitalizing the U.S. Semiconductor Ecosystem (White House, 2022) | 总统科技顾问委员会关于重振美国半导体生态系统的建议 | [White House](https://bidenwhitehouse.archives.gov/wp-content/uploads/2022/09/PCAST_Semiconductors-Report_Sep2022.pdf) |
| C-66 | The Geopolitics of the Semiconductor Industry (Carnegie, 2023) | 半导体产业地缘政治格局分析 | [Carnegie](https://carnegieendowment.org/research/2023/06/the-geopolitics-of-the-semiconductor-industry-and-indias-place-in-it) |
| C-67 | McKinsey on Semiconductors 2024 | McKinsey半导体行业洞察2024年刊 | [McKinsey](https://www.mckinsey.com/industries/semiconductors/our-insights) |
| C-68 | Gartner: Worldwide Semiconductor Revenue Grew 18% in 2024 | Gartner全球半导体营收统计（2024年$626B，增长18%） | [Gartner](https://www.gartner.com/en/newsroom/press-releases/2025-02-03-gartner-says-worldwide-semiconductor-revenue-grew-18-percent-in-2024) |
| C-69 | SIA 2024 Factbook (Semiconductor Industry Association) | 美国半导体行业协会2024年度行业数据手册 | [SIA](https://www.semiconductors.org/wp-content/uploads/2024/05/SIA-2024-Factbook.pdf) |
| C-70 | China's Semiconductor Self-Sufficiency Push (TrendForce, 2025) | 中国半导体自主化战略——出口管制影响与国产替代进展 | [TrendForce](https://www.trendforce.com/news/2025/02/14/news-chinas-semiconductor-equipment-industry-booming-self-sufficiency-to-reach-50-by-2025/) |

### 车载与边缘AI芯片（C-71 ~ C-75）

| 编号 | 标题 | 核心主题 | 链接 |
|------|------|----------|------|
| C-71 | Tesla FSD HW3.0: Custom AI Chip for Autonomous Driving (2019) | 特斯拉自研FSD芯片——14nm，双芯冗余，专为自动驾驶设计的神经网络处理器 | [AutopilotReview](https://www.autopilotreview.com/tesla-custom-ai-chips-hardware-3/) |
| C-72 | Horizon Robotics Journey Series 征程芯片架构 (2023) | 地平线征程系列车载AI芯片——面向智能驾驶的BPU架构 | [Horizon](https://www.horizon.auto/en) |
| C-73 | Functional Safety in Automotive Semiconductors: ISO 26262 Overview | ISO 26262在车载半导体设计中的功能安全实现综述 | [Semantic Scholar](https://www.semanticscholar.org/paper/FUNCTIONAL-SAFETY-IN-AUTOMOTIVE-SEMICONDUCTORS%3A-A-Rao/2eca536a41ebc8f4bf4944a54b9b86ea45eb4d82) |
| C-74 | Qualcomm Snapdragon Ride: Automotive SoC Platform (2022) | 高通Snapdragon Ride车载SoC平台——面向自动驾驶的异构计算架构 | [Qualcomm](https://www.qualcomm.com/products/automotive/snapdragon-ride-platform) |
| C-75 | Edge AI: Architecture and Deployment for Real-Time Inference (2023) | 边缘AI芯片的架构设计与实时推理部署策略 | [arXiv](https://arxiv.org/abs/2304.10891) |

---

## 📊 统计总览

| 等级 | 数量 | 说明 |
|------|------|------|
| **A级必读** | 10篇 | 奠基性论文/报告，包含详细的核心贡献和为什么必读 |
| **B级推荐** | 20