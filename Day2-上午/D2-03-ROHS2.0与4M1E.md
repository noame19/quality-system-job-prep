# D2-03｜ROHS 2.0 + 4M1E 制造业基础

> ⏱ 时长：60 min（09:30–10:30）
> 🎯 目标：背熟 RoHS 10 项物质 + 4M1E 五大要素
> 📎 输出物：RoHS 速查卡 + 生产流程图

---

## 一、RoHS 是什么

- **全称**：Restriction of Hazardous Substances（有害物质限制指令）
- **起源**：欧盟 2003 年发布 2002/95/EC 指令，2011 年升级为 **RoHS 2.0（2011/65/EU）**
- **目的**：限制电子电气产品中的有害物质使用
- **范围**：几乎所有电子电气产品（电源线、PCB、家电、连接器……）
- **核心地位**：进入欧盟市场的**强制门槛**（= 没做就进不去）

> **电子制造业不知道 RoHS = 文盲**

---

## 二、RoHS 2.0 十项有害物质（**必背**）

| # | 中文 | 英文 / 缩写 | 限值 ppm | 常见存在 |
|---|---|---|---|---|
| 1 | 铅 | Lead / Pb | **≤ 1000** | 焊料、玻璃、PVC 稳定剂 |
| 2 | 镉 | Cadmium / Cd | **≤ 100** | 开关、弹簧、连接器、PCB、电池 |
| 3 | 汞 | Mercury / Hg | ≤ 1000 | 温控器、传感器、开关、灯泡 |
| 4 | 六价铬 | Cr VI | ≤ 1000 | 金属防腐蚀涂层、电镀 |
| 5 | 多溴联苯 | PBB | ≤ 1000 | 阻燃剂（PCB、塑料外壳） |
| 6 | 多溴二苯醚 | PBDE | ≤ 1000 | 阻燃剂（PCB、塑料外壳） |
| 7 | 邻苯二甲酸二异丁酯 | DIBP | ≤ 1000 | PVC 增塑剂 |
| 8 | 邻苯二甲酸二丁酯 | DBP | ≤ 1000 | PVC、电缆、插座 |
| 9 | 邻苯二甲酸丁苄酯 | BBP | ≤ 1000 | PVC 地板、合成皮革 |
| 10 | 邻苯二甲酸二己酯 | DEHP | ≤ 1000 | PVC、电缆绝缘 |

**重点**：镉 Cd 的限值最严（100ppm），其他都是 1000ppm。

**4 个邻苯**（DEHP/DBP/BBP/DIBP）是 2015 年新增的，**俗称 RoHS 2.0 的 4 项新物质**。

---

## 三、RoHS 测试方法（文控岗不需要操作，但要懂）

| 物质 | 检测方法 |
|---|---|
| Pb、Cd、Hg | ICP-OES（电感耦合等离子体发射光谱仪） |
| Cr VI | UV-Vis（紫外可见分光光度计） |
| PBB、PBDE、DIBP、DBP、BBP、DEHP | GC-MS（气相色谱质谱联用仪） |

---

## 四、AC 电源线行业的 RoHS 重点

AC 电源线虽然结构简单，但 RoHS 涉及多个部件：

| 部件 | RoHS 风险点 |
|---|---|
| **导体**（铜丝） | 铜本身无问题，但镀锡工艺可能含 Pb |
| **绝缘层**（PVC） | 含 DIBP/DBP/BBP/DEHP（4 个邻苯） |
| **护套** | 同上 |
| **插头** | 铜片 + 塑料外壳，可能含 PBB/PBDE |
| **尾卡** | 油墨可能含 Pb/Cr VI |

**文控岗动作**：
- 收集每批原材料的 RoHS 报告（由供应商提供）
- 维护《RoHS 物质清单》
- 每年做 1 次 RoHS 检测（送第三方实验室，如 SGS/CTI/谱尼）
- 客户验厂时提供 RoHS 报告

---

## 五、RoHS vs REACH（**容易混淆**）

| | RoHS | REACH |
|---|---|---|
| 全称 | Restriction of Hazardous Substances | Registration, Evaluation, Authorisation and Restriction of Chemicals |
| 范围 | 电子电气产品 | **所有**化学物质 |
| 性质 | 限制有害物质在产品中的含量 | 限制有害化学品的生产和使用 |
| 国家 | 欧盟强制 | 欧盟强制 |
| 数量 | 10 项 | **233 项** SVHC 高关注物质（每年增加） |
| 测试 | 必测 | 部分产品需申报 |

> **面试金句**：RoHS 是"产品里有什么不能超标"，REACH 是"工厂里用什么化学品要先注册"。

---

## 六、生产五大要素（**4M1E**）—— 必背

任何生产过程，都由这 5 个要素决定质量：

| 要素 | 英文 | 中文 | 含义 | 文控岗相关 |
|---|---|---|---|---|
| **Man** | Man | 人 | 操作者技能、培训 | 培训记录归档 |
| **Machine** | Machine | 机 | 设备、工装、模具 | 设备台账、校准证书 |
| **Material** | Material | 料 | 原材料、外购件 | 物料规格书、RoHS 报告 |
| **Method** | Method | 法 | 工艺、作业方法 | **SOP/WI**（文控主战场） |
| **Measurement** | Measurement | 测 | 测量方法、仪器 | 测量系统分析 MSA |
| **Environment** | Environment | 环 | 温湿度、照明、噪声 | 环境监控记录 |

**口诀**：**人机料法测环**（rén jī liào fǎ cè huán）

---

## 七、生产流程（**IQC → IPQC → OQC**）

```
原材料采购
    ↓
来料检验 (IQC) ← 进料抽检，不良退货
    ↓
入库 / 上料
    ↓
制程巡检 (IPQC) ← 生产线抽检、不良隔离
    ↓
装配 / 加工
    ↓
首件确认 (FAI) ← 每批次开始第一件必检
    ↓
老化测试 / 可靠性测试 ← 部分产品
    ↓
成品检验 (OQC) ← 出货前抽检
    ↓
包装 / 入库
    ↓
出货
```

**缩写记忆**：
- **IQC** = Incoming Quality Control（来料）
- **IPQC** = In-Process Quality Control（制程）
- **OQC** = Outgoing Quality Control（出货）
- **FQC** = Final Quality Control（最终）

---

## 八、生产流程图（**画出来贴墙上**）

```
[客户订单]
    ↓
[订单评审] ← 销售/生产/品质三部门会签
    ↓
[采购原材料]
    ↓
[IQC 来料检验] ← 抽样标准 ANSI/ASQ Z1.4
    ↓
[生产排程]
    ↓
[领料 / 上料]
    ↓
[首件确认 FAI]
    ↓
[批量生产]
    ↓
[IPQC 制程巡检] ← 每 2 小时抽检
    ↓
[老化测试] ← AC 电源线：通电老化 1-4 小时
    ↓
[OQC 出货检验]
    ↓
[RoHS 测试报告] ← 每批必查
    ↓
[包装 / 入库]
    ↓
[出货 / 交付]
```

---

## 九、文控岗的"5 大要素"对应动作

| 4M1E | 文控岗对应文件 | 来源 |
|---|---|---|
| Man 人 | 培训记录、培训计划、培训签到表 | HR + QA 协同 |
| Machine 机 | 设备台账、校准证书、设备操作 WI | 设备部 |
| Material 料 | 物料规格书、RoHS 报告、供应商资质 | 采购 + QA |
| Method 法 | **SOP/WI、工艺流程图、ECN** | 工程部 |
| Measurement 测 | MSA 报告、测量设备校准证书 | QA |
| Environment 环 | 环境监控记录（温湿度） | 行政 |

---

## 十、推荐学习资源

### 📺 视频
1. **RoHS 2.0 详解**  
   https://search.bilibili.com/all?keyword=RoHS%202.0
2. **RoHS 检测方法 ICP-OES 原理**  
   https://search.bilibili.com/all?keyword=ICP-OES
3. **4M1E 五大要素讲解**  
   https://search.bilibili.com/all?keyword=4M1E

### 📖 文章
1. **RoHS 2.0 十项有害物质详解**  
   https://www.dgntek.org.cn/xinwenzixun/guojifaguidongtai/2021/1125/174904.html
2. **车灯研究院：欧盟 RoHS 2.0 指令详解**  
   https://www.dengdengschool.com/article/zixun/2220.html

---

## 十一、自测题

1. RoHS 2.0 十项物质是什么？
2. Cd（镉）的限值是多少？其他物质呢？
3. RoHS 和 REACH 的区别？
4. 4M1E 五大要素是什么？文控岗对应什么文件？
5. IQC/IPQC/OQC 分别指什么？

**参考答案**：
1. Pb、Cd、Hg、Cr VI、PBB、PBDE、DIBP、DBP、BBP、DEHP
2. Cd ≤ 100ppm；其他 ≤ 1000ppm
3. RoHS 管产品里的物质；REACH 管所有化学品
4. 人机料法测环（详见第九节）
5. 来料 / 制程 / 出货

---

## 十二、本节作业

- [ ] 背熟 RoHS 10 项（前 4 项必须按顺序）
- [ ] 画生产流程图（第七节）
- [ ] 默写 4M1E + 口诀