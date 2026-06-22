# Chapter 13：磁学与电磁学（Magnetism and Electromagnetism）

### 【AP Physics 2】Unit 12：Magnetism and Electromagnetism

| 编号 | 知识点 | 核心公式/概念 | 技能 |
|:--:|:--|:--|:--:|
| **12.1** | 磁场 | 磁感线 N → S（外部） | 1.A, 2.A |
| **12.2** | 磁场中的运动电荷 | $\vec{F}=q\vec{v}\times\vec{B}$；$F=qvB\sin\theta$；$r=\frac{mv}{qB}$ | 1.A, 2.B |
| **12.3** | 载流导线在磁场中 | $\vec{F}=I\vec{L}\times\vec{B}$；电动机原理 | 2.A, 3.B |
| **12.4** | 电磁感应与法拉第定律 | $\mathcal{E}=-\frac{d\Phi_B}{dt}$；$\Phi_B=BA\cos\theta$；楞次定律 | 2.A, 3.B |

### 【AP Physics C: E&M】Unit 4：Magnetic Fields（🟣 微积分深化）

| 编号 | 知识点 | 核心公式/概念 | 🟣 微积分关键 |
|:--:|:--|:--|:--|
| **4.1** | 磁场中的运动电荷 | $\vec{F}=q\vec{v}\times\vec{B}$；回旋 $r=\frac{mv}{qB}$ | — |
| **4.2** | 载流导线受力 | $d\vec{F}=I\,d\vec{l}\times\vec{B}$ | 🟣 线积分 |
| **4.3** | 长直载流导线磁场 | $B=\frac{\mu_0 I}{2\pi r}$ | — |
| **🔑 4.4** | **毕奥-萨伐尔定律 & 安培定律（独家）** | $d\vec{B}=\frac{\mu_0}{4\pi}\frac{I\,d\vec{l}\times\hat{r}}{r^2}$；$\oint\vec{B}\cdot d\vec{l}=\mu_0 I_{enc}$ | 🟣 **独家**：矢量积分 + 环路积分 |

---
---

# Chapter 13：磁学与电磁学 — 完整推导参考文档

**AP Physics 2 Unit 12 + AP Physics C: E&M Unit 4 · 以推导为中心**

---

## 绪论：磁学与静电学的对称性

静电学的核心：静止电荷产生电场 $\vec{E}$，电场对静止电荷施力 $\vec{F}=q\vec{E}$。
磁学的核心：**运动**电荷产生磁场 $\vec{B}$，磁场对**运动**电荷施力 $\vec{F}=q\vec{v}\times\vec{B}$。

**关键对比：**
- 电场力平行于场方向（$\vec{F} \parallel \vec{E}$），磁场力垂直于场和速度方向（$\vec{F} \perp \vec{B}, \vec{v}$）
- 电场力做功改变动能，磁场力**不做功**（$\because \vec{F}\perp\vec{v}$）
- 电场有源（$+\to-$），磁场无源（$\nabla\cdot\vec{B}=0$，磁单极不存在）

**逻辑链条：**
1. 磁场的定义：$\vec{F}=q\vec{v}\times\vec{B}$（洛伦兹力）
2. 电流产生磁场：毕奥-萨伐尔定律（线积分）$\Leftrightarrow$ 安培定律（环路积分）
3. 变化磁场产生电场：法拉第定律 $\mathcal{E}=-d\Phi_B/dt$
4. 能量守恒决定方向：楞次定律

---

# 12.1 / 4.1 磁场与洛伦兹力 — 四种推导

## 核心公式：$\vec{F}=q\vec{v}\times\vec{B}$，$F=qvB\sin\theta$，$r=mv/(qB)$

---

**推导1：磁场力的定义与叉积几何**

**实验基础：** 运动电荷在磁场中受到侧向力——方向垂直于速度和磁场方向。

数学形式（洛伦兹力）：$\vec{F} = q\vec{v}\times\vec{B}$

叉积大小：$F = |q|vB\sin\theta$，$\theta$ 为 $\vec{v}$ 与 $\vec{B}$ 的夹角。

方向判定（右手定则）：
- 右手四指从 $\vec{v}$ 方向弯向 $\vec{B}$ 方向
- 拇指指向为正电荷受力方向
- 负电荷受力方向与拇指相反

**磁场单位：** 特斯拉（T）。$1\text{T} = 1\text{N/(A·m)} = 1\text{N·s/(C·m)}$
地球磁场约 $5\times10^{-5}\text{T}$，MRI 磁场约 $1.5-3\text{T}$。

---

**推导2：磁场力不做功的证明**

瞬时功率：$P = \vec{F}\cdot\vec{v} = (q\vec{v}\times\vec{B})\cdot\vec{v}$

由矢量三重积性质：$(\vec{v}\times\vec{B})\cdot\vec{v} = 0$（叉积垂直于 $\vec{v}$，点积为零）

$P=0$ $\Rightarrow$ 磁场力不做功，不改变电荷速率，只改变方向。

**对比电场力：** $\vec{F}_E = q\vec{E}$，$P = q\vec{E}\cdot\vec{v}$ ——电场力可以做功，改变动能。
- 电场平行加速器：$v$ 增加
- 磁场回旋加速器：$|v|$ 不变，方向改变

---

**推导3：匀强磁场中的圆周运动**

设 $\vec{v}\perp\vec{B}$（最简情形）。

$\vec{F}=q\vec{v}\times\vec{B}$ 提供向心力，大小 $F=qvB$。

由牛顿第二定律和圆周运动：$qvB = m\frac{v^2}{r}$

**回旋半径（拉莫尔半径）：** $r = \frac{mv}{qB}$

**回旋周期：** $T = \frac{2\pi r}{v} = \frac{2\pi m}{qB}$

**回旋频率：** $f = \frac{1}{T} = \frac{qB}{2\pi m}$，$\omega = \frac{qB}{m}$

**$\Rightarrow$ $r\propto v$（能量越高半径越大），但 $T$ 和 $f$ 与速度无关！**

这个性质是回旋加速器的基础——无论粒子速度多大，回旋周期相同。

---

**推导4：一般情况下的螺旋运动**

若 $\vec{v}$ 有平行于 $\vec{B}$ 的分量 $v_{\parallel}$ 和垂直于 $\vec{B}$ 的分量 $v_{\perp}$：

- 垂直分量 $\vec{v}_{\perp}$ 产生圆周运动（半径 $r=mv_{\perp}/(qB)$）
- 平行分量 $v_{\parallel}$ 不受磁场力，沿磁场方向匀速运动
- 合运动为**等距螺旋线**：螺距 $p = v_{\parallel}T = \frac{2\pi m v_{\parallel}}{qB}$

**应用：** 磁约束（托卡马克）、磁瓶、极光（带电粒子沿地磁场螺旋运动，在两极进入大气）

---

# 12.3 / 4.2 载流导线在磁场中 — 三种推导

## 核心公式：$\vec{F}=I\vec{L}\times\vec{B}$，$d\vec{F}=I\,d\vec{l}\times\vec{B}$

---

**推导1：从运动电荷受力到载流导线受力**

导线中每个运动电荷受力 $q\vec{v}_d\times\vec{B}$。长度为 $L$ 的导线中有 $N = nAL$ 个自由电子。

总力：$\vec{F} = N(q\vec{v}_d\times\vec{B}) = nAL\cdot (-e\vec{v}_d\times\vec{B})$

由 $I = nAev_d$，且电流方向与电子运动方向相反：
$\vec{F} = nAeL(-\vec{v}_d)\times\vec{B} = I\vec{L}\times\vec{B}$

其中 $\vec{L}$ 为从电流起点指向终点的矢量，大小为 $L$，方向为电流方向。

对弯曲导线：$d\vec{F} = I\,d\vec{l}\times\vec{B}$，$\vec{F} = \int I\,d\vec{l}\times\vec{B}$

---

**推导2：两平行载流导线间的磁力**

**步骤1：** 导线1（电流 $I_1$）在距离 $r$ 处产生磁场 $B_1 = \mu_0 I_1/(2\pi r)$（方向由右手定则）
**步骤2：** 导线2（电流 $I_2$，长度 $L$）在 $B_1$ 中受力
$F = I_2 L B_1 = I_2 L \cdot \frac{\mu_0 I_1}{2\pi r} = \frac{\mu_0 I_1 I_2 L}{2\pi r}$

**方向：** 同向电流相互吸引，反向电流相互排斥。

**单位安培的定义：** 真空中相距 $1\text{m}$ 的两无限长平行细导线，通以相同电流，当每米受力为 $2\times10^{-7}\text{N}$ 时，电流定义为 $1\text{A}$。

---

**推导3：电动机原理 — 矩形线圈在磁场中的力矩**

矩形线圈（边长 $a,b$，$N$ 匝）在匀强磁场 $B$ 中，线圈法线与 $\vec{B}$ 夹角 $\theta$。

两边（长 $a$）受力 $F = NI aB$，方向相反，形成力偶。
力臂 $= b\sin\theta$（在磁场平面内的投影）
力矩：$\tau = N I aB \cdot b\sin\theta = N I AB\sin\theta$，$A=ab$ 为线圈面积

矢量形式：$\vec{\tau} = N I \vec{A}\times\vec{B}$（$\vec{A}$ 的法线方向由右手定则确定）

**直流电动机：** 换向器每半圈反转电流方向，使力矩始终同向。

---

# 12.4 电磁感应与法拉第定律 — 四次推导

## 核心公式：$\mathcal{E} = -d\Phi_B/dt$，$\Phi_B = BA\cos\theta$

---

**推导1：法拉第定律的实验基础**

**实验1：** 磁铁靠近/远离线圈 $\Rightarrow$ 产生感应电流（动生电动势）
**实验2：** 改变线圈面积（拉伸/压缩）$\Rightarrow$ 产生感应电流
**实验3：** 改变磁场强度（通断电）$\Rightarrow$ 产生感应电流
**实验4：** 旋转线圈在磁场中 $\Rightarrow$ 产生交变感应电流

**统一解释：** 穿过线圈的磁通量 $\Phi_B = \int\vec{B}\cdot d\vec{A}$ 随时间变化时，线圈中产生感应电动势。

$\mathcal{E} = -\frac{d\Phi_B}{dt}$

负号由楞次定律决定——感应电流产生的磁场**阻碍**磁通量的变化。

---

**推导2：楞次定律的物理推理**

楞次定律：感应电流的方向总是反抗引起感应的原因。

**判断步骤：**
1. 确定磁通量 $\Phi_B$ 的变化方向（增加/减少）
2. 感应电流产生的磁场 $\vec{B}_{\text{ind}}$ 应**反抗**这个变化
   - 若 $\Phi_B\uparrow$：$\vec{B}_{\text{ind}}$ 与 $\vec{B}$ 反向（试图抵消增加）
   - 若 $\Phi_B\downarrow$：$\vec{B}_{\text{ind}}$ 与 $\vec{B}$ 同向（试图补偿减少）
3. 由 $\vec{B}_{\text{ind}}$ 的方向，用右手定则确定感应电流方向

**能量守恒解释：** 如果感应电流方向不符合楞次定律，就会产生正反馈，导致无限能量——违反热力学第一定律。楞次定律本质上是能量守恒在电磁感应中的表现。

---

**推导3：动生电动势的微观推导**

导体棒长 $L$ 以速度 $v$ 垂直切割磁感线 $B$。

**微观图像：** 导体棒中的自由电子随棒运动，受到洛伦兹力 $\vec{F}= -e\vec{v}\times\vec{B}$，沿棒方向被推向一端，导致电荷分离——棒两端产生电势差。

洛伦兹力等效"非静电场"：$\vec{E}_{\text{非}} = \frac{\vec{F}}{-e} = \vec{v}\times\vec{B}$

感应电动势：$\mathcal{E} = \int\vec{E}_{\text{非}}\cdot d\vec{l} = \int_0^L vB\,dl = vBL$

**与法拉第定律的一致性：** 磁通量变化率
$\Phi_B = BA = BLx$（$x$ 为棒位置）
$\frac{d\Phi_B}{dt} = BL\frac{dx}{dt} = BLv$ $\Rightarrow$ $\mathcal{E} = BLv$ ✓

---

**推导4：法拉第电机的应用**

转动导体在磁场中产生感应电动势，是发电机和电动机的基础。

**例：** 半径为 $R$ 的导体盘在匀强磁场 $B$ 中以角速度 $\omega$ 旋转。

圆盘半径方向上各点线速度 $v = \omega r$。从中心到边缘的感应电动势：
$\mathcal{E} = \int_0^R B\omega r\,dr = \frac{1}{2}B\omega R^2$

这个装置可看作直流发电机——圆盘与外电路通过电刷连接产生持续电流。

---

# 4.3 / 4.4 毕奥-萨伐尔定律与安培定律 — 五次推导 ★ 核心

## 核心公式：$d\vec{B} = \dfrac{\mu_0}{4\pi}\dfrac{I\,d\vec{l}\times\hat{r}}{r^2}$，$\oint\vec{B}\cdot d\vec{l} = \mu_0 I_{\text{enc}}$

---

**推导1：毕奥-萨伐尔定律求长直导线磁场**

**设置：** 长直导线沿 $y$ 轴，电流 $I$ 向上。求 $x=a$ 处的磁场。

取电流元 $Id\vec{l} = I\,dy\,\hat{y}$ 在 $(0,y)$，到场点 $P(a,0)$ 的径矢 $\vec{r} = a\hat{x}-y\hat{y}$。

$d\vec{l}\times\hat{r} = dy\,\hat{y}\times\frac{a\hat{x}-y\hat{y}}{r} = dy\frac{a(\hat{y}\times\hat{x})-y(\hat{y}\times\hat{y})}{r} = \frac{a\,dy}{r}(-\hat{z})$

$dB = \frac{\mu_0}{4\pi}\frac{I a\,dy}{r^3}$，方向 $-\hat{z}$（进入纸面）

$r = \sqrt{a^2+y^2}$，$y = a\tan\theta$，$dy = a\sec^2\theta\,d\theta$

$B = \frac{\mu_0 I}{4\pi}\int_{-\infty}^\infty \frac{a\,dy}{(a^2+y^2)^{3/2}} = \frac{\mu_0 I}{4\pi a}\int_{-\pi/2}^{\pi/2}\cos\theta\,d\theta = \frac{\mu_0 I}{2\pi a}$

**最终：** $B = \frac{\mu_0 I}{2\pi r}$，方向由右手定则（拇指电流方向，四指磁场环绕方向）

---

**推导2：安培定律推导长直导线磁场（对比）**

取环绕导线的圆形安培回路（半径 $r$），由对称性 $\vec{B}$ 沿切线方向，大小处处相等。

$\oint\vec{B}\cdot d\vec{l} = B\cdot 2\pi r = \mu_0 I_{\text{enc}} = \mu_0 I$

$B = \frac{\mu_0 I}{2\pi r}$

**对比两种方法：**
- 毕奥-萨伐尔定律：积分更复杂（需处理矢量叉积），但可处理任意形状的载流导线
- 安培定律：运算简单，但**需要高度对称性**（无限长直导线、螺线管、环形线圈）

**方法选择：** 有对称性 $\Rightarrow$ 安培定律；无对称性 $\Rightarrow$ 毕奥-萨伐尔定律

---

**推导3：螺线管内部磁场（安培定律应用）**

长直螺线管，单位长度匝数 $n$，电流 $I$。

取矩形安培回路（长 $L$，一边在螺线管内，一边在外部）。

$\oint\vec{B}\cdot d\vec{l} = B_{\text{内}}L = \mu_0 I_{\text{enc}} = \mu_0 (nL I)$

$\Rightarrow$ $B_{\text{内}} = \mu_0 n I$

**假设：** 螺线管无限长，内部磁场均匀且平行于轴线，外部磁场近似为零。

**有限长螺线管：** 端部磁场约为内部的一半（$B_{\text{端}} = \frac{1}{2}\mu_0 n I$）。

---

**推导4：毕奥-萨伐尔定律求环形电流圆心磁场**

半径为 $R$ 的圆环，电流 $I$，求圆心磁场。

对任意电流元 $Id\vec{l}$，$d\vec{B} = \frac{\mu_0}{4\pi}\frac{I\,d\vec{l}\times\hat{r}}{R^2}$

对圆环圆心，$\hat{r}$ 沿半径向外，$d\vec{l}\perp\hat{r}$，$|d\vec{l}\times\hat{r}| = dl$

所有电流元在圆心产生的磁场方向相同（由右手定则，垂直纸面向外）。

$B = \frac{\mu_0 I}{4\pi R^2}\int dl = \frac{\mu_0 I}{4\pi R^2}\cdot 2\pi R = \frac{\mu_0 I}{2R}$

---

**推导5：安培定律的微分形式**

由斯托克斯定理：$\oint\vec{B}\cdot d\vec{l} = \int(\nabla\times\vec{B})\cdot d\vec{A}$

安培定律：$\oint\vec{B}\cdot d\vec{l} = \mu_0 I_{\text{enc}} = \mu_0\int\vec{J}\cdot d\vec{A}$

两式结合：$\int(\nabla\times\vec{B})\cdot d\vec{A} = \mu_0\int\vec{J}\cdot d\vec{A}$

对任意曲面成立：$\nabla\times\vec{B} = \mu_0\vec{J}$

**物理含义：** 磁场的"旋度"等于电流密度——电流是磁场的"涡旋源"。
- $\nabla\cdot\vec{B}=0$：磁场无源（无磁单极）
- $\nabla\times\vec{B}=\mu_0\vec{J}$：磁场有旋（电流产生环绕磁场）

**对比静电学：**
| | 电场 $\vec{E}$ | 磁场 $\vec{B}$ |
|:--|:--|:--|
| 散度 | $\nabla\cdot\vec{E} = \rho/\epsilon_0$ | $\nabla\cdot\vec{B}=0$ |
| 旋度 | $\nabla\times\vec{E}=0$（静电） | $\nabla\times\vec{B}=\mu_0\vec{J}$ |

---

## 附录：关键公式速查

| 公式 | 物理含义 | 适用条件 |
|:--|:--|:--|
| $\vec{F}=q\vec{v}\times\vec{B}$ | 洛伦兹力（磁分量） | 运动电荷在磁场中 |
| $r=mv/(qB)$ | 回旋半径 | $\vec{v}\perp\vec{B}$ |
| $T=2\pi m/(qB)$ | 回旋周期 | 与速度无关！ |
| $\vec{F}=I\vec{L}\times\vec{B}$ | 载流导线受力 | 均匀磁场 |
| $d\vec{F}=I\,d\vec{l}\times\vec{B}$ | 微分线元受力 | 非均匀磁场 |
| $\vec{\tau}=NI\vec{A}\times\vec{B}$ | 线圈力矩 | 均匀磁场 |
| $\Phi_B=\int\vec{B}\cdot d\vec{A}$ | 磁通量定义 | 通用 |
| $\mathcal{E}=-d\Phi_B/dt$ | 法拉第定律 | 电磁感应 |
| $d\vec{B}=\frac{\mu_0}{4\pi}\frac{I\,d\vec{l}\times\hat{r}}{r^2}$ | 毕奥-萨伐尔定律 | 电流元产生磁场 |
| $\oint\vec{B}\cdot d\vec{l}=\mu_0 I_{\text{enc}}$ | 安培定律 | 稳恒电流 |
| $B=\mu_0 I/(2\pi r)$ | 长直导线磁场 | 无限长 |
| $B=\mu_0 n I$ | 螺线管内部磁场 | 长直螺线管 |
| $B=\mu_0 I/(2R)$ | 环形电流圆心磁场 | 单匝圆环 |
| $\nabla\cdot\vec{B}=0$ | 磁场无源 | 无磁单极 |
| $\nabla\times\vec{B}=\mu_0\vec{J}$ | 安培定律微分形式 | 稳恒电流 |

---

## 常见概念陷阱

1. **洛伦兹力不做功：** $\vec{F}\perp\vec{v}$，所以磁场力只能改变带电粒子运动方向，不能改变速率
2. **$F=qvB\sin\theta$ 中的 $\theta$：** 是 $\vec{v}$ 与 $\vec{B}$ 之间的夹角，不是其他角度
3. **右手定则统一性：** 电流产生磁场、载流导线受力、感应电流方向——都用右手定则但具体手势不同，注意区分
4. **楞次定律 $\neq$ 法拉第定律的负号：** 负号是楞次定律的数学表达，但定律本身有独立物理含义（能量守恒）
5. **$\mu_0$ 的值：** $\mu_0=4\pi\times10^{-7}\ \text{T·m/A}$——精确值、定义值，来自安培的定义
6. **安培定律的局限：** 仅适用于稳恒电流。变化的电场也产生磁场（位移电流，麦克斯韦修正）——下一章的内容
7. **$\oint\vec{B}\cdot d\vec{l}$ 与 $\oint\vec{E}\cdot d\vec{l}$ 的区别：** 后者在静电学中为零（保守场），前者在存在电流时非零

---

## 核心推理方法总结

| 问题类型 | 方法 | 关键步骤 |
|:--|:--|:--|
| 运动电荷在磁场中 | $\vec{F}=q\vec{v}\times\vec{B}$ | 判断叉积方向，圆周/螺旋运动 |
| 载流导线受力 | $\vec{F}=I\vec{L}\times\vec{B}$ | 用叉积求力的大小和方向 |
| 求磁场（有对称性） | 安培定律 $\oint\vec{B}\cdot d\vec{l}=\mu_0 I_{\text{enc}}$ | 选对称安培回路 |
| 求磁场（无对称性） | 毕奥-萨伐尔定律 $d\vec{B}=\frac{\mu_0}{4\pi}\frac{I\,d\vec{l}\times\hat{r}}{r^2}$ | 矢量分解+积分 |
| 感应电动势 | $\mathcal{E}=-d\Phi_B/dt$ | 分析 $\Phi_B$ 变化来源 |
| 感应电流方向 | 楞次定律 | 判断 $\Phi_B$ 变化方向 |
| 动生电动势 | $\mathcal{E}=vBL$ 或 $\int(\vec{v}\times\vec{B})\cdot d\vec{l}$ | 洛伦兹力分离电荷 |

