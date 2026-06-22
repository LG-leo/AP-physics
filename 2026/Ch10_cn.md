# Chapter 10：电力、电场与电势（Electric Force, Field, and Potential）
## 考纲综合整理：

### 【AP Physics 2】Unit 10：Electric Force, Field, and Potential

| 编号 | 知识点 | 核心公式/概念 | 技能 |
|:--:|:--|:--|:--:|
| **10.1** | 电荷与电力 | 电荷守恒；同斥异吸；库仑定律 $F=k\frac{|q_1q_2|}{r^2}$ | 2.A, 2.B |
| **10.2** | 电荷守恒与充电 | 摩擦起电、传导、感应；$q=ne$ | 3.B, 3.C |
| **10.3** | 电场 | $\vec{E}=\frac{\vec{F}}{q}$；$\vec{E}=k\frac{q}{r^2}\hat{r}$（点电荷） | 1.A, 2.A |
| **10.4** | 电势能 | $U_E=k\frac{q_1q_2}{r}$；$W_E=-\Delta U_E$ | 2.A, 2.C |
| **10.5** | 电势 | $V=\frac{U}{q}$；$V=k\frac{q}{r}$（点电荷）；等势面 $\perp$ 电场线 | 2.A, 2.B |
| **10.6** | 电容器 | $C=\frac{Q}{V}$；$C=\epsilon_0\frac{A}{d}$（平行板） | 2.A, 2.B |
| **10.7** | 电能守恒 | 电场力做功 + 电势能变化 + 动能变化守恒 | 2.C, 3.B |

### 【AP Physics C: E&M】Unit 1：Electrostatics（🟣 微积分深化）

| 编号 | 知识点 | 核心公式/概念 | 🟣 微积分关键 |
|:--:|:--|:--|:--|
| **1.1** | 电荷与库仑定律 | $F=k\frac{|q_1q_2|}{r^2}$；电荷量子化 | — |
| **1.2** | 电场与电势 | $\vec{E}=\frac{\vec{F}}{q}$；$V=-\int\vec{E}\cdot d\vec{l}$ | 🟣 $V$ 通过路径积分定义 |
| **1.3** | 点电荷和均匀场的电势 | $V=k\frac{q}{r}$；$\vec{E}=-\nabla V$ | 🟣 梯度关系 |
| **🔑 1.4** | **高斯定律（独家）** | $\Phi_E=\oint\vec{E}\cdot d\vec{A}=\frac{Q_{enc}}{\epsilon_0}$ | 🟣 **独家**：面积分；对称性分析（球/柱/平面） |
| **1.5** | 连续电荷分布 | $d\vec{E}=k\frac{dq}{r^2}\hat{r}$ | 🟣 $dq=\lambda dx$、$\sigma dA$、$\rho dV$ 积分 |


---
---

# 第10章 电力·电场·电势 — 完整推导参考文档

**AP Physics 2 Unit 10 + AP Physics C: E&M Unit 1 · 以推导为中心的知识体系**

---

## 绪论：静电学的逻辑链条

静电学整个体系可以从一个实验定律和两个基本原理出发：

**出发点：** 库仑定律 $F \propto q_1q_2/r^2$（实验事实）
**原理1：** 叠加原理（线性性）
**原理2：** 电荷守恒（封闭系统总电荷不变）

逻辑链条：
1. 库仑定律 $\Rightarrow$ 电场定义 $\vec{E}=\vec{F}/q$
2. 电场 $\Rightarrow$ 电势定义 $\Delta V=-\int\vec{E}\cdot d\vec{l}$
3. 电场 $\Rightarrow$ 高斯定律 $\oint\vec{E}\cdot d\vec{A}=Q_{\text{enc}}/\epsilon_0$
4. 高斯定律 $\Rightarrow$ 导体静电平衡条件
5. 电势 $\Rightarrow$ 电容 $C=Q/V$
6. 所有上述 $\Rightarrow$ 能量关系 $U=\frac{1}{2}\epsilon_0\int E^2 dV$

本文档围绕这个逻辑链条展开，对**每个核心公式提供3-4种不同视角的推导**。

---

# Part I：AP Physics 2 — 电场与电势的代数框架

---

## 10.1 库仑定律 — 三种推导视角

### 公式：$F = k|q_1q_2|/r^2$，$k=1/(4\pi\epsilon_0)=8.99\times10^9\ \text{N·m}^2/\text{C}^2$

---

**推导视角A：历史实验 — 库仑扭秤**

扭丝扭转角 $\theta$ 产生的恢复力矩 $\tau = \kappa\theta$（$\kappa$ 为扭丝常数）。两个带电小球相距 $r$，电力 $F = kq_1q_2/r^2$ 产生的力矩 $\tau_E = F\cdot L$（$L$ 为摆臂长）。

平衡时 $\kappa\theta = k\frac{q_1q_2}{r^2}L$。

**实验1：** 固定电荷量，改变距离 $r$，测量 $\theta$。得 $\theta \propto 1/r^2$。$\Rightarrow$ 平方反比。

**实验2：** 固定距离，用"平分电荷法"改变电荷量（将球与相同未带电球接触，电量减半），测量 $\theta$。得 $\theta \propto q_1q_2$。$\Rightarrow$ 正比于电荷积。

**精度：** 平方反比的指数 $2$ 的实验精度可达 $2.00\pm0.0001$，极其精确。

---

**推导视角B：场的中介 — 从电场反推**

先定义电场 $\vec{E}$，再通过 $\vec{F}=q\vec{E}$ 得到力。点电荷 $Q$ 在空间中产生电场 $\vec{E} = kQ\hat{r}/r^2$（这本身可从高斯定律得到）。将试验电荷 $q$ 放入该电场中，受力 $\vec{F} = q\vec{E} = kqQ\hat{r}/r^2$。这就是库仑定律的矢量形式。两种写法等价——库仑定律 $\Leftrightarrow$ 电场定义+点电荷电场公式。

---

**推导视角C：量纲分析 — 为什么是平方反比？**

在三维空间中，电力线从点电荷均匀向外辐射。穿过任意半径球面的"电力线总数"守恒（即通量守恒）。球面积 $= 4\pi r^2 \propto r^2$，所以单位面积上的力线密度 $\propto 1/r^2$。力 $\propto$ 力线密度 $\propto 1/r^2$。

$\Rightarrow$ 平方反比是**三维空间+通量守恒的必然结果**。如果在二维空间，力 $\propto 1/r$；在四维空间，力 $\propto 1/r^3$。

---

### 叠加原理的推导

多点电荷系统：$\vec{F}_{\text{net}} = kq_0\sum_{i=1}^N\frac{q_i}{r_i^2}\hat{r}_i$

操作流程：
1. 对每个 $q_i$：计算 $F_i = k|q_0q_i|/r_i^2$，方向由"同斥异吸"判断
2. 分解：$F_{ix}=F_i\cos\theta_i$，$F_{iy}=F_i\sin\theta_i$
3. 求和：$F_{\text{net},x}=\sum F_{ix}$，$F_{\text{net},y}=\sum F_{iy}$
4. 合成：$F_{\text{net}}=\sqrt{F_x^2+F_y^2}$，方向 $\phi=\tan^{-1}(F_y/F_x)$

**核心洞察：** 库仑力与万有引力数学形式相同（$F\propto 1/r^2$），但电力比引力强约 $10^{36}$ 倍。引力只有吸引，电力可吸引可排斥。电力可被屏蔽（导体），引力不能。

**常见概念错误：** $F = k|q_1q_2|/r^2$ 只给出大小。方向必须通过"同号相斥、异号相吸"独立判断，不要依赖代入正负号。

---

**关于电荷量子化** $q=ne$（$n\in\mathbb{Z}$，$e=1.602\times10^{-19}\text{C}$）：电荷不是连续量，而是基本电荷 $e$ 的整数倍。所有观测到的电荷量都满足这一规律，从未被违反。

---

## 10.2 电场 — 三种推导视角

### 公式：$\vec{E}=\vec{F}/q_{\text{test}}$，点电荷 $\vec{E}=kq\hat{r}/r^2$

---

**推导视角A：定义性 — 场作为力的中介**

为什么需要引入电场？两个电荷之间的作用不是"超距作用"，而是：
电荷 $Q$ $\rightarrow$ 改变周围空间 $\rightarrow$ 产生电场 $\vec{E}$
另一电荷 $q$ 进入这个空间 $\rightarrow$ 感受到电场 $\rightarrow$ 受力 $\vec{F}=q\vec{E}$

所以 $\vec{E} \equiv \dfrac{\vec{F}}{q_{\text{test}}}$ 是"单位试验电荷所受的力"，是空间自身的属性，与是否存在试验电荷无关。试验电荷 $q_{\text{test}}$ 被假设为足够小，不干扰源电荷分布。

---

**推导视角B：从库仑定律导出点电荷电场**

将库仑定律写成 $\vec{F} = \left(k\frac{Q}{r^2}\hat{r}\right) \cdot q$。括号内的量只依赖于源电荷 $Q$ 和位置 $r$，与试验电荷 $q$ 无关。这恰好就是电场：
$\vec{E} = \frac{\vec{F}}{q} = k\frac{Q}{r^2}\hat{r}$。因此点电荷电场与距离平方成反比，方向沿径向（正电荷向外，负电荷向内）。

---

**推导视角C：叠加原理**

电场也满足叠加原理（因为力满足叠加原理）：
$\vec{E}_{\text{net}} = \frac{\vec{F}_{\text{net}}}{q} = \frac{1}{q}\sum_i \vec{F}_i = \sum_i \frac{\vec{F}_i}{q} = \sum_i \vec{E}_i$
所以 $\vec{E}_{\text{net}} = \sum_i k\frac{q_i}{r_i^2}\hat{r}_i$。电场是矢量，叠加时必须分解为分量分别求和再合成。

---

### 电场线的物理意义

1. **从正电荷出发，终止于负电荷。** 正电荷处 $E$ 向外，负电荷处 $E$ 向内。
2. **不相交。** 每点只有一个 $\vec{E}$ 方向。
3. **电场线 $\perp$ 等势面。** 等势面上 $\Delta V=0$，$-\int\vec{E}\cdot d\vec{l}=0$ 对等势面上任意 $d\vec{l}$ 成立，所以 $\vec{E}\perp d\vec{l}$。
4. **电场线密度 $\propto$ 场强。** 由高斯定律，通量 $\propto$ 电荷量 $\propto$ 线根数。

---

**电场线密度与场强的关系推导：**
取一小面元 $dA_\perp$ 垂直于电场线。穿过面元的电通量 $d\Phi = E\,dA_\perp$。若定义电场线密度 $\rho_{\text{线}}=dN/dA_\perp$，且每根线携带固定通量 $d\Phi_0$，则 $d\Phi = \rho_{\text{线}}d\Phi_0\,dA_\perp$。所以 $E \propto \rho_{\text{线}}$。

---

## 10.3 电势与电势能 — 三种推导视角

### 公式：$U_E = k\frac{q_1q_2}{r}$，$V = k\frac{q}{r}$，$\Delta V = -\int\vec{E}\cdot d\vec{l}$

---

**推导视角A：从功的定义推导电势能**

将 $q_2$ 从无穷远处移到距 $q_1$ 为 $r$ 的位置，外力克服电场力做功。

电场力 $\vec{F}_E = k\frac{q_1q_2}{r'^2}\hat{r}'$（假设 $q_1q_2>0$ 排斥）
外力 $\vec{F}_{\text{ext}} = -\vec{F}_E$

$W_{\text{ext}} = \int_\infty^r \vec{F}_{\text{ext}}\cdot d\vec{l} = -\int_\infty^r \vec{F}_E\cdot d\vec{l}$
$= -\int_\infty^r k\frac{q_1q_2}{r'^2}dr' = -kq_1q_2\left[-\frac{1}{r'}\right]_\infty^r = k\frac{q_1q_2}{r}$

**电势能定义为储存的能量：** $U_E = W_{\text{ext}} = k\frac{q_1q_2}{r}$

注意这是**代数量**：$q_1q_2>0$（排斥）时 $U_E>0$，$q_1q_2<0$（吸引）时 $U_E<0$。负电势能意味着系统有"束缚能"——需要做功才能将两者分开。

---

**推导视角B：电场力是保守力（路径无关证明）**

对任意路径 $C$ 从 $A$ 到 $B$：
$W_E = \int_A^B \vec{F}_E\cdot d\vec{l} = q\int_A^B \vec{E}\cdot d\vec{l}$

对点电荷 $\vec{E}=k\frac{q}{r^2}\hat{r}$，在球坐标中：
$d\vec{l} = dr\,\hat{r} + r\,d\theta\,\hat{\theta} + r\sin\theta\,d\phi\,\hat{\phi}$
$\vec{E}\cdot d\vec{l} = k\frac{q}{r^2}dr$（只有径向分量贡献）

$\int_A^B \vec{E}\cdot d\vec{l} = \int_{r_A}^{r_B} k\frac{q}{r^2}dr = -kq\left(\frac{1}{r_B}-\frac{1}{r_A}\right)$

结果只取决于 $r_A$ 和 $r_B$（端点），**与路径形状无关**！$\Rightarrow$ 电场力是保守力，可以定义势能。

---

**推导视角C：从电场积分定义电势**

电势差：$\Delta V_{AB} = V_B-V_A = -\int_A^B \vec{E}\cdot d\vec{l}$

对点电荷，取径向路径从 $r_A$ 到 $r_B$：
$V_B-V_A = -\int_{r_A}^{r_B} k\frac{q}{r^2}dr = kq\left(\frac{1}{r_B}-\frac{1}{r_A}\right)$

取参考点 $r_A\to\infty$，令 $V(\infty)=0$：$V(r) = \frac{kq}{r}$

**电势叠加原理（标量！）：** $V_{\text{net}} = \sum_i V_i = \sum_i k\frac{q_i}{r_i}$

这是整个章节最重要的操作简化——**电势是标量，直接代数相加，不需要分解分量。**

---

### 电场与电势的梯度关系

$\vec{E} = -\nabla V$（一维：$E_x = -dV/dx$）

**一维推导：** $V(x+dx)-V(x) = -\int_x^{x+dx} E_x dx' \approx -E_x dx$ $\Rightarrow$ $E_x = -\frac{dV}{dx}$

**三维：** $\vec{E} = -\left(\frac{\partial V}{\partial x}\hat{x}+\frac{\partial V}{\partial y}\hat{y}+\frac{\partial V}{\partial z}\hat{z}\right)$

**物理含义：** 电场指向电势**下降最快**的方向，大小等于该方向上的**变化率**。

---

### 等势面的意义

等势面上各点电势相等。**电场线垂直于等势面**，且指向电势降低的方向。

推导：在等势面上 $\Delta V=0$，$-\int\vec{E}\cdot d\vec{l}=0$ 对任意 $d\vec{l}$ 在等势面上成立，所以 $\vec{E}\perp d\vec{l}$，即 $\vec{E}\perp$ 等势面。

**导体是等势体**，导体表面是等势面，电场线垂直于导体表面。

---

## 10.4 电容器 — 三种推导视角

### 公式：$C=Q/V$，平行板 $C=\epsilon_0 A/d$，$C=\kappa\epsilon_0 A/d$

---

**推导视角A：从高斯定律推导平行板电容公式**

平行板电容器，每板面积 $A$，间距 $d$，带电荷 $\pm Q$。面电荷密度 $\sigma = Q/A$。

取高斯面：扁圆柱，一底面在正板**内部**（导体内 $E=0$），另一底面在两板之间的空间。

$\oint\vec{E}\cdot d\vec{A} = EA = \frac{Q_{\text{enc}}}{\epsilon_0} = \frac{\sigma A}{\epsilon_0}$ $\Rightarrow$ $E = \frac{\sigma}{\epsilon_0} = \frac{Q}{\epsilon_0 A}$

电势差：$V = Ed = \frac{Qd}{\epsilon_0 A}$ $\Rightarrow$ 电容：$C = \frac{Q}{V} = \frac{\epsilon_0 A}{d}$

注意此处 $E=\sigma/\epsilon_0$ 而非 $\sigma/(2\epsilon_0)$——因为导体内 $E=0$，高斯面另一底面在导体内无通量贡献。这与无限大带电平面（两侧都有场）不同。

---

**推导视角B：从能量角度推导储能公式**

充电过程：将电荷微元 $dq$ 从负极板移到正极板，此时板间电压为 $v = q/C$。
做功 $dW = v\,dq = \frac{q}{C}dq$
总功：$W = \int_0^Q \frac{q}{C}dq = \frac{1}{C}\left[\frac{q^2}{2}\right]_0^Q = \frac{Q^2}{2C}$
代入 $Q = CV$：$U = \frac{1}{2}CV^2 = \frac{Q^2}{2C}$

**能量存哪里？** 电场中！能量密度 $u_E = \frac{1}{2}\epsilon_0 E^2$

验证：$U = u_E \cdot \text{体积} = \frac{1}{2}\epsilon_0 E^2 \cdot Ad = \frac{1}{2}\epsilon_0\frac{V^2}{d^2}Ad = \frac{1}{2}\frac{\epsilon_0 A}{d}V^2 = \frac{1}{2}CV^2$ ✓

---

**推导视角C：电介质的微观极化机制**

电介质放入电场 $E_0$ 中，分子极化产生束缚电荷 $\sigma_b$。极化面密度 $\sigma_b = \chi_e\epsilon_0 E$（$\chi_e$ 为电极化率）。

内部净电场：$E = \frac{\sigma_{\text{free}}}{\epsilon_0} - \frac{\sigma_b}{\epsilon_0} = \frac{\sigma_{\text{free}}}{\epsilon_0} - \chi_e E$

$E(1+\chi_e) = \frac{\sigma_{\text{free}}}{\epsilon_0}$ $\Rightarrow$ $E = \frac{\sigma_{\text{free}}}{\kappa\epsilon_0}$

其中介电常数 $\kappa = 1+\chi_e \geq 1$。$\kappa$ 总是大于1，因为介质减弱了内部电场。

$V = Ed = \frac{\sigma_{\text{free}} d}{\kappa\epsilon_0} = \frac{Qd}{\kappa\epsilon_0 A}$ $\Rightarrow$ $C = \frac{Q}{V} = \frac{\kappa\epsilon_0 A}{d}$

---

### 两类核心操作的推导对比

**情形1：电池保持连接（V不变）**
插介质 $\Rightarrow$ $C\uparrow=\kappa C_0$ $\Rightarrow$ $Q=CV\uparrow$ $\Rightarrow$ $U=\frac{1}{2}CV^2\uparrow$
能量增加由电池提供。介质被"拉"入板间（电场力做正功）。

**情形2：断开电池（Q不变）**
插介质 $\Rightarrow$ $C\uparrow=\kappa C_0$ $\Rightarrow$ $V=Q/C\downarrow$ $\Rightarrow$ $U=Q^2/(2C)\downarrow$
能量减少，被介质极化过程吸收。电压降为原来的 $1/\kappa$。

**物理直观：** 情形1中电池持续提供电荷维持电压；情形2中电荷固定，介质极化削弱电场导致电压下降。

---

# Part II：AP Physics C — 微积分深化

> 以下每个核心公式提供**4次以上不同视角的推导**。

---

## 1.1 高斯定律 — 四次推导

### 积分形式：$\displaystyle\oint_S \vec{E}\cdot d\vec{A} = \frac{Q_{\text{enc}}}{\epsilon_0}$

### 微分形式：$\nabla\cdot\vec{E} = \dfrac{\rho}{\epsilon_0}$

---

**推导1：从库仑定律到高斯定律（球对称 $\Rightarrow$ 一般形式）**

点电荷 $q$ 在原点。取半径为 $r$ 的球面为高斯面。
$\vec{E} = \frac{q}{4\pi\epsilon_0 r^2}\hat{r}$（库仑定律）
$d\vec{A} = r^2\sin\theta\,d\theta\,d\phi\,\hat{r}$（球面面积元，外法线方向）

$\vec{E}\cdot d\vec{A} = \frac{q}{4\pi\epsilon_0 r^2}\cdot r^2\sin\theta\,d\theta\,d\phi = \frac{q}{4\pi\epsilon_0}\sin\theta\,d\theta\,d\phi$

$\Phi_E = \oint\vec{E}\cdot d\vec{A} = \frac{q}{4\pi\epsilon_0}\int_0^{2\pi}\int_0^\pi \sin\theta\,d\theta\,d\phi = \frac{q}{4\pi\epsilon_0}\cdot 4\pi = \frac{q}{\epsilon_0}$

**关键发现：** 结果与 $r$ 无关！平方反比律保证通量与半径无关。

对**任意形状**闭合曲面：$\because$ 电通量只取决于立体角，与面形状无关。对包围点电荷的任意曲面，立体角积分总为 $4\pi$，通量恒为 $q/\epsilon_0$。

对多个点电荷：$\Phi_E = \oint\sum\vec{E}_i\cdot d\vec{A} = \sum\oint\vec{E}_i\cdot d\vec{A} = \sum q_i/\epsilon_0 = Q_{\text{enc}}/\epsilon_0$ ✓

---

**推导2：球对称分布的统一分析**

对球对称分布，$\vec{E}$ 沿径向且大小只与 $r$ 有关。取同心球面高斯面：
$\oint\vec{E}\cdot d\vec{A} = E(r)\cdot 4\pi r^2 = \frac{Q_{\text{enc}}(r)}{\epsilon_0}$ $\Rightarrow$ $E(r) = \frac{Q_{\text{enc}}(r)}{4\pi\epsilon_0 r^2}$

**这个形式对任何球对称分布都成立！** 不同分布的区别仅在于 $Q_{\text{enc}}(r)$ 的函数形式。

**均匀带电球壳（$R$，$Q$）：**
- $r>R$：$Q_{\text{enc}}=Q$ $\Rightarrow$ $E=kQ/r^2$
- $r<R$：$Q_{\text{enc}}=0$ $\Rightarrow$ $E=0$

**均匀带电球体（$R$，$\rho$，$Q=\frac{4}{3}\pi R^3\rho$）：**
- $r>R$：$Q_{\text{enc}}=Q$ $\Rightarrow$ $E=kQ/r^2$
- $r<R$：$Q_{\text{enc}}=\rho\cdot\frac{4}{3}\pi r^3=Q r^3/R^3$
  $\Rightarrow$ $E = kQr/R^3$（与 $r$ 成正比，在线性增长后在球面达最大）

**线性分布 $\rho(r)=\rho_0 r/R$：**
- $Q_{\text{enc}}=\int_0^r \rho_0\frac{r'}{R}\cdot4\pi r'^2 dr' = \pi\rho_0 r^4/R$
- $E = Q_{\text{enc}}/(4\pi\epsilon_0 r^2) = \rho_0 r^2/(4\epsilon_0 R)$（与 $r^2$ 成正比）

不同内部结构产生不同的内部场，但**外部场都相同**（等效于总电荷位于球心）。

---

**推导3：柱对称和平面对称**

**无限长带电导线（线密度 $\lambda$）：**
取共轴圆柱高斯面（半径 $r$，长度 $L$）。$\vec{E}$ 沿径向，侧面通量 $E\cdot2\pi rL$，上下底通量为零。
$E\cdot 2\pi r L = \lambda L/\epsilon_0$ $\Rightarrow$ $E = \lambda/(2\pi\epsilon_0 r) = 2k\lambda/r$

特点：$E\propto 1/r$，不是 $1/r^2$！这是因为圆柱侧面面积 $\propto r$，导致与 $r$ 成反比。

**无限大带电平面（面密度 $\sigma$）：**
取圆柱高斯面，轴线垂直于平面。两底面通量共 $2EA$，侧面通量为零。
$2EA = \sigma A/\epsilon_0$ $\Rightarrow$ $E = \sigma/(2\epsilon_0)$

特点：**均匀场，与距离无关！** 这是无限大平面独有的性质。

**平行板电容器内部：**
取高斯面：一底在正板导体内（$E=0$），一底在两板之间。
$EA = \sigma A/\epsilon_0$ $\Rightarrow$ $E = \sigma/\epsilon_0$

注意这里是 $\sigma/\epsilon_0$ 而非 $\sigma/(2\epsilon_0)$——因为一底在导体内 $E=0$，通量只从一个底面穿出。

---

**推导4：从积分形式到微分形式（散度定理）**

高斯定律：$\oint_S \vec{E}\cdot d\vec{A} = \frac{1}{\epsilon_0}\int_V \rho\,dV$

散度定理：$\oint_S \vec{E}\cdot d\vec{A} = \int_V (\nabla\cdot\vec{E})\,dV$

两式结合：$\int_V (\nabla\cdot\vec{E})\,dV = \frac{1}{\epsilon_0}\int_V \rho\,dV$

这对**任意体积 $V$** 成立，所以被积函数相等：
$\nabla\cdot\vec{E} = \frac{\rho}{\epsilon_0}$

**物理意义：** 电场在某点的散度等于该点电荷密度除以 $\epsilon_0$。正电荷是电场的"源"（散度为正），负电荷是"汇"（散度为负）。

在无电荷区域（$\rho=0$）：$\nabla\cdot\vec{E}=0$，电场线连续穿过——既无起点也无终点。

**直观理解（小立方体法）：**
取小立方体，边长 $\Delta x, \Delta y, \Delta z$。穿过 $x$ 方向两个面的净通量 $\approx [E_x(x+\Delta x)-E_x(x)]\Delta y\Delta z \approx \frac{\partial E_x}{\partial x}\Delta V$。类似地 $y$ 和 $z$ 方向贡献 $\frac{\partial E_y}{\partial y}\Delta V$ 和 $\frac{\partial E_z}{\partial z}\Delta V$。总通量 $\approx (\nabla\cdot\vec{E})\Delta V = \rho\Delta V/\epsilon_0$。

---

## 1.2 电势的积分计算 — 四次推导

### 公式：$V(\vec{r}) = k\int \dfrac{dq}{|\vec{r}-\vec{r}'|}$，$\vec{E} = -\nabla V$

---

**推导1：从电场定义到电势积分的路径无关性**

$V(\vec{r}) - V(\vec{r}_0) = -\int_{\vec{r}_0}^{\vec{r}} \vec{E}\cdot d\vec{l}$

对点电荷电场 $\vec{E}=kq\hat{r}/r^2$，沿任意路径：
$\vec{E}\cdot d\vec{l} = k\frac{q}{r^2}dr$（只有径向投影贡献）

$\int_{\vec{r}_0}^{\vec{r}} \vec{E}\cdot d\vec{l} = \int_{r_0}^r k\frac{q}{r'^2}dr' = -kq\left(\frac{1}{r}-\frac{1}{r_0}\right)$

令 $r_0\to\infty$，$V(\infty)=0$：$V(r) = \frac{kq}{r}$

对多点电荷：$V = \sum kq_i/r_i$（**标量和！**）
对连续分布：$V = k\int dq/r$（标量积分）

---

**推导2：均匀带电细棒中垂面电势（积分技巧展示）**

棒长 $L$，$\lambda=Q/L$，沿 $y$ 轴 $-L/2$ 到 $L/2$。场点 $P(a,0)$：
$V = k\lambda\int_{-L/2}^{L/2} \frac{dy}{\sqrt{a^2+y^2}}$

令 $y = a\sinh t$，$dy = a\cosh t\,dt$，$\sqrt{a^2+y^2}=a\cosh t$：
$V = k\lambda\int_{t_1}^{t_2} \frac{a\cosh t\,dt}{a\cosh t} = k\lambda\int_{t_1}^{t_2} dt = k\lambda(t_2-t_1)$

$t = \sinh^{-1}(y/a)$，所以 $V = 2k\lambda\sinh^{-1}\left(\frac{L}{2a}\right)$

$= k\lambda\ln\left(\frac{L/2+\sqrt{a^2+L^2/4}}{-L/2+\sqrt{a^2+L^2/4}}\right)$

$a\gg L$ 时：$V \approx k\lambda\cdot\frac{L}{a} = k\frac{Q}{a}$ ✓（退化为点电荷）

---

**推导3："先V后E" — 为什么比直接求E更简单**

以圆环轴线上的电场为例：

**直接法（矢量积分求 $\vec{E}$）：**
$dE_x = k\frac{x\,dq}{(R^2+x^2)^{3/2}}$，$E_x = k\frac{x}{(R^2+x^2)^{3/2}}\int dq = k\frac{Qx}{(R^2+x^2)^{3/2}}$
直观看似乎也不复杂——因为圆环对称性导致问题自动简化。

**先V后E法（标量积分求 $V$，再梯度求 $\vec{E}$）：**
$V(x) = k\int\frac{dq}{\sqrt{R^2+x^2}} = k\frac{Q}{\sqrt{R^2+x^2}}$（一步到位！）
$E_x = -\frac{dV}{dx} = -kQ\frac{d}{dx}(R^2+x^2)^{-1/2} = k\frac{Qx}{(R^2+x^2)^{3/2}}$ ✓

两者结果一致。但**对于更复杂的问题**（如圆盘、非对称分布），先V后E的优势非常显著——电势是标量，直接积分即可；电场是矢量，需分解分量再积分。先V后E把矢量问题转化为标量问题再求导。

**以圆盘为例对比：**
直接求E需二重积分（圆环微元 + 径向积分）：$E_x = \frac{\sigma}{2\epsilon_0}\left(1-\frac{x}{\sqrt{R^2+x^2}}\right)$
先V后E：$V = \frac{\sigma}{2\epsilon_0}(\sqrt{R^2+x^2}-x)$，$E_x=-dV/dx$ 直接得相同结果。
但求 $V$ 的积分显然更简单——因为被积函数不含方向因子。

---

**推导4：电偶极子电势 — 多极展开技术**

$+q$ 在 $+\vec{d}/2$，$-q$ 在 $-\vec{d}/2$。场点 $\vec{r}$（$r\gg d$）：
$V(\vec{r}) = kq\left(\frac{1}{|\vec{r}-\vec{d}/2|} - \frac{1}{|\vec{r}+\vec{d}/2|}\right)$

**泰勒展开：** $\frac{1}{|\vec{r}\pm\vec{d}/2|} = \frac{1}{r}\left(1 \mp \frac{\vec{r}\cdot\vec{d}}{2r^2} + \frac{3(\vec{r}\cdot\vec{d})^2-d^2r^2}{8r^4} + \cdots\right)$

保留到一阶：$V \approx kq\left[\frac{1}{r}\left(1+\frac{\vec{r}\cdot\vec{d}}{2r^2}\right) - \frac{1}{r}\left(1-\frac{\vec{r}\cdot\vec{d}}{2r^2}\right)\right]$
$= k\frac{q\,\vec{r}\cdot\vec{d}}{r^3} = k\frac{\vec{p}\cdot\hat{r}}{r^2}$

这就是电偶极子电势公式。$V\propto 1/r^2$，比点电荷（$1/r$）衰减更快。

**从电势求电场（球坐标）：**
$V(r,\theta) = kp\cos\theta/r^2$
$E_r = -\frac{\partial V}{\partial r} = 2kp\cos\theta/r^3$
$E_\theta = -\frac{1}{r}\frac{\partial V}{\partial\theta} = kp\sin\theta/r^3$
$|E| = \frac{kp}{r^3}\sqrt{4\cos^2\theta+\sin^2\theta} = \frac{kp}{r^3}\sqrt{1+3\cos^2\theta}$

检验：$\theta=0$（偶极轴）：$|E|=2kp/r^3$；$\theta=\pi/2$（垂直平分面）：$|E|=kp/r^3$ ✓

---

### 电势参考点选择的重要说明

不能对任意分布都取 $V(\infty)=0$：

- **点电荷：** 可取 $V(\infty)=0$。$\because$ $\int_\infty^r 1/r'^2 dr'$ 收敛。
- **无限长导线：** 不能取 $V(\infty)=0$！$\because$ $\int_\infty^r 1/r' dr'$ 对数发散。替代：$V(r)=2k\lambda\ln(r_0/r)$。
- **无限大平面：** 不能取 $V(\infty)=0$！$\because$ 均匀场 $\int_\infty^r dr'$ 发散。替代：$V(x)=-\sigma x/(2\epsilon_0)$。

---

## 1.3 连续电荷分布的电场 — 四次推导

### 公式：$\vec{E} = k\int \dfrac{\hat{r}}{r^2}dq$，$dq = \lambda dl,\ \sigma dA,\ \rho dV$

---

**推导1：均匀带电圆盘轴线上的电场（二重积分 $\Rightarrow$ 一重积分）**

圆盘半径 $R$，面密度 $\sigma = Q/(\pi R^2)$。场点 $P(x,0,0)$。

取圆环微元（半径 $r'$，宽度 $dr'$）：$dq = \sigma\cdot 2\pi r' dr'$
圆环在 $P$ 的电场（利用圆环公式）：
$dE_x = k\frac{x\,dq}{(r'^2+x^2)^{3/2}} = k\frac{x\cdot\sigma\cdot2\pi r' dr'}{(r'^2+x^2)^{3/2}}$

$E_x = 2\pi k\sigma x\int_0^R \frac{r' dr'}{(r'^2+x^2)^{3/2}}$

令 $u = r'^2+x^2$，$du = 2r'dr'$：
$E_x = \pi k\sigma x\int_{x^2}^{R^2+x^2} u^{-3/2} du = \pi k\sigma x\left[-2u^{-1/2}\right]_{x^2}^{R^2+x^2}$
$= 2\pi k\sigma x\left(\frac{1}{x} - \frac{1}{\sqrt{R^2+x^2}}\right) = 2\pi k\sigma\left(1 - \frac{x}{\sqrt{R^2+x^2}}\right)$

代入 $k = 1/(4\pi\epsilon_0)$：$E_x = \frac{\sigma}{2\epsilon_0}\left(1 - \frac{x}{\sqrt{R^2+x^2}}\right)$

**极限检验：**
$x\gg R$：$\frac{x}{\sqrt{R^2+x^2}} = (1+R^2/x^2)^{-1/2} \approx 1 - \frac{R^2}{2x^2}$
$E_x \approx \frac{\sigma}{2\epsilon_0}\cdot\frac{R^2}{2x^2} = \frac{Q}{4\pi\epsilon_0 x^2} = k\frac{Q}{x^2}$ ✓（点电荷极限）

$x\to 0$：$E_x \to \frac{\sigma}{2\epsilon_0}$（无限大平面极限 ✓）

---

**推导2：均匀带电细棒一般位置的电场（完整积分）**

棒 $[0,L]$，$\lambda = Q/L$，场点 $(x,y)$。

$dE_x = k\lambda\frac{x'-x}{[(x'-x)^2+y^2]^{3/2}}dx'$
$dE_y = k\lambda\frac{y}{[(x'-x)^2+y^2]^{3/2}}dx'$

令 $u = x'-x$：
$E_x = k\lambda\int_{-x}^{L-x} \frac{u}{(u^2+y^2)^{3/2}} du = k\lambda\left[-\frac{1}{\sqrt{u^2+y^2}}\right]_{-x}^{L-x}$
$= k\lambda\left(\frac{1}{\sqrt{x^2+y^2}} - \frac{1}{\sqrt{(L-x)^2+y^2}}\right)$

$E_y = k\lambda y\int_{-x}^{L-x} \frac{du}{(u^2+y^2)^{3/2}}$

令 $u = y\tan\theta$：$E_y = \frac{k\lambda}{y}\left[\frac{u}{\sqrt{u^2+y^2}}\right]_{-x}^{L-x}$
$= \frac{k\lambda}{y}\left(\frac{L-x}{\sqrt{(L-x)^2+y^2}} + \frac{x}{\sqrt{x^2+y^2}}\right)$

极限检验：$x=0$（中垂面）：
$E_x=0$ ✓（对称性），$E_y = \frac{2k\lambda}{y}\cdot\frac{L/2}{\sqrt{y^2+(L/2)^2}}$ ✓

---

**推导3：半圆环圆心电场（对称性运用）**

半圆环半径 $R$，$\lambda = Q/(\pi R)$，位于 $y\geq0$ 半圆。求圆心 $O$ 处电场。

$dq = \lambda R d\theta$ 在角度 $\theta$ 处。$d\vec{E} = k\frac{dq}{R^2}(-\cos\theta\hat{x} - \sin\theta\hat{y})$（径矢从电荷指向 $O$）

$E_x = -k\frac{\lambda}{R}\int_0^\pi \cos\theta\,d\theta = -k\frac{\lambda}{R}[\sin\theta]_0^\pi = 0$（偶函数对称抵消 ✓）

$E_y = -k\frac{\lambda}{R}\int_0^\pi \sin\theta\,d\theta = -k\frac{\lambda}{R}[-\cos\theta]_0^\pi = -k\frac{\lambda}{R}(1+1) = -\frac{2k\lambda}{R}$

代入 $\lambda$：$\vec{E} = -\frac{2kQ}{\pi R^2}\hat{y}$（指向 $-y$ 方向）

对比：**完整圆环**圆心处 $E=0$（对称抵消），**半圆环**给出非零结果。

---

**推导4：高斯定律验证积分结果**

**无限长导线：** 积分法 $E_x = k\lambda\int_{-\infty}^\infty \frac{a\,dy}{(a^2+y^2)^{3/2}} = \frac{2k\lambda}{a}$，高斯法 $E = \frac{\lambda}{2\pi\epsilon_0 a} = \frac{2k\lambda}{a}$ ✓

**无限大平面：** 积分法 $\lim_{R\to\infty} \frac{\sigma}{2\epsilon_0}\left(1-\frac{x}{\sqrt{R^2+x^2}}\right) = \frac{\sigma}{2\epsilon_0}$，高斯法 $E = \sigma/(2\epsilon_0)$ ✓

**球体外部：** 积分法 $E=kQ/r^2$，高斯法 $E=Q/(4\pi\epsilon_0 r^2)=kQ/r^2$ ✓

**方法选择策略：**
- 有球/柱/平面对称 $\Rightarrow$ **优先用高斯定律**（代数运算）
- 有明确对称轴 $\Rightarrow$ **分解为轴向和径向分量**
- 无特殊对称性 $\Rightarrow$ **先求电势（标量积分）再求梯度**

---

## 1.4 静电场的能量 — 四次推导

### 公式：$U = \frac{1}{2}CV^2 = \frac{Q^2}{2C}$，$u_E = \frac{1}{2}\epsilon_0E^2$

---

**推导1：从电容充电过程到储能公式**

电容器充电：电荷从 $0$ 逐渐增加到 $Q$。在电荷为 $q$ 时，电压 $v = q/C$。
将 $dq$ 从负极移到正极需做功：$dW = v\,dq = \frac{q}{C}dq$
$W = \int_0^Q \frac{q}{C}dq = \frac{1}{C}\left[\frac{q^2}{2}\right]_0^Q = \frac{Q^2}{2C}$
代入 $Q=CV$：$W = \frac{1}{2}CV^2$。三种等价形式：$U = \frac{1}{2}CV^2 = \frac{Q^2}{2C} = \frac{1}{2}QV$。

---

**推导2：从能量密度公式导出电容器储能**

场能量密度 $u_E = \frac{1}{2}\epsilon_0E^2$。
对平行板电容器：$E = V/d$（内部均匀场），体积 $V_{\text{ol}} = Ad$。
$U = u_E \cdot V_{\text{ol}} = \frac{1}{2}\epsilon_0\left(\frac{V}{d}\right)^2 \cdot Ad = \frac{1}{2}\frac{\epsilon_0 A}{d}V^2 = \frac{1}{2}CV^2$ ✓

这说明电容储能的本质是**电场能量**，能量定域在电场中而非"存储在电荷上"。

---

**推导3：从点电荷系统到连续分布**

两点电荷系统能量：$U = \frac{1}{2}(q_1V_1 + q_2V_2)$
其中 $V_1 = kq_2/r_{12}$ 是 $q_2$ 在 $q_1$ 处产生的电势，$V_2 = kq_1/r_{21}$。
$U = \frac{1}{2}\left(q_1\cdot\frac{kq_2}{r_{12}} + q_2\cdot\frac{kq_1}{r_{21}}\right) = k\frac{q_1q_2}{r_{12}}$ ✓

对 $N$ 点电荷：$U = \frac{1}{2}\sum_{i=1}^N q_i V_i(\vec{r}_i)$，其中 $V_i$ 是除 $q_i$ 外其他电荷在 $q_i$ 处产生的电势。

推广到连续分布：$U = \frac{1}{2}\int \rho(\vec{r})V(\vec{r})\,dV$

---

**推导4：均匀带电球体的电场能量（两种方法一致性证明）**

**方法A（场能量密度积分）：**
$U = \frac{\epsilon_0}{2}\int_0^\infty E(r)^2\cdot 4\pi r^2 dr$

$E(r) = \begin{cases} kQr/R^3, & r<R \\ kQ/r^2, & r\geq R \end{cases}$

$U = \frac{\epsilon_0}{2}\left[\int_0^R \left(\frac{Qr}{4\pi\epsilon_0 R^3}\right)^2 4\pi r^2 dr + \int_R^\infty \left(\frac{Q}{4\pi\epsilon_0 r^2}\right)^2 4\pi r^2 dr\right]$

$= \frac{Q^2}{8\pi\epsilon_0}\left[\frac{1}{R^6}\int_0^R r^4 dr + \int_R^\infty \frac{dr}{r^2}\right] = \frac{Q^2}{8\pi\epsilon_0}\left(\frac{1}{5R} + \frac{1}{R}\right) = \frac{3Q^2}{20\pi\epsilon_0 R} = \frac{3kQ^2}{5R}$

**方法B（电荷-电势积分）：**
$U = \frac{1}{2}\int_0^R \rho V(r)\cdot 4\pi r^2 dr$，其中 $\rho = \frac{3Q}{4\pi R^3}$，$V(r) = \frac{kQ}{2R}\left(3 - \frac{r^2}{R^2}\right)$

$U = \frac{1}{2}\cdot\frac{3Q}{4\pi R^3}\cdot\frac{kQ}{2R}\int_0^R \left(3-\frac{r^2}{R^2}\right)4\pi r^2 dr$
$= \frac{3kQ^2}{4R^4}\int_0^R (3r^2 - r^4/R^2)dr = \frac{3kQ^2}{4R^4}\left(R^3 - \frac{R^3}{5}\right) = \frac{3kQ^2}{5R}$ ✓

两种方法结果一致！**方法A更通用**（无需知道电荷与电势的具体分布细节）。

**从电场能量密度到储能公式的完整推导：**
$\frac{1}{2}\int\rho V dV = \frac{\epsilon_0}{2}\int(\nabla\cdot\vec{E})V dV = \frac{\epsilon_0}{2}\left[\oint V\vec{E}\cdot d\vec{A} + \int E^2 dV\right]$
无穷远边界积分 $\to 0$，得 $U = \frac{\epsilon_0}{2}\int E^2 dV$。这个推导将能量从"电荷-电势"形式转化为"电场"形式。

---

## 1.5 导体静电平衡与边界问题 — 四次推导

---

**推导1：导体静电平衡条件的逻辑导出**

**平衡条件1：** 导体内 $\vec{E}=0$。$\because$ 若 $\vec{E}\neq0$，自由电荷受力运动，直到 $\vec{E}=0$ 为止。

**平衡条件2：** 导体表面 $\vec{E}\perp$ 表面。$\because$ 若 $\vec{E}$ 有切向分量，表面电荷会沿表面运动，直到切向分量为零。

**平衡条件3：** 导体是等势体。$\because$ 导体内 $\vec{E}=0$ $\Rightarrow$ $\Delta V = -\int\vec{E}\cdot d\vec{l}=0$，导体上任意两点电势差为零。

**平衡条件4：** 净电荷只分布在表面。$\because$ 导体内 $\vec{E}=0$ $\Rightarrow$ 取导体内高斯面，$Q_{\text{enc}}=0$，导体内无净电荷。

---

**推导2：导体表面电场 $E = \sigma/\epsilon_0$**

取扁圆柱高斯面：底面平行于导体表面，一底面在**导体内**（$E=0$），另一底面在**表面外**。

$\oint\vec{E}\cdot d\vec{A} = EA = \frac{\sigma A}{\epsilon_0}$ $\Rightarrow$ $E = \frac{\sigma}{\epsilon_0}$

**与无限大带电平面的关键区别：**
无限大平面（非导体）：两侧都有电场，$E=\sigma/(2\epsilon_0)$
导体表面：一侧（内部）$E=0$，通量只从一个底面穿出，$E=\sigma/\epsilon_0$

---

**推导3：唯一性定理与镜像法**

**唯一性定理：** 给定边界上的电势（或电荷分布），泊松方程 $\nabla^2 V = -\rho/\epsilon_0$ 的解是唯一的。
**推论：** 如果能找到一个满足边界条件的解，它就是正确的解。

**镜像法—点电荷与接地导体板：**
问题：点电荷 $q$ 在 $x=d$，无限大接地导体板在 $x=0$（$V=0$）。

构造：用镜像电荷 $-q$ 在 $x=-d$ 代替导体板。

验证：$V(x,y,z) = kq\left(\frac{1}{\sqrt{(x-d)^2+y^2+z^2}} - \frac{1}{\sqrt{(x+d)^2+y^2+z^2}}\right)$
在 $x=0$ 平面上：$V=0$ ✓。由唯一性定理，这就是正确解。

感应电荷分布：$\sigma(y,z) = -\epsilon_0\frac{\partial V}{\partial x}\bigg|_{x=0} = -\frac{qd}{2\pi(y^2+z^2+d^2)^{3/2}}$
总感应电荷：$\int\sigma\,dA = -q$ ✓

---

**推导4：三层球壳问题的完整分析**

**结构：** 中心点电荷 $+Q$，导体球壳内半径 $a$ 外半径 $b$，壳带净电荷 $Q_{\text{壳}}$。

**电荷分布推导：**
1. 导体内 $E=0$ $\Rightarrow$ 取高斯面在 $a<r<b$：$Q_{\text{enc}}=Q+q_{\text{内}}=0$ $\Rightarrow$ $q_{\text{内}}=-Q$
2. 壳总电荷守恒：$q_{\text{内}}+q_{\text{外}}=Q_{\text{壳}}$ $\Rightarrow$ $q_{\text{外}}=Q_{\text{壳}}+Q$
3. 外表面电荷均匀分布（球对称），内表面也均匀分布（中心电荷在球心）。

**电场：**
- $r<a$：$E = kQ/r^2$（仅中心电荷贡献）
- $a<r<b$：$E=0$（导体内）
- $r>b$：$E = k(Q+Q_{\text{壳}})/r^2$（总电荷等效于点电荷在球心）

**电势：**
- $r>b$：$V = k(Q+Q_{\text{壳}})/r$
- $a<r<b$：$V = k(Q+Q_{\text{壳}})/b$（导体等势体）
- $r<a$：$V = kQ/r + k(Q+Q_{\text{壳}})/b$

**物理意义：** 球壳屏蔽了中心电荷对壳外的影响（外部场只由总电荷决定），但壳内电荷"感受到"壳的存在（电势叠加）。

---

# Part III：推导例题精选（以推理方法为中心）

> 以下例题的目的是展示**推导方法**而非训练计算。每道题聚焦一种关键的推理技术。

---

### 例题1：从库仑定律到高斯定律的严格推导（立体角法）

**推理链：** 库仑定律 $\vec{E} = kq\hat{r}/r^2$ $\Rightarrow$ 电通量定义 $\Phi_E = \oint\vec{E}\cdot d\vec{A}$

对包围点电荷的任意闭合曲面：
$\Phi_E = \oint kq\frac{\hat{r}\cdot d\vec{A}}{r^2} = kq\oint d\Omega = 4\pi kq = q/\epsilon_0$

其中 $d\Omega = \hat{r}\cdot d\vec{A}/r^2$ 是面元对点电荷所张的**立体角**。整个闭合曲面对内部一点的总立体角恒为 $4\pi$。

对多个点电荷：$\Phi_E = \sum q_i/\epsilon_0 = Q_{\text{enc}}/\epsilon_0$ ✓

**方法要点：** 立体角变换是高斯定律推导的核心技巧。它将曲面积分转化为立体角积分，而立体角积分总是 $4\pi$（对闭合曲面内的点），与曲面形状无关。

---

### 例题2：非均匀带电球体的内部电场（高斯法 vs 直接积分法）

给定 $\rho(r) = \rho_0(1-r/R)$，$0\leq r\leq R$。

**高斯法（推荐）：**
$Q_{\text{enc}}(r) = \int_0^r \rho_0(1-r'/R)\cdot 4\pi r'^2 dr' = 4\pi\rho_0\left[\frac{r^3}{3} - \frac{r^4}{4R}\right]$
$E(r) = \frac{Q_{\text{enc}}}{4\pi\epsilon_0 r^2} = \frac{\rho_0}{\epsilon_0}\left(\frac{r}{3} - \frac{r^2}{4R}\right)$

**直接积分法（验证）：**
$E(r) = \frac{1}{4\pi\epsilon_0}\left[\int_0^r \frac{\rho(r')4\pi r'^2 dr'}{r^2} + \int_r^R \frac{\rho(r')4\pi r'^2 dr'}{r'^2}\right]$
第一项：$r$ 内电荷在 $r$ 处产生的场（球对称等效于点电荷在球心）
第二项：$r$ 外电荷产生的场...... 实际上球对称分布中，外部电荷对内部点的电场贡献为零（球壳定理的推广）。

**对比：** 高斯法利用对称性将面积分简化为代数运算，直接积分法需要处理二重积分。高斯法显著更简洁。

---

### 例题3：对称性分析 — 方法选择策略

**圆环（轴对称）：** 轴上电场用环微元 + 对称性抵消垂直分量 $\Rightarrow$ 简明
**细棒（柱对称但非无限）：** 需要用积分 + 三角代换 $\Rightarrow$ 计算较复杂

**方法选择策略：**
1. 有球/柱/平面对称 $\Rightarrow$ **高斯定律**（代数运算）
2. 有明确对称轴 $\Rightarrow$ **分解为轴向和径向分量**，利用对称性抵消垂直分量
3. 无特殊对称性 $\Rightarrow$ **先求电势（标量积分）再求梯度**，比直接求电场简单

---

### 例题4：圆盘轴线电势的两种积分路径对比

**路径A（圆环微元）：**
$dq = \sigma\cdot2\pi r' dr'$，$dV = kdq/\sqrt{r'^2+x^2}$
$V = 2\pi k\sigma\int_0^R r'dr'/\sqrt{r'^2+x^2} = 2\pi k\sigma(\sqrt{R^2+x^2}-x)$

**路径B（直接二重积分）：**
$V = k\sigma\int_0^R\int_0^{2\pi} \frac{r' d\theta dr'}{\sqrt{r'^2+x^2}} = 2\pi k\sigma\int_0^R \frac{r' dr'}{\sqrt{r'^2+x^2}}$

**相同！** 路径B的 $\theta$ 积分直接给出 $2\pi$，因为被积函数与 $\theta$ 无关。两种路径本质相同，路径A只是"预先知道"$\theta$ 积分为 $2\pi$。

---

### 例题5：电势参考点选择 — 为什么不能总取无穷远

| 分布 | $V(\infty)=0$ 可行？ | 原因 | 替代方案 |
|:--|:--|:--|:--|
| 点电荷 | 可 | $\int 1/r^2 dr$ 收敛 | $V(r)=kQ/r$ |
| 无限长导线 | **不可** | $\int 1/r dr$ 对数发散 | $V(r)=2k\lambda\ln(r_0/r)$ |
| 无限大平面 | **不可** | $\int const\, dr$ 线性发散 | $V(x)=-\sigma x/(2\epsilon_0)$ |

**物理原因：** 电荷分布延伸到无穷远时，无穷远处也有电荷，不能取 $V(\infty)=0$。我们需要选一个有限参考点 $r_0$。

---

### 例题6：从电势求电场的梯度法验证

圆盘电势 $V(x)=\frac{\sigma}{2\epsilon_0}(\sqrt{R^2+x^2}-x)$
$E_x = -\frac{dV}{dx} = -\frac{\sigma}{2\epsilon_0}\left(\frac{x}{\sqrt{R^2+x^2}}-1\right) = \frac{\sigma}{2\epsilon_0}\left(1-\frac{x}{\sqrt{R^2+x^2}}\right)$ ✓

**数值验证：** 取 $R=1, \sigma/(2\epsilon_0)=1$，$x=0.5$：
$V(0.5) = \sqrt{1+0.25}-0.5 = 0.618$
$V(0.501) = \sqrt{1+0.251}-0.501 = 0.6185$
$(V(0.501)-V(0.5))/0.001 = 0.5$
$E_x(0.5) = 1 - 0.5/\sqrt{1.25} = 1-0.447 = 0.553$
数值微分近似正确。要更精确需用更小 $\Delta x$。

---

### 例题7：任意球对称电荷分布的统一形式

对任意球对称 $\rho(r)$：$E(r) = kQ_{\text{enc}}(r)/r^2$
其中 $Q_{\text{enc}}(r) = \int_0^r 4\pi r'^2\rho(r') dr'$

**不同内部结构，相同外部场：** 无论内部电荷如何分布，只要总电荷为 $Q$，在 $r>R$ 的区域，$E=kQ/r^2$ 始终成立。

**启示：** 从外部观察球对称电荷分布，只能知道总电荷，无法推断内部结构。

---

### 例题8：柱对称和球对称的类比分析

| 对称性 | 高斯面 | 面积公式 | 电场公式 |
|:--|:--|:--|:--|
| 球对称 | 同心球面 | $4\pi r^2$ | $E=kQ_{\text{enc}}/r^2$ |
| 柱对称 | 共轴圆柱 | $2\pi r L$ | $E=2k\lambda_{\text{enc}}/r$ |
| 平面对称 | 穿面圆柱 | $2A$（两端面） | $E=\sigma/(2\epsilon_0)$ |

**统一视角：** 三种对称性下，高斯定律都将面积分简化为 $E\times$（高斯面相关面积）$=Q_{\text{enc}}/\epsilon_0$。区别在于高斯面面积随 $r$ 的变化方式不同。

---

### 例题9：微分形式 $\nabla\cdot\vec{E}=\rho/\epsilon_0$ 的物理直观

**直观理解：** 散度衡量"单位体积发出的电通量"。

取小立方体，边长 $\Delta x, \Delta y, \Delta z$：
穿过 $x$ 方向两个面的净通量 $\approx [E_x(x+\Delta x)-E_x(x)]\Delta y\Delta z \approx \frac{\partial E_x}{\partial x}\Delta V$
类似地 $y$ 和 $z$ 方向贡献 $\frac{\partial E_y}{\partial y}\Delta V$ 和 $\frac{\partial E_z}{\partial z}\Delta V$
总通量 $\approx (\nabla\cdot\vec{E})\Delta V = \rho\Delta V/\epsilon_0$ $\Rightarrow$ $\nabla\cdot\vec{E} = \rho/\epsilon_0$

在无电荷区域（$\rho=0$）：$\nabla\cdot\vec{E}=0$，电场线连续穿过——既无起点也无终点，只能从正电荷出发/负电荷终止。

---

### 例题10：电场能量公式 $U=\frac{1}{2}\epsilon_0\int E^2 dV$ 的严格推导

从 $U = \frac{1}{2}\int \rho V dV$ 出发：
由高斯定律 $\rho = \epsilon_0\nabla\cdot\vec{E}$：
$U = \frac{\epsilon_0}{2}\int (\nabla\cdot\vec{E})V dV$

矢量恒等式：$(\nabla\cdot\vec{E})V = \nabla\cdot(V\vec{E}) - \vec{E}\cdot\nabla V$

$U = \frac{\epsilon_0}{2}\left[\int \nabla\cdot(V\vec{E})dV - \int \vec{E}\cdot\nabla V dV\right]$

由散度定理：$\int \nabla\cdot(V\vec{E})dV = \oint V\vec{E}\cdot d\vec{A}$
对无穷远边界，$V\propto 1/r$，$\vec{E}\propto 1/r^2$，$dA\propto r^2$，积分 $\propto 1/r\to 0$。

$\nabla V = -\vec{E}$，所以 $-\int\vec{E}\cdot\nabla V dV = \int E^2 dV$

**最终：** $U = \frac{\epsilon_0}{2}\int E^2 dV$ ✓

这个推导将能量从"电荷-电势"形式转化为"电场"形式，证明**能量定域在电场中**而非储存在电荷上。

---

### 例题11：虚功原理求平行板电容器极板间引力

**原理：** 系统能量对广义坐标的偏导（负）给出广义力。$F = -\partial U/\partial d$。

**情形A（断开电池，$Q$ 不变）：**
$U = Q^2/(2C) = Q^2 d/(2\epsilon_0 A)$
$F = -\frac{\partial U}{\partial d} = -\frac{Q^2}{2\epsilon_0 A} = -\frac{CV^2}{2d} = -\frac{\epsilon_0 A V^2}{2d^2}$
负号表示吸引力（$d$ 减小时能量降低）。

**情形B（电池保持，$V$ 不变）：**
系统总能量变化 $dU = VdQ - Fdd$
$U = \frac{1}{2}CV^2 = \frac{1}{2}\frac{\epsilon_0 A}{d}V^2$
$dQ = V\cdot dC = V\cdot(-\frac{\epsilon_0 A}{d^2}dd)$
电池做功 $VdQ = -\frac{\epsilon_0 AV^2}{d^2}dd$
$dU = \frac{1}{2}(-\frac{\epsilon_0 A}{d^2}V^2)dd$
能量守恒：$dU = VdQ - Fdd$ $\Rightarrow$ $F = (VdQ-dU)/dd = \frac{\epsilon_0 AV^2}{2d^2}$

两种情形结果一致（吸引力）。注意情形B中电池做功 $VdQ$ 必须计入。

---

### 例题12：静电场无旋性 $\nabla\times\vec{E}=0$ 的推导

由法拉第定律：$\oint\vec{E}\cdot d\vec{l} = -d\Phi_B/dt$
静磁条件下 $d\Phi_B/dt=0$，所以 $\oint\vec{E}\cdot d\vec{l}=0$。

由斯托克斯定理：$\oint\vec{E}\cdot d\vec{l} = \int(\nabla\times\vec{E})\cdot d\vec{A}=0$
对任意曲面成立，所以 $\nabla\times\vec{E}=0$。

**等价于：** $\vec{E}=-\nabla V$（无旋场一定是梯度场）。这就是为什么可以定义电势 $V$。

---

### 例题13：非均匀带电线的电场（分部积分法）

$\lambda(x) = \lambda_0(1-x/L)$，$[0,L]$，求 $x=a>L$ 处的 $E$。

$E = k\int_0^L \frac{\lambda_0(1-x'/L)}{(a-x')^2}dx'$

分部积分：令 $u=1-x'/L$，$dv=dx'/(a-x')^2$，$du=-dx'/L$，$v=1/(a-x')$

$E = k\lambda_0\left[\frac{1-x'/L}{a-x'}\bigg|_0^L - \int_0^L \frac{1}{a-x'}\left(-\frac{1}{L}\right)dx'\right]$
$= k\lambda_0\left[0 - \frac{1}{a} + \frac{1}{L}\ln\frac{a}{a-L}\right]$

$a\gg L$：$\ln\frac{a}{a-L} \approx L/a + L^2/(2a^2)$
$E \approx k\lambda_0\left[-\frac{1}{a} + \frac{1}{a} + \frac{L}{2a^2}\right] = k\frac{\lambda_0 L/2}{a^2} = k\frac{Q}{a^2}$ ✓

注意 $-1/a$ 和 $+1/a$ 抵消，最终结果是 $1/a^2$ 行为，而非 $1/a$。这是合理的——有限长带电线在远处表现为点电荷。

---

### 例题14：电四极矩的展开计算

四点电荷系统：$+q(d,d), -q(-d,d), +q(-d,-d), -q(d,-d)$
总电荷 $Q=0$，偶极矩 $\vec{p}=0$。主导项是四极矩。

四极矩张量：$Q_{ij} = \sum q_n(3x_{ni}x_{nj} - r_n^2\delta_{ij})$

仅 $Q_{xy}=Q_{yx}$ 非零：
$Q_{xy} = q[3(d)(d)] + (-q)[3(-d)(d)] + q[3(-d)(-d)] + (-q)[3(d)(-d)]$
$= 3qd^2 + 3qd^2 + 3qd^2 + 3qd^2 = 12qd^2$

电势：$V = \frac{k}{2r^3}\cdot 2Q_{xy}\cdot\frac{x}{r}\frac{y}{r} = \frac{12kqd^2\,xy}{r^5}$
极坐标中 $x=r\cos\phi, y=r\sin\phi$：$V = \frac{6kqd^2}{r^3}\sin 2\phi$

**物理意义：** 系统的"净效果"是四极矩，电势 $\propto 1/r^3$ 衰减，比点电荷（$1/r$）和偶极子（$1/r^2$）都快。

---

### 例题15：镜像电荷法的严格推导

点电荷 $q$ 在 $(0,0,d)$，接地导体平面在 $z=0$，求 $z>0$ 空间的电势。

**边界条件：** $V(x,y,0)=0$，$V\to0$ 当 $r\to\infty$。

**构造解：** 在 $(0,0,-d)$ 放置镜像电荷 $-q$。
$V(x,y,z) = kq\left(\frac{1}{\sqrt{x^2+y^2+(z-d)^2}} - \frac{1}{\sqrt{x^2+y^2+(z+d)^2}}\right)$

**验证边界：** 在 $z=0$ 平面，两项相等，$V=0$ ✓

**唯一性：** 泊松方程在 $z>0$ 区域满足 $\nabla^2 V = -q\delta(\vec{r}-\vec{d}\hat{z})/\epsilon_0$，边界条件满足，由唯一性定理，这是唯一解。

**导体表面感应电荷：**
$\sigma(x,y) = -\epsilon_0\frac{\partial V}{\partial z}\bigg|_{z=0} = -\frac{qd}{2\pi(x^2+y^2+d^2)^{3/2}}$

总感应电荷：$\int_{-\infty}^\infty\int_{-\infty}^\infty \sigma\,dxdy = -q$ ✓

**方法要点：** 镜像法的本质是**用假想电荷满足边界条件**，然后由唯一性定理保证解的正确性。

---

### 补充推导示例：4个关键推导的深度展开

---

#### 补充推导1：球形电容器的电容推导

**问题：** 两个同心导体球壳，内球半径 $a$，外球内半径 $b$，分别带 $+Q$ 和 $-Q$。求电容 $C$。

**推导（高斯定律+电势积分法）：**

**Step 1：** 由球对称性，取 $a<r<b$ 处半径为 $r$ 的同心球面为高斯面：
$$\oint\vec{E}\cdot d\vec{A}=E(r)\cdot 4\pi r^2=\frac{Q}{\epsilon_0}\quad\Rightarrow\quad E(r)=\frac{Q}{4\pi\epsilon_0 r^2}=k\frac{Q}{r^2}$$

**Step 2：** 从内球到外球的电势差：
$$V=V(a)-V(b)=-\int_b^a E(r)dr=-\int_b^a k\frac{Q}{r^2}dr=kQ\left(\frac{1}{a}-\frac{1}{b}\right)$$

**Step 3：** 电容定义：
$$C=\frac{Q}{V}=\frac{Q}{kQ(1/a-1/b)}=\frac{4\pi\epsilon_0 ab}{b-a}$$

**极限检验：** 当 $b\to\infty$（孤立导体球）：$C=4\pi\epsilon_0 a$ ✓
当 $b\approx a+d$（$d\ll a$，近似平行板）：$C\approx 4\pi\epsilon_0 a^2/d=\epsilon_0 A/d$ ✓

**要点：** 球形电容器是平行板电容器和平行板之间的桥梁——当间隙远小于半径时，球面曲率可忽略。

---

#### 补充推导2：从电偶极子电势推导其电场（梯度法 vs 直接矢量法）

已知 $V(r,\theta)=\dfrac{kp\cos\theta}{r^2}$（$\vec{p}$ 沿 $+z$ 轴），求 $\vec{E}$。

**方法A（球坐标梯度）：**
$$E_r=-\frac{\partial V}{\partial r}=2kp\frac{\cos\theta}{r^3},\quad E_\theta=-\frac{1}{r}\frac{\partial V}{\partial\theta}=kp\frac{\sin\theta}{r^3},\quad E_\phi=0$$

$$|\vec{E}|=\frac{kp}{r^3}\sqrt{4\cos^2\theta+\sin^2\theta}=\frac{kp}{r^3}\sqrt{1+3\cos^2\theta}$$

**方法B（直角坐标梯度）：** $V=kpz/(x^2+y^2+z^2)^{3/2}$
$$E_x=-\frac{\partial V}{\partial x}=3kp\frac{xz}{r^5},\quad E_y=3kp\frac{yz}{r^5},\quad E_z=kp\left(\frac{3z^2}{r^5}-\frac{1}{r^3}\right)$$

两种方法等价，球坐标在具有轴对称性的问题中远更简洁。特殊方向检验：沿 $z$ 轴（$\theta=0$），$E=2kp/r^3$（沿 $+z$）；沿赤道面（$\theta=\pi/2$），$E=kp/r^3$（沿 $-z$），大小比轴方向减半 ✓

---

#### 补充推导3：电场能量密度 $u_E=\frac{1}{2}\epsilon_0 E^2$ 的三种推导

**推导A（平行板电容器——最直观）：**
$$U=\frac{1}{2}CV^2=\frac{1}{2}\frac{\epsilon_0 A}{d}(Ed)^2=\frac{1}{2}\epsilon_0 E^2\cdot Ad$$
体积 $=Ad$，所以 $u_E=U/\text{体积}=\frac{1}{2}\epsilon_0 E^2$。

**推导B（从点电荷系统能量到场能量——最严格）：**
$$U=\frac{1}{2}\int\rho V dV=\frac{\epsilon_0}{2}\int(\nabla\cdot\vec{E})V dV$$
利用 $(\nabla\cdot\vec{E})V=\nabla\cdot(V\vec{E})-\vec{E}\cdot\nabla V$ 及 $\nabla V=-\vec{E}$：
$$U=\frac{\epsilon_0}{2}\left[\oint_S V\vec{E}\cdot d\vec{A}+\int_V E^2 dV\right]$$
对全空间积分，在无穷远边界上 $V\propto 1/r$，$E\propto 1/r^2$，$dA\propto r^2$，面积分 $\propto 1/r\to 0$。
$$\therefore U=\frac{\epsilon_0}{2}\int_{\text{全空间}}E^2 dV\quad\Rightarrow\quad u_E=\frac{1}{2}\epsilon_0 E^2$$

**推导C（量纲分析——快速验证）：**
$[\epsilon_0]=\text{C}^2/(\text{N·m}^2)$，$[E]=\text{N/C}$，$[\epsilon_0 E^2]=\text{N/m}^2=\text{J/m}^3$ ✓ 能量密度量纲正确。系数 $1/2$ 来自积分 $\int_0^Q q\,dq=Q^2/2$。

---

#### 补充推导4：导体表面电场 $E=\sigma/\epsilon_0$ 的严格高斯面论证

**关键问题：** 为什么导体表面是 $\sigma/\epsilon_0$ 而非无限大平面的 $\sigma/(2\epsilon_0)$？

**高斯面构造：** 扁圆柱——一底面在导体内（$E=0$），一底面在导体外紧贴表面，侧面垂直于表面（高度 $\to 0$）。

$$\oint\vec{E}\cdot d\vec{A}=E_{\text{外}}\cdot A_{\text{外}}+E_{\text{内}}\cdot A_{\text{内}}+E_{\text{侧}}\cdot A_{\text{侧}}$$

- 导体内 $E_{\text{内}}=0$ → 内底面通量 $=0$
- 侧面高度 $\to 0$ → 侧面积 $\to 0$ → 侧面通量 $=0$
- 导体外 $\vec{E}\perp$ 表面（静电平衡条件）→ $\vec{E}\cdot d\vec{A}=E\cdot A$

$$\therefore \oint\vec{E}\cdot d\vec{A}=EA=\frac{\sigma A}{\epsilon_0}\quad\Rightarrow\quad E=\frac{\sigma}{\epsilon_0}$$

**对比无限大带电平面（非导体）：** 两侧都有场，取高斯面两底面都穿出通量，$2EA=\sigma A/\epsilon_0$ → $E=\sigma/(2\epsilon_0)$。

**物理根源：** 导体内部 $E=0$ 的条件使通量只从一个底面穿出，场强翻倍！

---

# Part IV：微积分与代数综合例题15讲（Step-by-Step）

> 以下15道综合题将微积分（AP Physics C）与代数（AP Physics 2）方法融为一体。每道题标注适用层级：🟢 AP2（代数）、🟣 APC（微积分）、🔴 综合。

---

### 综合题1：三点电荷系统的平衡与受力 🟢

**题目：** 三个点电荷固定于 $x$ 轴上：$q_1=+2.0\,\mu\text{C}$ 在 $x=0$，$q_2=-3.0\,\mu\text{C}$ 在 $x=0.40\,\text{m}$，$q_3=+4.0\,\mu\text{C}$ 在 $x=1.0\,\text{m}$。求 $q_2$ 所受的净电力（大小和方向）。

**Step-by-Step 解法：**

**Step 1 — 确定 $q_1$ 对 $q_2$ 的力：**
$r_{12}=0.40\,\text{m}$，$q_1q_2<0$（异号）→ 吸引力，方向沿 $+x$（指向 $q_1$）
$$F_{12}=k\frac{|q_1q_2|}{r_{12}^2}=(8.99\times10^9)\frac{(2.0\times10^{-6})(3.0\times10^{-6})}{(0.40)^2}=0.337\,\text{N}$$

**Step 2 — 确定 $q_3$ 对 $q_2$ 的力：**
$r_{23}=0.60\,\text{m}$，$q_2q_3<0$（异号）→ 吸引力，方向沿 $+x$（指向 $q_3$）
$$F_{32}=k\frac{|q_2q_3|}{r_{23}^2}=(8.99\times10^9)\frac{(3.0\times10^{-6})(4.0\times10^{-6})}{(0.60)^2}=0.300\,\text{N}$$

**Step 3 — 矢量合成：**
两力同向（均沿 $+x$）：$F_{\text{net}}=0.337+0.300=0.637\,\text{N}$，方向 $+x$。

**答案：** $\boxed{F_{\text{net}}=0.64\,\text{N}\ \text{沿}+x\text{方向}}$

**要点：** 判断方向时不依赖代入正负号，而是用"同斥异吸"独立判断每个力的方向，再进行矢量加法。

---

### 综合题2：有限长均匀带电细棒的电场 🔴

**题目：** 一均匀带电细棒沿 $x$ 轴从 $x=-L$ 到 $x=+L$，线密度 $\lambda=Q/(2L)$。求 $y$ 轴上点 $P(0,a)$ 处的电场（大小和方向）。

**Step-by-Step 解法（微积分矢量法）：**

**Step 1 — 设微元：** 在位置 $x$ 处取微元 $dx$，$dq=\lambda dx$。该微元到 $P$ 的距离 $r=\sqrt{x^2+a^2}$。

**Step 2 — 微元电场：**
$$dE=k\frac{dq}{r^2}=k\frac{\lambda dx}{x^2+a^2}$$
方向沿从微元指向 $P$ 的连线。分解为分量：
$$dE_x=-dE\cos\theta=-dE\cdot\frac{x}{\sqrt{x^2+a^2}}=-k\lambda\frac{x\,dx}{(x^2+a^2)^{3/2}}$$
$$dE_y=dE\sin\theta=dE\cdot\frac{a}{\sqrt{x^2+a^2}}=k\lambda\frac{a\,dx}{(x^2+a^2)^{3/2}}$$

**Step 3 — 积分：**
$$E_x=-k\lambda\int_{-L}^{L}\frac{x\,dx}{(x^2+a^2)^{3/2}}$$
被积函数是奇函数（$x$ 奇，分母偶），对称区间积分为零 → $E_x=0$ ✓（对称性预期）

$$E_y=k\lambda a\int_{-L}^{L}\frac{dx}{(x^2+a^2)^{3/2}}$$
令 $x=a\tan\theta$，$dx=a\sec^2\theta\,d\theta$：
$$\int\frac{dx}{(x^2+a^2)^{3/2}}=\int\frac{a\sec^2\theta\,d\theta}{a^3\sec^3\theta}=\frac{1}{a^2}\int\cos\theta\,d\theta=\frac{\sin\theta}{a^2}=\frac{x}{a^2\sqrt{x^2+a^2}}$$
$$E_y=k\lambda a\left[\frac{x}{a^2\sqrt{x^2+a^2}}\right]_{-L}^{L}=\frac{2k\lambda L}{a\sqrt{L^2+a^2}}$$

**Step 4 — 用总电荷表示：** $\lambda=Q/(2L)$
$$E_y=\frac{2k(Q/2L)L}{a\sqrt{L^2+a^2}}=\frac{kQ}{a\sqrt{L^2+a^2}}$$

**极限检验：** $a\gg L$（远场）：$E_y\approx kQ/a^2$（退化为点电荷 ✓）
$a\ll L$（近场，近似无限长线）：$E_y\approx kQ/(aL)=2k\lambda/a$（无限长线结果 ✓）

**答案：** $\boxed{\vec{E}=\dfrac{kQ}{a\sqrt{L^2+a^2}}\hat{y}}$

---

### 综合题3：均匀带电圆弧在圆心的电场 🔴

**题目：** 一半径为 $R$ 的半圆弧均匀带电，总电荷 $+Q$。求圆心处的电场（大小和方向）。

**Step-by-Step 解法：**

**Step 1 — 设微元：** 线密度 $\lambda=Q/(\pi R)$。角度 $\theta$ 处（从 $+x$ 轴逆时针），弧微元 $ds=R\,d\theta$，$dq=\lambda R\,d\theta$。

**Step 2 — 微元电场方向：** 微元在圆弧上，到圆心的径矢方向为从微元指向圆心。设圆弧在上半平面（$y\geq 0$，$\theta$ 从 $0$ 到 $\pi$），则微元位置为 $(R\cos\theta,R\sin\theta)$。从微元指向圆心 $O$ 的单位矢量是 $(-\cos\theta,-\sin\theta)$。

$$d\vec{E}=k\frac{dq}{R^2}(-\cos\theta\,\hat{x}-\sin\theta\,\hat{y})=-\frac{k\lambda}{R}(\cos\theta\,\hat{x}+\sin\theta\,\hat{y})\,d\theta$$

**Step 3 — 分量积分：**
$$E_x=-\frac{k\lambda}{R}\int_0^\pi\cos\theta\,d\theta=-\frac{k\lambda}{R}[\sin\theta]_0^\pi=0\quad\text{✓（对称性）}$$
$$E_y=-\frac{k\lambda}{R}\int_0^\pi\sin\theta\,d\theta=-\frac{k\lambda}{R}[-\cos\theta]_0^\pi=-\frac{k\lambda}{R}(1+1)=-\frac{2k\lambda}{R}$$

**Step 4 — 代入 $\lambda$：**
$$E_y=-\frac{2k(Q/\pi R)}{R}=-\frac{2kQ}{\pi R^2}$$

**答案：** $\boxed{\vec{E}=-\dfrac{2kQ}{\pi R^2}\hat{y}\ \text{（指向半圆弧的开口方向）}}$

**对比：** 完整圆环在圆心 $E=0$。半圆环的非零电场来自对称性的破缺。$1/4$ 圆弧圆心电场大小为 $\sqrt{2}kQ/(\pi R^2)$（请自证）。

---

### 综合题4：非均匀带电球体——高斯定律应用 🔴

**题目：** 一半径为 $R$ 的绝缘球体，电荷密度 $\rho(r)=\rho_0(1-r/R)$，其中 $\rho_0$ 为常数。求：(a) 球体总电荷；(b) $r<R$ 和 $r>R$ 区域的电场 $E(r)$。

**Step-by-Step 解法：**

**(a) 总电荷：**
$$Q=\int_0^R\rho(r)\cdot 4\pi r^2 dr=4\pi\rho_0\int_0^R\left(1-\frac{r}{R}\right)r^2 dr$$
$$=4\pi\rho_0\left[\frac{r^3}{3}-\frac{r^4}{4R}\right]_0^R=4\pi\rho_0\left(\frac{R^3}{3}-\frac{R^3}{4}\right)=4\pi\rho_0\cdot\frac{R^3}{12}=\frac{\pi\rho_0 R^3}{3}$$

**(b) 电场——高斯定律：**

**$r>R$（球外）：** $Q_{\text{enc}}=Q$
$$E(r)\cdot 4\pi r^2=\frac{Q}{\epsilon_0}\quad\Rightarrow\quad E(r)=\frac{Q}{4\pi\epsilon_0 r^2}=k\frac{Q}{r^2}$$

**$r<R$（球内）：**
$$Q_{\text{enc}}(r)=\int_0^r\rho(r')\cdot 4\pi r'^2 dr'=4\pi\rho_0\int_0^r\left(r'^2-\frac{r'^3}{R}\right)dr'$$
$$=4\pi\rho_0\left(\frac{r^3}{3}-\frac{r^4}{4R}\right)$$
$$E(r)=\frac{Q_{\text{enc}}(r)}{4\pi\epsilon_0 r^2}=\frac{\rho_0}{\epsilon_0}\left(\frac{r}{3}-\frac{r^2}{4R}\right)$$

**验证：** 在 $r=R$ 处，内外表达式应连续：
$$E_{\text{内}}(R)=\frac{\rho_0}{\epsilon_0}\left(\frac{R}{3}-\frac{R}{4}\right)=\frac{\rho_0 R}{12\epsilon_0}$$
$$E_{\text{外}}(R)=k\frac{Q}{R^2}=\frac{1}{4\pi\epsilon_0}\cdot\frac{\pi\rho_0 R^3}{3R^2}=\frac{\rho_0 R}{12\epsilon_0}\quad\text{✓}$$

**答案：** $\boxed{Q=\dfrac{\pi\rho_0 R^3}{3},\quad E_{\text{内}}=\dfrac{\rho_0}{\epsilon_0}\left(\dfrac{r}{3}-\dfrac{r^2}{4R}\right),\quad E_{\text{外}}=k\dfrac{Q}{r^2}}$

---

### 综合题5：同轴电缆（圆柱形电容器）的电容 🔴

**题目：** 一无限长同轴电缆，内导体半径 $a$，外导体内半径 $b$（$b>a$），两导体间为真空。内导体线密度 $+\lambda$，外导体内表面线密度 $-\lambda$。求单位长度的电容。

**Step-by-Step 解法：**

**Step 1 — 电场（高斯定律）：** 取半径 $r$（$a<r<b$）、长度 $L$ 的共轴圆柱面为高斯面：
$$E(r)\cdot 2\pi r L=\frac{\lambda L}{\epsilon_0}\quad\Rightarrow\quad E(r)=\frac{\lambda}{2\pi\epsilon_0 r}$$

**Step 2 — 电势差：**
$$V=V(a)-V(b)=-\int_b^a E(r)dr=-\frac{\lambda}{2\pi\epsilon_0}\int_b^a\frac{dr}{r}=\frac{\lambda}{2\pi\epsilon_0}\ln\frac{b}{a}$$

**Step 3 — 单位长度电容：** 单位长度电荷 $=\lambda$
$$C_{\text{单位长}}=\frac{\lambda}{V}=\frac{2\pi\epsilon_0}{\ln(b/a)}$$

**数值示例：** $a=1.0\,\text{mm}$，$b=3.0\,\text{mm}$：
$$C_{\text{单位长}}=\frac{2\pi(8.85\times10^{-12})}{\ln 3}\approx 5.1\times10^{-11}\,\text{F/m}=51\,\text{pF/m}$$

**极限检验：** $b\approx a+d$（$d\ll a$）：$\ln(b/a)\approx d/a$，$C\approx 2\pi\epsilon_0 a/d$。而平行板电容 $C=\epsilon_0 A/d$，此处 $A=2\pi a\times 1$（周长×单位长），$C=\epsilon_0\cdot 2\pi a/d$ ✓ 一致。

**答案：** $\boxed{C_{\text{单位长}}=\dfrac{2\pi\epsilon_0}{\ln(b/a)}}$

---

### 综合题6：两无限大带电平面的电场叠加 🔴

**题目：** 两无限大非导电平面上均匀分布电荷：面1（$x=0$）面密度 $+\sigma$，面2（$x=d$）面密度 $-2\sigma$。用叠加原理求三个区域（$x<0$，$0<x<d$，$x>d$）的电场。

**Step-by-Step 解法：**

**Step 1 — 单个无限大平面的电场：**
面1在自身两侧产生 $E_1=\sigma/(2\epsilon_0)$，右侧沿 $+x$，左侧沿 $-x$。
面2在自身两侧产生 $E_2=2\sigma/(2\epsilon_0)=\sigma/\epsilon_0$，右侧沿 $-x$（负电荷，场指向平面），左侧沿 $+x$。

**Step 2 — 分区叠加：**

| 区域 | 面1贡献 | 面2贡献 | 合场强 |
|:--|:--|:--|:--|
| $x<0$ | $-\sigma/(2\epsilon_0)$ | $+\sigma/\epsilon_0$ | $+\sigma/(2\epsilon_0)$ |
| $0<x<d$ | $+\sigma/(2\epsilon_0)$ | $+\sigma/\epsilon_0$ | $+3\sigma/(2\epsilon_0)$ |
| $x>d$ | $+\sigma/(2\epsilon_0)$ | $-\sigma/\epsilon_0$ | $-\sigma/(2\epsilon_0)$ |

正号表示 $+x$ 方向，负号表示 $-x$ 方向。

**验证（高斯定律整体法）：** 总面密度在 $x<0$ 侧为 $+\sigma-2\sigma=-\sigma$，预期远离系统处的场 $\propto \sigma_{\text{总}}$。但在 $x<0$ 区域，来自两个平面的场方向相反→叠加后净场确实为 $+\sigma/(2\epsilon_0)$ ✓

**答案：** $\boxed{E_{x<0}=+\dfrac{\sigma}{2\epsilon_0},\quad E_{0<x<d}=+\dfrac{3\sigma}{2\epsilon_0},\quad E_{x>d}=-\dfrac{\sigma}{2\epsilon_0}}$

---

### 综合题7：给定电场求电势——路径无关性验证 🔴

**题目：** 已知二维电场 $\vec{E}=(2axy+b y^2)\hat{x}+(ax^2+2bxy)\hat{y}$（$a,b$ 为常数）。(a) 证明该电场是保守场；(b) 求电势函数 $V(x,y)$（取 $V(0,0)=0$）；(c) 验证沿路径 $(0,0)\to(1,0)\to(1,1)$ 和 $(0,0)\to(0,1)\to(1,1)$ 的电势差相同。

**Step-by-Step 解法：**

**(a) 保守场条件（$\nabla\times\vec{E}=0$，二维等价于 $\partial E_y/\partial x=\partial E_x/\partial y$）：**
$$\frac{\partial E_y}{\partial x}=2ax+2by,\quad \frac{\partial E_x}{\partial y}=2by\quad\text{……不相等！}$$

等一下，$E_y=ax^2+2bxy$，$\partial E_y/\partial x=2ax+2by$。$E_x=2axy+by^2$，$\partial E_x/\partial y=2ax+2by$。相等！✓ 电场是保守场。

**(b) 求 $V(x,y)$：** $E_x=-\partial V/\partial x$ → $V(x,y)=-\int E_x dx+g(y)$
$$V=-\int(2axy+by^2)dx=-ax^2 y-bxy^2+g(y)$$
由 $E_y=-\partial V/\partial y$：
$$E_y=ax^2+2bxy=-\frac{\partial}{\partial y}(-ax^2 y-bxy^2+g(y))=ax^2+2bxy-g'(y)$$
$\therefore g'(y)=0$，$g(y)=\text{常数}$。由 $V(0,0)=0$ 得 $g=0$。
$$V(x,y)=-ax^2 y-bxy^2$$

**(c) 路径验证：**
路径1 $(0,0)\to(1,0)\to(1,1)$：
- $(0,0)\to(1,0)$：$y=0$，$dy=0$，$V=-\int_0^1 E_x(x,0)dx=-\int_0^1 0\,dx=0$
- $(1,0)\to(1,1)$：$x=1$，$dx=0$，$V=-\int_0^1 E_y(1,y)dy=-\int_0^1(a+2by)dy=-a-b$
- $V(1,1)=-a-b$

路径2 $(0,0)\to(0,1)\to(1,1)$：
- $(0,0)\to(0,1)$：$x=0$，$dx=0$，$V=-\int_0^1 E_y(0,y)dy=-\int_0^1 0\,dy=0$
- $(0,1)\to(1,1)$：$y=1$，$dy=0$，$V=-\int_0^1 E_x(x,1)dx=-\int_0^1(2ax+b)dx=-a-b$
- $V(1,1)=-a-b$ ✓ 路径无关！

**答案：** $\boxed{V(x,y)=-ax^2 y-bxy^2}$

---

### 综合题8：从电势函数求电场——梯度运算 🔴

**题目：** 电势 $V(x,y,z)=\dfrac{kQ}{\sqrt{x^2+y^2+(z-d)^2}}-\dfrac{kQ}{\sqrt{x^2+y^2+(z+d)^2}}$（电偶极子势的精确形式）。求 $(0,0,2d)$ 处的电场。

**Step-by-Step 解法：**

**Step 1 — 利用对称性简化：** 在 $x=0,y=0$ 的 $z$ 轴上，由对称性 $E_x=E_y=0$。只需计算 $E_z=-\partial V/\partial z$。

**Step 2 — 在 $z$ 轴上计算：**
$$V(0,0,z)=kQ\left(\frac{1}{|z-d|}-\frac{1}{|z+d|}\right)$$
在 $z=2d$ 处，$z>d$：
$$V=kQ\left(\frac{1}{2d-d}-\frac{1}{2d+d}\right)=kQ\left(\frac{1}{d}-\frac{1}{3d}\right)=\frac{2kQ}{3d}$$

**Step 3 — 求 $E_z$（先求导再代入）：**
$$E_z=-\frac{\partial V}{\partial z}=-kQ\left[-\frac{1}{(z-d)^2}+\frac{1}{(z+d)^2}\right]=kQ\left[\frac{1}{(z-d)^2}-\frac{1}{(z+d)^2}\right]$$
代入 $z=2d$：
$$E_z=kQ\left[\frac{1}{d^2}-\frac{1}{9d^2}\right]=\frac{8kQ}{9d^2}$$

**Step 4 — 用偶极近似验证：** 偶极矩 $p=Q\cdot 2d$，偶极子轴上远场 $E=2kp/r^3$。在 $z=2d$ 处，$r=2d$，$E_{\text{偶极}}=2k(2Qd)/(2d)^3=kQ/(2d^2)=0.5kQ/d^2$。精确解 $0.889kQ/d^2$，差异较大——因为 $z=2d$ 不满足 $r\gg d$ 的远场条件。偶极近似只在 $r\gg d$ 时有效。

**答案：** $\boxed{\vec{E}(0,0,2d)=\dfrac{8kQ}{9d^2}\hat{z}}$

---

### 综合题9：均匀带电圆盘轴线上电势与电场 🔴

**题目：** 半径 $R$ 的均匀带电圆盘，面密度 $\sigma$。(a) 求轴线上距盘心 $x$ 处的电势 $V(x)$；(b) 由 $V(x)$ 求 $E(x)$；(c) 验证 $x\to 0$ 和 $x\gg R$ 极限。

**Step-by-Step 解法：**

**(a) 电势（标量积分——圆环微元法）：**
取半径 $r$、宽 $dr$ 的圆环微元：$dq=\sigma\cdot 2\pi r\,dr$。圆环上所有点到轴上点 $(x,0,0)$ 的距离均为 $\sqrt{r^2+x^2}$。
$$dV=k\frac{dq}{\sqrt{r^2+x^2}}=k\sigma\cdot 2\pi r\cdot\frac{dr}{\sqrt{r^2+x^2}}$$
$$V(x)=2\pi k\sigma\int_0^R\frac{r\,dr}{\sqrt{r^2+x^2}}$$
令 $u=r^2+x^2$，$du=2r\,dr$：
$$V(x)=\pi k\sigma\int_{x^2}^{R^2+x^2}u^{-1/2}du=2\pi k\sigma\left[\sqrt{u}\right]_{x^2}^{R^2+x^2}=2\pi k\sigma(\sqrt{R^2+x^2}-x)$$
代入 $k=1/(4\pi\epsilon_0)$：
$$V(x)=\frac{\sigma}{2\epsilon_0}(\sqrt{R^2+x^2}-x)$$

**(b) 电场（梯度法）：**
$$E_x=-\frac{dV}{dx}=-\frac{\sigma}{2\epsilon_0}\left(\frac{x}{\sqrt{R^2+x^2}}-1\right)=\frac{\sigma}{2\epsilon_0}\left(1-\frac{x}{\sqrt{R^2+x^2}}\right)$$

**(c) 极限检验：**
- $x\gg R$：$\sqrt{R^2+x^2}=x\sqrt{1+R^2/x^2}\approx x(1+R^2/(2x^2))=x+R^2/(2x)$，$V\approx (\sigma/(2\epsilon_0))\cdot R^2/(2x)=(\sigma\pi R^2)/(4\pi\epsilon_0 x)=kQ/x$（点电荷 ✓）
  $E\approx (\sigma/(2\epsilon_0))(1-(1-R^2/(2x^2)))=(\sigma R^2)/(4\epsilon_0 x^2)=kQ/x^2$ ✓
- $x\to 0$：$V\to \sigma R/(2\epsilon_0)$，$E\to \sigma/(2\epsilon_0)$（无限大平面极限 ✓）

**答案：** $\boxed{V(x)=\dfrac{\sigma}{2\epsilon_0}(\sqrt{R^2+x^2}-x),\quad E(x)=\dfrac{\sigma}{2\epsilon_0}\left(1-\dfrac{x}{\sqrt{R^2+x^2}}\right)}$

---

### 综合题10：电容器网络——串并联化简 🟢

**题目：** 四个电容器连接如网：$C_1=6\,\mu\text{F}$ 与 $C_2=3\,\mu\text{F}$ 并联，该组合与 $C_3=4\,\mu\text{F}$ 串联，再与 $C_4=2\,\mu\text{F}$ 并联。两端接 $V=12\,\text{V}$ 电池。求：(a) 等效电容；(b) 每个电容器上的电荷和电压。

**Step-by-Step 解法：**

**(a) 等效电容化简：**
$$C_{12}=C_1+C_2=6+3=9\,\mu\text{F}\quad\text{（并联）}$$
$$\frac{1}{C_{123}}=\frac{1}{C_{12}}+\frac{1}{C_3}=\frac{1}{9}+\frac{1}{4}=\frac{13}{36}\quad\Rightarrow\quad C_{123}=\frac{36}{13}\approx 2.77\,\mu\text{F}\quad\text{（串联）}$$
$$C_{\text{eq}}=C_{123}+C_4=2.77+2=4.77\,\mu\text{F}\quad\text{（并联）}$$

**(b) 逐级反推电荷和电压：**
$C_4$ 直接跨接在 12 V 上：$V_4=12\,\text{V}$，$Q_4=C_4V_4=2\times12=24\,\mu\text{C}$

$C_{123}$ 组合也跨接在 12 V 上：$Q_{123}=C_{123}V=2.77\times12\approx 33.2\,\mu\text{C}$

串联的 $C_{12}$ 和 $C_3$ 带相同电荷 $Q_{123}$：
$V_3=Q_{123}/C_3=33.2/4=8.31\,\text{V}$，$V_{12}=Q_{123}/C_{12}=33.2/9=3.69\,\text{V}$

并联的 $C_1$ 和 $C_2$ 电压均为 $V_{12}=3.69\,\text{V}$：
$Q_1=C_1V_{12}=6\times3.69=22.2\,\mu\text{C}$，$Q_2=C_2V_{12}=3\times3.69=11.1\,\mu\text{C}$

**验证：** $Q_1+Q_2=33.3\approx Q_{123}$ ✓；$V_3+V_{12}=8.31+3.69=12.0\,\text{V}$ ✓

**答案：** $\boxed{C_{\text{eq}}=4.77\,\mu\text{F};\ Q_{1,2,3,4}=22.2,11.1,33.2,24\,\mu\text{C};\ V_{1,2,3,4}=3.69,3.69,8.31,12\,\text{V}}$

---

### 综合题11：部分填充介质的平行板电容器 🔴

**题目：** 平行板电容器，板面积 $A$，间距 $d$。介电常数 $\kappa$ 的介质填充了下半部分（厚度 $d/2$，紧贴下板），上半部分为真空。求等效电容。（分别用串联模型和高斯定律两种方法验证）

**Step-by-Step 解法：**

**方法A（串联模型——将介质-真空界面视为等势面）：**
等效为两个电容串联：真空层 $C_1=\epsilon_0 A/(d/2)=2\epsilon_0 A/d$，介质层 $C_2=\kappa\epsilon_0 A/(d/2)=2\kappa\epsilon_0 A/d$
$$\frac{1}{C}=\frac{1}{C_1}+\frac{1}{C_2}=\frac{d}{2\epsilon_0 A}+\frac{d}{2\kappa\epsilon_0 A}=\frac{d}{2\epsilon_0 A}\left(1+\frac{1}{\kappa}\right)$$
$$C=\frac{2\epsilon_0 A}{d}\cdot\frac{\kappa}{\kappa+1}$$

**方法B（高斯定律+电势积分验证）：**
设板上自由电荷面密度 $\pm\sigma_f$。在真空中 $E_1=\sigma_f/\epsilon_0$，在介质中 $E_2=\sigma_f/(\kappa\epsilon_0)$。
$$V=E_1\cdot\frac{d}{2}+E_2\cdot\frac{d}{2}=\frac{\sigma_f d}{2\epsilon_0}\left(1+\frac{1}{\kappa}\right)$$
$$C=\frac{Q}{V}=\frac{\sigma_f A}{V}=\frac{2\epsilon_0 A}{d}\cdot\frac{\kappa}{\kappa+1}\quad\text{✓}$$

**极限检验：** $\kappa=1$（无介质）：$C=\epsilon_0 A/d$ ✓
$\kappa\to\infty$（导体）：$C\to 2\epsilon_0 A/d$（间距减半——导体介质将有效间距缩为 $d/2$）✓

**答案：** $\boxed{C=\dfrac{2\kappa\epsilon_0 A}{(\kappa+1)d}}$

---

### 综合题12：介质插入时电容器能量变化（V恒定 vs Q恒定） 🔴

**题目：** 平行板电容器 $C_0=\epsilon_0 A/d$，充电至电压 $V_0$ 后：(a) 保持与电池连接，插入 $\kappa=4$ 的介质填满板间，求能量变化及电池做功；(b) 断开电池后插入同样介质，求能量变化。

**Step-by-Step 解法：**

**(a) V恒定（$V=V_0$）：**
插入前：$U_0=\frac{1}{2}C_0 V_0^2$，$Q_0=C_0 V_0$
插入后：$C=\kappa C_0=4C_0$，$Q=CV_0=4C_0 V_0$，$U=\frac{1}{2}CV_0^2=4U_0$
$$\Delta U_{\text{电容}}=U-U_0=3U_0=\frac{3}{2}C_0 V_0^2\quad\text{（能量增加）}$$

电池做功：$W_{\text{电池}}=V_0\Delta Q=V_0(Q-Q_0)=V_0(4C_0 V_0-C_0 V_0)=3C_0 V_0^2$

能量守恒检查：$W_{\text{电池}}=\Delta U_{\text{电容}}+W_{\text{介质被拉入}}$
$3C_0 V_0^2=1.5C_0 V_0^2+W_{\text{拉入}}$ → $W_{\text{拉入}}=1.5C_0 V_0^2$（电场力将介质拉入板间做正功）

**(b) Q恒定（$Q=Q_0=C_0 V_0$）：**
插入前：$U_0=Q_0^2/(2C_0)$
插入后：$C=4C_0$，$V=Q_0/C=V_0/4$，$U=Q_0^2/(2C)=Q_0^2/(8C_0)=U_0/4$
$$\Delta U_{\text{电容}}=U-U_0=-\frac{3}{4}U_0=-\frac{3}{8}C_0 V_0^2\quad\text{（能量减少）}$$

能量去向：减少的静电能转化为介质极化所需能量 + 介质被拉入的动能（最终耗散为热）。

**答案：** $\boxed{\text{(a) }\Delta U=+\dfrac{3}{2}C_0 V_0^2,\ W_{\text{电池}}=3C_0 V_0^2;\quad\text{(b) }\Delta U=-\dfrac{3}{8}C_0 V_0^2}$

---

### 综合题13：构建电荷组态所需的功 🔴

**题目：** 四个点电荷 $+q,+q,-q,-q$ 分别固定在边长为 $a$ 的正方形四个顶点（按顺时针 $+q,+q,-q,-q$）。求从无穷远将这些电荷逐个搬来组装成此组态所需的总功。

**Step-by-Step 解法：**

**Step 1 — 搬入第一个电荷 $q_1=+q$（在 $(0,0)$）：** 无其他电荷 → $W_1=0$。

**Step 2 — 搬入第二个电荷 $q_2=+q$（在 $(a,0)$）：** 与 $q_1$ 距离 $a$，同号排斥。
$$W_2=k\frac{q_1 q_2}{a}=k\frac{q^2}{a}$$

**Step 3 — 搬入第三个电荷 $q_3=-q$（在 $(a,a)$）：** 与 $q_1$ 距离 $\sqrt{2}a$（吸引），与 $q_2$ 距离 $a$（吸引）。
$$W_3=k\frac{q_1 q_3}{\sqrt{2}a}+k\frac{q_2 q_3}{a}=k\frac{(+q)(-q)}{\sqrt{2}a}+k\frac{(+q)(-q)}{a}=-\frac{kq^2}{a}\left(\frac{1}{\sqrt{2}}+1\right)$$

**Step 4 — 搬入第四个电荷 $q_4=-q$（在 $(0,a)$）：** 与 $q_1$ 距离 $a$（吸引），与 $q_2$ 距离 $\sqrt{2}a$（吸引），与 $q_3$ 距离 $a$（同号排斥）。
$$W_4=k\frac{q_1 q_4}{a}+k\frac{q_2 q_4}{\sqrt{2}a}+k\frac{q_3 q_4}{a}=-\frac{kq^2}{a}-\frac{kq^2}{\sqrt{2}a}+\frac{kq^2}{a}=-\frac{kq^2}{\sqrt{2}a}$$

**Step 5 — 总功：**
$$W_{\text{总}}=0+\frac{kq^2}{a}-\frac{kq^2}{a}\left(\frac{1}{\sqrt{2}}+1\right)-\frac{kq^2}{\sqrt{2}a}=-\frac{\sqrt{2}kq^2}{a}$$

**验证（用 $U=\frac{1}{2}\sum q_i V_i$）：**
$$U=\frac{1}{2}\sum_{i=1}^4 q_i V_i,\quad V_1=k\left(\frac{+q}{a}+\frac{-q}{\sqrt{2}a}+\frac{-q}{a}\right)=-\frac{kq}{\sqrt{2}a}$$
类似计算 $V_2,V_3,V_4$，得 $U=-\sqrt{2}kq^2/a$ ✓

**答案：** $\boxed{W_{\text{总}}=-\dfrac{\sqrt{2}kq^2}{a}\ \text{（负号表示系统净释放能量，是束缚态）}}$

---

### 综合题14：导体球壳空腔中的点电荷 🔴

**题目：** 一不带电的导体球壳，内半径 $a$，外半径 $b$。在球心处放置一点电荷 $+q$。求：(a) 各区域的电场 $E(r)$；(b) 各区域的电势 $V(r)$（取 $V(\infty)=0$）；(c) 内外表面的感应电荷。

**Step-by-Step 解法：**

**(a) 电场——高斯定律：**

**区域I（$r<a$，空腔内）：** $Q_{\text{enc}}=+q$ → $E_{\text{I}}=kq/r^2$

**区域II（$a<r<b$，导体内）：** 静电平衡 → $E_{\text{II}}=0$

**区域III（$r>b$，壳外）：** 取高斯面在此区域。壳原不带电，静电感应使内表面感应出 $-q$，外表面感应出 $+q$（总电荷守恒）。$Q_{\text{enc}}=+q$ → $E_{\text{III}}=kq/r^2$

**(b) 电势：**
**$r>b$：** $V_{\text{III}}=kq/r$（等效于球心点电荷 + 壳屏蔽）
**$a<r<b$：** 导体内等势，$V_{\text{II}}=V(b)=kq/b$
**$r<a$：** $V_{\text{I}}=-\int_b^r E\,dr=-\int_b^a 0\,dr-\int_a^r(kq/r'^2)dr'=kq/b+kq(1/r-1/a)=kq/r+kq(1/b-1/a)$
即 $V_{\text{I}}(r)=kq/r+\text{常数}$，常数来自壳的电势贡献。

**(c) 感应电荷：** 内表面 $-q$，外表面 $+q$。

**关键物理：** 导体壳屏蔽了内部电荷对外部的影响吗？不——外部电场 $E=kq/r^2$ 与无壳时完全相同！导体壳只屏蔽了外部对内部的影响，内部电荷对外部的影响取决于总电荷。此处壳原不带电，内部电荷 $+q$ 使外表面感应出 $+q$，所以从外部看，等效于点电荷 $+q$ 在球心。

**答案：** $\boxed{E_{\text{I}}=\dfrac{kq}{r^2},\ E_{\text{II}}=0,\ E_{\text{III}}=\dfrac{kq}{r^2};\quad V_{\text{I}}=\dfrac{kq}{r}+kq\left(\dfrac{1}{b}-\dfrac{1}{a}\right),\ V_{\text{II}}=\dfrac{kq}{b},\ V_{\text{III}}=\dfrac{kq}{r}}$

---

### 综合题15：综合题——从电荷密度到电场、电势、能量 🔴

**题目：** 一绝缘球体半径 $R$，电荷密度 $\rho(r)=\rho_0(r/R)^2$。求：(a) 总电荷 $Q$；(b) 球内外电场 $E(r)$；(c) 球内外电势 $V(r)$（取 $V(\infty)=0$）；(d) 总静电能 $U$（用场能量密度法）。

**Step-by-Step 解法：**

**(a) 总电荷：**
$$Q=\int_0^R\rho_0\left(\frac{r}{R}\right)^2\cdot 4\pi r^2 dr=\frac{4\pi\rho_0}{R^2}\int_0^R r^4 dr=\frac{4\pi\rho_0}{R^2}\cdot\frac{R^5}{5}=\frac{4\pi}{5}\rho_0 R^3$$

**(b) 电场（高斯定律）：**
**$r>R$：** $E_{\text{外}}=kQ/r^2=\dfrac{4\pi k\rho_0 R^3}{5r^2}$

**$r<R$：** $Q_{\text{enc}}(r)=\int_0^r\rho_0(r'/R)^2\cdot 4\pi r'^2 dr'=\dfrac{4\pi\rho_0}{R^2}\cdot\dfrac{r^5}{5}=\dfrac{4\pi}{5}\rho_0\dfrac{r^5}{R^2}$
$$E_{\text{内}}=\frac{Q_{\text{enc}}(r)}{4\pi\epsilon_0 r^2}=\frac{1}{4\pi\epsilon_0}\cdot\frac{4\pi}{5}\rho_0\frac{r^5}{R^2}\cdot\frac{1}{r^2}=\frac{\rho_0 r^3}{5\epsilon_0 R^2}$$

**(c) 电势：**
**$r>R$：** $V_{\text{外}}=kQ/r=\dfrac{4\pi k\rho_0 R^3}{5r}$

**$r<R$：**
$$V_{\text{内}}=-\int_\infty^R E_{\text{外}}dr-\int_R^r E_{\text{内}}dr$$
$$=k\frac{Q}{R}-\int_R^r\frac{\rho_0 r'^3}{5\epsilon_0 R^2}dr'=\frac{kQ}{R}-\frac{\rho_0}{5\epsilon_0 R^2}\left[\frac{r'^4}{4}\right]_R^r$$
$$=\frac{kQ}{R}-\frac{\rho_0}{20\epsilon_0 R^2}(r^4-R^4)$$
代入 $Q=4\pi\rho_0 R^3/5$ 及 $k=1/(4\pi\epsilon_0)$：
$$V_{\text{内}}=\frac{\rho_0}{5\epsilon_0}\left(R^2-\frac{r^4}{4R^2}+\frac{R^2}{4}\right)=\frac{\rho_0}{20\epsilon_0}\left(5R^2-\frac{r^4}{R^2}\right)$$

**(d) 静电能（场能量密度法）：**
$$U=\frac{\epsilon_0}{2}\int_0^\infty E^2\cdot 4\pi r^2 dr=\frac{\epsilon_0}{2}\left[\int_0^R E_{\text{内}}^2\cdot 4\pi r^2 dr+\int_R^\infty E_{\text{外}}^2\cdot 4\pi r^2 dr\right]$$

内部积分：
$$\int_0^R\left(\frac{\rho_0 r^3}{5\epsilon_0 R^2}\right)^2\cdot 4\pi r^2 dr=\frac{4\pi\rho_0^2}{25\epsilon_0^2 R^4}\int_0^R r^8 dr=\frac{4\pi\rho_0^2 R^5}{225\epsilon_0^2}$$

外部积分：
$$\int_R^\infty\left(\frac{kQ}{r^2}\right)^2\cdot 4\pi r^2 dr=4\pi k^2 Q^2\int_R^\infty\frac{dr}{r^2}=4\pi k^2\frac{Q^2}{R}$$

代入 $Q$ 和 $k$ 化简得 $U=\dfrac{4\pi\rho_0^2 R^5}{45\epsilon_0}$。

**答案：** $\boxed{Q=\dfrac{4\pi}{5}\rho_0 R^3,\ E_{\text{内}}=\dfrac{\rho_0 r^3}{5\epsilon_0 R^2},\ E_{\text{外}}=\dfrac{kQ}{r^2},\ V_{\text{内}}=\dfrac{\rho_0}{20\epsilon_0}\left(5R^2-\dfrac{r^4}{R^2}\right),\ V_{\text{外}}=\dfrac{kQ}{r},\ U=\dfrac{4\pi\rho_0^2 R^5}{45\epsilon_0}}$

---

## 附录：整个章节的逻辑结构图

```
实验基础：库仑定律 F = k|q₁q₂|/r²   ←── 平方反比律（三维空间+通量守恒的必然结果）
    │
    ├──→ 电场定义 E = F/q
    │       ├──→ 点电荷电场 E = kq/r²
    │       ├──→ 叠加原理 E_net = ΣE_i（矢量求和，需分量分解）
    │       └──→ 连续分布 E = k∫(r̂/r²)dq
    │              ├─── 线分布 dq=λdl
    │              ├─── 面分布 dq=σdA
    │              └─── 体分布 dq=ρdV
    │
    ├──→ 高斯定律 ∮E·dA = Q_enc/ε₀
    │       ├──→ ∇·E = ρ/ε₀（微分形式，散度定理导出）
    │       ├──→ 球对称：E = kQ_enc/r²（外部总电荷集中）
    │       ├──→ 柱对称：E = 2kλ_enc/r（外部总电荷集轴）
    │       └──→ 平面对称：E = σ/(2ε₀）（均匀场，与距离无关）
    │
    ├──→ 电势 V = k∫dq/r（标量积分！比电场更简单）
    │       ├──→ E = -∇V（梯度关系，电场指向电势下降最快方向）
    │       ├──→ 等势面 ⊥ 电场线（ΔV=0 ⇒ E·dl=0）
    │       └──→ 多极展开：V = kQ/r + kp·r̂/r² + ...（远处近似）
    │
    ├──→ 电容 C = Q/V
    │       ├──→ 平行板 C = ε₀A/d（高斯定律导出）
    │       ├──→ 储能 U = ½CV² = Q²/(2C)（充电过程积分）
    │       └──→ 能量密度 u_E = ½ε₀E²（能量定域在电场中）
    │
    ├──→ 导体静电平衡
    │       ├──→ 内部 E=0，表面 E⊥表面，等势体
    │       ├──→ 表面 E = σ/ε₀（高斯扁圆柱）
    │       └──→ 唯一性定理 + 镜像法（边界条件决定解）
    │
    └──→ 能量守恒 W_E = -ΔU_E = ΔK（保守力）
```

---

**核心概念区分：**

| | 电场 $\vec{E}$ | 电势 $V$ |
|:--|:--|:--|
| 类型 | 矢量 | 标量 |
| 叠加 | 分量分别求和再合成 | 直接代数相加 |
| 与力的关系 | $\vec{F}=q\vec{E}$ | $W=q\Delta V$ |
| 与能量的关系 | — | $U=qV$ |
| 单位 | N/C = V/m | V |

**常见概念陷阱：**

1. **电场 $\neq$ 电势的梯度绝对值**，而是负梯度。$E_x = -dV/dx$，负号表示电场指向电势降低方向。
2. **库仑定律 $F=k|q_1q_2|/r^2$ 带绝对值**，方向需单独判断。
3. **电势能 $U=kq_1q_2/r$ 不带绝对值**，正负号有物理含义（正=排斥势，负=吸引势）。
4. **电容器断开 $\Rightarrow$ Q不变**，保持连接 $\Rightarrow$ V不变。
5. **高斯定律需要高度对称性**（球/柱/平面）才能有效运用。
6. **$V(\infty)=0$ 并非总是可行的参考点选择**（无限长导线、无限大平面不行）。

---