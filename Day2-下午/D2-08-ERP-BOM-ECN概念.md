# D2-08｜ERP + BOM + ECN 概念（文控岗必备术语）

> ⏱ 时长：30 min（17:30–18:00）
> 🎯 目标：能讲清 3 个核心术语 + 知道文控岗在 ERP 里做什么
> 📎 输出物：名词解释卡

---

## 一、ERP 是什么（30 秒讲清）

- **全称**：Enterprise Resource Planning 企业资源计划
- **本质**：把公司所有业务（采购 / 销售 / 库存 / 生产 / 财务）装进一个软件
- **常见 ERP**（制造业）：
  - 用友 U8 / NC
  - 金蝶 K3 / Cloud
  - SAP（外资 / 大厂）
  - Oracle EBS（外资 / 大厂）
  - 鼎捷（台资）
  - 管家婆 / 速达（小厂）
- **文控岗用 ERP 的频率**：**每天**（查 BOM、改 ECN、走文件审批）

**面试金句**：ERP 是公司业务的"中央数据库"，所有部门共用一套数据，避免信息孤岛。

---

## 二、BOM（物料清单）

**全称**：Bill of Materials

### 1. 什么是 BOM
- **本质**：一份产品的"配方"——做出这个产品需要哪些物料、各多少
- **层级**：
  - **顶层 BOM**：成品（如 AC 电源线）
  - **子层 BOM**：半成品 / 组件（如插头组件）
  - **底层 BOM**：原材料（如铜丝、PVC 料）

### 2. AC 电源线 BOM 示例（**面试必背**）

| 序号 | 物料编码 | 物料名称 | 规格 | 单位 | 用量 | 损耗率 | 备注 |
|---|---|---|---|---|---|---|---|
| 1 | W-001 | 镀锡铜丝 | 0.75mm² | kg | 0.10 | 2% | 导体 |
| 2 | W-002 | PVC 绝缘料 | 70℃ 灰色 | kg | 0.05 | 3% | 绝缘层 |
| 3 | W-003 | PVC 护套料 | 70℃ 黑色 | kg | 0.08 | 3% | 护套 |
| 4 | P-001 | 国标三插 | 10A 250V | pcs | 1 | 1% | 插头 |
| 5 | A-001 | 尾卡 | 70×40mm | pcs | 1 | 0% | 标识 |
| 6 | A-002 | 扎带 | 100mm | pcs | 1 | 0% | 包装 |

### 3. BOM 维护的"5 个准确"

| 维度 | 含义 |
|---|---|
| **物料编码准确** | 不重号、不漏号 |
| **物料名称准确** | 与供应商、仓库口径一致 |
| **规格准确** | 尺寸 / 型号 / 颜色 |
| **用量准确** | 按实际工艺定（含损耗率） |
| **替代关系准确** | 主料 + 替代料（如铜丝涨价时换铜包钢） |

---

## 三、ECN（工程变更通知）

**全称**：Engineering Change Notice

### 1. 触发场景

| 触发原因 | 例子 |
|---|---|
| **客户要求** | Walmart 要求线材加粗到 1.0mm² |
| **法规变化** | RoHS 新增邻苯物质 |
| **成本优化** | PVC 供应商涨价，换更便宜的 |
| **质量问题** | 某插头不良率高，更换供应商 |
| **工艺改进** | 取消一道老化工序 |

### 2. ECN 全流程（**必背 7 步**）

```
1. 申请 → 工程师填《ECN 申请单》
       ↓
2. 评审 → 品质/采购/生产/销售会签
       ↓
3. 批准 → 工程经理 / 总经理
       ↓
4. 执行
   • 更新规格书 (SOP / SPEC)
   • 更新 BOM (ERP)
   • 更新工艺
   • 更新 RoHS 报告
   • 更新产品认证
       ↓
5. 【文控岗】编号 + 发放 + 旧版回收
       ↓
6. 首批试产 → IPQC/OQC 验证
       ↓
7. 量产 + 跟踪效果
```

### 3. ECN 模板

```
┌──────────────────────────────────────────────┐
│           工程变更通知 (ECN)                   │
├──────────────┬───────────────────────────────┤
│ ECN 编号     │ ECN-2024-015                  │
│ 申请日期     │ 2024-06-15                    │
│ 产品名称     │ AC 电源线 H05VV-F 3G 0.75mm² │
│ 变更类型     │ ☐ 设计 ☐ 工艺 ☑ 物料 ☐ 文件  │
│ 变更原因     │ 客户 Walmart 要求加粗到 1.0mm²│
├──────────────┴───────────────────────────────┤
│ 变更前:                                       │
│   物料 W-001: 0.75mm² 镀锡铜丝               │
│ 变更后:                                       │
│   物料 W-001: 1.0mm² 镀锡铜丝                │
├──────────────────────────────────────────────┤
│ 影响评估:                                     │
│   □ RoHS  □ 性能  ☑ 成本  □ 工艺              │
│   成本变化: +5%                              │
├──────────────────────────────────────────────┤
│ 申请人: 张三 (工程师)                         │
│ 评审: 李四(品保) / 王五(采购) / 赵六(生产)    │
│ 批准: 孙七 (总经理)  2024-06-18              │
├──────────────────────────────────────────────┤
│ 实施日期: 2024-06-25                          │
│ 首批试产日期: 2024-06-26                      │
└──────────────────────────────────────────────┘
```

### 4. 文控岗在 ECN 中的关键动作（**面试要点**）

1. **编号**：ECN-YYYY-NNN（年份+3 位流水号）
2. **发放**：E-MAIL 通知所有相关部门 + 文件夹存档
3. **旧版回收**：
   - 规格书旧版 → 收回
   - BOM 在 ERP 里更新（不能直接改原 BOM，要新建版本）
   - RoHS 报告 → 申请新版本
4. **更新文件总清单**
5. **跟踪**：确认试产通过、量产稳定

---

## 四、其他高频术语（30 个核心名词速查）

| 术语 | 全称 | 一句话解释 |
|---|---|---|
| **FAI** | First Article Inspection | 首件确认 |
| **PPAP** | Production Part Approval Process | 生产件批准程序（汽车业） |
| **APQP** | Advanced Product Quality Planning | 产品质量先期策划 |
| **FMEA** | Failure Mode and Effects Analysis | 失效模式分析 |
| **SPC** | Statistical Process Control | 统计过程控制 |
| **MSA** | Measurement System Analysis | 测量系统分析 |
| **CPK** | Process Capability Index | 过程能力指数 |
| **OEE** | Overall Equipment Effectiveness | 设备综合效率 |
| **5S** | 整理/整顿/清扫/清洁/素养 | 现场管理 |
| **CAPA** | Corrective and Preventive Action | 纠正预防措施 |
| **NCR** | Non-Conformance Report | 不符合项报告 |
| **SOP** | Standard Operating Procedure | 标准作业程序 |
| **WI** | Work Instruction | 作业指导书 |
| **DCC** | Document Control Center | 文控中心 |
| **PLM** | Product Lifecycle Management | 产品生命周期管理 |
| **MES** | Manufacturing Execution System | 制造执行系统 |
| **WMS** | Warehouse Management System | 仓库管理系统 |
| **CRM** | Customer Relationship Management | 客户关系管理 |
| **SRM** | Supplier Relationship Management | 供应商关系管理 |
| **CAR** | Corrective Action Request | 纠正措施要求 |
| **PAR** | Preventive Action Request | 预防措施要求 |
| **QSA** | Quality System Audit | 质量体系审核 |
| **QMS** | Quality Management System | 质量管理体系 |
| **EMS** | Environmental Management System | 环境管理体系 |
| **OHSMS** | Occupational Health & Safety MS | 职业健康安全管理体系 |
| **CNAS** | China National Accreditation | 中国合格评定国家认可委员会 |
| **CMA** | China Inspection Body accreditation | 检验检测机构资质认定 |
| **ANSI/ASQ Z1.4** | 抽样标准 | 计数抽样标准（美标） |
| **GB/T 2828.1** | 抽样标准 | 计数抽样标准（国标） |
| **ISO 17025** | 检测实验室能力 | 实验室认可标准 |

---

## 五、面试 Q&A

### Q1：你没用过 ERP 怎么办？

**答**：
> 我之前工作中接触较少，但我对 ERP 的原理理解——它是把公司所有业务（采购、库存、生产、销售、财务）装进一个系统，避免信息孤岛。我对 BOM、ECN 这些核心概念很熟。我学习软件上手很快（数字化背景），给我 1-2 周就能熟练操作。

### Q2：BOM 和 ECN 的关系是什么？

**答**：
> BOM 是产品的"配方"，ECN 是变更这个配方的"通知"。任何 BOM 变更都要走 ECN 流程——申请、评审、批准、执行、文控发放、首试、量产。ECN 是"流程"，BOM 是"内容"，文控岗要确保流程闭环、内容同步。

---

## 六、推荐学习资源

### 📺 视频
1. **ERP 系统入门（B 站）**  
   https://search.bilibili.com/all?keyword=ERP%20%E5%85%A5%E9%97%A8
2. **BOM 维护实操**  
   https://search.bilibili.com/all?keyword=BOM%20%E7%BB%B4%E6%8A%A4
3. **ECN 流程实例**  
   https://search.bilibili.com/all?keyword=ECN%20%E6%B5%81%E7%A8%8B

### 📖 文章
1. **ERP 是什么（一文读懂）**  
   https://www.zhihu.com/search?type=content&q=ERP%20%E6%98%AF%E4%BB%80%E4%B9%88
2. **制造业术语速查**  
   https://www.zhihu.com/search?type=content&q=%E5%88%B6%E9%80%A0%E4%B8%9A%20%E6%9C%AF%E8%AF%AD

---

## 七、自测题

1. ERP 是什么？列举 3 个常见 ERP。
2. BOM 的"5 个准确"是什么？
3. ECN 7 步流程是哪些？
4. 文控岗在 ECN 中的 5 个关键动作是什么？

**参考答案**：
1. 企业资源计划；用友 / 金蝶 / SAP
2. 编码 / 名称 / 规格 / 用量 / 替代关系 准确
3. 申请→评审→批准→执行→编号发放+回收→试产→量产
4. 编号、发放、旧版回收、更新总清单、跟踪

---

## 八、本节作业

- [ ] 背熟 ERP/BOM/ECN 3 个术语
- [ ] 默写 ECN 7 步流程
- [ ] 准备面试答案："BOM 和 ECN 的关系"
- [ ] 浏览名词速查表（30 个术语）