# Chapter 11：导体、电容器与电介质（Conductors, Capacitors, and Dielectrics）
## 考纲综合整理：

### 【AP Physics C: E&M】Unit 2：Conductors, Capacitors, Dielectrics

| 编号 | 知识点 | 核心公式/概念 | 🟣 微积分关键 |
|:--:|:--|:--|:--|
| **2.1** | 静电学中的导体 | 内部 $\vec{E}=0$；电荷在表面；等势体 | — |
| **2.2** | 电容器 | $C=\frac{Q}{V}$；平行板 $C=\epsilon_0\frac{A}{d}$ | 🟣 利用高斯定律推导 $C$ |
| **2.3** | 电介质 | $\kappa=\frac{C}{C_0}$；极化；击穿场强 | — |

---
---

# AP Physics C: E&M Unit 2 — Conductors, Capacitors, Dielectrics

**完整推导参考文档 · 以推理为中心**

---

## 绪论：这一章在问什么？

Unit 1 讨论了真空中的静电场——电荷产生场，场对电荷施力。但实际中我们总是用**导体**来操控电荷，用**电介质**来增强电容。

本章的核心问题链：

1. **导体（2.1）：** 电荷如何在导体上分布？电场在导体内外有何特征？
2. **电容器（2.2）：** 如何设计一个器件来储存电荷？如何计算不同几何结构的电容？
3. **电介质（2.3）：** 插入非导体材料如何改变电容？极化机制是什么？材料的极限是什么？

这三个问题环环相扣——导体的静电平衡条件 $E=0 \Rightarrow V=\text{常数}$ 直接引出电容定义 $C=Q/V$，而电介质通过极化增强电容 $C=\kappa C_0$。

---

# 2.1 静电学中的导体 — 四次推导

## 核心公式/概念：

| 概念 | 公式/条件 | 物理含义 |
|:--|:--|:--|
| 内部电场 | $\vec{E}_{\text{内部}}=0$ | 自由电荷移动至平衡 |
| 表面电场 | $E_{\text{表面}}=\sigma/\epsilon_0$ | 高斯扁圆柱 |
| 等势体 | $V_{\text{导体}}=\text{常数}$ | $\int\vec{E}\cdot d\vec{l}=0$ |
| 电荷分布曲面 | 小曲率半径处电荷密度大 | 尖端放电原理 |

---

### 推导1：导体静电平衡条件的完整逻辑链

**出发点：** 导体中存在大量自由电荷（自由电子），可以在导体内自由移动。

**推理链：**

1. **导体内 $\vec{E}=0$**
   - 假如导体内某处 $\vec{E}\neq0$，则该处的自由电荷受力 $\vec{F}=q\vec{E}\neq0$
   - 电荷会沿电场方向运动，直到它们重新分布使得 $\vec{E}=0$
   - 平衡时 $\Rightarrow$ $\vec{E}_{\text{内部}}=0$

2. **导体是等势体**
   - 导体内任意两点 $A,B$：$V_B-V_A = -\int_A^B \vec{E}\cdot d\vec{l} = 0$
   - $\because$ 导体内处处 $\vec{E}=0$，路径积分恒为零
   - $\Rightarrow$ 导体上所有点电势相等

3. **净电荷仅分布在表面**
   - 在导体内取任意闭合高斯面，$\oint\vec{E}\cdot d\vec{A}=0$（$\because$ 面上 $\vec{E}=0$）
   - $\Rightarrow$ $Q_{\text{enc}}=0$，导体内任何区域净电荷为零
   - $\Rightarrow$ 所有净电荷必须分布在表面

4. **表面 $\vec{E}\perp$ 表面**
   - 若 $\vec{E}$ 有切向分量 $E_{\parallel}$，则表面电荷受力沿表面运动
   - 平衡时切向分量为零 $\Rightarrow$ $\vec{E}\parallel \hat{n}$（垂直于表面）

---

### 推导2：导体表面电场 $E=\sigma/\epsilon_0$

取扁圆柱高斯面：底面平行于导体表面，一个底面在**导体内部**（$E=0$），另一个在**表面外部**。圆柱很扁，侧面积可忽略。

$\oint\vec{E}\cdot d\vec{A} = E_{\text{外}}A = \frac{Q_{\text{enc}}}{\epsilon_0} = \frac{\sigma A}{\epsilon_0}$

$\Rightarrow$ $E_{\text{外}} = \frac{\sigma}{\epsilon_0}$

**对比无限大带电平面的 $E=\sigma/(2\epsilon_0)$：**
- 无限大带电平面：两侧都有电场线向外辐射，总通量 $2EA$
- 导体表面：内侧电场为零，电场线只从外侧发出，通量 $EA$

**这个区别的物理原因：** 导体内部的自由电荷"吸收"了指向内侧的电场线。如果有另一侧电场线需要"终结"，它们终结在导体内部而非表面。

---

### 推导3：导体空腔 — 静电屏蔽

**情形1：空腔内部无电荷**
- 取高斯面包围空腔（完全在导体内），$\Phi_E=0$ $\Rightarrow$ $Q_{\text{enc}}=0$
- 若空腔表面有不均匀电荷，会在导体内产生电场——但 $\vec{E}=0$ 要求表面电荷均匀分布
- $\Rightarrow$ 空腔表面净电荷为零，空腔内部电场为零

**情形2：空腔内部有电荷 $+q$**
- 取高斯面包围空腔（在导体内），$\Phi_E=0$
- $\Rightarrow$ $Q_{\text{enc}} = q + q_{\text{腔内壁}} = 0$ $\Rightarrow$ $q_{\text{腔内壁}} = -q$
- 由电荷守恒，导体外表面获得 $+q$（若导体原本不带电）
- 空腔内有电场（由 $+q$ 和 $-q$ 产生），但导体外部的观察者"看"不到空腔内的细节——外部场只由导体外表面总电荷决定

**静电屏蔽结论：**
- 空腔内部电荷 $\Rightarrow$ 导体外表面感应等量同号电荷，外部场不受腔内细节影响
- 外部电荷 $\Rightarrow$ 导体内部的空腔区电场为零（$\because$ 导体内 $E=0$）
- **屏蔽是双向的：** 内部不影响外部，外部不影响内部

---

### 推导4：尖端放电原理 — 曲率与电荷密度

**定性推理：**
- 导体是等势体，表面各处电势相等 $V=\text{常数}$
- 对孤立导体，$V=kQ_{\text{总}}/R_{\text{等效}}$（近似），但不同曲率处局域电势应相同
- 尖端（小曲率半径 $r$）处，局域电场 $E \propto V/r$，面电荷密度 $\sigma = \epsilon_0 E \propto 1/r$
- **$\Rightarrow$ 曲率半径越小处，面电荷密度越大，表面电场越强**

**定量推导（两个带电球连接）：**
两个半径 $R_1$、$R_2$ 的导体球用细导线连接，总电荷 $Q$ 在两球间分配。

平衡时两球电势相等：$V_1 = \frac{kQ_1}{R_1} = V_2 = \frac{kQ_2}{R_2}$ $\Rightarrow$ $\frac{Q_1}{R_1} = \frac{Q_2}{R_2}$

表面电场：$E_1 = \frac{kQ_1}{R_1^2} = \frac{kQ_2/R_2}{R_1} = \frac{V}{R_1}$，$E_2 = \frac{V}{R_2}$

$E_1/E_2 = R_2/R_1$ ——半径小的球表面电场更强。

**应用：** 避雷针利用尖端放电原理——尖端电场极强，使空气电离，引导闪电击中针而非建筑。

---

# 2.2 电容器 — 五次推导

## 核心公式：$C = Q/V$，平行板 $C = \epsilon_0 A/d$
## 储能：$U = \frac{1}{2}CV^2 = Q^2/(2C)$
## 能量密度：$u = \frac{1}{2}\epsilon_0 E^2$

---

### 推导1：平行板电容器 — 高斯定律推导

两平行导体板，面积 $A$，间距 $d$（$d \ll \sqrt{A}$，可忽略边缘效应），带电荷 $\pm Q$。

**步骤1（电场）：** 取高斯扁圆柱，一底面在导体内（$E=0$），一底面在两板间。
$\oint\vec{E}\cdot d\vec{A} = EA = \frac{\sigma A}{\epsilon_0} = \frac{Q}{\epsilon_0}$ $\Rightarrow$ $E = \frac{\sigma}{\epsilon_0} = \frac{Q}{\epsilon_0 A}$

**步骤2（电势差）：** 从负极板到正极板沿电场线积分。
$V = V_+ - V_- = \int_{-}^{+} \vec{E}\cdot d\vec{l} = \int_0^d E\,dz = Ed = \frac{Qd}{\epsilon_0 A}$

**步骤3（电容）：** $C = \frac{Q}{V} = \frac{\epsilon_0 A}{d}$

**注意：** 此处 $E = \sigma/\epsilon_0$ 而非 $\sigma/(2\epsilon_0)$，因为高斯面一底面在导体内 $E=0$。

---

### 推导2：圆柱形电容器 $C = \dfrac{2\pi\epsilon_0 L}{\ln(b/a)}$

由两个共轴圆柱导体构成，内柱半径 $a$，外筒内半径 $b$，长度 $L$（$L \gg b$），带电荷 $\pm Q$。

**步骤1（电场）：** 取共轴圆柱高斯面（半径 $r$，$a<r<b$，长度 $l$）。
$\oint\vec{E}\cdot d\vec{A} = E\cdot 2\pi r l = \frac{\lambda l}{\epsilon_0}$ $\Rightarrow$ $E = \frac{\lambda}{2\pi\epsilon_0 r}$

其中 $\lambda = Q/L$ 为线电荷密度。

**步骤2（电势差）：**
$V = V_a - V_b = \int_a^b \vec{E}\cdot d\vec{r} = \int_a^b \frac{\lambda}{2\pi\epsilon_0 r} dr = \frac{\lambda}{2\pi\epsilon_0}\ln\frac{b}{a}$

**步骤3（电容）：** $C = \frac{Q}{V} = \frac{\lambda L}{\frac{\lambda}{2\pi\epsilon_0}\ln(b/a)} = \frac{2\pi\epsilon_0 L}{\ln(b/a)}$

**检验：** $b \to a$ 时 $\ln(b/a)\to 0$，$C\to\infty$——两柱面非常接近时电容极大，但实际中会击穿。

---

### 推导3：球形电容器 $C = 4\pi\epsilon_0\dfrac{ab}{b-a}$

两个同心导体球壳，内球半径 $a$，外球内半径 $b$，带电荷 $\pm Q$。

**步骤1（电场）：** 取同心球面高斯面（半径 $r$，$a<r<b$）。
$\oint\vec{E}\cdot d\vec{A} = E\cdot 4\pi r^2 = \frac{Q}{\epsilon_0}$ $\Rightarrow$ $E = \frac{Q}{4\pi\epsilon_0 r^2}$

**步骤2（电势差）：**
$V = \int_a^b \frac{Q}{4\pi\epsilon_0 r^2} dr = \frac{Q}{4\pi\epsilon_0}\left(\frac{1}{a} - \frac{1}{b}\right) = \frac{Q}{4\pi\epsilon_0}\frac{b-a}{ab}$

**步骤3（电容）：** $C = \frac{Q}{V} = 4\pi\epsilon_0\frac{ab}{b-a}$

**特例：** $b\to\infty$（孤立导体球）：$C = 4\pi\epsilon_0 a$——这就是孤立导体球的电容公式。

---

### 推导4：电容器储能公式的三种推导路径

**路径A（充电过程积分）：**
充电时电荷从 $0$ 逐渐增加到 $Q$。在电荷为 $q$ 时电压 $v = q/C$。
将 $dq$ 从负极移到正极做功：$dW = v\,dq = \frac{q}{C}dq$
$W = \int_0^Q \frac{q}{C}dq = \frac{Q^2}{2C} = \frac{1}{2}CV^2$

**路径B（能量密度积分）：**
$U = \int u\,dV = \frac{\epsilon_0}{2}\int E^2 dV$
对平行板：$E = V/d$，体积 $Ad$：
$U = \frac{\epsilon_0}{2}\left(\frac{V}{d}\right)^2 Ad = \frac{1}{2}\frac{\epsilon_0 A}{d}V^2 = \frac{1}{2}CV^2$ ✓

**路径C（从电场力做功）：**
假设两板从 $d_1$ 拉到 $d_2$（$Q$ 不变），电场力做功 $=$ 储能减少。
$F = \frac{Q^2}{2\epsilon_0 A}$（吸引力，见下节），$W = \int_{d_1}^{d_2} F\,dd = \frac{Q^2}{2\epsilon_0 A}(d_2-d_1)$
$U(d_2) - U(d_1) = -W = -\frac{Q^2}{2\epsilon_0 A}(d_2-d_1)$
所以 $U(d) = \frac{Q^2d}{2\epsilon_0 A} + \text{常数} = \frac{Q^2}{2C}$（取常数=0）✓

---

### 推导5：虚功原理求平行板间吸引力

**情形A：$Q$ 不变（断开电池）**
$U = \frac{Q^2}{2C} = \frac{Q^2 d}{2\epsilon_0 A}$
$F = -\frac{\partial U}{\partial d} = -\frac{Q^2}{2\epsilon_0 A} = -\frac{CV^2}{2d}$
负号表示吸引力（$d$ 减小时能量降低）

**情形B：$V$ 不变（电池保持连接）**
需计入电池做功。系统能量变化 $dU = VdQ + Fdd$（此处约定正 $F$ 为拉力方向）。
$U = \frac{1}{2}CV^2 = \frac{1}{2}\frac{\epsilon_0 A}{d}V^2$
$dU = -\frac{1}{2}\frac{\epsilon_0 A}{d^2}V^2 dd$
$dQ = VdC = V\cdot\left(-\frac{\epsilon_0 A}{d^2}dd\right)$
电池做功 $VdQ = -\frac{\epsilon_0 A V^2}{d^2}dd$
由能量守恒：$-\frac{1}{2}\frac{\epsilon_0 A V^2}{d^2}dd = -\frac{\epsilon_0 A V^2}{d^2}dd + Fdd$
$F = \frac{\epsilon_0 A V^2}{2d^2} = \frac{CV^2}{2d}$（与情形A相同，都是吸引力）

**数值意义：** 一平行板电容器 $A=100\text{cm}^2$，$d=1\text{mm}$，$V=100\text{V}$。
$F = \frac{\epsilon_0 A V^2}{2d^2} = \frac{(8.85\times10^{-12})(0.01)(10^4)}{2(10^{-6})} = 4.43\times10^{-4}\text{N}$
这个力很小——电容器的能量密度决定了吸引力不大。

---

### 推导6：电容器串并联公式

**并联：** 电压相同 $V$，总电荷 $Q = Q_1+Q_2 = C_1V+C_2V = (C_1+C_2)V$
$\Rightarrow$ $C_{\text{eq}} = C_1 + C_2$（电容相加，类似电阻串联）

**串联：** 电荷相同 $Q$，总电压 $V = V_1+V_2 = Q/C_1+Q/C_2 = Q(1/C_1+1/C_2)$
$\Rightarrow$ $1/C_{\text{eq}} = 1/C_1 + 1/C_2$（倒数相加，类似电阻并联）

**物理直观：** 并联增加面积（$A$ 变大），串联增加间距（$d$ 变大），所以并联 $\uparrow C$，串联 $\downarrow C$。

---

# 2.3 电介质 — 四次推导

## 核心公式：$\kappa = C/C_0$，$C = \kappa\epsilon_0 A/d$，$E = E_0/\kappa$

---

### 推导1：电介质极化的微观机制

**极化过程：** 电介质中分子在外电场 $E_0$ 作用下：
- 非极性分子：电子云相对原子核位移，产生感应偶极矩 $\vec{p} = \alpha\vec{E}_{\text{loc}}$
- 极性分子：固有偶极矩转向外电场方向

**极化强度 $\vec{P}$：** 单位体积内的电偶极矩总和。
$\vec{P} = \chi_e\epsilon_0\vec{E}$，其中 $\chi_e$ 为电极化率（材料属性）

**束缚电荷：** 极化导致电介质表面出现束缚电荷。
- 面密度：$\sigma_b = \vec{P}\cdot\hat{n}$
- 体密度：$\rho_b = -\nabla\cdot\vec{P}$（若 $\vec{P}$ 不均匀）

---

### 推导2：电介质增强电容 $C = \kappa C_0$

**无电介质时：** 平行板电场 $E_0 = \sigma/\epsilon_0$，电压 $V_0 = E_0d = \sigma d/\epsilon_0$
**有电介质时：** 自由电荷 $\sigma_f$ 产生场 $E_f = \sigma_f/\epsilon_0$，束缚电荷 $-\sigma_b$ 产生相反场 $E_b = -\sigma_b/\epsilon_0$
净电场：$E = E_f + E_b = \frac{\sigma_f}{\epsilon_0} - \frac{\sigma_b}{\epsilon_0}$

由 $\sigma_b = P = \chi_e\epsilon_0 E$（各向同性线性介质）：
$E = \frac{\sigma_f}{\epsilon_0} - \chi_e E$ $\Rightarrow$ $E(1+\chi_e) = \frac{\sigma_f}{\epsilon_0}$
$E = \frac{\sigma_f}{\epsilon_0(1+\chi_e)} = \frac{\sigma_f}{\kappa\epsilon_0}$，其中 $\kappa = 1+\chi_e$

电压：$V = Ed = \frac{\sigma_f d}{\kappa\epsilon_0} = \frac{Qd}{\kappa\epsilon_0 A}$
电容：$C = \frac{Q}{V} = \frac{\kappa\epsilon_0 A}{d} = \kappa C_0$ ✓

**物理图像：** 电介质极化产生的束缚电荷"屏蔽"了部分自由电荷的电场，使板间电场减弱为原来的 $1/\kappa$。因此相同电荷下电压降低，电容增大。

---

### 推导3：电位移 $\vec{D}$ 与高斯定律的推广

定义电位移：$\vec{D} = \epsilon_0\vec{E} + \vec{P}$

对线性介质：$\vec{P} = \chi_e\epsilon_0\vec{E}$，$\vec{D} = \epsilon_0\vec{E} + \chi_e\epsilon_0\vec{E} = \epsilon_0(1+\chi_e)\vec{E} = \epsilon_0\kappa\vec{E}$

**含电介质的高斯定律：**
$\oint\vec{D}\cdot d\vec{A} = Q_{f,\text{enc}}$
这比原始高斯定律 $\oint\epsilon_0\vec{E}\cdot d\vec{A} = Q_{\text{总,enc}}$ 更有用——因为它不包含束缚电荷，只涉及自由电荷。

**推导：** 原始高斯定律 $\oint\epsilon_0\vec{E}\cdot d\vec{A} = Q_{f,\text{enc}} + Q_{b,\text{enc}}$
其中 $Q_{b,\text{enc}} = -\oint\vec{P}\cdot d\vec{A}$
$\oint\epsilon_0\vec{E}\cdot d\vec{A} = Q_{f,\text{enc}} - \oint\vec{P}\cdot d\vec{A}$
$\oint(\epsilon_0\vec{E} + \vec{P})\cdot d\vec{A} = Q_{f,\text{enc}}$ $\Rightarrow$ $\oint\vec{D}\cdot d\vec{A} = Q_{f,\text{enc}}$ ✓

---

### 推导4：电介质中的电能

**电容储能：** $U = \frac{1}{2}CV^2 = \frac{1}{2}\kappa C_0 V^2$
- $V$ 不变（电池连接）：$U = \kappa U_0$（能量增加，电池提供）
- $Q$ 不变（断开电池）：$U = Q^2/(2\kappa C_0) = U_0/\kappa$（能量减少，被极化吸收）

**电场能量密度（含电介质）：**
$u = \frac{1}{2}\vec{E}\cdot\vec{D} = \frac{1}{2}\kappa\epsilon_0 E^2$

**推导：** 电容器体积 $Ad$，能量密度 $u = \frac{U}{Ad} = \frac{\frac{1}{2}CV^2}{Ad} = \frac{\frac{1}{2}\kappa\epsilon_0 A/d\cdot (Ed)^2}{Ad} = \frac{1}{2}\kappa\epsilon_0 E^2$ ✓

**物理意义：** 电介质中的能量密度是真空中的 $\kappa$ 倍——因为极化过程吸纳了额外能量。

---

### 推导5：介电击穿与最大储能

**击穿场强 $E_{\text{bd}}$：** 电场超过某阈值时，电介质中的电子被"扯"出原子，材料开始导电。

常见介质击穿场强：
- 空气：$3\times10^6\ \text{V/m}$
- 云母：$10^7\ \text{V/m}$ 量级
- 陶瓷：$10^7-10^8\ \text{V/m}$

**最大储能：** 给定电容 $C = \kappa\epsilon_0 A/d$，最大电压 $V_{\max} = E_{\text{bd}}d$
$U_{\max} = \frac{1}{2}C V_{\max}^2 = \frac{1}{2}\kappa\epsilon_0 A d E_{\text{bd}}^2 = \frac{1}{2}\kappa\epsilon_0 (\text{体积}) E_{\text{bd}}^2$

所以提高储能密度的途径：高 $\kappa$（材料选择）+ 高 $E_{\text{bd}}$（抗击穿）+ 大体积。

**注意高 $\kappa$ 与高 $E_{\text{bd}}$ 通常矛盾：** 高 $\kappa$ 材料往往击穿场强较低。

---

## 附录：关键公式速查

| 公式 | 物理含义 | 适用条件 |
|:--|:--|:--|
| $\vec{E}_{\text{内部}}=0$ | 导体静电平衡 | 所有导体 |
| $E_{\text{表面}}=\sigma/\epsilon_0$ | 表面附近电场 | 导体外法线方向 |
| $C=Q/V$ | 电容定义 | 任何双导体系统 |
| $C=\epsilon_0 A/d$ | 平行板电容 | $d\ll\sqrt{A}$ |
| $C=2\pi\epsilon_0 L/\ln(b/a)$ | 圆柱电容 | $L\gg b$ |
| $C=4\pi\epsilon_0 ab/(b-a)$ | 球形电容 | 同心球壳 |
| $U=\frac{1}{2}CV^2=Q^2/(2C)$ | 电容储能 | 任何电容器 |
| $u=\frac{1}{2}\epsilon_0 E^2$ | 电场能量密度 | 真空 |
| $\kappa=C/C_0$ | 介电常数 | 线性介质 |
| $C=\kappa\epsilon_0 A/d$ | 含介质平行板 | 各向同性线性介质 |
| $\vec{D}=\epsilon_0\vec{E}+\vec{P}=\kappa\epsilon_0\vec{E}$ | 电位移定义 | 线性介质 |
| $\oint\vec{D}\cdot d\vec{A}=Q_{f,\text{enc}}$ | 推广高斯定律 | 含介质时使用 |
| $u=\frac{1}{2}\kappa\epsilon_0 E^2$ | 介质中能量密度 | 线性介质 |

---

## 常见概念陷阱

1. **$E=\sigma/\epsilon_0$ vs $E=\sigma/(2\epsilon_0)$：** 导体表面用前者（一侧面无场），无限大带电平面用后者（两侧都有场）
2. **电容器断开 $\Rightarrow$ $Q$ 不变：** 插入介质时 $C\uparrow$，$V\downarrow$，$U\downarrow$
3. **电容器连接 $\Rightarrow$ $V$ 不变：** 插入介质时 $C\uparrow$，$Q\uparrow$，$U\uparrow$
4. **串并联判定：** 并联增加面积（$C$ 变大），串联增加距离（$C$ 变小）
5. **电位移 $\vec{D}$ 的边界条件：** 在两种介质界面上，$D_{\perp}$ 连续（若无自由面电荷），$E_{\parallel}$ 连续
6. **虚功原理：** 计算静电力时，$Q$ 不变用 $F=-\partial U/\partial d$，$V$ 不变需考虑电池做功

---

## 核心推理方法总结

| 问题类型 | 方法 | 关键步骤 |
|:--|:--|:--|
| 求电容 | 1. 设电荷 $\pm Q$ | 2. 高斯定律求 $\vec{E}$ | 3. 积分求 $V$ | 4. $C=Q/V$ |
| 求储能 | 1. 求 $C$ | 2. 用 $U=\frac12CV^2$ 或 $U=\frac12\int D\cdot E\,dV$ |
| 求电场力 | 1. 虚功原理 $F=-\partial U/\partial d$ | 2. 注意 $Q$ 不变 vs $V$ 不变 |
| 含介质 | 1. 用 $\oint\vec{D}\cdot d\vec{A}=Q_f$ 先求 $\vec{D}$ | 2. 由 $\vec{E}=\vec{D}/(\kappa\epsilon_0)$ 得 $\vec{E}$ |
| 导体空腔 | 1. 导体内 $E=0$ $\Rightarrow$ 高斯面内 $Q_{\text{enc}}=0$ | 2. 确定感应电荷分布 |
