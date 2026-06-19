<!-- markdownlint-disable MD033 MD041 -->

<div align="center">

# 📚 AP Physics — 功、能与功率

> **Work, Energy & Power — 完整综合版**
>
> 覆盖 AP Physics 1（代数）+ AP Physics C（微积分）全难度层级

[![AP Physics](https://img.shields.io/badge/AP-Physics-001845?style=for-the-badge&logo=apache&logoColor=white)](https://ap.collegeboard.org/)
[![Physics 1](https://img.shields.io/badge/AP%20Physics-1-FF6B35?style=flat-square)]()
[![Physics C](https://img.shields.io/badge/AP%20Physics-C-004E89?style=flat-square)]()

</div>

---

## 📑 目录

- [3.1 功](#31-功work)
- [3.2 动能与功-动能定理](#32-动能与功-动能定理kinetic-energy-and-work-energy-theorem)
- [3.3 势能](#33-势能potential-energy)
- [3.4 机械能守恒](#34-机械能守恒conservation-of-mechanical-energy)
- [3.5 功率](#35-功率power)
- [综合例题](#ch3-综合例题10题)

---

# 3.1 功（Work）

## Part A：基础层（AP Physics 1 必备）

### 一、恒力做功

> **功（Work）** 是力在位移方向上的分量与位移大小的乘积，是能量转移的一种度量。
>
> $$
> \boxed{W = \vec{F} \cdot \Delta\vec{x} = F \Delta x \cos\theta}
> $$
>
> 其中 $\theta$ 是力 $\vec{F}$ 与位移 $\Delta\vec{x}$ 之间的夹角。

| 项目 | 说明 |
|:--|:--|
| 类别 | **标量**——只有大小，没有方向 |
| 单位 | 焦耳（J），$1\ \text{J} = 1\ \text{N} \cdot \text{m}$ |
| 物理含义 | 力在位移方向上的累积效应 |

#### 功的正负

| 情况 | $\theta$ 范围 | 功的正负 | 物理含义 |
|:--|:--:|:--:|:--|
| 力与位移同向 | $\theta = 0^\circ$ | $W > 0$ 正功 | 力对物体做正功，能量传递给物体 |
| 力与位移垂直 | $\theta = 90^\circ$ | $W = 0$ 零功 | 力不做功 |
| 力与位移反向 | $\theta = 180^\circ$ | $W < 0$ 负功 | 力对物体做负功（物体克服该力做功） |

### 二、功的深度理解

#### 2.1 功是能量传递的「货币」

功不是一种「拥有的东西」——它是能量在系统和环境之间**传递的量度**。当力做正功时，能量从施力物体流向受力物体；当力做负功时，能量从受力物体流向施力物体（或转化为热）。

> 🧠 **核心直觉**：功 = 能量交换。$W > 0$ 意味着系统获得能量，$W < 0$ 意味着系统失去能量。

#### 2.2 做功的三个必要条件

力要做功，必须同时满足：

1. **有力的作用**——没有力就没有功
2. **有位移**——有力但没有位移（如推一堵墙），没有做功
3. **力在位移方向有分量**——$\cos\theta \neq 0$，即力不能完全垂直于位移

> ⚠️ 最常见的错误：认为「用力」就等于「做功」。提着箱子站着不动虽然累，但物理学上**没有做功**（位移为零）。

#### 2.3 功与路径——保守力 vs 非保守力

| 力类型 | 功与路径的关系 | 实例 | 是否可以定义势能 |
|:--|:--|:--|:--:|
| **保守力** | 功只与起点和终点有关，与路径无关 | 重力、弹力、静电力 | ✅ 是 |
| **非保守力** | 功依赖于具体路径 | 摩擦力、空气阻力 | ❌ 否 |

> 💡 保守力做功 = 势能减少（$W_c = -\Delta U$）。非保守力做功通常转化为热。

#### 2.4 功的几何解释——$F$-$x$ 图下的面积

在 $F$-$x$ 图中，力曲线与位移轴围成的面积 = 力做的功。恒力下是矩形，变力下需要积分。这一几何视角是理解功-能定理的钥匙。

#### 2.5 功与动能的变化

功-动能定理 $W_{\text{net}} = \Delta K$ 告诉我们：合外力做的总功等于动能的变化。这提供了一个比运动学更通用的分析工具——无需知道加速度的具体过程，只需知道始末状态。

---

#### 3.1.1 🧪 推导 1：恒力做功的矢量形式

**题目**：从定义 $W = \vec{F} \cdot \Delta\vec{x}$ 出发，证明恒力做功与路径无关，只与起点和终点的位置有关。

**推导**：

设力 $\vec{F}$ 为恒力（大小和方向都不变），物体沿任意路径从起点 A 运动到终点 B。

将位移分解为平行于力和垂直于力的分量：

$$
\Delta\vec{x} = \Delta\vec{x}_\parallel + \Delta\vec{x}_\perp
$$

由点积的定义：

$$
W = \vec{F} \cdot \Delta\vec{x} = \vec{F} \cdot (\Delta\vec{x}_\parallel + \Delta\vec{x}_\perp) = \vec{F} \cdot \Delta\vec{x}_\parallel + \vec{F} \cdot \Delta\vec{x}_\perp
$$

由于 $\vec{F} \perp \Delta\vec{x}_\perp$，所以 $\vec{F} \cdot \Delta\vec{x}_\perp = 0$：

$$
W = \vec{F} \cdot \Delta\vec{x}_\parallel = F \cdot |\Delta\vec{x}_\parallel| = F \cdot \Delta x \cos\theta
$$

> 💡 **核心结论**：恒力做功只取决于力的大小、位移的大小以及它们之间的夹角，**与具体的路径形状无关**。这在物理中称为"路径无关性"。

#### 3.1.2 🧪 推导 2：总功等于各力做功的代数和

**题目**：物体同时受到多个恒力 $\vec{F}_1, \vec{F}_2, \dots, \vec{F}_n$ 的作用，证明合外力做的总功等于各力单独做功的代数和。

**推导**：

合外力为 $\vec{F}_{net} = \vec{F}_1 + \vec{F}_2 + \cdots + \vec{F}_n$

合外力做的功：

$$
W_{net} = \vec{F}_{net} \cdot \Delta\vec{x} = (\vec{F}_1 + \vec{F}_2 + \cdots + \vec{F}_n) \cdot \Delta\vec{x}
$$

由点积的分配律：

$$
W_{net} = \vec{F}_1 \cdot \Delta\vec{x} + \vec{F}_2 \cdot \Delta\vec{x} + \cdots + \vec{F}_n \cdot \Delta\vec{x}
$$

$$
\boxed{W_{net} = W_1 + W_2 + \cdots + W_n}
$$

> ⭐ **重要结论**：**总功等于各力做功的代数和**。即使各力方向不同，由于功是标量，直接代数相加即可。这极大简化了多力情况下的功的计算！

#### 3.1.3 🧪 推导 3（AP C）：变力做功的积分形式

**题目**：当力随位置变化时，即 $\vec{F} = \vec{F}(\vec{r})$，推导变力做功的表达式。

**推导**：

将路径分成无数个微小位移微元 $d\vec{r}$。在每个微元上，力可以视为恒力。

微元功：$dW = \vec{F} \cdot d\vec{r}$

总功为所有微元功之和，即沿路径的线积分：

$$
\boxed{W = \int_{A}^{B} \vec{F} \cdot d\vec{r}}
$$

在一维情况下，力沿 $x$ 方向，上式简化为：

$$
\boxed{W = \int_{x_i}^{x_f} F(x)\ dx}
$$

> ⭐ **对比记忆**：
> - 恒力做功：$W = F \Delta x \cos\theta$（简洁的代数式）
> - 变力做功：$W = \displaystyle\int \vec{F} \cdot d\vec{r}$（需要积分）
>
> 恒力做功是变力做功公式中 $\vec{F}$ 为常数时的特例！

#### 3.1.4 🧪 例题 1：恒力做功的计算

**题目**：一个 $10\ \text{kg}$ 的物体在水平面上受到 $50\ \text{N}$ 的水平拉力，移动了 $5\ \text{m}$。物体与地面的动摩擦因数 $\mu_k = 0.3$。求：(a) 拉力做的功；(b) 摩擦力做的功；(c) 总功。（$g = 10\ \text{m/s}^2$）

**解答**：

**(a)** 拉力与位移同向（$\theta = 0^\circ$）：

$$
W_F = F \cdot \Delta x \cdot \cos 0^\circ = 50 \times 5 \times 1 = \mathbf{250\ J}
$$

**(b)** 摩擦力 $f_k = \mu_k mg = 0.3 \times 10 \times 10 = 30\ \text{N}$，摩擦力与位移反向（$\theta = 180^\circ$）：

$$
W_f = f_k \cdot \Delta x \cdot \cos 180^\circ = 30 \times 5 \times (-1) = \mathbf{-150\ J}
$$

**(c)** 总功等于各力做功的代数和：

$$
W_{net} = W_F + W_f = 250 + (-150) = \mathbf{100\ J}
$$

> ✅ 也可以先求合外力：$F_{net} = 50 - 30 = 20\ \text{N}$，$W_{net} = 20 \times 5 = 100\ \text{J}$

#### 3.1.5 🧪 例题 2：斜面上拉力的功

**题目**：一个 $5\ \text{kg}$ 的物体在倾角 $30^\circ$ 的粗糙斜面上，受到沿斜面向上 $60\ \text{N}$ 的拉力，沿斜面上升 $4\ \text{m}$。动摩擦因数 $\mu_k = 0.2$。求各力做的功。（$g = 10\ \text{m/s}^2$）

**解答**：

物体受力：拉力 $F$、重力 $mg$、法向力 $N$、动摩擦力 $f_k$。

**(1)** 拉力 $F = 60\ \text{N}$（与位移同向）：

$$
W_F = F \cdot \Delta x = 60 \times 4 = \mathbf{240\ J}
$$

**(2)** 重力 $mg = 50\ \text{N}$（竖直向下），位移沿斜面向上，重力与位移夹角 $\theta = 120^\circ$：

$$
W_g = mg \cdot \Delta x \cdot \cos 120^\circ = 50 \times 4 \times \left(-\frac{1}{2}\right) = \mathbf{-100\ J}
$$

> 💡 重力做的功也可以写成 $W_g = -mgh = -mg \cdot \Delta x \sin\theta = -50 \times 4 \times 0.5 = -100\ \text{J}$

**(3)** 法向力 $N = mg\cos\theta = 50 \times \frac{\sqrt{3}}{2} \approx 43.3\ \text{N}$，$N \perp \Delta x$：

$$
W_N = 0
$$

**(4)** 动摩擦力 $f_k = \mu_k N = 0.2 \times 43.3 \approx 8.66\ \text{N}$，摩擦力与位移反向：

$$
W_f = f_k \cdot \Delta x \cdot \cos 180^\circ = -8.66 \times 4 \approx \mathbf{-34.6\ J}
$$

**(5)** 总功：

$$
W_{net} = 240 - 100 + 0 - 34.6 = \mathbf{105.4\ J}
$$

---

## Part B：AP Physics C 微积分扩展

#### 3.1.6 🧪 推导 4（AP C）：弹簧弹力做功

**题目**：一个物体连在劲度系数为 $k$ 的轻弹簧上，从 $x_i$ 运动到 $x_f$（以平衡位置为原点）。求弹簧弹力做的功。

**推导**：

弹簧弹力 $F_s = -kx$（胡克定律），方向沿 $x$ 轴。

一维变力做功公式：

$$
W_s = \int_{x_i}^{x_f} F_s(x)\ dx = \int_{x_i}^{x_f} (-kx)\ dx
$$

$$
W_s = -k \int_{x_i}^{x_f} x\ dx = -k \left[\frac{x^2}{2}\right]_{x_i}^{x_f}
$$

$$
\boxed{W_s = -\frac{1}{2}k(x_f^2 - x_i^2)}
$$

> 💡 **物理含义**：
> - 若 $|x_f| > |x_i|$（弹簧被拉得更长或压得更深），$W_s < 0$——弹力做负功
> - 若 $|x_f| < |x_i|$（弹簧回复），$W_s > 0$——弹力做正功

#### 3.1.7 🧪 例题 3（AP C）：弹簧变力做功

**题目**：一个 $2\ \text{kg}$ 的物体连在 $k = 200\ \text{N/m}$ 的轻弹簧上，放在光滑水平面上。将弹簧从平衡位置拉伸 $0.1\ \text{m}$ 后释放。求物体从 $x = 0.1\ \text{m}$ 回到 $x = 0$ 的过程中弹力做的功。

**解答**：

$$
W_s = -\frac{1}{2}k(x_f^2 - x_i^2) = -\frac{1}{2} \times 200 \times (0^2 - 0.1^2)
$$

$$
W_s = -100 \times (-0.01) = \mathbf{1\ J}
$$

> ✅ 弹力做正功 $1\ \text{J}$，将弹簧的弹性势能转化为物体的动能。

---

# 3.2 动能与功-动能定理（Kinetic Energy and Work-Energy Theorem）

## Part A：基础层（AP Physics 1 必备）

### 一、动能

> **动能（Kinetic Energy）** 是物体由于运动而具有的能量。
>
> $$
> \boxed{K = \frac{1}{2}mv^2}
> $$

| 项目 | 说明 |
|:--|:--|
| 类别 | **标量**——只有大小，没有方向 |
| 单位 | 焦耳（J） |
| 性质 | 动能永远 **非负**（$v^2 \ge 0$） |
| 相对性 | 动能大小取决于参考系 |

### 二、动能的深度理解

#### 2.1 动能——运动的能量

动能是标量——只依赖于质量和速率，与运动方向无关。两个质量相同、速率相同但方向相反的物体具有相同的动能。

#### 2.2 动能的物理直觉

| 质量 $m$ | 速度 $v$ | 动能 $K$ | 直觉 |
|:--|:--|:--|:--|
| 翻倍 | 不变 | 翻倍 | 质量越大，能量越多 |
| 不变 | 翻倍 | 4倍！ | $v^2$ 的增长极快 |

> 🧠 速度对动能的影响是平方级别的——高速碰撞比低速碰撞危险得多的根本原因。

#### 2.3 动能定理的威力

功-动能定理 $W_{\text{net}} = \Delta K$ 绕过了加速度和时间——只需始末速度。适用于变力，且是标量方程无需分解矢量。

#### 2.4 动能定理的解题五步法

1. **确定系统** 2. **画受力图** 3. **计算每个力做的功** 4. **求和得到净功** 5. **应用 $W_{\text{net}} = \frac{1}{2}mv_f^2 - \frac{1}{2}mv_i^2$**

---

#### 3.2.1 🧪 推导 1：动能表达式的由来

**题目**：从牛顿第二定律出发，推导动能 $K = \dfrac{1}{2}mv^2$ 的表达式。

**推导**：

设质量为 $m$ 的物体在合外力 $F_{net}$ 作用下沿 $x$ 轴做匀加速直线运动。

由牛顿第二定律：$F_{net} = ma = m\dfrac{dv}{dt}$

合外力做功：

$$
W_{net} = \int_{x_i}^{x_f} F_{net}\ dx = \int_{x_i}^{x_f} m\frac{dv}{dt}\ dx
$$

利用链式法则 $\dfrac{dv}{dt} = \dfrac{dv}{dx} \cdot \dfrac{dx}{dt} = v\dfrac{dv}{dx}$：

$$
W_{net} = \int_{x_i}^{x_f} m v \frac{dv}{dx}\ dx = \int_{v_i}^{v_f} m v\ dv
$$

$$
W_{net} = m \int_{v_i}^{v_f} v\ dv = m\left[\frac{v^2}{2}\right]_{v_i}^{v_f} = \frac{1}{2}mv_f^2 - \frac{1}{2}mv_i^2
$$

定义动能 $K = \dfrac{1}{2}mv^2$，即得功-动能定理。

> 💡 **物理含义**：动能表达式中 $v^2$ 的出现不是偶然的——它源于速度的平方在积分中的自然出现！

### 二、功-动能定理

> **功-动能定理**：合外力对物体做的总功等于物体动能的变化量。
>
> $$
> \boxed{W_{net} = \Delta K = K_f - K_i = \frac{1}{2}mv_f^2 - \frac{1}{2}mv_i^2}
> $$

| 要点 | 说明 |
|:--|:--|
| **标量关系** | 功和动能都是标量，无需考虑方向 |
| **适用范围** | 适用于恒力和变力、直线和曲线运动 |
| **物理含义** | 做功是能量转移的方式，动能的变化量度了总功 |

#### 3.2.2 🧪 推导 2（AP C）：变力下的功-动能定理（一般证明）

**题目**：证明功-动能定理在一般情况下（变力、曲线运动）也成立。

**推导**：

考虑质量为 $m$ 的物体在变力 $\vec{F}(\vec{r})$ 作用下沿任意路径运动。

牛顿第二定律：$\vec{F} = m\dfrac{d\vec{v}}{dt}$

合外力做的功：

$$
W_{net} = \int_{A}^{B} \vec{F} \cdot d\vec{r} = \int_{A}^{B} m\frac{d\vec{v}}{dt} \cdot d\vec{r}
$$

由于 $d\vec{r} = \vec{v}\ dt$：

$$
W_{net} = \int_{t_i}^{t_f} m\frac{d\vec{v}}{dt} \cdot \vec{v}\ dt = \int_{t_i}^{t_f} m \vec{v} \cdot \frac{d\vec{v}}{dt}\ dt
$$

注意到 $\dfrac{d}{dt}(v^2) = \dfrac{d}{dt}(\vec{v} \cdot \vec{v}) = 2\vec{v} \cdot \dfrac{d\vec{v}}{dt}$，所以 $\vec{v} \cdot \dfrac{d\vec{v}}{dt} = \dfrac{1}{2}\dfrac{d}{dt}(v^2)$：

$$
W_{net} = \int_{t_i}^{t_f} \frac{m}{2} \frac{d}{dt}(v^2)\ dt = \frac{m}{2} \int_{v_i^2}^{v_f^2} d(v^2)
$$

$$
\boxed{W_{net} = \frac{1}{2}mv_f^2 - \frac{1}{2}mv_i^2}
$$

> ⭐ **核心结论**：功-动能定理是牛顿第二定律对空间的积分结果，**普适成立**，无论力是恒力还是变力，运动是直线还是曲线！

#### 3.2.3 🧪 推导 3：动能定理在匀加速运动中的验证

**题目**：用匀加速运动的运动学公式验证功-动能定理。

**推导**：

物体做匀加速直线运动，加速度为 $a$，位移为 $\Delta x = \dfrac{v_f^2 - v_i^2}{2a}$。

合外力 $F_{net} = ma$，合外力做功：

$$
W_{net} = F_{net} \cdot \Delta x = ma \cdot \frac{v_f^2 - v_i^2}{2a} = \frac{1}{2}mv_f^2 - \frac{1}{2}mv_i^2
$$

✅ **验证成功！** 功-动能定理与运动学公式完全一致！

> 💡 **两种路径得到相同结果**：
> - 路径一（运动学）：先求加速度 → 位移 → 做功
> - 路径二（动能定理）：直接由初末速度求动能变化
>
> 动能定理往往更为便捷！

#### 3.2.4 🧪 例题 1：动能定理的基本应用

**题目**：一个 $0.5\ \text{kg}$ 的物体从静止开始，在 $20\ \text{N}$ 的恒力作用下移动了 $4\ \text{m}$。求物体的末速度。

**解答**：

由动能定理：

$$
W_{net} = F \cdot \Delta x = \frac{1}{2}mv_f^2 - \frac{1}{2}mv_i^2
$$

$v_i = 0$，所以：

$$
20 \times 4 = \frac{1}{2} \times 0.5 \times v_f^2
$$

$$
80 = 0.25 v_f^2 \quad\Rightarrow\quad v_f^2 = 320
$$

$$
v_f = \sqrt{320} = 8\sqrt{5} \approx \mathbf{17.9\ \text{m/s}}
$$

> ✅ 用运动学验证：$a = F/m = 40\ \text{m/s}^2$，$v_f^2 = 2a\Delta x = 2 \times 40 \times 4 = 320$，$v_f \approx 17.9\ \text{m/s}$

#### 3.2.5 🧪 例题 2：含摩擦的动能定理应用

**题目**：一个 $2\ \text{kg}$ 的物体以 $10\ \text{m/s}$ 的初速度在粗糙水平面上滑行，$\mu_k = 0.4$。求物体滑行的距离。（$g = 10\ \text{m/s}^2$）

**解答**：

物体受摩擦力 $f_k = \mu_k mg = 0.4 \times 2 \times 10 = 8\ \text{N}$（与运动方向相反）。

只有摩擦力做功，由动能定理：

$$
W_{net} = -f_k \cdot d = \frac{1}{2}mv_f^2 - \frac{1}{2}mv_i^2
$$

末速度 $v_f = 0$：

$$
-8d = 0 - \frac{1}{2} \times 2 \times 10^2 = -100
$$

$$
d = \frac{100}{8} = \mathbf{12.5\ \text{m}}
$$

> ⚠️ 如果不使用动能定理，需要先求加速度 $a = -\mu_k g = -4\ \text{m/s}^2$，再用 $v_f^2 = v_i^2 + 2a\Delta x$，步骤更多！

#### 3.2.6 🧪 例题 3（AP C）：变力下的动能定理

**题目**：一个 $1\ \text{kg}$ 的物体沿 $x$ 轴运动，受变力 $F(x) = 4x - 2\ \text{N}$（$x$ 以米计）。物体从 $x = 0$ 处从静止开始运动。求物体到达 $x = 3\ \text{m}$ 时的速度。

**解答**：

由动能定理：

$$
W_{net} = \int_0^3 F(x)\ dx = \frac{1}{2}mv_f^2 - 0
$$

$$
\int_0^3 (4x - 2)\ dx = \left[2x^2 - 2x\right]_0^3 = (18 - 6) = 12\ \text{J}
$$

$$
12 = \frac{1}{2} \times 1 \times v_f^2 \quad\Rightarrow\quad v_f^2 = 24
$$

$$
v_f = \sqrt{24} = 2\sqrt{6} \approx \mathbf{4.90\ \text{m/s}}
$$

---

# 3.3 势能（Potential Energy）

## Part A：基础层（AP Physics 1 必备）

### 一、保守力与势能

> **保守力（Conservative Force）**：做功与路径无关，只与起点和终点位置有关的力。
>
> 对于保守力，可以定义 **势能（Potential Energy）** $U$，满足：
>
> $$
> \boxed{W_{cons} = -\Delta U = -(U_f - U_i)}
> $$
>
> 即 **保守力做的功等于势能减少量**。

| 常见保守力 | 对应的势能 |
|:--|:--|
| 重力（近地表） | 重力势能 $U_g = mgh$ |
| 万有引力 | 引力势能 $U_g = -\dfrac{GMm}{r}$ |
| 弹簧弹力 | 弹性势能 $U_s = \dfrac{1}{2}kx^2$ |

| 非保守力 | 特点 |
|:--|:--|
| 摩擦力、空气阻力 | 做功与路径有关，不能定义势能 |

### 二、保守力与非保守力的深度辨析

#### 2.1 保守力的数学定义（🟣 C 版）

保守力 $F$ 满足 $\oint \vec{F} \cdot d\vec{r} = 0$（沿任意闭合路径做功为零）。等价地，存在势能函数 $U$ 使得 $\vec{F} = -\nabla U$。

#### 2.2 为什么摩擦力不是保守力？

摩擦力始终与运动方向相反——沿闭合路径走一圈，摩擦力始终做负功，总功不为零。因此摩擦力没有对应的「摩擦势能」。

#### 2.3 势能零点的选择

| 势能类型 | 零势能点 | 是否可以任意选 |
|:--|:--|:--:|
| 重力势能 $mgy$ | $y = 0$ | ✅ 任意 |
| 弹性势能 $\frac{1}{2}kx^2$ | $x = 0$（自然长度） | ❌ 固定 |
| 万有引力势能 $-\frac{GMm}{r}$ | $r \to \infty$ | ❌ 约定无穷远为零 |

> ⚠️ 只有势能**差**有物理意义——零势能点只是计算方便的参考。

---

#### 3.3.1 🧪 推导 1：重力势能的表达式

**题目**：证明重力是保守力，并推导重力势能 $U_g = mgh$。

**推导**：

**Step 1**：证明重力做功与路径无关

考虑物体从 A 到 B 沿任意路径运动，重力 $\vec{F}_g = -mg\hat{j}$（向下）。

重力做功：

$$
W_g = \int_A^B \vec{F}_g \cdot d\vec{r} = \int_A^B (-mg\hat{j}) \cdot (dx\hat{i} + dy\hat{j} + dz\hat{k})
$$

$$
W_g = \int_A^B -mg\ dy = -mg \int_{y_A}^{y_B} dy = -mg(y_B - y_A)
$$

功只与起点和终点的 $y$ 坐标有关，与路径无关！✅ **重力是保守力**。

**Step 2**：定义重力势能

设参考零势面在 $y = 0$ 处（即 $U(0) = 0$），由 $W_g = -\Delta U$：

$$
W_g = -(U_B - U_A) = U_A - U_B
$$

取 $y_A = h$，$y_B = 0$，则 $U_B = 0$：

$$
U_A = W_g = -mg(0 - h) = mgh
$$

所以重力势能表达式为：

$$
\boxed{U_g = mgh}
$$

其中 $h$ 是物体相对于参考零势面的高度。

> ⚠️ **注意事项**：
> - 重力势能的大小是 **相对的**——取决于零势面的选择
> - 重力势能的变化是 **绝对的**——与零势面选择无关
> - 重力势能属于 **物体-地球系统**，而非单独属于物体

#### 3.3.2 🧪 推导 2：弹性势能的表达式

**题目**：证明弹簧弹力是保守力，并推导弹性势能 $U_s = \dfrac{1}{2}kx^2$。

**推导**：

**Step 1**：弹簧弹力 $F_s = -kx$，沿 $x$ 轴方向。

弹力做功：

$$
W_s = \int_{x_i}^{x_f} F_s\ dx = \int_{x_i}^{x_f} (-kx)\ dx = -\frac{1}{2}k(x_f^2 - x_i^2)
$$

功只与起点和终点的 $x$ 坐标有关，与路径无关！✅ **弹簧弹力是保守力**。

**Step 2**：定义弹性势能

设平衡位置 $x = 0$ 处势能为零（$U(0) = 0$），由 $W_s = -\Delta U$：

$$
W_s = -\frac{1}{2}k(x_f^2 - x_i^2) = -(U_f - U_i)
$$

取 $x_i = 0$（$U_i = 0$），$x_f = x$：

$$
U_s = -W_s = \frac{1}{2}kx^2
$$

$$
\boxed{U_s = \frac{1}{2}kx^2}
$$

> 💡 **弹性势能的特点**：
> - 总是 **非负** 的（$x^2 \ge 0$）
> - 无论是拉伸（$x > 0$）还是压缩（$x < 0$），弹性势能都为正
> - 在平衡位置 $x = 0$ 处弹性势能为零

#### 3.3.3 🧪 推导 3（AP C）：万有引力势能

**题目**：证明万有引力是保守力，并推导引力势能 $U(r) = -\dfrac{GMm}{r}$。

**推导**：

**Step 1**：万有引力 $\vec{F} = -G\dfrac{Mm}{r^2}\hat{r}$（负号表示吸引力，方向指向原点）。

万有引力做功：

$$
W = \int_{r_i}^{r_f} \vec{F} \cdot d\vec{r} = \int_{r_i}^{r_f} \left(-G\frac{Mm}{r^2}\right) dr
$$

$$
W = -GMm \int_{r_i}^{r_f} r^{-2}\ dr = -GMm\left[-\frac{1}{r}\right]_{r_i}^{r_f} = GMm\left(\frac{1}{r_f} - \frac{1}{r_i}\right)
$$

功只与起点和终点的距离 $r$ 有关，与路径无关！✅ **万有引力是保守力**。

**Step 2**：定义引力势能

约定无穷远处势能为零：$U(\infty) = 0$。

由 $W = -\Delta U$，将物体从 $r$ 处移到无穷远：

$$
U(r) - U(\infty) = -\int_r^\infty \vec{F} \cdot d\vec{r}
$$

$$
U(r) = -\int_r^\infty \left(-G\frac{Mm}{r^2}\right) dr = GMm \int_r^\infty r^{-2}\ dr
$$

$$
U(r) = GMm\left[-\frac{1}{r}\right]_r^\infty = -\frac{GMm}{r}
$$

$$
\boxed{U(r) = -\frac{GMm}{r}}
$$

> ⚠️ **关键理解**：
> - 约定无穷远处势能为零，所以有限距离处的引力势能为 **负** 值
> - $U(r)$ 为负代表 **束缚态**——物体需要输入能量才能脱离引力束缚
> - 引力势能随 $r$ 增大而增大（从负值趋近于零）

#### 3.3.4 🧪 推导 4（AP C）：力与势能的关系

**题目**：证明保守力与势能的关系为 $\vec{F} = -\nabla U$（力是势能的负梯度），并在一维情况下简化。

**推导**：

由保守力的定义：$W = -\Delta U = -\int dU$

而微元功 $dW = \vec{F} \cdot d\vec{r}$，所以：

$$
\vec{F} \cdot d\vec{r} = -dU
$$

在三维直角坐标系中，$dU = \dfrac{\partial U}{\partial x}dx + \dfrac{\partial U}{\partial y}dy + \dfrac{\partial U}{\partial z}dz$，且 $\vec{F} \cdot d\vec{r} = F_x dx + F_y dy + F_z dz$：

$$
F_x dx + F_y dy + F_z dz = -\left(\frac{\partial U}{\partial x}dx + \frac{\partial U}{\partial y}dy + \frac{\partial U}{\partial z}dz\right)
$$

对比系数得：

$$
F_x = -\frac{\partial U}{\partial x},\quad F_y = -\frac{\partial U}{\partial y},\quad F_z = -\frac{\partial U}{\partial z}
$$

写成矢量形式：

$$
\boxed{\vec{F} = -\nabla U = -\left(\frac{\partial U}{\partial x}\hat{i} + \frac{\partial U}{\partial y}\hat{j} + \frac{\partial U}{\partial z}\hat{k}\right)}
$$

**一维特例**：$F(x) = -\dfrac{dU}{dx}$

> ⭐ **物理含义**：
> - 力指向势能 **下降最快** 的方向（负梯度方向）
> - 势能曲线的斜率（梯度）决定了力的大小和方向
> - 势能局部极小值对应 **稳定平衡**；局部极大值对应 **不稳定平衡**

#### 3.3.5 🧪 例题 1：重力势能的计算

**题目**：一个 $2\ \text{kg}$ 的物体从高度 $10\ \text{m}$ 处自由下落。以地面为零势面，求：(a) 初始重力势能；(b) 下落 $4\ \text{m}$ 后的重力势能；(c) 重力做的功。（$g = 10\ \text{m/s}^2$）

**解答**：

**(a)** $U_i = mgh_i = 2 \times 10 \times 10 = \mathbf{200\ J}$

**(b)** $h_f = 10 - 4 = 6\ \text{m}$：

$$
U_f = mgh_f = 2 \times 10 \times 6 = \mathbf{120\ J}
$$

**(c)** 重力做功等于势能减少量：

$$
W_g = -\Delta U = -(120 - 200) = \mathbf{80\ J}
$$

> ✅ 也可以直接计算：$W_g = mg \cdot \Delta h = 2 \times 10 \times 4 = 80\ \text{J}$

#### 3.3.6 🧪 例题 2：弹性势能的计算

**题目**：一个 $0.3\ \text{kg}$ 的物体连在 $k = 150\ \text{N/m}$ 的轻弹簧上。将弹簧从平衡位置压缩 $0.08\ \text{m}$，求弹性势能。若从该位置释放，物体经过平衡位置时的速率是多少？（忽略摩擦）

**解答**：

**(a)** 弹性势能：

$$
U_s = \frac{1}{2}kx^2 = \frac{1}{2} \times 150 \times (0.08)^2 = 75 \times 0.0064 = \mathbf{0.48\ J}
$$

**(b)** 由机械能守恒（只有保守力做功）：

$$
\frac{1}{2}kx^2 = \frac{1}{2}mv^2
$$

$$
0.48 = \frac{1}{2} \times 0.3 \times v^2 \quad\Rightarrow\quad v^2 = \frac{0.96}{0.3} = 3.2
$$

$$
v = \sqrt{3.2} \approx \mathbf{1.79\ \text{m/s}}
$$

#### 3.3.7 🧪 例题 3（AP C）：万有引力势能的应用

**题目**：一质量为 $m$ 的卫星在距地面高度为 $h$ 的圆轨道上运行。地球质量为 $M$，半径为 $R$。求卫星的引力势能。

**解答**：

卫星距地心距离 $r = R + h$：

$$
U = -\frac{GMm}{r} = -\frac{GMm}{R + h}
$$

> 💡 卫星被"束缚"在地球引力场中，势能为负值。要使卫星完全脱离地球引力（逃逸），需要提供足够的能量使其总能量 $\ge 0$。

---

# 3.4 机械能守恒（Conservation of Mechanical Energy）

## Part A：基础层（AP Physics 1 必备）

### 一、机械能守恒定律

> **机械能（Mechanical Energy）** $E$ 是动能和势能的总和：
>
> $$
> E = K + U
> $$

> **机械能守恒定律**：如果系统内只有保守力做功（没有非保守力做功），则系统的机械能保持不变。
>
> $$
> \boxed{E_i = E_f \quad\Longleftrightarrow\quad K_i + U_i = K_f + U_f}
> $$

| 条件 | 结论 |
|:--|:--|
| 只有保守力做功 | 机械能守恒 $\Delta E = 0$ |
| 有非保守力做功 | 机械能不守恒 $\Delta E = W_{nc}$ |

#### 3.4.1 🧪 推导 1：机械能守恒定律的推导

**题目**：从功-动能定理出发，推导机械能守恒的条件和表达式。

**推导**：

由功-动能定理：$W_{net} = \Delta K$

将总功分为保守力做功 $W_c$ 和非保守力做功 $W_{nc}$：

$$
W_c + W_{nc} = \Delta K
$$

由保守力的性质：$W_c = -\Delta U$

代入得：

$$
-\Delta U + W_{nc} = \Delta K
$$

$$
W_{nc} = \Delta K + \Delta U = \Delta(K + U) = \Delta E
$$

当 **没有非保守力做功** 时（$W_{nc} = 0$）：

$$
\Delta E = 0 \quad\Rightarrow\quad \boxed{K_i + U_i = K_f + U_f}
$$

> ⭐ **核心逻辑链条**：
> $$
> \text{只有保守力做功} \Rightarrow W_{nc} = 0 \Rightarrow \Delta E = 0 \Rightarrow \text{机械能守恒}
> $$

#### 3.4.2 🧪 推导 2（AP C）：机械能守恒是运动方程的一次积分

**题目**：对于一个受保守力 $F(x) = -dU/dx$ 作用的一维运动，证明机械能守恒是从牛顿第二定律导出的一次积分。

**推导**：

由牛顿第二定律：

$$
m\frac{d^2x}{dt^2} = F(x) = -\frac{dU}{dx}
$$

两边乘以 $v = dx/dt$：

$$
m\frac{d^2x}{dt^2} \cdot \frac{dx}{dt} = -\frac{dU}{dx} \cdot \frac{dx}{dt}
$$

左边：$m\frac{dv}{dt} \cdot v = \frac{d}{dt}\left(\frac{1}{2}mv^2\right) = \frac{dK}{dt}$

右边：$-\frac{dU}{dx} \cdot \frac{dx}{dt} = -\frac{dU}{dt}$

所以：

$$
\frac{dK}{dt} = -\frac{dU}{dt} \quad\Rightarrow\quad \frac{d}{dt}(K + U) = 0
$$

$$
\boxed{K + U = \text{常数}}
$$

> ⭐ **深刻理解**：机械能守恒是牛顿第二定律对时间的 **一次积分** 结果。它不包含新的物理，但提供了解决问题的强大工具——允许我们绕过加速度和力的细节，直接建立初末状态的联系！

#### 3.4.3 🧪 推导 3：有非保守力时的机械能变化

**题目**：证明非保守力做的功等于机械能的变化量。

**推导**：

由前面的推导：

$$
W_{nc} = \Delta K + \Delta U = \Delta E
$$

即非保守力做功等于机械能的变化量。

对于摩擦力（典型的非保守力），它总是做负功，导致机械能减少。减少的机械能转化为内能（热能）：

$$
\boxed{W_{nc} = \Delta E = E_f - E_i < 0 \quad\text{（摩擦力使机械能减少）}}
$$

> ⚠️ **注意**：虽然机械能不守恒了，但 **总能量**（机械能 + 内能 + 其他形式能）仍然守恒！

#### 3.4.4 🧪 例题 1：自由落体——机械能守恒

**题目**：一个 $0.5\ \text{kg}$ 的物体从 $20\ \text{m}$ 高处由静止自由下落。用机械能守恒求物体落地时的速度。（$g = 10\ \text{m/s}^2$）

**解答**：

以地面为零势面，只有重力做功（保守力），机械能守恒。

初始：$K_i = 0$，$U_i = mgh = 0.5 \times 10 \times 20 = 100\ \text{J}$

末态：$U_f = 0$，$K_f = \frac{1}{2}mv^2$

由机械能守恒：

$$
K_i + U_i = K_f + U_f
$$

$$
0 + 100 = \frac{1}{2} \times 0.5 \times v^2 + 0
$$

$$
100 = 0.25v^2 \quad\Rightarrow\quad v^2 = 400
$$

$$
v = \mathbf{20\ \text{m/s}}
$$

> ✅ 用运动学验证：$v^2 = 2gh = 2 \times 10 \times 20 = 400$，$v = 20\ \text{m/s}$

#### 3.4.5 🧪 例题 2：摆球的机械能守恒

**题目**：一个摆长为 $L = 2\ \text{m}$ 的单摆，摆球从与竖直方向成 $60^\circ$ 角的位置由静止释放。求摆球经过最低点时的速度。（$g = 10\ \text{m/s}^2$）

**解答**：

以最低点为零势面。只有重力做功，机械能守恒。

初始高度：$h_i = L - L\cos\theta = L(1 - \cos 60^\circ) = 2 \times (1 - 0.5) = 1\ \text{m}$

初始：$K_i = 0$，$U_i = mgh_i$

最低点：$U_f = 0$，$K_f = \frac{1}{2}mv^2$

由机械能守恒：

$$
mgh_i = \frac{1}{2}mv^2
$$

$$
v = \sqrt{2gh_i} = \sqrt{2 \times 10 \times 1} = \sqrt{20} \approx \mathbf{4.47\ \text{m/s}}
$$

> ⭐ **关键**：机械能守恒让我们绕过了复杂的圆周运动向心力分析，直接得到速度！

#### 3.4.6 🧪 例题 3：有摩擦的机械能变化

**题目**：一个 $1\ \text{kg}$ 的物体从 $5\ \text{m}$ 高处沿粗糙滑梯滑下，到达底端时的速度为 $6\ \text{m/s}$。求摩擦力做的功。（$g = 10\ \text{m/s}^2$）

**解答**：

初始：$K_i = 0$，$U_i = mgh = 1 \times 10 \times 5 = 50\ \text{J}$

末态：$K_f = \frac{1}{2}mv^2 = \frac{1}{2} \times 1 \times 36 = 18\ \text{J}$，$U_f = 0$

由 $W_{nc} = \Delta E = (K_f + U_f) - (K_i + U_i)$：

$$
W_{nc} = (18 + 0) - (0 + 50) = \mathbf{-32\ J}
$$

> 💡 摩擦力做了 $-32\ \text{J}$ 的功，这些机械能转化为内能（滑梯和物体发热）。

---

# 3.5 功率（Power）

## Part A：基础层（AP Physics 1 必备）

### 一、平均功率

> **平均功率（Average Power）** 是做功的快慢，等于做功与所用时间的比值。
>
> $$
> \boxed{P_{avg} = \frac{W}{\Delta t}}
> $$

| 项目 | 说明 |
|:--|:--|
| 类别 | **标量** |
| 单位 | 瓦特（W），$1\ \text{W} = 1\ \text{J/s}$ |
| 常用单位 | $1\ \text{hp} = 746\ \text{W}$（马力） |

### 二、功率与速度的关系

#### 3.5.1 🧪 推导 1：功率与速度的关系

**题目**：证明当力 $\vec{F}$ 与速度 $\vec{v}$ 方向相同时，功率 $P = Fv$。

**推导**：

由功率定义：

$$
P = \frac{W}{\Delta t} = \frac{\vec{F} \cdot \Delta\vec{x}}{\Delta t} = \vec{F} \cdot \frac{\Delta\vec{x}}{\Delta t} = \vec{F} \cdot \vec{v}
$$

当 $\vec{F} \parallel \vec{v}$ 时：

$$
\boxed{P = Fv}
$$

> 💡 **物理含义**：功率是力与速度的点积。对于相同的力，速度越大，功率越大；对于相同的速度，力越大，功率越大。

#### 3.5.2 🧪 推导 2（AP C）：瞬时功率

**题目**：推导瞬时功率的表达式 $P = \vec{F} \cdot \vec{v}$。

**推导**：

瞬时功率是平均功率在时间间隔趋近于零时的极限：

$$
P = \lim_{\Delta t \to 0} \frac{W}{\Delta t} = \lim_{\Delta t \to 0} \frac{\vec{F} \cdot \Delta\vec{x}}{\Delta t}
$$

$$
P = \vec{F} \cdot \lim_{\Delta t \to 0} \frac{\Delta\vec{x}}{\Delta t} = \vec{F} \cdot \vec{v}
$$

$$
\boxed{P(t) = \vec{F}(t) \cdot \vec{v}(t)}
$$

或者从功的微元形式 $dW = \vec{F} \cdot d\vec{r}$ 出发：

$$
P = \frac{dW}{dt} = \frac{\vec{F} \cdot d\vec{r}}{dt} = \vec{F} \cdot \frac{d\vec{r}}{dt} = \boxed{\vec{F} \cdot \vec{v}}
$$

> ⭐ **AP C 考点**：当力和速度都随时间变化时，瞬时功率 $P(t) = F(t)v(t)\cos\theta(t)$ 也随时间变化。

#### 3.5.3 🧪 例题 1：平均功率的计算

**题目**：一台起重机在 $5\ \text{s}$ 内将 $500\ \text{kg}$ 的重物匀速提升 $10\ \text{m}$。求起重机的输出功率。（$g = 10\ \text{m/s}^2$）

**解答**：

起重机做功：$W = mgh = 500 \times 10 \times 10 = 50000\ \text{J}$

平均功率：

$$
P = \frac{W}{t} = \frac{50000}{5} = \mathbf{10000\ \text{W} = 10\ \text{kW}}
$$

> ✅ 也可以用力乘以速度：匀速提升 $F = mg = 5000\ \text{N}$，$v = 10/5 = 2\ \text{m/s}$，$P = Fv = 5000 \times 2 = 10000\ \text{W}$

#### 3.5.4 🧪 例题 2：汽车上坡的功率

**题目**：一辆 $1200\ \text{kg}$ 的汽车以 $15\ \text{m/s}$（$54\ \text{km/h}$）的恒定速度沿 $5^\circ$ 的斜坡上坡。发动机需提供多大的功率？（忽略摩擦和空气阻力，$g = 10\ \text{m/s}^2$）

**解答**：

汽车匀速上坡，发动机的牵引力需要克服重力沿斜面的分量：

$$
F = mg\sin\theta = 1200 \times 10 \times \sin 5^\circ
$$

$$
F = 12000 \times 0.0872 \approx 1046\ \text{N}
$$

功率：

$$
P = Fv = 1046 \times 15 \approx \mathbf{15690\ \text{W} \approx 15.7\ \text{kW}}
$$

> 💡 如果考虑摩擦和空气阻力，实际需要的功率会更大。

#### 3.5.5 🧪 例题 3（AP C）：变力变速度的瞬时功率

**题目**：一个 $0.2\ \text{kg}$ 的物体受变力 $F(t) = 2t\ \text{N}$ 作用，从静止开始沿光滑水平面运动。求 $t = 2\ \text{s}$ 时的瞬时功率。

**解答**：

加速度：$a(t) = \dfrac{F(t)}{m} = \dfrac{2t}{0.2} = 10t\ \text{m/s}^2$

速度：$v(t) = \int_0^t a(\tau)\ d\tau = \int_0^t 10\tau\ d\tau = 5t^2\ \text{m/s}$

$t = 2\ \text{s}$ 时：

$$
F(2) = 4\ \text{N}, \quad v(2) = 5 \times 4 = 20\ \text{m/s}
$$

瞬时功率：

$$
P(2) = F(2) \cdot v(2) = 4 \times 20 = \mathbf{80\ W}
$$

---

# Ch3 综合例题（10题）

---

### 🟢 综合题 1（AP Physics 1 风格）：水平拉动物体

> 一个 $4\ \text{kg}$ 的物体在水平面上受到 $30\ \text{N}$ 的水平拉力，从静止开始移动了 $6\ \text{m}$。物体与地面间的动摩擦因数 $\mu_k = 0.25$。求：
> (a) 拉力做的功
> (b) 摩擦力做的功
> (c) 物体的末速度
> ($g = 10\ \text{m/s}^2$)

**解答**：

**(a)** $W_F = F \cdot \Delta x = 30 \times 6 = \mathbf{180\ J}$

**(b)** $f_k = \mu_k mg = 0.25 \times 4 \times 10 = 10\ \text{N}$

$$
W_f = -f_k \cdot \Delta x = -10 \times 6 = \mathbf{-60\ J}
$$

**(c)** 方法一（动能定理）：

$$
W_{net} = 180 - 60 = 120\ \text{J} = \frac{1}{2}mv^2 - 0
$$

$$
v = \sqrt{\frac{2 \times 120}{4}} = \sqrt{60} \approx \mathbf{7.75\ \text{m/s}}
$$

方法二（牛顿定律）：

$$
a = \frac{F - f_k}{m} = \frac{30 - 10}{4} = 5\ \text{m/s}^2
$$

$$
v^2 = 2a\Delta x = 2 \times 5 \times 6 = 60 \quad\Rightarrow\quad v \approx 7.75\ \text{m/s}
$$

> ✅ 两种方法结果一致，但动能定理更直接！

---

### 🟢 综合题 2（AP Physics 1 风格）：自由落体与机械能守恒

> 一个 $0.2\ \text{kg}$ 的球从 $45\ \text{m}$ 高的楼顶由静止释放。不计空气阻力，求：
> (a) 球落地时的速度
> (b) 球下落 $2\ \text{s}$ 时的动能和重力势能
> ($g = 10\ \text{m/s}^2$)

**解答**：

**(a)** 机械能守恒（以地面为零势面）：

$$
mgh = \frac{1}{2}mv^2 \quad\Rightarrow\quad v = \sqrt{2gh} = \sqrt{2 \times 10 \times 45} = \sqrt{900} = \mathbf{30\ \text{m/s}}
$$

**(b)** 下落 $2\ \text{s}$ 时：

速度：$v = gt = 10 \times 2 = 20\ \text{m/s}$

动能：$K = \frac{1}{2}mv^2 = \frac{1}{2} \times 0.2 \times 400 = \mathbf{40\ J}$

下落距离：$h_{drop} = \frac{1}{2}gt^2 = \frac{1}{2} \times 10 \times 4 = 20\ \text{m}$

当前高度：$h = 45 - 20 = 25\ \text{m}$

重力势能：$U = mgh = 0.2 \times 10 \times 25 = \mathbf{50\ J}$

验证机械能守恒：$K + U = 40 + 50 = 90\ \text{J} = mgh_0$ ✅

---

### 🟢 综合题 3（AP Physics 1 风格）：弹簧-摆系统

> 一个 $1\ \text{kg}$ 的物体连在劲度系数 $k = 400\ \text{N/m}$ 的轻弹簧上，放在光滑水平面上。将弹簧压缩 $0.2\ \text{m}$ 后释放。求：
> (a) 最大弹性势能
> (b) 物体经过平衡位置时的最大速度
> (c) 物体在 $x = 0.1\ \text{m}$ 处的速度

**解答**：

**(a)** 最大弹性势能（在 $x = \pm 0.2\ \text{m}$ 处）：

$$
U_{max} = \frac{1}{2}kA^2 = \frac{1}{2} \times 400 \times (0.2)^2 = 200 \times 0.04 = \mathbf{8\ J}
$$

**(b)** 在平衡位置 $x = 0$ 处，势能全部转化为动能：

$$
\frac{1}{2}mv_{max}^2 = \frac{1}{2}kA^2
$$

$$
v_{max} = A\sqrt{\frac{k}{m}} = 0.2 \times \sqrt{\frac{400}{1}} = 0.2 \times 20 = \mathbf{4\ \text{m/s}}
$$

**(c)** 在 $x = 0.1\ \text{m}$ 处，机械能守恒：

$$
\frac{1}{2}kA^2 = \frac{1}{2}kx^2 + \frac{1}{2}mv^2
$$

$$
\frac{1}{2} \times 400 \times 0.04 = \frac{1}{2} \times 400 \times 0.01 + \frac{1}{2} \times 1 \times v^2
$$

$$
8 = 2 + 0.5v^2 \quad\Rightarrow\quad v^2 = 12
$$

$$
v = \sqrt{12} = 2\sqrt{3} \approx \mathbf{3.46\ \text{m/s}}
$$

---

### 🟢 综合题 4（AP Physics 1 风格）：斜面上的机械能守恒

> 一个 $3\ \text{kg}$ 的物体从光滑斜面顶端由静止滑下，斜面高 $4\ \text{m}$、长 $8\ \text{m}$。求：
> (a) 物体到达底端时的速度
> (b) 物体滑过中点时的速度

**解答**：

**(a)** 机械能守恒（斜面光滑，无摩擦）：

$$
mgh = \frac{1}{2}mv^2 \quad\Rightarrow\quad v = \sqrt{2gh} = \sqrt{2 \times 10 \times 4} = \sqrt{80} \approx \mathbf{8.94\ \text{m/s}}
$$

> ⚠️ **注意**：速度与斜面的倾角无关！只与高度差有关！

**(b)** 在中点，高度为 $h/2 = 2\ \text{m}$：

$$
mg\frac{h}{2} = \frac{1}{2}mv_{mid}^2
$$

$$
v_{mid} = \sqrt{gh} = \sqrt{10 \times 4} = \sqrt{40} \approx \mathbf{6.32\ \text{m/s}}
$$

> 💡 中点速度是底端速度的 $1/\sqrt{2}$ 倍，不是一半！

---

### 🟢 综合题 5（AP Physics 1 风格）：弹丸射入弹簧

> 一个 $0.05\ \text{kg}$ 的子弹以 $400\ \text{m/s}$ 的速度射入一个放在光滑水平面上的 $2\ \text{kg}$ 的木块，子弹嵌入木块后与木块一起压缩前方的轻弹簧（$k = 5000\ \text{N/m}$）。求弹簧的最大压缩量。

**解答**：

**Step 1**：子弹射入木块——完全非弹性碰撞（动量守恒）：

$$
m_b v_b = (m_b + m_M)v'
$$

$$
0.05 \times 400 = (0.05 + 2) \times v' \quad\Rightarrow\quad v' = \frac{20}{2.05} \approx 9.76\ \text{m/s}
$$

**Step 2**：木块（含子弹）压缩弹簧——机械能守恒（水平面光滑）：

$$
\frac{1}{2}(m_b + m_M)v'^2 = \frac{1}{2}kx_{max}^2
$$

$$
\frac{1}{2} \times 2.05 \times (9.76)^2 = \frac{1}{2} \times 5000 \times x_{max}^2
$$

$$
x_{max} = \sqrt{\frac{2.05 \times 95.3}{5000}} \approx \sqrt{0.0391} \approx \mathbf{0.198\ \text{m} \approx 19.8\ \text{cm}}
$$

> ⭐ **多阶段问题**：识别每个阶段遵循的守恒律（动量守恒 OR 机械能守恒）是关键！

---

### 🟢 综合题 6（AP Physics 1 风格）：过山车与机械能守恒

> 一个过山车从高度 $H = 30\ \text{m}$ 处由静止开始沿光滑轨道滑下，轨道包含一个半径为 $R = 8\ \text{m}$ 的竖直圆环。求：
> (a) 过山车在圆环最高点的速度
> (b) 过山车在圆环最高点受到轨道的支持力（过山车质量 $m = 500\ \text{kg}$）
> ($g = 10\ \text{m/s}^2$)

**解答**：

**(a)** 以圆环最低点为零势面。机械能守恒：

初始高度 $H = 30\ \text{m}$，圆环最高点高度 $h = 2R = 16\ \text{m}$

$$
mgH = mg(2R) + \frac{1}{2}mv_{top}^2
$$

$$
gH = 2gR + \frac{1}{2}v_{top}^2
$$

$$
v_{top}^2 = 2g(H - 2R) = 2 \times 10 \times (30 - 16) = 2 \times 10 \times 14 = 280
$$

$$
v_{top} = \sqrt{280} \approx \mathbf{16.73\ \text{m/s}}
$$

**(b)** 在最高点，重力与支持力共同提供向心力：

$$
mg + N = m\frac{v_{top}^2}{R}
$$

$$
N = m\left(\frac{v_{top}^2}{R} - g\right) = 500 \times \left(\frac{280}{8} - 10\right) = 500 \times (35 - 10) = \mathbf{12500\ N}
$$

> ⚠️ **AP 常见问题**：验证是否满足不脱轨条件 $v_{top} \ge \sqrt{gR} = \sqrt{80} \approx 8.94\ \text{m/s}$。这里 $16.73 > 8.94$，安全！✅

---

### 🔵 综合题 7（AP Physics C 风格）：变力做功与动能定理

> 一个 $2\ \text{kg}$ 的物体沿 $x$ 轴运动，所受合力 $F(x) = 12x - 3x^2\ \text{N}$（$x$ 以米计）。物体从 $x = 0$ 处从静止开始运动。求：
> (a) 物体到达 $x = 4\ \text{m}$ 时的速度
> (b) 合外力做的总功

**解答**：

**(a)** 由动能定理：

$$
W_{net} = \int_0^4 F(x)\ dx = \frac{1}{2}mv^2
$$

$$
\int_0^4 (12x - 3x^2)\ dx = \left[6x^2 - x^3\right]_0^4 = (96 - 64) = 32\ \text{J}
$$

$$
32 = \frac{1}{2} \times 2 \times v^2 \quad\Rightarrow\quad v^2 = 32
$$

$$
v = \sqrt{32} = 4\sqrt{2} \approx \mathbf{5.66\ \text{m/s}}
$$

**(b)** 总功即为上面计算的 $W_{net} = \mathbf{32\ J}$。

> 💡 如果力是位置 $x$ 的函数，动能定理的积分形式是首选方法。

---

### 🔵 综合题 8（AP Physics C 风格）：功率与变力

> 一辆 $1500\ \text{kg}$ 的电动汽车从静止开始加速，发动机提供的功率恒为 $P = 60\ \text{kW}$。忽略摩擦和空气阻力。求：
> (a) $t = 5\ \text{s}$ 时汽车的速度
> (b) $t = 5\ \text{s}$ 时汽车的加速度
> (c) 汽车能达到的最大速度（若阻力与速度成正比 $f = bv$，$b = 300\ \text{N·s/m}$）

**解答**：

**(a)** 恒定功率条件下，$P = Fv = m\dfrac{dv}{dt}v$，即：

$$
m v \frac{dv}{dt} = P \quad\Rightarrow\quad mv\ dv = P\ dt
$$

积分：

$$
\int_0^v mv\ dv = \int_0^t P\ dt
$$

$$
\frac{1}{2}mv^2 = Pt \quad\Rightarrow\quad v = \sqrt{\frac{2Pt}{m}}
$$

$t = 5\ \text{s}$：

$$
v = \sqrt{\frac{2 \times 60000 \times 5}{1500}} = \sqrt{\frac{600000}{1500}} = \sqrt{400} = \mathbf{20\ \text{m/s}\ (72\ \text{km/h})}
$$

**(b)** 加速度：

由 $P = Fv$ 得 $F = \dfrac{P}{v} = \dfrac{60000}{20} = 3000\ \text{N}$

$$
a = \frac{F}{m} = \frac{3000}{1500} = \mathbf{2\ \text{m/s}^2}
$$

**(c)** 有阻力时，最大速度出现在牵引力等于阻力时：

$$
F = \frac{P}{v} = bv \quad\Rightarrow\quad v_{max} = \sqrt{\frac{P}{b}} = \sqrt{\frac{60000}{300}} = \sqrt{200} \approx \mathbf{14.14\ \text{m/s}}
$$

> ⚠️ 注意：有阻力时的最大速度反而小于无阻力时 $5\ \text{s}$ 的速度，说明阻力不可忽略！

---

### 🔵 综合题 9（AP Physics C 风格）：势能曲线与平衡

> 一个质量为 $m$ 的物体在一维势场 $U(x) = 2x^2 - x^4$（SI 单位）中运动。
> (a) 求力 $F(x)$ 的表达式
> (b) 找出所有平衡位置，并判断其稳定性
> (c) 若物体在 $x = 1$ 处从静止释放，描述其运动

**解答**：

**(a)** 由 $F(x) = -\dfrac{dU}{dx}$：

$$
F(x) = -\frac{d}{dx}(2x^2 - x^4) = -(4x - 4x^3) = 4x^3 - 4x
$$

$$
\boxed{F(x) = 4x(x^2 - 1)}
$$

**(b)** 平衡位置：$F(x) = 0$

$$
4x(x^2 - 1) = 0 \quad\Rightarrow\quad x = 0,\ x = \pm 1
$$

稳定性判断（二阶导数法）：

$$
\frac{d^2U}{dx^2} = \frac{d}{dx}(4x - 4x^3) = 4 - 12x^2
$$

- 在 $x = 0$：$\dfrac{d^2U}{dx^2} = 4 > 0$ ⇒ **稳定平衡** ✅（势能局部极小值）
- 在 $x = \pm 1$：$\dfrac{d^2U}{dx^2} = 4 - 12 = -8 < 0$ ⇒ **不稳定平衡** ❌（势能局部极大值）

**(c)** 在 $x = 1$ 处（不稳定平衡点），$U(1) = 2 - 1 = 1\ \text{J}$。

从 $x = 1$ 静止释放，由于该点是不稳定平衡点，微小的扰动会使物体向 $x < 1$ 方向运动，并最终在 $x = -1$ 和 $x = 1$ 之间振荡（因为 $U(x)$ 在 $x = 0$ 处有势能阱）。

> ⭐ **AP C 重点**：势能曲线的局部极小值对应稳定平衡，局部极大值对应不稳定平衡。物体倾向于在势能极小值附近振荡。

---

### 🔵 综合题 10（AP Physics C 风格）：万有引力与逃逸速度

> 从地面竖直向上发射一枚火箭，地球半径 $R = 6.37 \times 10^6\ \text{m}$，地球质量 $M = 5.97 \times 10^{24}\ \text{kg}$，$G = 6.67 \times 10^{-11}\ \text{N·m}^2/\text{kg}^2$。
> (a) 求火箭的逃逸速度（忽略空气阻力）
> (b) 若火箭以 $\dfrac{1}{2}v_{esc}$ 的速度竖直上抛，求它能达到的最大高度（以地球半径的倍数表示）

**解答**：

**(a)** 逃逸速度：物体从地面出发，刚好能到达无穷远处（$r \to \infty$），且末速度为零。

机械能守恒：

$$
\frac{1}{2}mv_{esc}^2 - \frac{GMm}{R} = 0 + 0
$$

$$
\frac{1}{2}mv_{esc}^2 = \frac{GMm}{R}
$$

$$
v_{esc} = \sqrt{\frac{2GM}{R}}
$$

代入数据：

$$
v_{esc} = \sqrt{\frac{2 \times 6.67 \times 10^{-11} \times 5.97 \times 10^{24}}{6.37 \times 10^6}}
$$

$$
v_{esc} = \sqrt{\frac{7.96 \times 10^{14}}{6.37 \times 10^6}} = \sqrt{1.25 \times 10^8} \approx \mathbf{1.12 \times 10^4\ \text{m/s} \approx 11.2\ \text{km/s}}
$$

**(b)** 初速度 $v_0 = \dfrac{1}{2}v_{esc} = 5.6\ \text{km/s}$。设最大高度为 $h$（距地心 $r = R + h$）。

机械能守恒：

$$
\frac{1}{2}mv_0^2 - \frac{GMm}{R} = 0 - \frac{GMm}{r}
$$

代入 $v_0^2 = \dfrac{1}{4}v_{esc}^2 = \dfrac{GM}{2R}$：

$$
\frac{1}{2}m \cdot \frac{GM}{2R} - \frac{GMm}{R} = -\frac{GMm}{r}
$$

$$
\frac{GMm}{4R} - \frac{GMm}{R} = -\frac{GMm}{r}
$$

$$
-\frac{3GMm}{4R} = -\frac{GMm}{r}
$$

$$
r = \frac{4R}{3} \quad\Rightarrow\quad h = r - R = \frac{4R}{3} - R = \frac{R}{3}
$$

所以最大高度为 $h = \dfrac{R}{3} \approx \mathbf{2123\ \text{km}}$。

> ⭐ **关键理解**：
> - 逃逸速度与物体的质量无关，只与天体的质量和半径有关
> - 以半逃逸速度发射，不能到达无穷远，最大高度仅为 $R/3$
> - 万有引力势能取负值，在机械能守恒计算中要特别注意符号！

