<!-- markdownlint-disable MD033 MD041 -->

<div align="center">

# 📚 AP Physics — 力学 2：力与平动动力学

> **Force & Translational Dynamics — 完整综合版**
>
> 覆盖 AP Physics 1（代数）+ AP Physics C（微积分）全难度层级

[![AP Physics](https://img.shields.io/badge/AP-Physics-001845?style=for-the-badge&logo=apache&logoColor=white)](https://ap.collegeboard.org/)
[![Physics 1](https://img.shields.io/badge/AP%20Physics-1-FF6B35?style=flat-square)]()
[![Physics C](https://img.shields.io/badge/AP%20Physics-C-004E89?style=flat-square)]()

</div>

---

## 📑 目录

- [2.1 系统与质心](#21-系统与质心systems-and-center-of-mass)
- [2.2 力与自由体图](#22-力与自由体图forces-and-free-body-diagrams)
- [2.3 牛顿第三定律](#23-牛顿第三定律newtons-third-law)
- [2.4 牛顿第一定律（惯性）](#24-牛顿第一定律惯性newtons-first-law)
- [2.5 牛顿第二定律](#25-牛顿第二定律newtons-second-law)
- [2.6 引力](#26-引力gravitational-force)
- [2.7 静摩擦力与动摩擦力](#27-静摩擦力与动摩擦力static-and-kinetic-friction)
- [2.8 弹簧力（胡克定律）](#28-弹簧力胡克定律spring-force-hookes-law)
- [2.9 圆周运动](#29-圆周运动circular-motion)
- [2.10 阻力（AP Physics C 独家）](#210-阻力ap-physics-c-独家drag-force)
- [综合例题](#ch2-综合例题10题)

---

# 2.1 系统与质心（Systems and Center of Mass）

## Part A：基础层（AP Physics 1 必备）

### 一、系统的概念

> **系统（System）** 是我们在分析物理问题时选定的研究对象集合。系统边界外的物体称为 **外界（Environment/Surroundings）**。

| 概念 | 说明 |
|:--|:--|
| **孤立系统** | 与外界无质量、能量交换 |
| **闭合系统** | 与外界有能量交换，无质量交换 |
| **开放系统** | 与外界有质量和能量交换 |

> ⚠️ **AP 重点**：正确划定系统边界是列方程的第一步！系统不同，哪些力是"内力"、哪些是"外力"也会不同。

### 二、质心（Center of Mass）

#### 2.1.1 离散系统的质心

对于由 $n$ 个质点组成的系统，质心位置为各质点位置的 **质量加权平均**：

$$
\boxed{x_{cm} = \frac{\sum_{i=1}^{n} m_i x_i}{\sum_{i=1}^{n} m_i} = \frac{m_1 x_1 + m_2 x_2 + \cdots + m_n x_n}{m_1 + m_2 + \cdots + m_n}}
$$

三维推广：

$$
\boxed{\vec{r}_{cm} = \frac{\sum m_i \vec{r}_i}{\sum m_i}}
$$

| 项目 | 说明 |
|:--|:--|
| 类别 | **位置矢量**——描述系统整体位置 |
| 物理含义 | 系统质量分布的平均位置 |
| 单位 | 米（m） |

#### 2.1.2 质心的性质

1. **质心运动定理**：系统所受合外力等于总质量乘以质心加速度
   $$ \Sigma \vec{F}_{ext} = M \vec{a}_{cm} $$
2. **质心速度**：$\vec{v}_{cm} = \dfrac{\sum m_i \vec{v}_i}{M}$
3. 如果没有合外力，质心保持匀速直线运动或静止

#### 2.1.3 🧪 推导 1：两质点系统的质心

**题目**：两个质量分别为 $m_1$ 和 $m_2$ 的质点位于 $x_1$ 和 $x_2$ 处，求质心位置。

**推导**：

由质心定义：

$$
x_{cm} = \frac{m_1 x_1 + m_2 x_2}{m_1 + m_2}
$$

为了更直观，引入总质量 $M = m_1 + m_2$ 和相对位置 $d = x_2 - x_1$：

设 $x_1 = 0$（将第一个质点放在原点），则：

$$
x_{cm} = \frac{m_1 \cdot 0 + m_2 \cdot d}{m_1 + m_2} = \frac{m_2}{m_1 + m_2} d
$$

> 💡 **物理直觉**：质心更靠近质量较大的物体。若 $m_1 \gg m_2$，则 $x_{cm} \approx 0$（靠近 $m_1$）；若 $m_1 = m_2$，则 $x_{cm} = d/2$（正中间）。

#### 2.1.4 🧪 推导 2：质心运动定理的证明

由牛二定律，对每个质点：

$$
\vec{F}_i^{ext} + \sum_{j \neq i} \vec{F}_{ij}^{int} = m_i \vec{a}_i
$$

对所有质点求和：

$$
\sum_i \vec{F}_i^{ext} + \sum_i \sum_{j \neq i} \vec{F}_{ij}^{int} = \sum_i m_i \vec{a}_i
$$

由牛三定律，内力成对抵消：$\sum_i \sum_{j \neq i} \vec{F}_{ij}^{int} = 0$

根据质心定义 $\vec{r}_{cm} = \dfrac{\sum m_i \vec{r}_i}{M}$，两边对时间求两次导：

$$
\vec{a}_{cm} = \frac{d^2 \vec{r}_{cm}}{dt^2} = \frac{\sum m_i \vec{a}_i}{M}
$$

代入得：

$$
\boxed{\Sigma \vec{F}_{ext} = M \vec{a}_{cm}}
$$

> ⭐ **核心结论**：质心的运动完全由 **合外力** 决定，**内力不影响质心的运动**！

#### 2.1.5 🧪 例题 1：两质点系统的质心

**题目**：质量分别为 $2\ \text{kg}$ 和 $3\ \text{kg}$ 的两个物体位于 $x=0$ 和 $x=5\ \text{m}$ 处。求：(a) 质心位置；(b) 若 $2\ \text{kg}$ 物体移动到 $x=2\ \text{m}$，新的质心位置。

**解答**：

**(a)** 

$$
x_{cm} = \frac{2 \times 0 + 3 \times 5}{2 + 3} = \frac{15}{5} = \mathbf{3\ m}
$$

**(b)** 

$$
x_{cm} = \frac{2 \times 2 + 3 \times 5}{2 + 3} = \frac{4 + 15}{5} = \frac{19}{5} = \mathbf{3.8\ m}
$$

> ⚠️ 质心随着质量分布的变化而移动！

#### 2.1.6 🧪 例题 2：三质点系统的质心

**题目**：三个质点位于 $xy$ 平面内：$m_1 = 1\ \text{kg}$ 在 $(0,0)$，$m_2 = 2\ \text{kg}$ 在 $(4,0)$，$m_3 = 3\ \text{kg}$ 在 $(0,3)$。求质心位置。

**解答**：

$$
x_{cm} = \frac{1 \times 0 + 2 \times 4 + 3 \times 0}{1 + 2 + 3} = \frac{8}{6} = \frac{4}{3} \approx 1.33\ \text{m}
$$

$$
y_{cm} = \frac{1 \times 0 + 2 \times 0 + 3 \times 3}{1 + 2 + 3} = \frac{9}{6} = 1.5\ \text{m}
$$

所以质心在 $\boxed{(1.33\ \text{m},\ 1.5\ \text{m})}$。

---

## Part B：AP Physics C 微积分扩展

#### 2.1.7 🧪 推导 3：连续物体的质心（积分形式）

对于质量连续分布的物体，质心公式从求和变为积分：

$$
\boxed{\vec{r}_{cm} = \frac{1}{M} \int \vec{r}\ dm}
$$

其中 $dm$ 是质量微元。根据不同的质量分布形式：

| 分布类型 | $dm$ 表达式 | 说明 |
|:--|:--|:--|
| **线分布** | $dm = \lambda\ dl$ | $\lambda$ 为线密度（kg/m），$dl$ 为长度微元 |
| **面分布** | $dm = \sigma\ dA$ | $\sigma$ 为面密度（kg/m²），$dA$ 为面积微元 |
| **体分布** | $dm = \rho\ dV$ | $\rho$ 为体密度（kg/m³），$dV$ 为体积微元 |

**推导思路**：

将连续物体分割成无数个质量微元 $dm$，每个微元的位置为 $\vec{r}$。质心公式为：

$$
\vec{r}_{cm} = \lim_{\Delta m_i \to 0} \frac{\sum \vec{r}_i \Delta m_i}{\sum \Delta m_i} = \frac{\int \vec{r}\ dm}{\int dm} = \frac{1}{M} \int \vec{r}\ dm
$$

#### 2.1.8 🧪 推导 4：均匀细杆的质心

**题目**：一根长度为 $L$、质量为 $M$ 的均匀细杆，沿 $x$ 轴放置，一端在原点。求质心位置。

**推导**：

线密度 $\lambda = M/L$，质量微元 $dm = \lambda\ dx = \frac{M}{L}dx$

$$
x_{cm} = \frac{1}{M} \int_0^L x\ dm = \frac{1}{M} \int_0^L x \cdot \frac{M}{L}\ dx = \frac{1}{L} \int_0^L x\ dx
$$

$$
x_{cm} = \frac{1}{L} \left[ \frac{x^2}{2} \right]_0^L = \frac{1}{L} \cdot \frac{L^2}{2} = \boxed{\frac{L}{2}}
$$

> 💡 均匀细杆的质心在几何中心。但如果是 **非均匀** 杆（密度随位置变化），质心就不在中心了！

#### 2.1.9 🧪 例题 3（AP C）：半圆环的质心

**题目**：一个半径为 $R$、质量为 $M$ 的均匀半圆环（线密度均匀），求其质心位置。

**解答**：

由对称性，$x_{cm} = 0$（半圆环关于 $y$ 轴对称）。

对于 $y$ 方向：线密度 $\lambda = M/(\pi R)$

取角度微元 $d\theta$，对应的弧长 $dl = R\ d\theta$，质量 $dm = \lambda R\ d\theta$

$$
y_{cm} = \frac{1}{M} \int y\ dm = \frac{1}{M} \int_0^\pi (R\sin\theta)(\lambda R\ d\theta)
$$

$$
y_{cm} = \frac{\lambda R^2}{M} \int_0^\pi \sin\theta\ d\theta = \frac{\lambda R^2}{M} \left[ -\cos\theta \right]_0^\pi
$$

$$
y_{cm} = \frac{\lambda R^2}{M} (1 + 1) = \frac{2\lambda R^2}{M} = \frac{2R^2}{M} \cdot \frac{M}{\pi R} = \boxed{\frac{2R}{\pi} \approx 0.637R}
$$

> ⭐ **对称性简化**：利用对称性可以减少一个维度的计算！

---

# 2.2 力与自由体图（Forces and Free Body Diagrams）

## Part A：基础层（AP Physics 1 必备）

### 一、力的基本概念

> **力（Force）** 是物体之间的相互作用，是改变物体运动状态的原因。

| 项目 | 说明 |
|:--|:--|
| 类别 | **矢量**——既有大小又有方向 |
| 单位 | 牛顿（N），$1\ \text{N} = 1\ \text{kg} \cdot \text{m/s}^2$ |
| 分类 | 接触力（摩擦力、弹力、张力等）和非接触力（重力、电磁力等） |

#### 2.2.1 常见力类型

| 力 | 符号 | 方向 | 公式 |
|:--|:--:|:--|:--|
| **重力** | $\vec{F}_g$ 或 $\vec{W}$ | 竖直向下 | $F_g = mg$ |
| **法向力** | $\vec{N}$ 或 $\vec{F}_N$ | 垂直于接触面 | 大小可变 |
| **静摩擦力** | $\vec{f}_s$ | 平行于接触面，与运动趋势相反 | $f_s \le \mu_s N$ |
| **动摩擦力** | $\vec{f}_k$ | 平行于接触面，与运动方向相反 | $f_k = \mu_k N$ |
| **张力** | $\vec{T}$ | 沿绳子方向，拉离物体 | 大小可变 |
| **弹簧力** | $\vec{F}_s$ | 与形变方向相反（恢复力） | $F_s = -kx$ |
| **空气阻力** | $\vec{F}_D$ | 与速度方向相反 | $F_D \propto v$ 或 $v^2$ |

### 二、自由体图（Free Body Diagram, FBD）

#### 2.2.2 FBD 作图步骤

> **自由体图** 是将研究对象从周围环境中隔离出来，画出所有作用在其上的外力。

| 步骤 | 操作 |
|:--:|:--|
| **1** | 选定研究对象（系统） |
| **2** | 将物体画成一个点或简单图形 |
| **3** | 识别所有 **外力**（重力、法向力、摩擦力、张力等） |
| **4** | 从物体中心画出各力的矢量箭头，标注符号 |
| **5** | 建立合适的坐标系，分解不在坐标轴上的力 |

> ⚠️ **常见错误**：在 FBD 中画了"惯性力"、"加速度"或"运动方向"——这些都是 **不画** 的！

#### 2.2.3 🧪 推导 1：斜面上物体的受力分析

**题目**：一个质量为 $m$ 的物体静止在倾角为 $\theta$ 的粗糙斜面上，推导其所受各力的表达式。

**推导**：

**Step 1**：选择物体为研究对象

**Step 2**：画出 FBD，受力有：
- 重力 $\vec{F}_g = mg$ 竖直向下
- 法向力 $\vec{N}$ 垂直于斜面向上
- 静摩擦力 $\vec{f}_s$ 沿斜面向上（阻止下滑）

**Step 3**：选择坐标系——通常选择沿斜面和垂直斜面方向

**Step 4**：分解重力

$$
F_{g\parallel} = mg\sin\theta \quad\text{（沿斜面分量，向下）}
$$
$$
F_{g\perp} = mg\cos\theta \quad\text{（垂直斜面分量）}
$$

**Step 5**：列平衡方程

垂直斜面方向（无运动）：$N - mg\cos\theta = 0$ ⇒ $N = mg\cos\theta$

沿斜面方向（静止）：$f_s - mg\sin\theta = 0$ ⇒ $f_s = mg\sin\theta$

> 💡 **FBD 的价值**：将物理问题转化为数学方程，是解决力学问题的核心技能！

#### 2.2.4 🧪 推导 2：连接体系统的 FBD 分析

**题目**：两个物体 $m_1$ 和 $m_2$ 通过轻绳连接，$m_1$ 放在光滑水平桌面上，$m_2$ 悬挂在桌边。分析系统的受力。

**推导**：

分别对 $m_1$ 和 $m_2$ 画 FBD：

**$m_1$ 的受力**：
- 重力 $m_1g$ 向下
- 法向力 $N$ 向上（$N = m_1g$，竖直方向平衡）
- 张力 $T$ 向右（绳子拉动）

**$m_2$ 的受力**：
- 重力 $m_2g$ 向下
- 张力 $T$ 向上

列方程（设 $m_2$ 向下为正方向）：

对 $m_1$（水平方向）：$T = m_1 a$
对 $m_2$（竖直方向）：$m_2g - T = m_2 a$

联立解得：

$$
a = \frac{m_2}{m_1 + m_2} g, \quad T = \frac{m_1 m_2}{m_1 + m_2} g
$$

> ⭐ **关键思想**：连接体中张力处处相等（轻绳、无摩擦滑轮），但不同物体的加速度大小相同。

#### 2.2.5 🧪 例题 1：斜面上的物体

**题目**：一个 $5\ \text{kg}$ 的物体静止在 $30^\circ$ 的斜面上。求法向力和静摩擦力的大小。（$g = 10\ \text{m/s}^2$）

**解答**：

$$
N = mg\cos\theta = 5 \times 10 \times \cos 30^\circ = 50 \times \frac{\sqrt{3}}{2} \approx 43.3\ \text{N}
$$

$$
f_s = mg\sin\theta = 5 \times 10 \times \sin 30^\circ = 50 \times \frac{1}{2} = 25\ \text{N}
$$

> ✅ 因为物体静止，$f_s = mg\sin\theta$，不需要用到 $\mu_s$ 的信息。

#### 2.2.6 🧪 例题 2：连接体加速度

**题目**：$m_1 = 4\ \text{kg}$，$m_2 = 1\ \text{kg}$，桌面光滑。求加速度和绳子张力。

**解答**：

$$
a = \frac{m_2}{m_1 + m_2} g = \frac{1}{4 + 1} \times 10 = \frac{10}{5} = \mathbf{2\ \text{m/s}^2}
$$

$$
T = m_1 a = 4 \times 2 = \mathbf{8\ N}
$$

---

# 2.3 牛顿第三定律（Newton's Third Law）

## Part A：基础层（AP Physics 1 必备）

### 一、定律内容

> **牛顿第三定律（作用力与反作用力定律）**：
>
> 当物体 A 对物体 B 施加一个力 $\vec{F}_{AB}$ 时，物体 B 同时对物体 A 施加一个大小相等、方向相反的力 $\vec{F}_{BA}$。
>
> $$
> \boxed{\vec{F}_{AB} = -\vec{F}_{BA}}
> $$

| 关键点 | 说明 |
|:--|:--|
| **大小相等** | $|\vec{F}_{AB}| = |\vec{F}_{BA}|$ |
| **方向相反** | $\vec{F}_{AB}$ 与 $\vec{F}_{BA}$ 的方向相反 |
| **同一直线** | 两力沿同一直线 |
| **作用在不同物体上** | ⚠️ 这是与平衡力最本质的区别！ |
| **同时产生、同时消失** | 作用力与反作用力成对出现 |

> ⚠️ **AP 常见错误**：作用力与反作用力 **不会抵消**，因为它们作用在 **不同** 的物体上！

### 二、作用力-反作用力 vs 平衡力

| 对比项 | 作用力与反作用力 | 平衡力 |
|:--|:--|:--|
| 作用对象 | **两个不同** 物体 | **同一个** 物体 |
| 大小关系 | 相等 | 相等 |
| 方向关系 | 相反 | 相反 |
| 能否抵消 | ❌ 不能（作用在不同物体） | ✅ 能（作用在同一物体） |
| 性质 | 同一性质（如都是重力或都是弹力） | 可以是不同性质的力 |

#### 2.3.1 🧪 推导 1：人推墙的受力分析

**题目**：一个人站在地面上用手推墙，分析所有作用力与反作用力对。

**推导**：

**力的对**：
1. **人推墙的力** $\vec{F}_{person/wall}$（向右）↔ **墙推人的力** $\vec{F}_{wall/person}$（向左）
2. **地球拉人的重力** $\vec{F}_{earth/person}$（向下）↔ **人拉地球的力** $\vec{F}_{person/earth}$（向上）
3. **地面推人的法向力** $\vec{F}_{ground/person}$（向上）↔ **人压地面的力** $\vec{F}_{person/ground}$（向下）

**注意**：
- 墙推人的力（向左）与地面对人的摩擦力（向右）构成 **平衡力**（都作用在人身上）
- 而墙推人的力是人对墙的力的 **反作用力**（作用在不同物体上）

> ⭐ **AP 考点**：题目常常给出一个情境，问"哪个力是XX力的反作用力？"这时要找 **施力者和受力者对调** 的那个力！

#### 2.3.2 🧪 推导 2：马拉车问题——经典第三定律误区

**题目**：马用绳子拉车前进。有人说"马对车的拉力等于车对马的拉力，所以马不可能拉动车"。这个说法错在哪里？

**推导**：

**正确分析**：

马对车的拉力和车对马的拉力是一对 **作用力与反作用力**，大小相等，方向相反。

但 **它们作用在不同的物体上**：
- 马对车的拉力作用在车上
- 车对马的拉力作用在马上

**车为什么能前进？**

对 **车** 受力分析：马对车的拉力 $T$ 大于地面对车的摩擦力 $f_{car}$，所以车加速前进。

对 **马** 受力分析：地面对马的摩擦力 $f_{horse}$（向前）大于车对马的拉力 $T$，所以马加速前进。

> ⭐ **核心结论**：作用力与反作用力大小相等并不矛盾——车的加速取决于 **车所受的合外力**（拉力 - 摩擦阻力），马的加速取决于 **马所受的合外力**（地面的推力 - 拉力）。

#### 2.3.3 🧪 例题 1：判断作用力与反作用力

**题目**：一本书静止在水平桌面上。以下哪对力是作用力与反作用力？
> 
> A) 书的重力 vs 桌面对书的支持力
> B) 书对桌面的压力 vs 桌面对书的支持力
> C) 书的重力 vs 书对地球的引力
> D) 桌面对书的支持力 vs 书对桌面的压力

**解答**：

选项 A 是 **平衡力**（作用在同一物体上），不是作用力与反作用力。

选项 B 和 D 是 **同一对** 作用力与反作用力（书对桌面施加压力，桌面对书施加支持力）。✅

选项 C 是另一对作用力与反作用力（地球吸引书 vs 书吸引地球）。✅

**答案**：B 和 D（同一对），以及 C ✅

> ⚠️ **AP 陷阱**：题目可能会问"书的重力的反作用力是什么？"——是 **书对地球的引力**，而不是桌面对书的支持力！

#### 2.3.4 🧪 例题 2：碰撞中的第三定律

**题目**：一辆质量为 $1000\ \text{kg}$ 的汽车以 $20\ \text{m/s}$ 的速度追尾一辆质量为 $800\ \text{kg}$ 的静止汽车。碰撞过程中，哪辆车受到的力更大？

**解答**：

根据牛顿第三定律，碰撞时两车之间的作用力是 **大小相等、方向相反** 的。

所以 **两车受到的力一样大**！✅

但两车的 **加速度不同**（因为质量不同）：$a = F/m$，质量小的车加速度更大。

> ⭐ **AP 必考**：碰撞中 $\vec{F}_{12} = -\vec{F}_{21}$，无论质量、速度如何，**力总是大小相等**！

---

# 2.4 牛顿第一定律（惯性）

## Part A：基础层（AP Physics 1 必备）

### 一、定律内容

> **牛顿第一定律（惯性定律）**：
>
> 任何物体都保持静止或匀速直线运动状态，除非作用在其上的合外力迫使它改变这种状态。
>
> $$
> \boxed{\Sigma \vec{F} = 0 \quad\Longleftrightarrow\quad \vec{a} = 0}
> $$

| 概念 | 说明 |
|:--|:--|
| **惯性（Inertia）** | 物体保持原有运动状态的性质 |
| **质量是惯性的量度** | 质量越大，惯性越大，运动状态越难改变 |
| **平衡态** | 静止或匀速直线运动（$\vec{a}=0$） |

> ⚠️ **第一定律 vs 第二定律**：第一定律定义了 **惯性参考系**，并给出了 **力** 的定性定义；第二定律给出了 **力** 的定量度量。

### 二、平衡态的分析

#### 2.4.1 🧪 推导 1：共点力平衡的矢量三角形法

**题目**：一个物体受三个共点力作用处于平衡状态，证明这三个力的矢量可以构成封闭三角形。

**推导**：

由平衡条件：$\vec{F}_1 + \vec{F}_2 + \vec{F}_3 = 0$

移项得：$\vec{F}_1 + \vec{F}_2 = -\vec{F}_3$

将 $\vec{F}_1$ 和 $\vec{F}_2$ 按平行四边形法则合成，其合矢量 $\vec{F}_{12} = \vec{F}_1 + \vec{F}_2$ 应与 $\vec{F}_3$ 大小相等、方向相反。

将三个力首尾相连，它们构成一个 **封闭三角形**：

```
    ╱╲
  F₁╱  ╲F₃
  ╱    ╲
  ╲    ╱
  F₂╲  ╱
    ╲╱
```

$$
\vec{F}_1 + \vec{F}_2 + \vec{F}_3 = 0 \quad\Longleftrightarrow\quad \text{矢量首尾相连构成封闭图形}
$$

> 💡 **应用**：利用正弦定理或余弦定理求解未知力的大小和方向。

#### 2.4.2 🧪 推导 2：悬挂物体的平衡分析

**题目**：一个质量为 $m$ 的物体用两根轻绳悬挂在天花板上，两根绳与竖直方向的夹角分别为 $\alpha$ 和 $\beta$。求两根绳中的张力。

**推导**：

**Step 1**：画 FBD，物体受三个力：重力 $mg$ 向下，张力 $T_1$ 沿绳1方向，张力 $T_2$ 沿绳2方向。

**Step 2**：建立坐标系（水平为 $x$，竖直为 $y$），分解各力：

$$
T_{1x} = -T_1\sin\alpha, \quad T_{1y} = T_1\cos\alpha
$$
$$
T_{2x} = T_2\sin\beta, \quad T_{2y} = T_2\cos\beta
$$

**Step 3**：列平衡方程：

水平：$-T_1\sin\alpha + T_2\sin\beta = 0$  ⇒ $T_1\sin\alpha = T_2\sin\beta$

竖直：$T_1\cos\alpha + T_2\cos\beta - mg = 0$

**Step 4**：解方程组：

由水平方程：$T_2 = T_1 \dfrac{\sin\alpha}{\sin\beta}$

代入竖直方程：

$$
T_1\cos\alpha + T_1\frac{\sin\alpha}{\sin\beta}\cos\beta = mg
$$

$$
T_1\left(\cos\alpha + \frac{\sin\alpha\cos\beta}{\sin\beta}\right) = mg
$$

$$
\boxed{T_1 = \frac{mg}{\cos\alpha + \sin\alpha\cot\beta}}, \quad \boxed{T_2 = \frac{mg}{\cos\beta + \sin\beta\cot\alpha}}
$$

当 $\alpha = \beta$ 时，$T_1 = T_2 = \dfrac{mg}{2\cos\alpha}$。

> ⭐ **特殊情况**：两绳对称时，张力相等；角度越大，张力越大。

#### 2.4.3 🧪 例题 1：水平面上的平衡

**题目**：一个 $10\ \text{kg}$ 的箱子静止在水平地面上，一个人用 $40\ \text{N}$ 的水平力推箱子，箱子仍然静止。求地面对箱子的静摩擦力。

**解答**：

箱子静止 ⇒ $\Sigma F_x = 0$

水平方向只有推力和静摩擦力：

$$
40 - f_s = 0 \quad\Rightarrow\quad f_s = \mathbf{40\ N}
$$

> 💡 静摩擦力的大小会随着外力的变化而 **自适应调整**，但有一个上限 $\mu_s N$。

#### 2.4.4 🧪 例题 2：悬挂物体的平衡

**题目**：一个 $5\ \text{kg}$ 的物体悬挂在两根绳子之间，两绳与竖直方向的夹角分别为 $30^\circ$ 和 $60^\circ$。求两绳的张力。（$g = 10\ \text{m/s}^2$）

**解答**：

由对称性公式，$\alpha = 30^\circ$，$\beta = 60^\circ$：

$$
T_1 = \frac{mg}{\cos30^\circ + \sin30^\circ\cot60^\circ} = \frac{50}{\frac{\sqrt{3}}{2} + \frac{1}{2} \cdot \frac{1}{\sqrt{3}}}
$$

$$
T_1 = \frac{50}{\frac{\sqrt{3}}{2} + \frac{1}{2\sqrt{3}}} = \frac{50}{\frac{3+1}{2\sqrt{3}}} = \frac{50}{\frac{4}{2\sqrt{3}}} = \frac{50}{\frac{2}{\sqrt{3}}} = 25\sqrt{3} \approx 43.3\ \text{N}
$$

$$
T_2 = T_1\frac{\sin30^\circ}{\sin60^\circ} = 25\sqrt{3} \times \frac{1/2}{\sqrt{3}/2} = 25\sqrt{3} \times \frac{1}{\sqrt{3}} = 25\ \text{N}
$$

> ✅ 验证：$T_1$ 更大，因为绳1更接近竖直方向（承担更多重量）。

---

# 2.5 牛顿第二定律（Newton's Second Law）

## Part A：基础层（AP Physics 1 必备）

### 一、定律内容

> **牛顿第二定律**：
>
> 物体加速度的大小与所受合外力成正比，与质量成反比，加速度方向与合外力方向相同。
>
> $$
> \boxed{\Sigma \vec{F} = m\vec{a}}
> $$

| 项目 | 说明 |
|:--|:--|
| **矢量性** | $\vec{a}$ 的方向与 $\Sigma \vec{F}$ 的方向相同 |
| **瞬时性** | $\vec{a}$ 与 $\Sigma \vec{F}$ 同时产生、同时变化、同时消失 |
| **独立性** | 各力独立产生加速度，合加速度为各分加速度的矢量和 |
| **单位** | $1\ \text{N} = 1\ \text{kg} \cdot \text{m/s}^2$ |

### 二、应用牛顿第二定律的步骤

| 步骤 | 操作 |
|:--:|:--|
| **1** | 确定研究对象，画出 FBD |
| **2** | 建立合适的坐标系 |
| **3** | 将不在坐标轴上的力分解 |
| **4** | 沿各坐标轴方向写出 $\Sigma F = ma$ |
| **5** | 解方程，检查答案的合理性和单位 |

#### 2.5.1 🧪 推导 1：从动量角度推导牛顿第二定律

**原始表述**：牛顿第二定律最初表述为 **动量变化率** 的形式：

$$
\Sigma \vec{F} = \frac{d\vec{p}}{dt}, \quad \vec{p} = m\vec{v}
$$

**推导**：

$$
\Sigma \vec{F} = \frac{d(m\vec{v})}{dt} = m\frac{d\vec{v}}{dt} + \vec{v}\frac{dm}{dt}
$$

在经典力学中，质量 $m$ 为常数，$\dfrac{dm}{dt} = 0$，所以：

$$
\boxed{\Sigma \vec{F} = m\frac{d\vec{v}}{dt} = m\vec{a}}
$$

> 💡 这个原始形式在 **变质量系统**（如火箭）中仍然适用，而 $F=ma$ 只适用于质量不变的系统！

#### 2.5.2 🧪 推导 2：阿特伍德机的加速度

**题目**：两个质量分别为 $m_1$ 和 $m_2$（$m_1 > m_2$）的物体通过轻绳挂在定滑轮两侧。求系统的加速度和绳子张力。

**推导**：

**Step 1**：分别对 $m_1$ 和 $m_2$ 画 FBD。

**Step 2**：设 $m_1$ 向下运动为正方向（两物体加速度大小相等）。

对 $m_1$：$m_1g - T = m_1 a$
对 $m_2$：$T - m_2g = m_2 a$

**Step 3**：两式相加消去 $T$：

$$
m_1g - m_2g = (m_1 + m_2)a
$$

$$
\boxed{a = \frac{m_1 - m_2}{m_1 + m_2} g}
$$

**Step 4**：代入求张力：

$$
T = m_1(g - a) = m_1\left(g - \frac{m_1 - m_2}{m_1 + m_2}g\right)
$$

$$
\boxed{T = \frac{2m_1 m_2}{m_1 + m_2} g}
$$

> ⭐ **特殊情况**：若 $m_1 = m_2$，则 $a = 0$（平衡）；若 $m_2 = 0$，则 $a = g$（自由落体）。

#### 2.5.3 🧪 推导 3（AP C）：变力作用下的运动

**题目**：一个质量为 $m$ 的物体在变力 $F(t) = F_0(1 - e^{-t})$ 的作用下从静止开始沿 $x$ 轴运动（无摩擦）。求 $v(t)$ 和 $x(t)$。

**推导**：

由牛顿第二定律：

$$
m\frac{dv}{dt} = F_0(1 - e^{-t})
$$

分离变量并积分：

$$
\int_0^v dv = \frac{F_0}{m} \int_0^t (1 - e^{-t})\ dt
$$

$$
v(t) = \frac{F_0}{m} \left[ t + e^{-t} \right]_0^t = \frac{F_0}{m} (t + e^{-t} - 1)
$$

再积分求位置：

$$
x(t) = \int_0^t v(\tau)\ d\tau = \frac{F_0}{m} \int_0^t (\tau + e^{-\tau} - 1)\ d\tau
$$

$$
x(t) = \frac{F_0}{m} \left[ \frac{\tau^2}{2} - \tau - e^{-\tau} \right]_0^t
$$

$$
\boxed{x(t) = \frac{F_0}{m} \left( \frac{t^2}{2} - t - e^{-t} + 1 \right)}
$$

> 💡 当 $t \to \infty$ 时，$F(t) \to F_0$，物体做匀加速运动。

#### 2.5.4 🧪 例题 1：水平面上的加速运动

**题目**：一个 $2\ \text{kg}$ 的物体在水平面上受到 $10\ \text{N}$ 的水平拉力。物体与地面间的动摩擦因数为 $0.2$。求物体的加速度。（$g = 10\ \text{m/s}^2$）

**解答**：

由 FBD分析：
- 水平方向：$F - f_k = ma$
- 竖直方向：$N - mg = 0$ ⇒ $N = mg$

动摩擦力：$f_k = \mu_k N = 0.2 \times 2 \times 10 = 4\ \text{N}$

水平方向：$10 - 4 = 2a$

$$
a = \frac{6}{2} = \mathbf{3\ \text{m/s}^2}
$$

#### 2.5.5 🧪 例题 2：阿特伍德机

**题目**：$m_1 = 3\ \text{kg}$，$m_2 = 1\ \text{kg}$，求加速度和张力。（$g = 10\ \text{m/s}^2$）

**解答**：

$$
a = \frac{m_1 - m_2}{m_1 + m_2}g = \frac{3 - 1}{3 + 1} \times 10 = \frac{2}{4} \times 10 = \mathbf{5\ \text{m/s}^2}
$$

$$
T = \frac{2m_1m_2}{m_1+m_2}g = \frac{2 \times 3 \times 1}{3 + 1} \times 10 = \frac{6}{4} \times 10 = \mathbf{15\ N}
$$

#### 2.5.6 🧪 例题 3（AP C）：变力问题

**题目**：一个 $0.5\ \text{kg}$ 的物体受变力 $F(t) = 4 - 2t\ \text{N}$ 作用，从静止开始运动。求 $t = 3\ \text{s}$ 时的速度。

**解答**：

$$
a(t) = \frac{F(t)}{m} = \frac{4 - 2t}{0.5} = 8 - 4t\ \text{m/s}^2
$$

$$
v(t) = \int_0^t a(\tau)\ d\tau = \int_0^t (8 - 4\tau)\ d\tau = \left[8\tau - 2\tau^2\right]_0^t = 8t - 2t^2
$$

$$
v(3) = 8 \times 3 - 2 \times 9 = 24 - 18 = \mathbf{6\ \text{m/s}}
$$

---

# 2.6 引力（Gravitational Force）

## Part A：基础层（AP Physics 1 必备）

### 一、地表附近的重力

> 在地球表面附近，物体所受重力为：
>
> $$
> \boxed{F_g = mg}
> $$
>
> 其中 $g \approx 9.8\ \text{m/s}^2$ 是重力加速度。

### 二、万有引力定律

> **牛顿万有引力定律**：任意两个质点之间存在相互吸引的力，大小与它们的质量乘积成正比，与距离的平方成反比。
>
> $$
> \boxed{F = G\frac{m_1 m_2}{r^2}}
> $$
>
> 其中 $G = 6.67 \times 10^{-11}\ \text{N} \cdot \text{m}^2/\text{kg}^2$ 是万有引力常量。

| 项目 | 说明 |
|:--|:--|
| 方向 | 沿两质点连线，相互吸引 |
| 适用范围 | 质点、均匀球体（可视为质点） |
| 与质量关系 | 与两物体质量乘积成正比 |
| 与距离关系 | 与距离平方成反比（平方反比律） |

#### 2.6.1 🧪 推导 1：$g$ 随高度变化的公式

**题目**：证明重力加速度 $g$ 随高度 $h$ 的变化关系为 $g(h) = g_0 \left(\dfrac{R}{R+h}\right)^2$。

**推导**：

在地表：$mg_0 = G\dfrac{Mm}{R^2}$ ⇒ $g_0 = \dfrac{GM}{R^2}$

在高度 $h$ 处：$mg(h) = G\dfrac{Mm}{(R+h)^2}$ ⇒ $g(h) = \dfrac{GM}{(R+h)^2}$

两式相除：

$$
\frac{g(h)}{g_0} = \frac{R^2}{(R+h)^2}
$$

$$
\boxed{g(h) = g_0 \left(\frac{R}{R+h}\right)^2}
$$

> 💡 **近似公式**：当 $h \ll R$ 时，由二项式展开：
> $$ g(h) \approx g_0 \left(1 - \frac{2h}{R}\right) $$
> 即高度每升高 $1\ \text{km}$，$g$ 约减少 $0.0031\ \text{m/s}^2$。

#### 2.6.2 🧪 推导 2：匀质球壳内部的引力

**题目**：证明在均匀球壳内部任意一点处，球壳对该点的万有引力合力为零（牛顿球壳定理）。

**推导**：

考虑球壳内一点 P。过 P 点作两条很接近的直线，与球壳交于两个小面元 $A_1$ 和 $A_2$。

由几何关系，两小面元的面积之比为 $(r_1/r_2)^2$，因此质量之比也为 $(r_1/r_2)^2$。

$A_1$ 在 P 点产生的引力：$F_1 = G\dfrac{M_1}{r_1^2}$
$A_2$ 在 P 点产生的引力：$F_2 = G\dfrac{M_2}{r_2^2}$

因为 $\dfrac{M_1}{r_1^2} = \dfrac{M_2}{r_2^2}$（$M_1/M_2 = r_1^2/r_2^2$），所以 $F_1 = F_2$。

两力的方向相反，正好抵消。对整个球壳积分，所有部分都成对抵消，因此 **球壳内任意一点的合引力为零**。

> ⭐ **重要推论**：
> - 在地球内部距地心 $r$ 处，只有半径 $r$ 以内的部分产生引力
> - 若地球密度均匀，地球内部的 $g \propto r$

#### 2.6.3 🧪 推导 3（AP C）：万有引力是保守力

**题目**：证明万有引力是保守力，并推导引力势能表达式。

**推导**：

两个质点间的万有引力 $\vec{F} = -G\dfrac{Mm}{r^2}\hat{r}$（负号表示引力方向指向对方）。

将质点 $m$ 从 $r_1$ 移到 $r_2$，引力做功：

$$
W = \int_{r_1}^{r_2} \vec{F} \cdot d\vec{r} = \int_{r_1}^{r_2} \left(-G\frac{Mm}{r^2}\right) dr
$$

$$
W = -GMm \int_{r_1}^{r_2} r^{-2}\ dr = -GMm \left[-\frac{1}{r}\right]_{r_1}^{r_2} = GMm\left(\frac{1}{r_2} - \frac{1}{r_1}\right)
$$

功只与初末位置有关，与路径无关 ⇒ **万有引力是保守力** ✅

引力势能定义 $U(r) = -\int_{\infty}^r \vec{F} \cdot d\vec{r}$：

$$
U(r) = -\int_{\infty}^r \left(-G\frac{Mm}{r^2}\right) dr = GMm \int_{\infty}^r r^{-2}\ dr
$$

$$
U(r) = GMm \left[-\frac{1}{r}\right]_{\infty}^r = -\frac{GMm}{r}
$$

$$
\boxed{U(r) = -\frac{GMm}{r}}
$$

> ⚠️ **注意**：约定无穷远处势能为零，所以在有限距离处引力势能为 **负**。

#### 2.6.4 🧪 例题 1：不同高度的重力加速度

**题目**：地球半径 $R \approx 6400\ \text{km}$，地表 $g_0 = 9.8\ \text{m/s}^2$。求：(a) $h = 100\ \text{km}$ 处的 $g$ 值；(b) $h = 1000\ \text{km}$ 处的 $g$ 值。

**解答**：

**(a)** $h = 100\ \text{km}$：

$$
g = g_0\left(\frac{R}{R+h}\right)^2 = 9.8 \times \left(\frac{6400}{6400+100}\right)^2 = 9.8 \times \left(\frac{6400}{6500}\right)^2
$$

$$
g = 9.8 \times (0.9846)^2 = 9.8 \times 0.9694 \approx \mathbf{9.50\ \text{m/s}^2}
$$

**(b)** $h = 1000\ \text{km}$：

$$
g = 9.8 \times \left(\frac{6400}{6400+1000}\right)^2 = 9.8 \times \left(\frac{6400}{7400}\right)^2
$$

$$
g = 9.8 \times (0.8649)^2 = 9.8 \times 0.748 \approx \mathbf{7.33\ \text{m/s}^2}
$$

> 💡 在 $100\ \text{km}$ 高度（约卡门线），$g$ 仅减小约 $3\%$；但在 $1000\ \text{km}$ 高度，$g$ 减小了约 $25\%$。

#### 2.6.5 🧪 例题 2：两个物体之间的万有引力

**题目**：两个 $50\ \text{kg}$ 的人相距 $1\ \text{m}$ 站立。求他们之间的万有引力。

**解答**：

$$
F = G\frac{m_1 m_2}{r^2} = 6.67 \times 10^{-11} \times \frac{50 \times 50}{1^2} = 6.67 \times 10^{-11} \times 2500
$$

$$
F \approx 1.67 \times 10^{-7}\ \text{N}
$$

> 💡 这个力非常小（约等于 $0.017$ 毫克物体的重量），在日常生活中可以忽略不计。

---

# 2.7 静摩擦力与动摩擦力（Static and Kinetic Friction）

## Part A：基础层（AP Physics 1 必备）

### 一、摩擦力概述

> **摩擦力（Friction）** 是两个接触表面之间阻碍相对运动（或运动趋势）的力。

| 类型 | 条件 | 大小 | 方向 |
|:--|:--|:--|:--|
| **静摩擦力** $f_s$ | 物体有相对运动趋势但未滑动 | $f_s \le \mu_s N$ | 与运动趋势相反 |
| **动摩擦力** $f_k$ | 物体正在相对滑动 | $f_k = \mu_k N$ | 与相对运动方向相反 |

#### 2.7.1 🧪 推导 1：静摩擦力的自适应性

**题目**：一个质量为 $m$ 的物体放在水平地面上，用水平力 $F$ 推它。分析静摩擦力随 $F$ 的变化。

**推导**：

当 $F = 0$ 时：$f_s = 0$（无运动趋势）

当 $F$ 从 $0$ 逐渐增大时：$f_s = F$（静摩擦力随之增大以保持平衡）

当 $F$ 增大到 $F_{max} = \mu_s N = \mu_s mg$ 时：静摩擦力达到最大值

当 $F > \mu_s mg$ 时：物体开始滑动，摩擦力变为动摩擦力 $f_k = \mu_k mg$

通常 $\mu_k < \mu_s$，所以 **最大静摩擦力大于动摩擦力**。

```
f
↑
μ_sN ┤    ╱
     │   ╱  ← 静摩擦区
μ_kN ┤  ╱───  ← 动摩擦区
     │ ╱
     │╱
     └─────────→ F
```

> ⭐ **关键理解**：静摩擦力不是固定值，而是一个 **范围**（$0 \le f_s \le \mu_s N$），大小由平衡条件决定！

#### 2.7.2 🧪 推导 2：摩擦角的推导（自锁现象）

**题目**：一个物体放在粗糙水平面上，$\mu_s$ 为静摩擦因数。证明当外力与法线方向的夹角 $\theta$ 满足 $\tan\theta \le \mu_s$ 时，无论外力多大，物体都不会运动（自锁现象）。

**推导**：

设外力 $F$ 与法线方向夹角为 $\theta$（即与水平面夹角为 $90^\circ - \theta$）。

分解外力：
- 水平分量：$F\sin\theta$（使物体运动）
- 竖直分量：$F\cos\theta$（增加正压力）

正压力：$N = mg + F\cos\theta$
最大静摩擦力：$f_{s,max} = \mu_s N = \mu_s(mg + F\cos\theta)$

物体不滑动的条件：$F\sin\theta \le f_{s,max}$

$$
F\sin\theta \le \mu_s(mg + F\cos\theta)
$$

$$
F\sin\theta \le \mu_s mg + \mu_s F\cos\theta
$$

$$
F(\sin\theta - \mu_s\cos\theta) \le \mu_s mg
$$

当 $\sin\theta - \mu_s\cos\theta \le 0$ 即 $\tan\theta \le \mu_s$ 时，左边 $\le 0 \le \mu_s mg$ 恒成立

所以当 $\tan\theta \le \mu_s$ 时，**无论 $F$ 多大**，物体都不会滑动！✅

> ⭐ **自锁条件**：$\theta \le \tan^{-1}(\mu_s)$，其中 $\tan^{-1}(\mu_s)$ 称为 **摩擦角**。

#### 2.7.3 🧪 推导 3：斜面上的临界滑动角（安息角）

**题目**：一个物体放在粗糙斜面上，静摩擦因数为 $\mu_s$。求物体开始滑动的临界角度。

**推导**：

**Step 1**：当斜面倾角 $\theta$ 逐渐增大时，沿斜面的重力分量 $mg\sin\theta$ 增大。

**Step 2**：物体即将滑动时，静摩擦力达到最大值：

$$
f_s = f_{s,max} = \mu_s N = \mu_s mg\cos\theta
$$

**Step 3**：临界条件：$mg\sin\theta_{crit} = \mu_s mg\cos\theta_{crit}$

$$
\boxed{\tan\theta_{crit} = \mu_s \quad\Rightarrow\quad \theta_{crit} = \tan^{-1}(\mu_s)}
$$

> 💡 **安息角**：自然堆积的散料（如沙堆）形成的最大倾角正好等于 $\tan^{-1}(\mu_s)$。这就是为什么沙子堆成的圆锥有固定的最大坡度。

#### 2.7.4 🧪 例题 1：水平面上的摩擦

**题目**：一个 $10\ \text{kg}$ 的箱子放在水平地面上，$\mu_s = 0.5$，$\mu_k = 0.3$。（$g = 10\ \text{m/s}^2$）
(a) 用 $30\ \text{N}$ 的水平力推箱子，摩擦力多大？
(b) 用 $60\ \text{N}$ 的水平力推箱子，摩擦力多大？加速度多大？

**解答**：

最大静摩擦力：$f_{s,max} = \mu_s N = \mu_s mg = 0.5 \times 10 \times 10 = 50\ \text{N}$

**(a)** $F = 30\ \text{N} < 50\ \text{N}$，箱子不动：

$$
f_s = F = \mathbf{30\ \text{N}}
$$

**(b)** $F = 60\ \text{N} > 50\ \text{N}$，箱子滑动：

$$
f_k = \mu_k N = 0.3 \times 100 = \mathbf{30\ \text{N}}
$$

加速度：$F - f_k = ma$ ⇒ $60 - 30 = 10a$

$$
a = \mathbf{3\ \text{m/s}^2}
$$

> ⚠️ **AP 陷阱**：滑动后摩擦力从 $50\ \text{N}$ 降到 $30\ \text{N}$，这就是为什么推动物体后它会"突然"加速！

#### 2.7.5 🧪 例题 2：斜面上的临界角

**题目**：一个物体放在斜面上，$\mu_s = 0.4$。求物体开始滑动的临界角度。

**解答**：

$$
\tan\theta_{crit} = \mu_s = 0.4 \quad\Rightarrow\quad \theta_{crit} = \tan^{-1}(0.4) \approx \mathbf{21.8^\circ}
$$

> 💡 当斜面倾角小于 $21.8^\circ$ 时，物体可以静止在斜面上。

---

# 2.8 弹簧力（胡克定律）

## Part A：基础层（AP Physics 1 必备）

### 一、胡克定律

> **胡克定律**：在弹性限度内，弹簧的弹力与形变量成正比，方向与形变方向相反。
>
> $$
> \boxed{F_s = -kx}
> $$
>
> 其中 $k$ 为弹簧的 **劲度系数**（单位 $\text{N/m}$），$x$ 为 **形变量**（伸长或压缩的长度）。

| 项目 | 说明 |
|:--|:--|
| **方向** | 总是指向平衡位置（恢复力） |
| **性质** | 线性恢复力 |
| **适用范围** | 弹性限度以内 |

#### 2.8.1 🧪 推导 1：弹簧串联与并联的等效劲度系数

**题目**：两弹簧的劲度系数分别为 $k_1$ 和 $k_2$，求串联和并联时的等效劲度系数。

**推导**：

**串联**：两弹簧首尾相连

设系统受拉力 $F$，两弹簧伸长量分别为 $x_1$ 和 $x_2$。

$$
F = k_1 x_1 = k_2 x_2 \quad\Rightarrow\quad x_1 = \frac{F}{k_1},\ x_2 = \frac{F}{k_2}
$$

总伸长量 $x = x_1 + x_2 = F\left(\frac{1}{k_1} + \frac{1}{k_2}\right)$

等效劲度系数 $k_{eq}$ 满足 $F = k_{eq} x$：

$$
\frac{1}{k_{eq}} = \frac{1}{k_1} + \frac{1}{k_2} \quad\Rightarrow\quad \boxed{k_{eq} = \frac{k_1 k_2}{k_1 + k_2}}
$$

> 💡 串联弹簧的等效劲度系数小于任何一个分弹簧的劲度系数。

**并联**：两弹簧并排放置，两端固定

两弹簧伸长量相同 $x_1 = x_2 = x$。

合力 $F = F_1 + F_2 = k_1 x + k_2 x = (k_1 + k_2)x$

$$
\boxed{k_{eq} = k_1 + k_2}
$$

> 💡 并联弹簧的等效劲度系数大于任何一个分弹簧的劲度系数。

#### 2.8.2 🧪 推导 2：弹簧-质量系统的振动周期

**题目**：一个质量为 $m$ 的物体连在劲度系数为 $k$ 的轻弹簧上，放在光滑水平面上。证明其做简谐振动并求周期。

**推导**：

由胡克定律 $F = -kx$，由牛顿第二定律：

$$
-kx = m\frac{d^2x}{dt^2}
$$

$$
\frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

这是简谐振动的微分方程，令 $\omega = \sqrt{k/m}$：

$$
\frac{d^2x}{dt^2} + \omega^2 x = 0
$$

通解为 $x = A\cos(\omega t + \phi)$。

周期：

$$
\boxed{T = \frac{2\pi}{\omega} = 2\pi\sqrt{\frac{m}{k}}}
$$

> ⭐ **关键结论**：弹簧振子的周期只与质量和劲度系数有关，与振幅无关（等时性）。

#### 2.8.3 🧪 推导 3（AP C）：弹簧势能的积分推导

**题目**：推导弹簧弹性势能的表达式 $U_s = \dfrac{1}{2}kx^2$。

**推导**：

将弹簧从平衡位置拉伸 $x$，外力克服弹力做功：

$$
W = \int_0^x F_{ext}\ dx' = \int_0^x kx'\ dx' = k \int_0^x x'\ dx'
$$

$$
W = k \left[\frac{x'^2}{2}\right]_0^x = \frac{1}{2}kx^2
$$

该功转化为弹簧的弹性势能：

$$
\boxed{U_s = \frac{1}{2}kx^2}
$$

> 💡 弹性势能总是 **非负** 的，无论是拉伸还是压缩，只要 $x \neq 0$，$U_s > 0$。

#### 2.8.4 🧪 例题 1：弹簧的伸长

**题目**：一个 $0.5\ \text{kg}$ 的物体挂在劲度系数 $k = 100\ \text{N/m}$ 的弹簧下端。求弹簧的伸长量。（$g = 10\ \text{m/s}^2$）

**解答**：

平衡时：$mg = kx$

$$
x = \frac{mg}{k} = \frac{0.5 \times 10}{100} = \frac{5}{100} = \mathbf{0.05\ \text{m} = 5\ \text{cm}}
$$

#### 2.8.5 🧪 例题 2：弹簧串并联

**题目**：两个弹簧的劲度系数分别为 $k_1 = 200\ \text{N/m}$ 和 $k_2 = 300\ \text{N/m}$。求：(a) 串联的等效劲度系数；(b) 并联的等效劲度系数。

**解答**：

**(a)** 串联：

$$
k_{eq} = \frac{k_1 k_2}{k_1 + k_2} = \frac{200 \times 300}{200 + 300} = \frac{60000}{500} = \mathbf{120\ \text{N/m}}
$$

**(b)** 并联：

$$
k_{eq} = k_1 + k_2 = 200 + 300 = \mathbf{500\ \text{N/m}}
$$

---

# 2.9 圆周运动（Circular Motion）

## Part A：基础层（AP Physics 1 必备）

### 一、匀速圆周运动

> **匀速圆周运动** 是物体以恒定速率沿圆周路径的运动。

#### 2.9.1 基本概念

| 物理量 | 符号 | 公式 | 单位 |
|:--|:--|:--|:--:|
| 周期 | $T$ | $T = \dfrac{2\pi r}{v}$ | s |
| 频率 | $f$ | $f = \dfrac{1}{T}$ | Hz |
| 角速度 | $\omega$ | $\omega = \dfrac{2\pi}{T} = 2\pi f$ | rad/s |
| 线速度 | $v$ | $v = \omega r$ | m/s |

#### 2.9.2 🧪 推导 1：向心加速度公式的几何推导

**题目**：推导匀速圆周运动的向心加速度 $a_c = \dfrac{v^2}{r}$。

**推导**：

考虑物体在 $\Delta t$ 时间内从 A 点运动到 B 点，速度方向变化了 $\Delta\theta$。

速度矢量变化 $\Delta\vec{v}$ 的方向指向圆心（当 $\Delta t \to 0$ 时）。

由几何关系：$|\Delta\vec{v}| = v\Delta\theta$（小角度近似）

角速度 $\omega = \dfrac{\Delta\theta}{\Delta t} = \dfrac{v}{r}$

加速度大小：

$$
a_c = \lim_{\Delta t\to 0} \frac{|\Delta\vec{v}|}{\Delta t} = \lim_{\Delta t\to 0} \frac{v\Delta\theta}{\Delta t} = v \cdot \frac{d\theta}{dt} = v\omega = \frac{v^2}{r}
$$

$$
\boxed{a_c = \frac{v^2}{r} = \omega^2 r}
$$

**方向**：指向圆心（向心加速度）。

> ⚠️ **注意**：匀速圆周运动的 **速率不变**，但 **速度方向不断变化**，因此存在 **向心加速度**。

#### 2.9.3 🧪 推导 2：水平弯道的最大安全速度

**题目**：一辆汽车在水平弯道上行驶，弯道半径为 $r$，轮胎与地面的静摩擦因数为 $\mu_s$。求不侧滑的最大安全速度。

**推导**：

汽车转弯时，静摩擦力提供向心力：

$$
f_s = m\frac{v^2}{r}
$$

静摩擦力有上限：$f_s \le f_{s,max} = \mu_s N = \mu_s mg$

因此：

$$
m\frac{v^2}{r} \le \mu_s mg
$$

$$
v^2 \le \mu_s g r
$$

$$
\boxed{v_{max} = \sqrt{\mu_s g r}}
$$

> ⭐ **核心结论**：最大安全速度与 $\sqrt{\mu_s}$、$\sqrt{g}$、$\sqrt{r}$ 成正比。弯道越急（$r$ 越小）或路面越滑（$\mu_s$ 越小），安全速度越小。

#### 2.9.4 🧪 推导 3（AP C）：圆锥摆的周期

**题目**：一个质量为 $m$ 的小球用长为 $L$ 的轻绳悬挂在天花板上，在水平面内做匀速圆周运动，绳与竖直方向夹角为 $\theta$。求小球的运动周期。

**推导**：

**Step 1**：受力分析
- 重力 $mg$ 向下
- 张力 $T$ 沿绳方向

**Step 2**：分解张力
- 竖直方向：$T\cos\theta = mg$（平衡重力）
- 水平方向：$T\sin\theta = m\omega^2 r$（提供向心力）

**Step 3**：由竖直方向得 $T = \dfrac{mg}{\cos\theta}$

**Step 4**：代入水平方向：

$$
\frac{mg}{\cos\theta} \cdot \sin\theta = m\omega^2 r \quad\Rightarrow\quad g\tan\theta = \omega^2 r
$$

**Step 5**：几何关系 $r = L\sin\theta$：

$$
g\tan\theta = \omega^2 L\sin\theta \quad\Rightarrow\quad \omega^2 = \frac{g}{L\cos\theta}
$$

**Step 6**：周期 $T = \dfrac{2\pi}{\omega}$：

$$
\boxed{T = 2\pi\sqrt{\frac{L\cos\theta}{g}}}
$$

> 💡 当 $\theta$ 很小时，$\cos\theta \approx 1$，$T \approx 2\pi\sqrt{L/g}$——接近单摆周期！

#### 2.9.5 🧪 例题 1：水平弯道

**题目**：一辆汽车在半径 $50\ \text{m}$ 的水平弯道上行驶，$\mu_s = 0.8$。求不侧滑的最大速度。（$g = 10\ \text{m/s}^2$）

**解答**：

$$
v_{max} = \sqrt{\mu_s g r} = \sqrt{0.8 \times 10 \times 50} = \sqrt{400} = \mathbf{20\ \text{m/s}\ (72\ \text{km/h})}
$$

#### 2.9.6 🧪 例题 2：竖直平面内的圆周运动（过山车）

**题目**：一个过山车在半径为 $10\ \text{m}$ 的竖直圆轨道上运行。求：(a) 在最高点不脱轨的最小速度；(b) 若在最高点速度为 $15\ \text{m/s}$，轨道对车的支持力（车质量 $500\ \text{kg}$，$g=10\ \text{m/s}^2$）。

**解答**：

**(a)** 在最高点，重力和支持力共同提供向心力：

$$
mg + N = m\frac{v^2}{r}
$$

恰好不脱轨时 $N = 0$：

$$
mg = m\frac{v_{min}^2}{r} \quad\Rightarrow\quad v_{min} = \sqrt{gr} = \sqrt{10 \times 10} = \mathbf{10\ \text{m/s}}
$$

**(b)** $v = 15\ \text{m/s} > v_{min}$：

$$
N = m\frac{v^2}{r} - mg = 500 \times \frac{225}{10} - 500 \times 10 = 500 \times 22.5 - 5000
$$

$$
N = 11250 - 5000 = \mathbf{6250\ N}
$$

> ⚠️ **AP 必考**：竖直圆周运动在最高点的临界条件——$\mathbf{v_{min} = \sqrt{gr}}$！

---

# 2.10 阻力（AP Physics C 独家）

### 一、空气阻力模型

> **阻力（Drag Force）** 是物体在流体中运动时受到的阻碍力。AP Physics C 中主要考虑两种模型：

| 模型 | 公式 | 适用场景 |
|:--|:--|:--|
| **线性阻力** | $F_D = -bv$ | 低速运动、黏滞流体 |
| **二次阻力** | $F_D = -\frac{1}{2}C\rho A v^2$ | 高速运动、空气阻力 |

其中 $b$ 为阻尼系数，$C$ 为阻力系数，$\rho$ 为流体密度，$A$ 为横截面积。

#### 2.10.1 🧪 推导 1：线性阻力下的终端速度

**题目**：一个质量为 $m$ 的物体在竖直下落过程中受到线性阻力 $F_D = -bv$（向上）。求物体的终端速度。

**推导**：

设向下为正方向，物体受重力 $mg$ 向下，阻力 $bv$ 向上。

由牛顿第二定律：

$$
m\frac{dv}{dt} = mg - bv
$$

终端速度是阻力与重力平衡时的速度，即 $\dfrac{dv}{dt} = 0$：

$$
mg - bv_T = 0 \quad\Rightarrow\quad \boxed{v_T = \frac{mg}{b}}
$$

> ⭐ **物理意义**：终端速度与重力成正比，与阻尼系数成反比。在空气中，$b$ 较小的物体（如降落伞）有较小的终端速度。

#### 2.10.2 🧪 推导 2：线性阻力下的速度-时间关系

**题目**：在推导 1 的条件下，物体从静止开始下落。求 $v(t)$ 和 $y(t)$。

**推导**：

由 $m\dfrac{dv}{dt} = mg - bv$，分离变量：

$$
\frac{dv}{g - \frac{b}{m}v} = dt
$$

令 $\tau = m/b$（时间常数），$v_T = mg/b$，则：

$$
\frac{dv}{v_T - v} = \frac{dt}{\tau}
$$

两边积分：$\int_0^v \frac{dv'}{v_T - v'} = \frac{1}{\tau} \int_0^t dt'$

$$
-\ln\left(1 - \frac{v}{v_T}\right) = \frac{t}{\tau}
$$

解得：

$$
\boxed{v(t) = v_T(1 - e^{-t/\tau})}
$$

再积分求位置：

$$
y(t) = \int_0^t v(t')\ dt' = v_T \int_0^t (1 - e^{-t'/\tau})\ dt'
$$

$$
\boxed{y(t) = v_T t - v_T\tau(1 - e^{-t/\tau})}
$$

> 💡 当 $t \to \infty$ 时，$v \to v_T$（达到终端速度），$y \to v_T t - v_T\tau$（匀速下落）。

#### 2.10.3 🧪 推导 3：二次阻力下的终端速度

**题目**：一个质量为 $m$ 的物体在空气中下落，受到二次阻力 $F_D = \frac{1}{2}C\rho A v^2$。求终端速度。

**推导**：

由牛顿第二定律（向下为正）：

$$
m\frac{dv}{dt} = mg - \frac{1}{2}C\rho A v^2
$$

终端速度时 $\dfrac{dv}{dt} = 0$：

$$
mg = \frac{1}{2}C\rho A v_T^2
$$

$$
\boxed{v_T = \sqrt{\frac{2mg}{C\rho A}}}
$$

> ⭐ **与线性阻力的区别**：二次阻力下的终端速度与质量的平方根成正比，与横截面积的平方根成反比。这就是为什么降落伞（增大 $A$）可以显著降低终端速度。

#### 2.10.4 🧪 例题 1（AP C）：终端速度计算

**题目**：一个 $80\ \text{kg}$ 的跳伞员在空气中下落，$C = 1.0$，$\rho_{air} = 1.2\ \text{kg/m}^3$，横截面积 $A = 0.8\ \text{m}^2$（收拢姿态）。求终端速度。

**解答**：

$$
v_T = \sqrt{\frac{2mg}{C\rho A}} = \sqrt{\frac{2 \times 80 \times 10}{1.0 \times 1.2 \times 0.8}} = \sqrt{\frac{1600}{0.96}} = \sqrt{1666.7} \approx \mathbf{40.8\ \text{m/s}\ (约147\ \text{km/h})}
$$

> 💡 打开降落伞后 $A$ 大幅增大，终端速度可降到 $5\text{-}6\ \text{m/s}$，保证安全着陆。

#### 2.10.5 🧪 例题 2（AP C）：线性阻力下的运动

**题目**：一个 $2\ \text{kg}$ 的物体在水中下落，阻尼系数 $b = 10\ \text{N·s/m}$。求：(a) 终端速度；(b) 时间常数；(c) $t = 0.2\ \text{s}$ 时的速度。

**解答**：

**(a)** $v_T = \dfrac{mg}{b} = \dfrac{2 \times 10}{10} = \mathbf{2\ \text{m/s}}$

**(b)** $\tau = \dfrac{m}{b} = \dfrac{2}{10} = \mathbf{0.2\ \text{s}}$

**(c)** $v(0.2) = v_T(1 - e^{-t/\tau}) = 2(1 - e^{-0.2/0.2}) = 2(1 - e^{-1}) = 2(1 - 0.368) = \mathbf{1.26\ \text{m/s}}$

> 💡 经过一个时间常数 $\tau$，速度达到终端速度的 $63.2\%$。

---

# Ch2 综合例题（10题）

---

### 🟢 综合题 1（AP Physics 1 风格）：连接体与摩擦

> 质量 $m_1 = 4\ \text{kg}$ 的物体放在粗糙水平面上（$\mu_k = 0.2$），通过轻绳跨过光滑定滑轮与 $m_2 = 2\ \text{kg}$ 的悬挂物体相连。系统从静止释放。求：
> (a) 系统的加速度
> (b) 绳子的张力
> ($g = 10\ \text{m/s}^2$)

**解答**：

对 $m_1$（水平方向）：$T - f_k = m_1 a$，$f_k = \mu_k m_1 g = 0.2 \times 4 \times 10 = 8\ \text{N}$

对 $m_2$（竖直向下）：$m_2 g - T = m_2 a$

联立：$m_2 g - f_k = (m_1 + m_2)a$

$$
a = \frac{m_2 g - \mu_k m_1 g}{m_1 + m_2} = \frac{2 \times 10 - 8}{4 + 2} = \frac{12}{6} = \mathbf{2\ \text{m/s}^2}
$$

$$
T = m_1 a + f_k = 4 \times 2 + 8 = \mathbf{16\ N}
$$

---

### 🟢 综合题 2（AP Physics 1 风格）：斜面上的连接体

> 两个物体 $m_1 = 3\ \text{kg}$ 和 $m_2 = 5\ \text{kg}$ 通过轻绳连接，跨过光滑定滑轮。$m_1$ 放在 $30^\circ$ 的光滑斜面上，$m_2$ 悬挂在斜面外。求加速度和张力。（$g = 10\ \text{m/s}^2$）

**解答**：

设 $m_2$ 向下运动为正方向。

对 $m_1$（沿斜面向上）：$T - m_1 g\sin\theta = m_1 a$
对 $m_2$（向下）：$m_2 g - T = m_2 a$

联立：$m_2 g - m_1 g\sin\theta = (m_1 + m_2)a$

$$
a = \frac{m_2 g - m_1 g\sin30^\circ}{m_1 + m_2} = \frac{5 \times 10 - 3 \times 10 \times 0.5}{3 + 5} = \frac{50 - 15}{8} = \frac{35}{8} = \mathbf{4.375\ \text{m/s}^2}
$$

$$
T = m_2(g - a) = 5(10 - 4.375) = 5 \times 5.625 = \mathbf{28.125\ N}
$$

---

### 🟢 综合题 3（AP Physics 1 风格）：三力平衡

> 一个 $10\ \text{kg}$ 的物体用两根轻绳悬挂在天花板上。绳 OA 与竖直方向成 $30^\circ$，绳 OB 水平。求两绳的张力。（$g = 10\ \text{m/s}^2$）

**解答**：

水平方向：$T_{OA}\sin30^\circ = T_{OB}$
竖直方向：$T_{OA}\cos30^\circ = mg$

由竖直方向：

$$
T_{OA} = \frac{mg}{\cos30^\circ} = \frac{100}{\sqrt{3}/2} = \frac{200}{\sqrt{3}} \approx \mathbf{115.5\ \text{N}}
$$

由水平方向：

$$
T_{OB} = T_{OA}\sin30^\circ = \frac{200}{\sqrt{3}} \times \frac{1}{2} = \frac{100}{\sqrt{3}} \approx \mathbf{57.7\ \text{N}}
$$

---

### 🟢 综合题 4（AP Physics 1 风格）：汽车加速与摩擦力

> 一辆 $1200\ \text{kg}$ 的汽车从静止开始加速，发动机提供的牵引力为 $3600\ \text{N}$，路面与轮胎的 $\mu_k = 0.3$。求：
> (a) 汽车的加速度
> (b) $5\ \text{s}$ 后的速度
> (c) $5\ \text{s}$ 内的位移
> ($g = 10\ \text{m/s}^2$)

**解答**：

**(a)** 摩擦力 $f_k = \mu_k mg = 0.3 \times 1200 \times 10 = 3600\ \text{N}$

$F_{net} = F - f_k = 3600 - 3600 = 0$ ⇒ $a = \mathbf{0\ \text{m/s}^2}$

> ⚠️ 牵引力刚好等于摩擦力，汽车匀速运动！

**(b)** $v = v_0 + at = 0 + 0 \times 5 = \mathbf{0\ \text{m/s}}$（未运动）

> 等等——牵引力等于摩擦力时，汽车恰好匀速（若初速为零则保持静止）。

实际上，当 $F = f_k$ 时，若从静止开始，需要先克服 $f_s$（最大静摩擦）才能启动。假设 $\mu_s > \mu_k$（通常如此），则实际牵引力需大于最大静摩擦力才能使车启动。

---

### 🟢 综合题 5（AP Physics 1 风格）：爬坡汽车

> 一辆 $1500\ \text{kg}$ 的汽车以 $20\ \text{m/s}$ 的速度沿 $10^\circ$ 的斜坡上坡。发动机提供的牵引力为 $5000\ \text{N}$，阻力（摩擦+空气阻力）为 $800\ \text{N}$。求加速度。（$g = 10\ \text{m/s}^2$）

**解答**：

沿斜坡方向（向上为正）：

$$
F_{net} = F - f - mg\sin\theta
$$

$$
F_{net} = 5000 - 800 - 1500 \times 10 \times \sin10^\circ
$$

$$
F_{net} = 5000 - 800 - 1500 \times 10 \times 0.1736 = 5000 - 800 - 2604 = 1596\ \text{N}
$$

$$
a = \frac{F_{net}}{m} = \frac{1596}{1500} = \mathbf{1.064\ \text{m/s}^2}
$$

---

### 🟢 综合题 6（AP Physics 1 风格）：水平转弯的汽车

> 一辆 $1000\ \text{kg}$ 的汽车以 $15\ \text{m/s}$ 的速度在水平弯道上转弯，弯道半径 $30\ \text{m}$。路面与轮胎的 $\mu_s = 0.7$。问汽车是否会侧滑？

**解答**：

所需向心力：$F_c = m\dfrac{v^2}{r} = 1000 \times \dfrac{15^2}{30} = 1000 \times \dfrac{225}{30} = 7500\ \text{N}$

最大静摩擦力：$f_{s,max} = \mu_s mg = 0.7 \times 1000 \times 10 = 7000\ \text{N}$

因为 $F_c = 7500\ \text{N} > 7000\ \text{N}$，所以 **汽车会侧滑** ❌

> ⚠️ 应减速到 $v_{max} = \sqrt{\mu_s g r} = \sqrt{0.7 \times 10 \times 30} = \sqrt{210} \approx 14.5\ \text{m/s}$ 以下才能安全通过。

---

### 🔵 综合题 7（AP Physics C 风格）：变力作用

> 一个 $2\ \text{kg}$ 的物体在水平面上受变力 $F(t) = 6t - 2\ \text{N}$ 作用（$t$ 以秒计），动摩擦因数 $\mu_k = 0.1$。物体从 $t=0$ 时从静止开始运动。求 $t = 3\ \text{s}$ 时的速度。（$g = 10\ \text{m/s}^2$）

**解答**：

摩擦力恒为 $f_k = \mu_k mg = 0.1 \times 2 \times 10 = 2\ \text{N}$

合外力：$F_{net}(t) = F(t) - f_k = 6t - 2 - 2 = 6t - 4\ \text{N}$

加速度：$a(t) = \dfrac{F_{net}}{m} = \dfrac{6t - 4}{2} = 3t - 2\ \text{m/s}^2$

速度：

$$
v(3) = \int_0^3 a(t)\ dt = \int_0^3 (3t - 2)\ dt = \left[\frac{3}{2}t^2 - 2t\right]_0^3
$$

$$
v(3) = \frac{3}{2} \times 9 - 2 \times 3 = 13.5 - 6 = \mathbf{7.5\ \text{m/s}}
$$

---

### 🔵 综合题 8（AP Physics C 风格）：质心计算

> 一根长度为 $L = 2\ \text{m}$、质量为 $M = 6\ \text{kg}$ 的非均匀细杆沿 $x$ 轴放置，其线密度 $\lambda(x) = 3x\ \text{kg/m}$（$x$ 以米计）。求质心位置。

**解答**：

先验证总质量：

$$
M = \int_0^L \lambda(x)\ dx = \int_0^2 3x\ dx = 3\left[\frac{x^2}{2}\right]_0^2 = 3 \times 2 = 6\ \text{kg} ✅
$$

质心位置：

$$
x_{cm} = \frac{1}{M} \int_0^L x\lambda(x)\ dx = \frac{1}{6} \int_0^2 x \cdot 3x\ dx = \frac{3}{6} \int_0^2 x^2\ dx
$$

$$
x_{cm} = \frac{1}{2} \left[\frac{x^3}{3}\right]_0^2 = \frac{1}{2} \times \frac{8}{3} = \frac{4}{3} \approx \mathbf{1.33\ \text{m}}
$$

> 💡 因为右端密度大，质心偏右（不在几何中心 $1\ \text{m}$ 处）。

---

### 🔵 综合题 9（AP Physics C 风格）：阻力与运动

> 一个 $0.5\ \text{kg}$ 的物体从静止开始在有阻力 $F_D = -bv$（$b = 2\ \text{N·s/m}$）的介质中下落。求：
> (a) 终端速度
> (b) 达到 $90\%$ 终端速度所需时间
> ($g = 10\ \text{m/s}^2$)

**解答**：

**(a)** $v_T = \dfrac{mg}{b} = \dfrac{0.5 \times 10}{2} = \mathbf{2.5\ \text{m/s}}$

**(b)** $v(t) = v_T(1 - e^{-t/\tau})$，$\tau = \dfrac{m}{b} = \dfrac{0.5}{2} = 0.25\ \text{s}$

令 $v = 0.9v_T$：

$$
0.9v_T = v_T(1 - e^{-t/\tau}) \quad\Rightarrow\quad 0.9 = 1 - e^{-t/\tau}
$$

$$
e^{-t/\tau} = 0.1 \quad\Rightarrow\quad -\frac{t}{\tau} = \ln 0.1
$$

$$
t = -\tau \ln 0.1 = 0.25 \times \ln 10 \approx 0.25 \times 2.303 = \mathbf{0.576\ \text{s}}
$$

---

### 🔵 综合题 10（AP Physics C 风格）：弹簧与变力综合

> 一个 $1\ \text{kg}$ 的物体连在劲度系数 $k = 100\ \text{N/m}$ 的轻弹簧上，放在光滑水平面上。物体在 $t = 0$ 时位于 $x = 0.1\ \text{m}$ 处从静止释放（弹簧已被拉伸）。
> (a) 求 $x(t)$ 表达式
> (b) 求第一次经过平衡位置的速度
> (c) 求振动周期

**解答**：

**(a)** 由胡克定律和牛二定律：

$$
-kx = m\frac{d^2x}{dt^2} \quad\Rightarrow\quad \frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

$\omega = \sqrt{k/m} = \sqrt{100/1} = 10\ \text{rad/s}$

初始条件：$x(0) = 0.1\ \text{m}$，$v(0) = 0$

通解：$x(t) = A\cos(\omega t + \phi)$

代入得：$A = 0.1\ \text{m}$，$\phi = 0$

$$
\boxed{x(t) = 0.1\cos(10t)\ \text{m}}
$$

**(b)** 第一次经过平衡位置时 $\cos(10t) = 0$ ⇒ $10t = \pi/2$

速度：$v(t) = -A\omega\sin(\omega t)$

$$
v_{max} = A\omega = 0.1 \times 10 = \mathbf{1\ \text{m/s}}
$$

**(c)** 周期：

$$
T = \frac{2\pi}{\omega} = \frac{2\pi}{10} = \frac{\pi}{5} \approx \mathbf{0.628\ \text{s}}
$$

---

<div align="center">

**📖 AP Physics — Mechanics Ch2: Force & Translational Dynamics**

*Made with ❤️ for AP Physics learners*

</div>

