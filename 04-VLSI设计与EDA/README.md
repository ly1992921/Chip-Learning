# 04 - VLSI设计与EDA

> VLSI设计是将逻辑变为物理硅片的过程。理解设计流程，是芯片PM协调团队的基础。

## 📚 本章节学习目标

- [ ] 理解从RTL到GDSII的完整设计流程
- [ ] 了解主流EDA工具链
- [ ] 理解时序分析和物理设计
- [ ] 了解形式化验证和测试

## 🎯 核心知识点

### 4.1 设计流程概览
- 前端设计：RTL → 综合 → 门级网表
- 后端设计：Floorplan → Place → Route → Signoff
- 验证：功能验证、形式化验证、物理验证
- **PM视角**: 理解每个阶段的交付物和里程碑

### 4.2 逻辑综合
- RTL到门级网表的转换
- 约束文件（SDC）
- 优化策略（面积/速度/功耗）
- **PM视角**: 综合质量直接影响后端实现

### 4.3 物理设计
- Floorplan（布局规划）
- Placement（标准单元放置）
- Clock Tree Synthesis（时钟树综合）
- Routing（布线）
- **PM视角**: 物理设计决定芯片面积和功耗

### 4.4 时序分析
- Setup/Hold时间
- 静态时序分析（STA）
- 时序收敛
- **PM视角**: 时序不收敛 = 芯片可能无法工作

### 4.5 EDA工具链
- Synopsys: Design Compiler, ICC2, PrimeTime
- Cadence: Genus, Innovus, Tempus
- Mentor: Calibre, Questa
- **PM视角**: 工具链选择影响成本和效率

## 🔗 推荐资源

| 资源类型 | 名称 | 链接 | 难度 |
|----------|------|------|------|
| 教材 | 《CMOS VLSI Design》(Weste & Harris) | [Addison Wesley](https://www.pearson.com) | ⭐⭐⭐ |
| 教材 | 《Physical Design for VLSI》 | ⭐⭐⭐ |
| 课程 | NTU VLSI Design | [YouTube](https://www.youtube.com/) | ⭐⭐⭐ |
| 工具 | OpenROAD/OpenLANE | [GitHub](https://github.com/The-OpenROAD-Project) | ⭐⭐ |

## ✅ 检查清单

- [ ] 理解RTL到GDSII的完整流程
- [ ] 理解逻辑综合的作用
- [ ] 理解物理设计各阶段
- [ ] 理解Setup/Hold时序
- [ ] 了解主流EDA工具
