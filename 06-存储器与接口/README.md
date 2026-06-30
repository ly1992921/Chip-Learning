# 06 - 存储器与接口

> 存储器是芯片系统的核心组件。"内存墙"是当前AI计算面临的最大瓶颈之一。

## 📚 本章节学习目标

- [ ] 理解SRAM、DRAM、Flash的原理和特性
- [ ] 掌握DDR、PCIe、CXL等接口技术
- [ ] 了解HBM和新型存储器
- [ ] 理解存储层次对AI性能的影响

## 🎯 核心知识点

### 6.1 SRAM
- 6T单元结构
- 速度快、密度低、功耗较高
- L1/L2/L3缓存实现
- **PM视角**: 缓存大小和层次影响CPU性能

### 6.2 DRAM
- 1T1C单元结构
- 需要刷新操作
- DDR4/DDR5/LPDDR演进
- **PM视角**: 内存容量和带宽是系统瓶颈

### 6.3 Flash存储
- NAND Flash结构
- 3D NAND技术
- SLC/MLC/TLC/QLC
- **PM视角**: 存储密度与寿命的权衡

### 6.4 HBM (High Bandwidth Memory)
- 3D堆叠结构
- TSV技术
- HBM2/HBM2E/HBM3
- **PM视角**: HBM是AI芯片的关键使能技术

### 6.5 接口技术
- DDR: 内存接口
- PCIe: 高速串行互联
- CXL: 内存扩展互联
- UCIe: Chiplet互联
- **PM视角**: 接口带宽决定系统扩展性

## 🔗 推荐资源

| 资源类型 | 名称 | 链接 | 难度 |
|----------|------|------|------|
| 教材 | 《Memory Systems》(Bruce Jacob) | [Morgan Kaufmann](https://www.elsevier.com) | ⭐⭐⭐ |
| 论文 | HBM Architecture | [IEEE JSSC](https://ieeexplore.ieee.org) | ⭐⭐⭐ |
| 标准 | JEDEC DDR5 | [JEDEC](https://www.jedec.org) | ⭐⭐⭐ |
| 报告 | Memory Market Analysis | [Yole](https://www.yolegroup.com) | ⭐⭐ |

## ✅ 检查清单

- [ ] 理解SRAM/DRAM/Flash的基本原理
- [ ] 理解DDR/PCIe/CXL接口
- [ ] 理解HBM架构
- [ ] 了解新型存储器（ReRAM/PCM/MRAM）
- [ ] 理解存储层次对性能的影响
