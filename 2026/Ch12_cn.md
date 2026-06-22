# Chapter 12：电路（Circuits）
## 考纲综合整理：

### 【AP Physics 2】Unit 11：Electric Circuits

| 编号 | 知识点 | 核心公式/概念 | 技能 |
|:--:|:--|:--|:--:|
| **11.1** | 电流 | $I=\frac{\Delta Q}{\Delta t}$ | 2.A, 2.B |
| **11.2** | 简单电路 | 串联（电流相同）、并联（电压相同） | 1.A, 2.C |
| **11.3** | 电阻与欧姆定律 | $R=\rho\frac{L}{A}$；$V=IR$ | 2.A, 2.B |
| **11.4** | 电功率 | $P=IV=I^2R=\frac{V^2}{R}$ | 2.B, 2.D |
| **11.5** | 复合直流电路 | 串并联组合等效电阻 $R_{eq}$ | 2.A, 2.B |
| **11.6** | 基尔霍夫回路法则 | $\Sigma V=0$ 绕回路一周 | 2.A, 3.B |
| **11.7** | 基尔霍夫节点法则 | $\Sigma I_{in}=\Sigma I_{out}$ | 2.A, 3.B |
| **11.8** | RC 电路 | 充电 $q(t)=Q_f(1-e^{-t/RC})$；放电 $q(t)=Q_0e^{-t/RC}$；$\tau=RC$ | 1.C, 2.D |

### 【AP Physics C: E&M】Unit 3：Electric Circuits（🟣 微积分深化）

| 编号 | 知识点 | 核心公式/概念 | 🟣 微积分关键 |
|:--:|:--|:--|:--|
| **3.1** | 电流与电阻 | $I=\frac{dQ}{dt}$；$R=\rho\frac{L}{A}$ | 🟣 $I=dQ/dt$ |
| **3.2** | 功率 | $P=I^2R=IV$ | — |
| **3.3** | 稳态直流电路 | 基尔霍夫法则；串并联分析 | 🟣 矩阵方法解多回路 |
| **🔑 3.4** | **含电容器的电路（独家深化）** | RC 充放电 $q(t)=Q_f(1-e^{-t/RC})$ | 🟣 **微分方程推导**：$R\frac{dq}{dt}+\frac{q}{C}=\mathcal{E}$ |


---
---

# Chapter 11 / Unit 3：直流电路 — 完整推导参考文档

**AP Physics 2 Unit 11 + AP Physics C: E&M Unit 3 · 以推导为中心**

---

## 绪论：电路的逻辑链条

电路理论可以看作静电学的自然延伸——电场 $\vec{E}$ 在导体中驱动电荷运动形成电流，而电流流过电阻将电能转化为热能。

**逻辑链条：**
1. **电场 $\Rightarrow$ 电流：** $\vec{E} \neq 0$ 在导体内 $\Rightarrow$ 自由电荷受力 $\Rightarrow$ 定向运动 $\Rightarrow$ 电流 $I = dQ/dt$
2. **电流 $\Rightarrow$ 电压降：** 电荷流过电阻消耗能量 $\Rightarrow$ 电势降低 $\Rightarrow$ 欧姆定律 $V=IR$
3. **能量转化：** 电场能 $\rightarrow$ 热能（电阻）、磁场能（电感，后续章节）、化学能（电池）
4. **守恒律：** 能量守恒（基尔霍夫回路法则）+ 电荷守恒（基尔霍夫节点法则）
5. **动态过程：** 储能元件（电容）使电流随时间变化 $\rightarrow$ 微分方程

---

# 11.1 / 3.1 电流 — 三种推导视角

## 核心公式：$I = \dfrac{dQ}{dt}$，$I = nAev_d$

---

**推导1：电流的定义与微观表述**

**宏观定义：** $I = \frac{dQ}{dt}$——单位时间内通过导体横截面的电荷量。方向定义为正电荷运动方向（实际电子运动的反方向）。

**微观模型：** 导体中自由电子密度 $n$（单位体积内的自由电子数），导体横截面积 $A$，电子漂移速度 $v_d$。

在时间 $\Delta t$ 内，电子移动距离 $\Delta x = v_d\Delta t$。通过横截面 $A$ 的体积为 $A v_d\Delta t$，包含的电子数为 $n A v_d\Delta t$，电荷量为 $\Delta Q = nA v_d\Delta t \cdot e$。

$I = \frac{\Delta Q}{\Delta t} = nAev_d$

**数量级估算：** 铜导线中 $n \approx 8.5\times10^{28}\ \text{m}^{-3}$，$A=1\ \text{mm}^2$，$I=1\ \text{A}$：
$v_d = \frac{I}{nAe} = \frac{1}{(8.5\times10^{28})(10^{-6})(1.6\times10^{-19})} \approx 7.4\times10^{-5}\ \text{m/s}$

电子漂移速度仅约 $0.074$ mm/s！但电路中"开灯瞬间就亮"是因为电磁场以光速传播——电子本身移动缓慢，但电场变化信号传播极快。

---

**推导2：电流密度 $\vec{J}$ 与欧姆定律的微观形式**

定义电流密度：$\vec{J} = nq\vec{v}_d$，单位 $\text{A/m}^2$。$I = \int\vec{J}\cdot d\vec{A}$

微观欧姆定律：$\vec{J} = \sigma\vec{E}$（$\sigma$ 为电导率，$\rho = 1/\sigma$ 为电阻率）

**推导：** 电子在电场中受力 $\vec{F} = -e\vec{E}$，加速 $a = -e\vec{E}/m_e$。与晶格碰撞产生阻力，平均漂移速度 $v_d = -\frac{e\tau}{m_e}E$（$\tau$ 为平均自由时间）。$\vec{J} = -ne\vec{v}_d = \frac{ne^2\tau}{m_e}\vec{E}$，所以 $\sigma = \frac{ne^2\tau}{m_e}$。

---

**推导3：从 $\vec{J}=\sigma\vec{E}$ 到 $V=IR$**

对长度为 $L$、横截面积 $A$ 的均匀导体，内部电场均匀 $E = V/L$（假设沿长度方向）。

$I = JA = \sigma EA = \sigma\frac{V}{L}A = \frac{V}{\rho L/A} = \frac{V}{R}$

所以电阻 $R = \rho\frac{L}{A}$，电阻率 $\rho = 1/\sigma$。

**物理直观：** 电阻与长度成正比（长路径更多碰撞），与横截面积成反比（宽路径更多电子同时通过）。

---

# 11.2 / 3.3 简单电路与串并联

## 核心公式：串联 $R_{eq}=R_1+R_2$，并联 $1/R_{eq}=1/R_1+1/R_2$

---

**推导1：串联电路**

串联：各元件依次连接，电流相同 $I$，总电压等于各元件电压之和。

$V_{\text{总}} = V_1 + V_2 = IR_1 + IR_2 = I(R_1+R_2)$
$R_{eq} = \frac{V_{\text{总}}}{I} = R_1 + R_2$

**物理原因：** 串联增加了"阻碍长度"，电子必须穿过更多电阻——等效于增加长度。

---

**推导2：并联电路**

并联：各元件两端电压相同 $V$，总电流等于各支路电流之和。

$I_{\text{总}} = I_1 + I_2 = \frac{V}{R_1} + \frac{V}{R_2} = V\left(\frac{1}{R_1}+\frac{1}{R_2}\right)$
$\frac{1}{R_{eq}} = \frac{I_{\text{总}}}{V} = \frac{1}{R_1}+\frac{1}{R_2}$

**物理原因：** 并联增加了"通道数量"，电子有更多路径可选——等效于增加横截面积。

---

**推导3：串联 vs 并联的类比**

串联 $\leftrightarrow$ 增加长度：$R \propto L$
并联 $\leftrightarrow$ 增加面积：$R \propto 1/A$

这个类比来自 $R = \rho L/A$——串联接长了导体，并联加粗了导体。

---

# 11.3 / 3.1 电阻与欧姆定律 — 四种推导

## 核心公式：$V=IR$，$R=\rho L/A$，$\rho = \rho_0[1+\alpha(T-T_0)]$

---

**推导1：从微观电子运动推导欧姆定律**

电子在电场中的运动方程：$m\frac{d\vec{v}}{dt} = -e\vec{E} - \frac{m}{\tau}\vec{v}$

稳态解（$\frac{d\vec{v}}{dt}=0$）：$0 = -e\vec{E} - \frac{m}{\tau}\vec{v}_d$ $\Rightarrow$ $\vec{v}_d = -\frac{e\tau}{m}\vec{E}$

电流密度：$\vec{J} = -ne\vec{v}_d = \frac{ne^2\tau}{m}\vec{E} = \sigma\vec{E}$

所以 $I = JA = \sigma EA = \sigma\frac{V}{L}A = \frac{V}{\rho L/A} = \frac{V}{R}$ ✓

其中 $\tau$ 是平均自由时间（$10^{-14}$ s 量级），$n$ 是自由电子密度（$10^{28}-10^{29}$ m$^{-3}$ 量级）。

---

**推导2：温度对电阻的影响**

电阻率 $\rho$ 随温度升高而增加（金属）：
$\rho(T) = \rho_0[1 + \alpha(T-T_0)]$

**微观解释：** 温度升高 $\Rightarrow$ 晶格振动加剧 $\Rightarrow$ 电子与晶格碰撞更频繁 $\Rightarrow$ 平均自由时间 $\tau$ 减小 $\Rightarrow$ 电导率 $\sigma \propto \tau$ 降低 $\Rightarrow$ 电阻率 $\rho$ 升高。

**半导体例外：** 温度升高时更多电子从价带跃迁到导带，$n$ 增加主导 $\Rightarrow$ 电阻率降低。这就是热敏电阻（NTC）的原理。

---

**推导3：非欧姆器件的分析**

欧姆定律 $V=IR$ 对部分器件不成立：
- 二极管：正向导通大电流，反向几乎不导通——$I-V$ 关系指数型
- 热敏电阻：$R$ 随 $T$ 非线性变化
- 气体放电管：击穿前近似绝缘，击穿后电流剧增

**区分方法：** 欧姆器件 $I-V$ 曲线是过原点的直线（$R$ 常数），非欧姆器件 $I-V$ 曲线非线性。

---

**推导4：电阻颜色编码的系统解读**

电阻的四色环或五色环编码：
- 前两/三环表有效数字，下一环表10的幂次（乘数），最后一环表容差

例：红-红-棕-金 $\Rightarrow$ $22 \times 10^1 = 220\ \Omega$，$\pm5\%$

---

# 11.4 / 3.2 电功率 — 三种推导

## 核心公式：$P = IV = I^2R = V^2/R$

---

**推导1：从电场力做功推导**

电荷 $q$ 通过电势差 $V$ 时，电场做功 $W = qV$。
功率为单位时间做功：$P = \frac{W}{t} = \frac{qV}{t} = IV$

由欧姆定律 $V=IR$ 代入：
$P = I(IR) = I^2R$ 或 $P = \frac{V}{R}\cdot V = \frac{V^2}{R}$

**三种形式等价（对纯电阻电路），但适用场景不同：**
- $P=IV$：最通用，适合任何电路元件（包括非欧姆）
- $P=I^2R$：适合已知电流——串联电路中常用（电流相同）
- $P=V^2/R$：适合已知电压——并联电路中常用（电压相同）

---

**推导2：焦耳热的微观图像**

电子在电场中加速获得动能，与晶格碰撞时将能量传递给晶格（即转化为热）。

单个电子在两次碰撞间从电场获得的能量 $\approx eE \cdot v_d\tau$。
功率密度（单位体积发热率）：$p = n\cdot eE v_d = J\cdot E = \sigma E^2 = \frac{J^2}{\sigma}$

总功率：$P = \int p\,dV = \sigma E^2 AL = \sigma\left(\frac{V}{L}\right)^2 AL = \frac{\sigma A}{L}V^2 = \frac{V^2}{R}$ ✓

---

**推导3：电池输出功率与外阻关系**

电池电动势 $\mathcal{E}$，内阻 $r$，外电阻 $R$。
回路电流：$I = \frac{\mathcal{E}}{R+r}$
输出功率（外电阻上消耗）：$P = I^2R = \frac{\mathcal{E}^2R}{(R+r)^2}$

**最大功率传输定理：** $dP/dR = 0$ 时 $P$ 取最大值。
$P = \mathcal{E}^2 R (R+r)^{-2}$
$\frac{dP}{dR} = \mathcal{E}^2\left[(R+r)^{-2} - 2R(R+r)^{-3}\right] = \frac{\mathcal{E}^2}{(R+r)^3}(r-R)=0$
$\Rightarrow$ $R = r$（外阻等于内阻时输出功率最大）

最大功率：$P_{\max} = \frac{\mathcal{E}^2}{4r}$

---

# 11.6-7 / 3.3 基尔霍夫法则 — 四种推导

## 核心公式：$\sum I_{\text{in}} = \sum I_{\text{out}}$，$\sum V = 0$ 绕回路

---

**推导1：节点法则的物理基础 — 电荷守恒**

在任一节点处，电荷不能累积（稳态下）。流入节点的总电流 = 流出节点的总电流。
$\sum I_{\text{in}} = \sum I_{\text{out}}$

**等价于：** $\sum I = 0$（约定流入为正，流出为负）

**微观解释：** 若 $\sum I_{\text{in}} \neq \sum I_{\text{out}}$，节点处电荷会不断积累——但积累电荷会产生电场阻止更多电荷流入，直到平衡。稳态下必然相等。

---

**推导2：回路法则的物理基础 — 能量守恒**

绕闭合回路一周，总电势变化为零（回到同一点，电势相同）。
$\sum \Delta V = 0$

穿过的元件：
- 电阻（电流方向与绕行方向相同）：$\Delta V = -IR$；相反：$\Delta V = +IR$
- 电池（从负极到正极通过电池内部）：$\Delta V = +\mathcal{E}$；相反：$\Delta V = -\mathcal{E}$

**物理原因：** 电场是保守场，$\oint\vec{E}\cdot d\vec{l}=0$。电势是单值函数——绕一圈回到起点电势必须相同。

---

**推导3：基尔霍夫法则分析电路的完整框架**

步骤：
1. 标定所有未知电流的方向（任意假设，结果为负说明实际方向相反）
2. 在节点处应用节点法则（$n-1$ 个独立方程，$n$ 为节点数）
3. 选择独立回路，应用回路法则（$m$ 个方程，$m$ 为网孔数）
4. 解线性方程组

**例：两回路电路**
回路1（含 $\mathcal{E}_1, R_1, R_3$）：$\mathcal{E}_1 - I_1R_1 - I_3R_3 = 0$
回路2（含 $\mathcal{E}_2, R_2, R_3$）：$\mathcal{E}_2 - I_2R_2 - I_3R_3 = 0$
节点：$I_3 = I_1 + I_2$

三个方程，三个未知数 $(I_1, I_2, I_3)$，可解。

---

**推导4：等效电阻的递推方法 — $Y-\Delta$ 变换（进阶）**

对于不能用简单串并联化简的桥式电路，可用 $Y-\Delta$ 变换：

$R_a = \frac{R_{12}R_{13}}{R_{12}+R_{13}+R_{23}}$，$R_b = \frac{R_{12}R_{23}}{R_{12}+R_{13}+R_{23}}$，$R_c = \frac{R_{13}R_{23}}{R_{12}+R_{13}+R_{23}}$

反过来 $\Delta$ 转 $Y$：$R_{12} = \frac{R_aR_b+R_aR_c+R_bR_c}{R_c}$，同理其他。

这提供了另一种解复杂回路的方法，但基尔霍夫法则更通用。

---

# 11.8 / 3.4 RC 电路 — 五次推导 ★ 核心

## 核心公式：充电 $q(t)=Q_f(1-e^{-t/RC})$，放电 $q(t)=Q_0e^{-t/RC}$，$\tau=RC$

---

**推导1：RC充电 — 从微分方程到解析解（标准方法）**

串联 RC 电路，电池 $\mathcal{E}$，电阻 $R$，电容 $C$。

**回路方程：** $\mathcal{E} - IR - \frac{q}{C} = 0$

由 $I = dq/dt$：$\mathcal{E} - R\frac{dq}{dt} - \frac{q}{C} = 0$

**整理为标准一阶线性微分方程：**
$R\frac{dq}{dt} + \frac{q}{C} = \mathcal{E}$ $\Rightarrow$ $\frac{dq}{dt} = \frac{\mathcal{E}}{R} - \frac{q}{RC}$

**分离变量：** $\frac{dq}{\mathcal{E}C - q} = \frac{dt}{RC}$

积分：$\int_0^q \frac{dq'}{\mathcal{E}C - q'} = \int_0^t \frac{dt'}{RC}$

$-\ln(\mathcal{E}C - q) + \ln(\mathcal{E}C) = \frac{t}{RC}$

$\ln\frac{\mathcal{E}C}{\mathcal{E}C - q} = \frac{t}{RC}$ $\Rightarrow$ $\frac{\mathcal{E}C}{\mathcal{E}C - q} = e^{t/RC}$

$\mathcal{E}C - q = \mathcal{E}C e^{-t/RC}$ $\Rightarrow$ $q(t) = \mathcal{E}C(1 - e^{-t/RC})$

**对时间的导数（电流）：**
$I(t) = \frac{dq}{dt} = \frac{\mathcal{E}}{R}e^{-t/RC}$

---

**推导2：RC放电 — 从微分方程到解析解**

电容初始电荷 $Q_0$，**无电池**，回路方程（仅电阻+电容）：

$IR + \frac{q}{C} = 0$，其中 $I = dq/dt$（注意放电时电流方向与充电相反，此处 $I$ 为放电电流大小）

$R\frac{dq}{dt} + \frac{q}{C} = 0$ $\Rightarrow$ $\frac{dq}{dt} = -\frac{q}{RC}$

**分离变量：** $\frac{dq}{q} = -\frac{dt}{RC}$

积分：$\int_{Q_0}^q \frac{dq'}{q'} = -\int_0^t \frac{dt'}{RC}$

$\ln\frac{q}{Q_0} = -\frac{t}{RC}$ $\Rightarrow$ $q(t) = Q_0 e^{-t/RC}$

**电流：** $I(t) = -\frac{dq}{dt} = \frac{Q_0}{RC}e^{-t/RC} = \frac{V_0}{R}e^{-t/RC}$（负号代表方向与充电相反）

---

**推导3：时间常数 $\tau = RC$ 的物理意义**

**含义1：** 电容电压上升到终值的 $63.2\%$（或下降到初始值的 $36.8\%$）所需时间。

$V_C(\tau) = \mathcal{E}(1-e^{-1}) = \mathcal{E}(1-0.368) = 0.632\mathcal{E}$ ✓

**含义2：** 曲线在该点的切线斜率与时间轴交于 $\tau$。

$I(t) = \frac{\mathcal{E}}{R}e^{-t/RC}$，$I(0) = \mathcal{E}/R$
初始切线：$I(t) \approx \frac{\mathcal{E}}{R}(1 - t/RC)$，$I=0$ 时 $t=RC=\tau$

**含义3：** 经过 $5\tau$ 后，电容基本充/放电完毕（$e^{-5} \approx 0.007$，不到 $1\%$）。

---

**推导4：RC电路的通用解（通过积分因子法）**

一阶线性微分方程：$\frac{dq}{dt} + \frac{q}{RC} = \frac{\mathcal{E}}{R}$

积分因子 $\mu(t) = e^{\int dt/(RC)} = e^{t/RC}$

两边乘 $\mu$：$\frac{d}{dt}(qe^{t/RC}) = \frac{\mathcal{E}}{R}e^{t/RC}$

$qe^{t/RC} = \frac{\mathcal{E}}{R}\int e^{t/RC} dt = \mathcal{E}C e^{t/RC} + K$

$q(t) = \mathcal{E}C + Ke^{-t/RC}$

$q(0)=0$：$0 = \mathcal{E}C + K$ $\Rightarrow$ $K = -\mathcal{E}C$

$q(t) = \mathcal{E}C(1-e^{-t/RC})$ ✓

放电时 $\mathcal{E}=0$，$q(0)=Q_0$：$q(t) = Q_0 e^{-t/RC}$ ✓

---

**推导5：RC电路的能量分析**

**充电过程能量分配：**
电池提供的总能量：$W_{\text{电池}} = \int_0^\infty \mathcal{E}I(t)dt = \mathcal{E}\int_0^\infty \frac{\mathcal{E}}{R}e^{-t/RC}dt = \frac{\mathcal{E}^2}{R}\cdot RC = \mathcal{E}^2C$

电容最终储能：$U_C = \frac{1}{2}C\mathcal{E}^2$（恰好是总能量的一半！）

电阻消耗的能量：$W_R = \int_0^\infty I^2R\,dt = \int_0^\infty \frac{\mathcal{E}^2}{R}e^{-2t/RC}dt = \frac{\mathcal{E}^2}{R}\cdot\frac{RC}{2} = \frac{1}{2}C\mathcal{E}^2$

所以：$W_{\text{电池}} = U_C + W_R$ ✓ —— 一半储存在电容中，一半转化为电阻上的热量。

---

**推导6：RC电路的时间分析（数值计算）**

一个 RC 电路，$\tau=1\text{s}$：

| 时间 | 充电 $q/Q_f$ | 放电 $q/Q_0$ |
|:--|:--|:--|
| $0$ | $0$ | $1$ |
| $\tau$ | $0.632$ | $0.368$ |
| $2\tau$ | $0.865$ | $0.135$ |
| $3\tau$ | $0.950$ | $0.050$ |
| $5\tau$ | $0.993$ | $0.007$ |

**关键洞察：** RC 电路的"响应速度"由 $\tau=RC$ 唯一决定。大 $R$ 限制电流，大 $C$ 需要更多电荷——都需要更长时间。

---

## 附录：关键公式速查

| 公式 | 物理含义 | 适用条件 |
|:--|:--|:--|
| $I = dQ/dt$ | 电流定义 | 通用 |
| $I = nAev_d$ | 微观电流 | 金属导体 |
| $\vec{J} = nq\vec{v}_d = \sigma\vec{E}$ | 电流密度 | 通用 |
| $V=IR$ | 欧姆定律 | 欧姆器件 |
| $R = \rho L/A$ | 电阻公式 | 均匀截面导体 |
| $\rho = \rho_0[1+\alpha(T-T_0)]$ | 电阻率温度关系 | 金属（近似） |
| $P = IV = I^2R = V^2/R$ | 电功率 | 纯电阻电路 |
| $P_{\max} = \mathcal{E}^2/(4r)$ | 最大输出功率 | $R=r$ 时 |
| $R_{eq,\text{串联}} = \sum R_i$ | 串联等效电阻 | 电流相同 |
| $1/R_{eq,\text{并联}} = \sum 1/R_i$ | 并联等效电阻 | 电压相同 |
| $\sum I_{\text{in}} = \sum I_{\text{out}}$ | 基尔霍夫节点法则 | 稳态电路 |
| $\sum \Delta V = 0$ 绕回路 | 基尔霍夫回路法则 | 闭合回路 |
| $q(t) = \mathcal{E}C(1-e^{-t/RC})$ | RC充电 | 初始无电荷 |
| $q(t) = Q_0 e^{-t/RC}$ | RC放电 | 无电池 |
| $\tau = RC$ | 时间常数 | RC串联 |
| $I(t) = (\mathcal{E}/R)e^{-t/RC}$ | 充电电流 | 同上 |

---

## 常见概念陷阱

1. **电流方向：** 约定方向是正电荷运动方向，实际电子移动方向与此相反
2. **欧姆定律 $V=IR$ 的适用范围：** 仅对纯电阻欧姆器件成立，二极管、热敏电阻不适用
3. **串并联判定：** 若两元件间无分叉→串联；若两端直接连接→并联
4. **基尔霍夫符号：** 绕行方向与电流方向相同→$\Delta V=-IR$；从负极到正极穿过电池→$+\mathcal{E}$
5. **RC 电路初始/稳态分析：** 电容初始不充电时 $t=0$ 视为短路（$V_C=0$），稳态时视为开路（$I=0$）
6. **功率公式选择：** 串联电路中 $I$ 相同，用 $P=I^2R$；并联电路中 $V$ 相同，用 $P=V^2/R$
7. **时间常数 $\tau=RC$：** 大 $\tau$ 意味着充放电慢，小 $\tau$ 意味着充放电快

---

## 核心推理方法总结

| 问题类型 | 方法 | 关键步骤 |
|:--|:--|:--|
| 等效电阻 | 从最内层开始逐层化简 | 识别串并联关系 |
| 复杂电路分析 | 基尔霍夫法则 | 列方程 $\to$ 求解线性方程组 |
| RC 充放电 | 微分方程 $\to$ 分离变量/积分因子 | $\tau=RC$ 是核心参数 |
| 最大功率 | 求导 $dP/dR=0$ | $R=r$ 时输出最大 |
| 能量分配 | 积分 $\int_0^\infty I^2R\,dt$ | 一半在电容，一半在电阻 |

