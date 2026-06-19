<!-- markdownlint-disable MD033 MD041 -->

<div align="center">

# 📚 AP Physics — 振动

> **Oscillations — 完整综合版**
>
> 覆盖 AP Physics 1（代数）+ AP Physics C（微积分）全难度层级

[![AP Physics](https://img.shields.io/badge/AP-Physics-001845?style=for-the-badge&logo=apache&logoColor=white)](https://ap.collegeboard.org/)
[![Physics 1](https://img.shields.io/badge/AP%20Physics-1-FF6B35?style=flat-square)]()
[![Physics C](https://img.shields.io/badge/AP%20Physics-C-004E89?style=flat-square)]()

</div>

---

## 📑 目录

- [7.1 定义简谐运动](#71-定义简谐运动defining-shm)
- [7.2 频率与周期](#72-频率与周期frequency-and-period)
- [7.3 表示与分析 SHM](#73-表示与分析-shmrepresenting-and-analyzing-shm)
- [7.4 简谐振子的能量](#74-简谐振子的能量energy-of-the-sho)
- [7.5 单摆与物理摆](#75-单摆与物理摆simple-and-physical-pendulum)
- [综合例题](#ch7-综合例题)

---

# 7.1 定义简谐运动（Defining Simple Harmonic Motion）

## Part A：基础层（AP Physics 1 必备）

### 一、什么是简谐运动

> **简谐运动（Simple Harmonic Motion，简称 SHM）** 是自然界中最基本、最普遍的振动形式。当一个物体所受的恢复力与其偏离平衡位置的位移成正比且方向相反时，物体所做的往复运动就是简谐运动。
>
> **简谐运动的定义性方程**：
> $$
> \boxed{F = -kx}
> $$
> 其中 $k$ 是力常数（劲度系数），$x$ 是偏离平衡位置的位移，负号表示力的方向始终指向平衡位置。

简谐运动在自然界和工程中无处不在——从钟摆的摆动、弹簧振子的振动、吉他的琴弦、到原子间的振动和量子谐振子，SHM 是物理学中最具普遍性的运动模型之一。理解 SHM 不仅是为了通过 AP 考试，更是因为它是连接经典物理与现代物理（量子力学中的谐振子）的桥梁。

### 二、SHM 的三个本质特征

| 特征 | 数学表达 | 物理含义 |
|:--|:--|:--|
| **恢复力与位移成正比** | $F \propto -x$ | 偏离越远，拉回平衡位置的力越大 |
| **加速度与位移成正比且反向** | $a = -\dfrac{k}{m}x$ | 由 $F=ma$ 直接推出 |
| **位移是时间的正弦（或余弦）函数** | $x(t) = A\cos(\omega t + \phi)$ | SHM 的动力学解 |

### 三、SHM 的运动学特征

从 $F = -kx$ 和 $F = ma$ 出发：

$$
ma = -kx \quad \Rightarrow \quad a = -\frac{k}{m}x
$$

这意味着：
- **在最大位移处**（$x = \pm A$）：$a = \mp\frac{k}{m}A$（加速度最大，指向平衡位置）
- **在平衡位置**（$x = 0$）：$a = 0$（加速度为零，但速度最大）
- $a$ 始终与 $x$ 反向——物体总是在加速回到平衡位置

### 四、SHM 与非简谐振动的区别

| 运动类型 | 恢复力 | 方程 | 周期 |
|:--|:--|:--|:--|
| **简谐运动** | $F = -kx$ | 线性 | 与振幅**无关** |
| 非简谐振动 | $F \neq -kx$ | 非线性 | 通常与振幅有关 |

> ⚠️ **重要判定标准**：只有恢复力严格满足 $F = -kx$ 的运动才是 SHM。单摆仅在小角度（$\theta \ll 1$）时近似为 SHM——随着角度增大，偏离越来越显著。

### 五、从动力学方程到运动学解的完整逻辑链

SHM 的逻辑结构是物理学中最优美的推导链之一：

$$
\text{恢复力 } F = -kx \xrightarrow{F=ma} \text{加速度 } a = -\frac{k}{m}x \xrightarrow{a = d^2x/dt^2} \text{微分方程 } \frac{d^2x}{dt^2} + \frac{k}{m}x = 0 \xrightarrow{\text{求解}} \text{正弦/余弦解 } x = A\cos(\omega t + \phi)
$$

这个链条中的每一步都是可逆的——这正是 SHM 理论自洽性的体现。

### 六、SHM 的系统示例

| 系统 | 恢复力 | $k_{\text{eff}}$ | 平衡位置 |
|:--|:--|:--|:--|
| 水平弹簧-质量系统 | $F = -kx$ | $k$ | 弹簧原长处 |
| 竖直弹簧-质量系统 | $F_{\text{net}} = -kx$ | $k$ | $x_0 = mg/k$（拉伸位置） |
| 单摆（小角度） | $F_t = -\dfrac{mg}{L}s$ | $\dfrac{mg}{L}$ | 最低点 |
| 物理摆（小角度） | $\tau = -mgd\,\theta$ | $mgd$（转动） | 最低点 |

---

#### 7.1.1 🧪 推导 1：从 $F = -kx$ 导出 SHM 的加速度特征方程

**推导目标**：证明 SHM 中加速度与位移成正比且反向——$a = -\omega^2 x$，并从中引出角频率 $\omega = \sqrt{k/m}$。

**推导过程**：

**第一步**：由牛顿第二定律和胡克定律联立。

水平光滑面上的弹簧-质量系统（最纯粹的 SHM 模型）。弹簧施加的恢复力为 $F = -kx$。由 $F = ma$：

$$
ma = -kx
$$

$$
a = -\frac{k}{m}x
$$

**第二步**：定义角频率 $\omega$。

令 $\omega^2 = \dfrac{k}{m}$，即：
$$
\boxed{\omega = \sqrt{\frac{k}{m}}}
$$

代入加速度表达式：

$$
\boxed{a = -\omega^2 x}
$$

**第三步**：验证 $\omega$ 的物理含义。

$\omega$ 的单位：$\sqrt{\dfrac{\text{N/m}}{\text{kg}}} = \sqrt{\dfrac{\text{kg·m/s}^2/\text{m}}{\text{kg}}} = \sqrt{\dfrac{1}{\text{s}^2}} = \dfrac{1}{\text{s}} = \text{rad/s}$——正是角频率的单位。

> 💡 **$\omega = \sqrt{k/m}$ 是 SHM 最重要的公式之一**。它表明：劲度系数越大（弹簧越硬），振动越快；质量越大（惯性越大），振动越慢。角频率只取决于系统的固有属性（$k$ 和 $m$），与振幅无关——这是 SHM 最核心的特征。

**代数法验证**（AP Physics 1）：

对于做匀速圆周运动的质点，向心加速度 $a_c = \omega^2 r$，方向指向圆心。将其投影到 $x$ 轴上：$a_x = -\omega^2 x$（负号因为加速度指向原点）。这恰好是 $a = -\omega^2 x$——从而建立起圆周运动投影与 SHM 的等价关系。

---

#### 7.1.2 🧪 推导 2：从 $a = -\omega^2 x$ 导出 SHM 的微分方程与其正弦解

**推导目标**：证明 $x = A\cos(\omega t + \phi)$ 是 $a = -\omega^2 x$ 的解，并由此建立 SHM 的完整数学描述。

**推导过程**：

**第一步**：写出微分方程。

加速度是位移对时间的二阶导数：$a = \dfrac{d^2x}{dt^2}$。代入 $a = -\omega^2 x$：

$$
\frac{d^2x}{dt^2} = -\omega^2 x
$$

整理为标准形式：
$$
\boxed{\frac{d^2x}{dt^2} + \omega^2 x = 0}
$$

这是一个二阶线性常系数齐次微分方程——物理学中最常见也最重要的微分方程之一。

**第二步**：验证 $x = A\cos(\omega t + \phi)$ 是解。

对 $x = A\cos(\omega t + \phi)$ 求一阶导数：
$$
v = \frac{dx}{dt} = -A\omega\sin(\omega t + \phi)
$$

求二阶导数：
$$
a = \frac{d^2x}{dt^2} = -A\omega^2\cos(\omega t + \phi) = -\omega^2 \cdot A\cos(\omega t + \phi) = -\omega^2 x
$$

代入微分方程：$-\omega^2 x + \omega^2 x = 0$ ✓

**第三步**：理解解的物理含义。

- $A$（振幅）：最大位移，由初始条件决定
- $\omega$（角频率）：由系统参数决定（$\omega = \sqrt{k/m}$）
- $\phi$（初相位）：由初始时刻的位置和速度决定
- $T = 2\pi/\omega$（周期）：完成一次完整振动所需的时间

> 💡 **$x = A\cos(\omega t + \phi)$ 中的三个参数各有其物理来源**：$\omega$ 来自系统本身（弹簧的 $k$ 和质量 $m$），$A$ 和 $\phi$ 来自初始条件（你如何启动振动）。这体现了物理学的一个普遍原则：系统的动力学方程决定了运动的形式，初始条件决定了具体的运动。

**🟣 C 版深化——特征方程法**：

微分方程 $\dfrac{d^2x}{dt^2} + \omega^2 x = 0$ 的特征方程为 $r^2 + \omega^2 = 0$，根为 $r = \pm i\omega$。通解为：

$$
x(t) = C_1\cos(\omega t) + C_2\sin(\omega t) = A\cos(\omega t + \phi)
$$

其中 $A = \sqrt{C_1^2 + C_2^2}$，$\phi = \arctan(-C_2/C_1)$。

---

#### 7.1.2b 🧪 推导 3：从能量守恒导出 SHM 的微分方程

**推导目标**：证明能量守恒 $\frac{1}{2}mv^2 + \frac{1}{2}kx^2 = E$ 对时间求导可以导出 SHM 的动力学微分方程——展示能量法与动力学法的等价性。

**推导过程**：

总能量守恒：
$$
\frac{1}{2}mv^2 + \frac{1}{2}kx^2 = E = \text{常数}
$$

对时间 $t$ 求导（使用链式法则，$v = dx/dt$，$a = dv/dt$）：

$$
\frac{d}{dt}\left(\frac{1}{2}mv^2\right) + \frac{d}{dt}\left(\frac{1}{2}kx^2\right) = 0
$$

$$
\frac{1}{2}m \cdot 2v\frac{dv}{dt} + \frac{1}{2}k \cdot 2x\frac{dx}{dt} = 0
$$

$$
mv a + kx v = 0
$$

$$
v(ma + kx) = 0
$$

由于 $v$ 不恒为零（物体在振动），括号内必须为零：

$$
ma + kx = 0 \quad \Rightarrow \quad a = -\frac{k}{m}x = -\omega^2 x
$$

这恰好是 SHM 的加速度特征方程。将 $a = d^2x/dt^2$ 代入即得微分方程：

$$
\boxed{\frac{d^2x}{dt^2} + \omega^2 x = 0}
$$

> 💡 **深刻洞察**：$F = -kx$（动力学）和 $E = K + U = \text{常数}$（能量守恒）不是两个独立的定律——一个是另一个的微分形式。对于保守力系统（如弹簧），力是势能的负梯度 $F = -dU/dx$，$U = \frac{1}{2}kx^2$ 自动给出 $F = -kx$。SHM 的优雅之处在于动力学描述和能量描述完全自洽。

---

#### 7.1.2c 🧪 推导 4：$x = A\sin(\omega t)$ 与 $x = A\cos(\omega t + \phi)$ 的等价性

**推导目标**：证明正弦形式和余弦形式描述的是同一物理运动，只是计时零点的选择不同——并严格展示初相位 $\phi$ 如何从初始条件中产生。

**推导过程**：

余弦形式：$x_1(t) = A\cos(\omega t)$。这意味着 $t = 0$ 时 $x_1(0) = A$（从最大位移释放）。

正弦形式：$x_2(t) = A\sin(\omega t)$。这意味着 $t = 0$ 时 $x_2(0) = 0$（从平衡位置出发，初速度 $v_0 = A\omega$）。

利用三角恒等式 $\cos(\omega t - \pi/2) = \sin(\omega t)$：

$$
x_2(t) = A\sin(\omega t) = A\cos\!\left(\omega t - \frac{\pi}{2}\right)
$$

因此正弦形式只是余弦形式在 $\phi = -\pi/2$ 时的特例。

一般形式 $x = A\cos(\omega t + \phi)$ 涵盖了所有可能的初相位。$t = 0$ 时：

$$
x_0 = A\cos\phi,\quad v_0 = -A\omega\sin\phi
$$

由此可唯一确定 $\phi$（模 $2\pi$）：
$$
\boxed{\tan\phi = -\frac{v_0}{\omega x_0}}
$$

| $\phi$ | 运动描述 | $x_0$ | $v_0$ |
|:--:|:--|:--:|:--:|
| $0$ | 从 $+A$ 释放 | $+A$ | $0$ |
| $\pi/2$ | 过平衡位置向 $-x$ | $0$ | $-A\omega$ |
| $\pi$ | 从 $-A$ 释放 | $-A$ | $0$ |
| $-\pi/2$ | 过平衡位置向 $+x$ | $0$ | $+A\omega$ |

> 💡 **选择余弦还是正弦？** AP 考试中余弦形式更常用（因为 $t=0$ 时从最大位移释放是常见情景），但正弦形式在某些初始条件下更自然（如击打平衡位置的物块使其振动）。无论哪种形式，关键是正确匹配初始条件。

---

#### 7.1.3 🧪 例题 1：判定是否为 SHM

**题目**：判断以下系统中质量为 $m$ 的物体是否做简谐运动。若是，求有效劲度系数 $k_{\text{eff}}$ 和角频率 $\omega$。
(a) 水平光滑面上连接一根弹簧（劲度系数 $k$）的物块
(b) 竖直悬挂在同一根弹簧上的物块（考虑重力）
(c) 连接两根相同弹簧（并联，劲度系数均为 $k$）的物块

**题目分析**：

> SHM 的判定标准：恢复力是否满足 $F = -(\text{常数}) \times (\text{偏离平衡位置的位移})$。关键是找准**平衡位置**——恢复力必须从平衡位置量起。

**解答**：

**(a)** 水平弹簧-质量系统：

平衡位置在弹簧原长处。偏离 $x$ 时，弹簧力 $F = -kx$——直接满足 $F = -kx$ 的形式。

- $k_{\text{eff}} = k$
- $\omega = \sqrt{k/m}$
- ✅ 是 SHM

**(b)** 竖直弹簧-质量系统：

平衡位置：弹簧拉伸 $\Delta y_0 = mg/k$，此时 $k\Delta y_0 = mg$。

取平衡位置为坐标原点，向下为正。物块偏离平衡位置 $y$ 时：
- 弹簧力向上：$F_s = -k(\Delta y_0 + y)$
- 重力向下：$F_g = +mg$

合力：$F_{\text{net}} = -k(\Delta y_0 + y) + mg = -k\Delta y_0 - ky + mg$

由平衡条件 $k\Delta y_0 = mg$，代入：
$$
F_{\text{net}} = -mg - ky + mg = -ky
$$

- **结论**：重力被平衡位置的弹簧拉力抵消，净恢复力仍然满足 $F = -ky$。
- $k_{\text{eff}} = k$，$\omega = \sqrt{k/m}$
- ✅ 是 SHM

> 💡 **重要洞察**：竖直弹簧-质量系统的 SHM 与水平系统完全相同——重力只改变了平衡位置，不影响振动频率。这是 SHM 的一个重要性质：**恒定外力不会改变振动频率**，只会移动平衡位置。

**(c)** 两根相同弹簧并联：

两弹簧伸长量相同（均为 $x$），各自施加力 $-kx$，合力 $F = -2kx$。

- $k_{\text{eff}} = 2k$
- $\omega = \sqrt{2k/m}$
- ✅ 是 SHM

---

#### 7.1.4 🧪 例题 2：从力-位移关系求振动参数

**题目**：一个 $m = 0.50\ \text{kg}$ 的物块在光滑水平面上连接一根弹簧。当物块从平衡位置移动 $0.10\ \text{m}$ 时，弹簧施加 $3.0\ \text{N}$ 的恢复力。求：
(a) 弹簧的劲度系数 $k$
(b) 系统的角频率 $\omega$ 和周期 $T$
(c) 若将弹簧截去一半长度后重新连接，新的角频率是多少？

**题目分析**：

> **已知**：$m = 0.50\ \text{kg}$，$x = 0.10\ \text{m}$，$F = 3.0\ \text{N}$
>
> **求**：$k$、$\omega$、$T$、截半后的 $\omega'$
>
> **策略**：由 $F = -kx$ 求 $k$，再用 $\omega = \sqrt{k/m}$ 和 $T = 2\pi/\omega$。

**解答**：

**(a)** $k = \dfrac{|F|}{|x|} = \dfrac{3.0}{0.10} = \mathbf{30\ \text{N/m}}$

**(b)** $\omega = \sqrt{\dfrac{k}{m}} = \sqrt{\dfrac{30}{0.50}} = \sqrt{60} \approx \mathbf{7.75\ \text{rad/s}}$

$T = \dfrac{2\pi}{\omega} = \dfrac{2\pi}{7.75} \approx \mathbf{0.811\ \text{s}}$

**(c)** 将弹簧截去一半：弹簧的劲度系数与长度成反比（$k \propto 1/L$）。截半后 $k' = 2k = 60\ \text{N/m}$。

$$
\omega' = \sqrt{\frac{k'}{m}} = \sqrt{\frac{60}{0.50}} = \sqrt{120} \approx \mathbf{11.0\ \text{rad/s}}
$$

> 💡 **弹簧截半后 $\omega$ 增大 $\sqrt{2}$ 倍**——更短的弹簧更硬（$k$ 翻倍），振动更快。这个结论可以从弹簧的微观结构理解：截半后每一圈的变形量加倍，因此恢复力加倍。

---

#### 7.1.5 🧪 例题 3：从运动方程反推系统参数

**题目**：一个物体的 SHM 位移方程为 $x(t) = 0.25\cos(4.0t + 0.50)\ \text{m}$。求：
(a) 振幅 $A$、角频率 $\omega$、初相位 $\phi$、周期 $T$、频率 $f$
(b) 该物体的质量 $m$，已知弹簧劲度系数 $k = 32\ \text{N/m}$
(c) $t = 0$ 时物体的位置和速度

**题目分析**：

> 从标准形式 $x = A\cos(\omega t + \phi)$ 中直接读取 $A$、$\omega$、$\phi$。

**解答**：

**(a)** $A = \mathbf{0.25\ \text{m}}$，$\omega = \mathbf{4.0\ \text{rad/s}}$，$\phi = \mathbf{0.50\ \text{rad}}$

$T = \dfrac{2\pi}{\omega} = \dfrac{2\pi}{4.0} \approx \mathbf{1.57\ \text{s}}$

$f = \dfrac{1}{T} \approx \mathbf{0.637\ \text{Hz}}$

**(b)** $\omega = \sqrt{k/m}$ → $m = \dfrac{k}{\omega^2} = \dfrac{32}{16} = \mathbf{2.0\ \text{kg}}$

**(c)** $x(0) = 0.25\cos(0.50) \approx 0.25 \times 0.8776 \approx \mathbf{0.219\ \text{m}}$

$v(0) = -A\omega\sin(\phi) = -0.25 \times 4.0 \times \sin(0.50) \approx -1.0 \times 0.4794 \approx \mathbf{-0.479\ \text{m/s}}$

> 💡 $\phi = 0.50\ \text{rad} \approx 28.6^\circ$——物块从 $x \approx 0.88A$ 处开始，向 $-x$ 方向运动。运动方程包含了系统全部信息。

---

#### 7.1.6 🧪 例题 4：SHM 与非 SHM 的边界

**题目**：一个物块在光滑水平面上连接一根弹簧（$k = 40\ \text{N/m}$）。当弹簧被压缩超过 $0.30\ \text{m}$ 时，弹簧进入非线性区，恢复力变为 $F = -kx - \beta x^3$（$\beta = 200\ \text{N/m}^3$）。求：
(a) 当物块在 $x = 0.10\ \text{m}$ 时，恢复力与线性近似的相对误差
(b) 当物块在 $x = 0.40\ \text{m}$ 时，恢复力与线性近似的相对误差
(c) 判断什么振幅范围内系统可近似为 SHM

**题目分析**：

> 比较实际恢复力 $F_{\text{real}} = -kx - \beta x^3$ 与线性近似 $F_{\text{lin}} = -kx$。

**解答**：

**(a)** $x = 0.10\ \text{m}$：
- $F_{\text{lin}} = -40 \times 0.10 = -4.0\ \text{N}$
- $F_{\text{real}} = -4.0 - 200 \times 0.001 = -4.0 - 0.20 = -4.20\ \text{N}$
- 相对误差 $= \dfrac{0.20}{4.0} = \mathbf{5\%}$

**(b)** $x = 0.40\ \text{m}$：
- $F_{\text{lin}} = -40 \times 0.40 = -16\ \text{N}$
- $F_{\text{real}} = -16 - 200 \times 0.064 = -16 - 12.8 = -28.8\ \text{N}$
- 相对误差 $= \dfrac{12.8}{16} = \mathbf{80\%}$

**(c)** 若接受 $5\%$ 误差为 SHM 近似的上限，则 $A \lesssim 0.10\ \text{m}$。当 $A$ 较大时，非线性项 $\beta x^3$ 主导，振动周期将随振幅增大而增大——不再是 SHM。

> 💡 **SHM 是真实世界的近似**：真实弹簧只在小变形下遵循胡克定律。当变形过大时，材料进入非线性区，振动不再是 SHM。这也是为什么「小振幅」假设在物理中如此普遍。

---

#### 7.1.7 🧪 例题 5：参考圆法中位移-速度-加速度的对应

**题目**：一个参考圆半径为 $R = 0.12\ \text{m}$，以 $\omega = 6.0\ \text{rad/s}$ 逆时针旋转。求其 $x$ 轴投影（SHM）的：
(a) 振幅和角频率
(b) $t = \pi/12\ \text{s}$（假设 $\phi = 0$）时的 $x$、$v$、$a$
(c) 最大速度和最大加速度

**解答**：

**(a)** $A = R = \mathbf{0.12\ \text{m}}$，$\omega = \mathbf{6.0\ \text{rad/s}}$

**(b)** $\omega t = 6.0 \times \pi/12 = \pi/2\ \text{rad}$：

$x = A\cos(\pi/2) = \mathbf{0}$（在平衡位置）

$v = -A\omega\sin(\pi/2) = -0.12 \times 6.0 \times 1 = \mathbf{-0.72\ \text{m/s}}$

$a = -A\omega^2\cos(\pi/2) = \mathbf{0}$

**(c)** $v_{\max} = A\omega = 0.72\ \text{m/s}$，$a_{\max} = A\omega^2 = 0.12 \times 36 = \mathbf{4.32\ \text{m/s}^2}$

> 💡 参考圆法将 SHM 与匀速圆周运动完美映射——圆周上的位置 $(R\cos\theta, R\sin\theta)$ 的 $x$ 坐标就是 SHM 位移，圆周切向速度的 $x$ 分量就是 SHM 速度。这种几何直觉在定性分析中极为有用。

---

### 本节总结

SHM 的判定和基本描述：

1. **定义性方程**：$F = -kx$（恢复力与位移成正比且反向）
2. **加速度特征**：$a = -\omega^2 x$，其中 $\omega = \sqrt{k/m}$
3. **微分方程**：$\dfrac{d^2x}{dt^2} + \omega^2 x = 0$
4. **通解**：$x = A\cos(\omega t + \phi)$
5. **恒定外力不改变 $\omega$**——只移动平衡位置

# 7.2 频率与周期（Frequency and Period）

## Part A：基础层（AP Physics 1 必备）

### 一、描述振动快慢的三个物理量

> SHM 的快慢由三个相互关联的物理量描述——**周期 $T$**（完成一次完整振动所需的时间）、**频率 $f$**（单位时间内的振动次数）和**角频率 $\omega$**（单位时间内的相位变化量，以弧度计）。
>
> $$
> \boxed{T = \frac{1}{f} = \frac{2\pi}{\omega}},\quad \boxed{f = \frac{1}{T} = \frac{\omega}{2\pi}},\quad \boxed{\omega = 2\pi f = \frac{2\pi}{T}}
> $$

这三个量本质上是同一信息的三种不同表达方式——选哪个取决于问题的语境。周期 $T$ 适合讨论「一次振动多久」，频率 $f$ 适合讨论「每秒振动几次」，角频率 $\omega$ 适合数学表达（因为三角函数以 $2\pi$ 为周期）。

### 二、弹簧-质量系统的周期

由 $\omega = \sqrt{k/m}$ 和 $T = 2\pi/\omega$：

$$
\boxed{T = 2\pi\sqrt{\frac{m}{k}}},\quad \boxed{f = \frac{1}{2\pi}\sqrt{\frac{k}{m}}}
$$

这是 SHM 中最重要的公式之一。它揭示了一个重要事实：

> 🎯 **SHM 的周期与振幅无关！**

无论你将弹簧拉开 $1\ \text{cm}$ 还是 $10\ \text{cm}$，周期完全相同。这一性质称为**等时性（Isochronism）**，是 SHM 区别于其他振动的标志性特征。伽利略在比萨大教堂观察吊灯摆动时首次发现了这一现象。

### 三、$T = 2\pi\sqrt{m/k}$ 的物理直觉

- **$m$ 在分子上** → 质量越大，惯性越大，周期越长（振动越慢）
- **$k$ 在分母上** → 弹簧越硬，恢复力越大，周期越短（振动越快）
- **$m$ 翻倍** → $T$ 增大 $\sqrt{2}$ 倍 ≈ 1.414 倍
- **$k$ 翻倍** → $T$ 减小 $1/\sqrt{2}$ 倍 ≈ 0.707 倍

### 四、周期与初始条件

初始条件（初始位移 $x_0$ 和初始速度 $v_0$）决定振幅 $A$ 和初相位 $\phi$，但**不决定周期**：

$$
A = \sqrt{x_0^2 + \left(\frac{v_0}{\omega}\right)^2},\quad \phi = \arctan\left(-\frac{v_0}{\omega x_0}\right)
$$

周期 $T = 2\pi/\omega = 2\pi\sqrt{m/k}$ 仅由 $m$ 和 $k$ 决定。

### 五、参考圆——SHM 与匀速圆周运动的关系

> SHM 可以看作匀速圆周运动在直径上的投影。圆周运动的角速度 $\omega$ 恰好是 SHM 的角频率。这一对应关系是理解 SHM 的几何钥匙。

| 圆运动 | SHM 投影 | 对应关系 |
|:--|:--|:--|
| 半径 $A$ | 振幅 $A$ | 圆半径 = 最大位移 |
| 角速度 $\omega$ | 角频率 $\omega$ | 完全相同 |
| $x = A\cos(\omega t + \phi)$ | SHM 位移 | 圆上点在 $x$ 轴的投影 |
| $v_{\text{tan}} = A\omega$ | $v_{\text{max}} = A\omega$ | 最大速度 = 圆周切向速率 |
| $a_c = A\omega^2$ | $a_{\text{max}} = A\omega^2$ | 最大加速度 = 向心加速度 |

---

#### 7.2.1 🧪 推导 1：从 $F = -kx$ 和圆周运动投影导出 $T = 2\pi\sqrt{m/k}$

**推导目标**：用两种独立方法导出弹簧-质量系统的周期公式。

**推导过程**：

**方法一**：从 $\omega = \sqrt{k/m}$ 出发。

由 7.1 节推导，$a = -\dfrac{k}{m}x = -\omega^2 x$，其中 $\omega = \sqrt{k/m}$。

周期与角频率的关系为 $T = \dfrac{2\pi}{\omega}$（因为 $\omega$ 是 $2\pi$ 除以周期的商）：

$$
T = \frac{2\pi}{\omega} = \frac{2\pi}{\sqrt{k/m}} = 2\pi\sqrt{\frac{m}{k}}
$$

**方法二**：参考圆法。

做匀速圆周运动的质点在 $x$ 轴上的投影做 SHM。圆周运动的周期为 $T = 2\pi/\omega$。

圆周运动的向心力为 $F_c = m\omega^2 A$（其中 $A$ 是圆半径 = SHM 振幅）。

对于 SHM，最大恢复力 $F_{\max} = kA$。当投影在最大位移处时，恢复力恰好等于向心力在 $x$ 方向的投影（此时即为向心力本身）：

$$
kA = m\omega^2 A
$$

消去 $A$：
$$
\omega^2 = \frac{k}{m} \quad \Rightarrow \quad T = \frac{2\pi}{\omega} = 2\pi\sqrt{\frac{m}{k}}
$$

两种方法殊途同归——第一种直接从 SHM 动力学出发，第二种利用圆周运动的几何直观。

> 💡 **参考圆法的威力**：一旦建立起 SHM 与圆周运动投影的等价关系，SHM 中的所有运动学量（位移、速度、加速度）都可以从圆周运动的几何关系直接「读」出来。

---

#### 7.2.2 🧪 推导 2：从量纲分析推导周期公式的形式

**推导目标**：利用量纲分析证明 $T$ 必须正比于 $\sqrt{m/k}$，这是物理学家在不知道详细方程时使用的强大工具。

**推导过程**：

$T$ 的量纲是 $[T]$（时间）。系统的参数只有 $m$（质量，$[M]$）和 $k$（劲度系数，$[M][T]^{-2}$，因为 $k = F/x$）。

假设 $T \propto m^\alpha k^\beta$，则量纲方程为：

$$
[T] = [M]^\alpha \cdot ([M][T]^{-2})^\beta = [M]^{\alpha+\beta}[T]^{-2\beta}
$$

比较左右两侧的量纲指数：
- $[T]$：$1 = -2\beta$ → $\beta = -1/2$
- $[M]$：$0 = \alpha + \beta$ → $\alpha = -\beta = 1/2$

因此：
$$
T \propto m^{1/2}k^{-1/2} = \sqrt{\frac{m}{k}}
$$

与完整推导的结果一致！量纲分析无法给出 $2\pi$ 这个因子，但确定了 $T$ 对 $m$ 和 $k$ 的依赖关系。

> 💡 **量纲分析的哲学**：物理公式的形式受量纲的严格约束。如果你忘记了 $T$ 的公式，量纲分析至少能告诉你 $T \propto \sqrt{m/k}$——这在选择题中足以排除大多数错误选项。

---

#### 7.2.2b 🧪 推导 3：弹簧串联与并联的等效劲度系数

**推导目标**：严格推导弹簧串联和并联时的等效劲度系数公式。

**推导过程**：

**并联**：$N$ 根弹簧并排连接同一物块。物块位移 $x$ 时，每根弹簧均伸长 $x$，各自施加力 $-k_i x$。合力：

$$
F = -\sum_i k_i x = -\left(\sum_i k_i\right)x
$$

因此：
$$
\boxed{k_{\text{eff}} = \sum_i k_i = k_1 + k_2 + \cdots + k_N}
$$

并联弹簧的总劲度系数等于各弹簧劲度系数之和——并联使系统更硬。

**串联**：$N$ 根弹簧首尾相连。物块位移 $x$ 时，总伸长量 $x$ 由 $N$ 根弹簧分担：$x = x_1 + x_2 + \cdots + x_N$。串联中每根弹簧受力相同（均为 $F$），每根弹簧满足 $F = -k_i x_i$ → $x_i = -F/k_i$。因此：

$$
x = -\frac{F}{k_1} - \frac{F}{k_2} - \cdots - \frac{F}{k_N} = -F\left(\frac{1}{k_1} + \frac{1}{k_2} + \cdots + \frac{1}{k_N}\right)
$$

即：
$$
\frac{1}{k_{\text{eff}}} = \sum_i \frac{1}{k_i}
$$

$$
\boxed{k_{\text{eff}} = \left(\frac{1}{k_1} + \frac{1}{k_2} + \cdots + \frac{1}{k_N}\right)^{-1}}
$$

串联弹簧的总劲度系数小于任何一根单独的弹簧——串联使系统更软。

> 💡 **类比电阻**：弹簧并联类似电阻并联（$1/R_{\text{eff}} = \sum 1/R_i$？不对，弹簧并联是直接相加 $k$，而电阻串联是直接相加 $R$）。实际上弹簧串联/并联的公式与电容器恰好「互换」——弹簧并联 = 电容并联，弹簧串联 = 电容串联。这来自 $F = kx$ 与 $Q = CV$ 在形式上的对应。

---

#### 7.2.2c 🧪 推导 4：从 $\omega$-$T$-$f$ 关系导出 SHM 的完整参数链

**推导目标**：建立 $\omega$、$T$、$f$ 与 $m$、$k$ 之间的完整参数链，展示所有 SHM 参数如何从一个基本关系 $\omega = \sqrt{k/m}$ 中派生。

**推导过程**：

从 $\omega = \sqrt{k/m}$ 出发：

$$
T = \frac{2\pi}{\omega} = 2\pi\sqrt{\frac{m}{k}}
$$

$$
f = \frac{1}{T} = \frac{1}{2\pi}\sqrt{\frac{k}{m}}
$$

反过来从 $T$ 可反推系统参数：

$$
\frac{k}{m} = \frac{4\pi^2}{T^2}
$$

若已知 $m$ 和 $T$：$k = \dfrac{4\pi^2 m}{T^2}$
若已知 $k$ 和 $T$：$m = \dfrac{kT^2}{4\pi^2}$

**应用——用 SHM 测量未知质量**：在弹簧上测量周期 $T_0$（已知质量 $m_0$），再测量待测质量 $m_x$ 的周期 $T_x$：

$$
\frac{T_x}{T_0} = \sqrt{\frac{m_x}{m_0}} \quad \Rightarrow \quad \boxed{m_x = m_0\left(\frac{T_x}{T_0}\right)^2}
$$

这就是航天员在失重环境下测量自身质量的方法（太空中的体质量测量仪 SMMD）——用弹簧振子的周期来确定质量，因为周期不依赖于重力加速度。

> 💡 SHM 的全部参数由 $\omega = \sqrt{k/m}$ 这个单一关系确定。$m$ 和 $k$ 是两个「输入参数」，$\omega$、$T$、$f$ 是三个「等价输出」——它们只是同一信息的不同表达。

---

#### 7.2.3 🧪 例题 1：改变质量与弹簧对周期的影响

**题目**：一个 $m = 0.40\ \text{kg}$ 的物块连接在 $k = 25\ \text{N/m}$ 的弹簧上做 SHM。求：
(a) 周期 $T$ 和频率 $f$
(b) 若物块质量增加到 $1.60\ \text{kg}$，周期变为多少？
(c) 若用另一根 $k = 100\ \text{N/m}$ 的弹簧替换，周期变为多少？

**题目分析**：

> **已知**：$m_0 = 0.40\ \text{kg}$，$k_0 = 25\ \text{N/m}$
>
> **求**：$T_0$、$f_0$、变化后的周期

**解答**：

**(a)** $T_0 = 2\pi\sqrt{\dfrac{0.40}{25}} = 2\pi\sqrt{0.016} = 2\pi \times 0.1265 \approx \mathbf{0.795\ \text{s}}$

$f_0 = \dfrac{1}{T_0} \approx \mathbf{1.26\ \text{Hz}}$

**(b)** $m = 1.60\ \text{kg}$（4 倍于原始质量）：
$$
T = 2\pi\sqrt{\frac{1.60}{25}} = 2\pi\sqrt{0.064} = 2\pi \times 0.253 \approx \mathbf{1.59\ \text{s}}
$$

验证：$T/T_0 = \sqrt{1.60/0.40} = \sqrt{4} = 2$ → $T = 2 \times 0.795 = 1.59\ \text{s}$ ✓

**(c)** $k = 100\ \text{N/m}$（4 倍于原始 $k$），$m = 0.40\ \text{kg}$：
$$
T = 2\pi\sqrt{\frac{0.40}{100}} = 2\pi\sqrt{0.004} = 2\pi \times 0.0632 \approx \mathbf{0.397\ \text{s}}
$$

验证：$T/T_0 = \sqrt{25/100} = \sqrt{1/4} = 1/2$ → $T = 0.795/2 = 0.3975\ \text{s}$ ✓

> 💡 **平方根关系的实用意义**：要使周期翻倍，质量需增加到 4 倍（或弹簧软到 1/4）。这意味着周期对参数变化不太敏感——在实验设计中，测量周期是检验 $k$ 或 $m$ 的有效方法。

---

#### 7.2.4 🧪 例题 2：组合弹簧系统的等效劲度系数

**题目**：两根相同的弹簧（劲度系数均为 $k = 20\ \text{N/m}$）以两种方式连接一个 $m = 0.50\ \text{kg}$ 的物块：
(a) 并联（两根弹簧并排连接物块）
(b) 串联（两根弹簧首尾相连，一端固定，另一端连物块）
求每种情况下的等效劲度系数和振动周期。

**题目分析**：

> 并联时弹簧伸长相同，力叠加；串联时弹簧受力相同，伸长量叠加。

**解答**：

**(a)** 并联：

物块位移 $x$ 时，两根弹簧各自施加力 $-kx$（伸长量同为 $x$）。合力 $F = -kx - kx = -2kx$。

$$
k_{\text{eff}} = 2k = \mathbf{40\ \text{N/m}}
$$

$$
T_{\text{parallel}} = 2\pi\sqrt{\frac{m}{2k}} = 2\pi\sqrt{\frac{0.50}{40}} \approx \mathbf{0.702\ \text{s}}
$$

**(b)** 串联：

物块位移 $x$ 时，每根弹簧只伸长 $x/2$（总伸长量 $x$ 由两根弹簧平均分担）。每根弹簧施加的力为 $F = -k(x/2)$。由于串联中每根弹簧受力相同（$F$ 也等于物块受到的恢复力）：

$$
F = -k \cdot \frac{x}{2} \quad \Rightarrow \quad k_{\text{eff}} = \frac{F}{x} = \frac{k}{2}
$$

弹簧串联的等效劲度系数公式：$\dfrac{1}{k_{\text{eff}}} = \dfrac{1}{k} + \dfrac{1}{k} = \dfrac{2}{k}$

$$
k_{\text{eff}} = \frac{k}{2} = \mathbf{10\ \text{N/m}}
$$

$$
T_{\text{series}} = 2\pi\sqrt{\frac{m}{k/2}} = 2\pi\sqrt{\frac{0.50}{10}} \approx \mathbf{1.40\ \text{s}}
$$

> 💡 **并联 vs 串联对比**：

| 连接方式 | $k_{\text{eff}}$ | $T$ | 直观理解 |
|:--|:--:|:--:|:--|
| 并联 | $2k = 40$ | $0.702\ \text{s}$ | 弹簧「合力」更硬 |
| 串联 | $k/2 = 10$ | $1.40\ \text{s}$ | 弹簧「接力」更软 |
| 单根 | $k = 20$ | $0.993\ \text{s}$ | 基准 |

并联周期是单根的 $1/\sqrt{2} \approx 0.707$ 倍，串联周期是单根的 $\sqrt{2} \approx 1.414$ 倍。

---

#### 7.2.5 🧪 例题 3：太空中的质量测量

**题目**：宇航员在太空中使用弹簧振子测量自己的质量。她先测量一个已知质量 $m_0 = 10.0\ \text{kg}$ 的校准块的振动周期 $T_0 = 1.20\ \text{s}$，然后自己坐在连接到同一弹簧的椅子上，测得周期 $T = 2.80\ \text{s}$。求宇航员的质量（椅子质量 $m_c = 5.0\ \text{kg}$）。

**题目分析**：

> 太空失重环境 → 无重力干扰 → 弹簧振子周期仅由 $m$ 和 $k$ 决定。由 $T \propto \sqrt{m}$。

**解答**：

由 $T_0 = 2\pi\sqrt{m_0/k_{\text{eff}}}$，$T = 2\pi\sqrt{(m + m_c)/k_{\text{eff}}}$。

取比值消去 $k_{\text{eff}}$：
$$
\frac{T}{T_0} = \sqrt{\frac{m + m_c}{m_0}}
$$

$$
m + m_c = m_0\left(\frac{T}{T_0}\right)^2 = 10.0 \times \left(\frac{2.80}{1.20}\right)^2 = 10.0 \times 5.444 \approx 54.4\ \text{kg}
$$

$$
m = 54.4 - 5.0 = \mathbf{49.4\ \text{kg}}
$$

> 💡 太空中的体质量测量仪（SMMD）正是基于此原理——在失重环境下，普通体重秤无法使用，但弹簧振子的周期法可以精确测量质量。

---

#### 7.2.6 🧪 例题 4：弹簧截断对周期的影响

**题目**：一根原长 $L_0 = 0.60\ \text{m}$、劲度系数 $k = 30\ \text{N/m}$ 的弹簧连接 $m = 0.50\ \text{kg}$ 的物块做 SHM。若将弹簧截去 $1/3$ 长度（剩下 $0.40\ \text{m}$）后重新连接，求：
(a) 新弹簧的劲度系数 $k'$
(b) 新周期 $T'$
(c) 若截下的 $1/3$ 与剩下的 $2/3$ 并联，周期又是多少？

**题目分析**：

> $k \propto 1/L$——弹簧越短越硬。截后的两段可串联或并联。

**解答**：

**(a)** 弹簧劲度系数与长度成反比：$kL = \text{常数}$（同种材料、同种绕法）。

原弹簧：$kL_0 = 30 \times 0.60 = 18\ \text{N}$

截去 $1/3$ 后剩下 $L' = 0.40\ \text{m}$：$k' = \dfrac{18}{0.40} = \mathbf{45\ \text{N/m}}$

**(b)** $T' = 2\pi\sqrt{\dfrac{m}{k'}} = 2\pi\sqrt{\dfrac{0.50}{45}} \approx 2\pi \times 0.1054 \approx \mathbf{0.662\ \text{s}}$

原周期 $T_0 = 2\pi\sqrt{0.50/30} \approx 0.811\ \text{s}$，$T'/T_0 = \sqrt{30/45} = \sqrt{2/3} \approx 0.816$。

**(c)** 截下的 $1/3$ 长 $0.20\ \text{m}$：$k_1 = 18/0.20 = 90\ \text{N/m}$

剩下的 $2/3$ 长 $0.40\ \text{m}$：$k_2 = 18/0.40 = 45\ \text{N/m}$

并联：$k_{\text{eff}} = 90 + 45 = \mathbf{135\ \text{N/m}}$

$T_{\text{parallel}} = 2\pi\sqrt{0.50/135} \approx \mathbf{0.382\ \text{s}}$

> 💡 将一根弹簧截断后并联——$k_{\text{eff}}$ 从 $30$ 变为 $135$（增大 $4.5$ 倍），周期缩小到原来的 $1/\sqrt{4.5} \approx 0.471$ 倍。这就是为什么短而粗的弹簧振动极快。

---

#### 7.2.7 🧪 例题 5：测量未知行星的重力加速度

**题目**：宇航员在某未知行星表面用一个 $L = 0.80\ \text{m}$ 的单摆测量了 $N = 50$ 次完整摆动的时间为 $t = 142\ \text{s}$。求该行星表面的重力加速度 $g$。

**题目分析**：

> 单摆周期 $T = 2\pi\sqrt{L/g}$ → 测量 $T$ → 求 $g$。

**解答**：

周期：$T = \dfrac{142}{50} = 2.84\ \text{s}$

$$
T = 2\pi\sqrt{\frac{L}{g}} \quad \Rightarrow \quad g = \frac{4\pi^2 L}{T^2}
$$

$$
g = \frac{4\pi^2 \times 0.80}{(2.84)^2} = \frac{31.58}{8.066} \approx \mathbf{3.92\ \text{m/s}^2}
$$

> 💡 该行星的 $g \approx 3.92\ \text{m/s}^2$ 约为地球的 $40\%$，与火星表面（$g \approx 3.7\ \text{m/s}^2$）接近。测量 $N = 50$ 次而非 1 次是为了减小测量误差——$N$ 次摆动的平均周期误差仅为单次测量的 $1/\sqrt{N}$。

---

### 本节总结

1. **$T = 2\pi\sqrt{m/k}$** — SHM 周期的核心公式
2. **$T \propto \sqrt{m}$**，**$T \propto 1/\sqrt{k}$** — 平方根依赖关系
3. **$T$ 与振幅无关** — SHM 的等时性
4. **参考圆** — SHM 与圆周运动投影的等价关系
5. **量纲分析** — 不用解方程也能推断公式形式

# 7.3 表示与分析 SHM（Representing and Analyzing SHM）

## Part A：基础层（AP Physics 1 必备）

### 一、SHM 的三个运动学函数

> SHM 的位移、速度和加速度都是时间的正弦（或余弦）函数。三者之间存在精确的相位关系——速度领先位移 $90^\circ$（$\pi/2$），加速度领先速度 $90^\circ$（即与位移反相，相差 $180^\circ$ 或 $\pi$）。
>
> $$
> \boxed{x(t) = A\cos(\omega t + \phi)}
> $$
> $$
> \boxed{v(t) = \frac{dx}{dt} = -A\omega\sin(\omega t + \phi) = A\omega\cos\!\left(\omega t + \phi + \frac{\pi}{2}\right)}
> $$
> $$
> \boxed{a(t) = \frac{dv}{dt} = -A\omega^2\cos(\omega t + \phi) = -\omega^2 x(t)}
> $$

这三个函数构成了 SHM 运动学的完整描述——知道其中任何一个，就可以导出另外两个（通过求导或积分）。

### 二、相位与相位差

> **相位（Phase）** 是描述振动在周期中位置的量，以弧度表示。$\phi$ 是**初相位**——$t = 0$ 时的相位值，由初始条件决定。

| 初相位 $\phi$ | $x(0)$ | $v(0)$ | 物理情景 |
|:--:|:--|:--|:--|
| $0$ | $+A$ | $0$ | 从最大正位移释放 |
| $\pi/2$ | $0$ | $-A\omega$ | 从平衡位置向左推 |
| $\pi$ | $-A$ | $0$ | 从最大负位移释放 |
| $3\pi/2$（或 $-\pi/2$） | $0$ | $+A\omega$ | 从平衡位置向右推 |

### 三、三个运动学量的极值

| 物理量 | 最大值 | 出现在 | 最小值 | 出现在 |
|:--|:--|:--|:--|:--|
| $x$ | $+A$ | $\omega t + \phi = 0, 2\pi, \ldots$ | $-A$ | $\omega t + \phi = \pi, 3\pi, \ldots$ |
| $v$ | $+A\omega$ | $\omega t + \phi = 3\pi/2$（过平衡位置向右） | $-A\omega$ | $\omega t + \phi = \pi/2$（过平衡位置向左） |
| $a$ | $+A\omega^2$ | $\omega t + \phi = \pi$（最大负位移处） | $-A\omega^2$ | $\omega t + \phi = 0$（最大正位移处） |

### 四、SHM 的 $x$-$v$-$a$-$t$ 图像

| 图像 | 形状 | 关键特征 |
|:--|:--|:--|
| $x$-$t$ | 余弦曲线 | $x_{\max} = A$，$x_{\min} = -A$ |
| $v$-$t$ | 负正弦曲线 | $v_{\max} = A\omega$（$x=0$ 时），$v=0$（$x=\pm A$ 时） |
| $a$-$t$ | 负余弦曲线 | 与 $x$-$t$ 镜像对称（反相），$a_{\max} = A\omega^2$ |
| $v$-$x$ | 椭圆 | $v^2 = \omega^2(A^2 - x^2)$ |

### 五、从初始条件确定 $A$ 和 $\phi$

给定初始位移 $x_0$ 和初始速度 $v_0$：

$$
\boxed{A = \sqrt{x_0^2 + \left(\frac{v_0}{\omega}\right)^2}},\quad \boxed{\tan\phi = -\frac{v_0}{\omega x_0}}
$$

这两个公式可以从 $x(0) = A\cos\phi = x_0$ 和 $v(0) = -A\omega\sin\phi = v_0$ 联立解出——是 AP Physics C 的常考推导。

---

#### 7.3.1 🧪 推导 1：从 $x(t)$ 通过求导得到 $v(t)$ 和 $a(t)$

**推导目标**：严格推导 SHM 的速度和加速度函数，并证明 $a = -\omega^2 x$。

**推导过程**：

**第一步**：对位移求导得速度。

$x(t) = A\cos(\omega t + \phi)$

使用链式法则对 $t$ 求导：

$$
v(t) = \frac{dx}{dt} = A \cdot [-\sin(\omega t + \phi)] \cdot \frac{d}{dt}(\omega t + \phi) = -A\omega\sin(\omega t + \phi)
$$

验证单位：$[A\omega] = \text{m} \cdot \text{rad/s} = \text{m/s}$ ✓

**第二步**：对速度求导得加速度。

$$
a(t) = \frac{dv}{dt} = -A\omega \cdot [\cos(\omega t + \phi)] \cdot \frac{d}{dt}(\omega t + \phi) = -A\omega^2\cos(\omega t + \phi)
$$

**第三步**：建立 $a$ 与 $x$ 的关系。

注意到 $A\cos(\omega t + \phi) = x(t)$，因此：

$$
a(t) = -\omega^2 \cdot A\cos(\omega t + \phi) = -\omega^2 x(t)
$$

这正是 SHM 的定义性方程 $a = -\omega^2 x$。

**第四步**：导出 $v$ 与 $x$ 的关系——椭圆方程。

由 $\sin^2\theta + \cos^2\theta = 1$：
$$
\left(\frac{x}{A}\right)^2 + \left(\frac{v}{A\omega}\right)^2 = \cos^2(\omega t + \phi) + \sin^2(\omega t + \phi) = 1
$$

$$
\boxed{\frac{x^2}{A^2} + \frac{v^2}{A^2\omega^2} = 1}
$$

即：
$$
\boxed{v = \pm\omega\sqrt{A^2 - x^2}}
$$

> 💡 **$v$-$x$ 椭圆关系是 SHM 能量分析的几何等价物**——后面会看到，它等价于 $\frac{1}{2}mv^2 + \frac{1}{2}kx^2 = \frac{1}{2}kA^2$。

---

#### 7.3.2 🧪 推导 2：从 $x$-$v$ 椭圆关系导出振幅公式

**推导目标**：证明振幅 $A = \sqrt{x_0^2 + (v_0/\omega)^2}$。

**推导过程**：

由 $v^2 = \omega^2(A^2 - x^2)$（来自 $v$-$x$ 椭圆关系），在 $t = 0$ 时：

$$
v_0^2 = \omega^2(A^2 - x_0^2)
$$

解出 $A^2$：
$$
A^2 = x_0^2 + \frac{v_0^2}{\omega^2}
$$

$$
\boxed{A = \sqrt{x_0^2 + \left(\frac{v_0}{\omega}\right)^2}}
$$

**三种特殊情况验证**：

| 初始条件 | $A$ | 含义 |
|:--|:--|:--|
| $v_0 = 0$，$x_0 \neq 0$ | $A = |x_0|$ | 从位移释放，振幅 = 初始位移 |
| $x_0 = 0$，$v_0 \neq 0$ | $A = |v_0|/\omega$ | 击打平衡位置的物块 |
| $x_0 = 0$，$v_0 = 0$ | $A = 0$ | 不振——物块在平衡位置静止 |

**初相位 $\phi$ 的确定**：

由 $x_0 = A\cos\phi$ 和 $v_0 = -A\omega\sin\phi$：
$$
\frac{v_0}{x_0} = -\omega\tan\phi \quad \Rightarrow \quad \boxed{\tan\phi = -\frac{v_0}{\omega x_0}}
$$

> 💡 **$A$ 和 $\phi$ 的物理角色**：$A$ 是振动的「规模」（多大幅度），$\phi$ 是振动的「起始时刻」（$t=0$ 时处在周期的哪个阶段）。两者都由初始条件决定，而 $\omega$ 仅由系统参数决定——这是 SHM 最核心的三分法。

---

#### 7.3.2b 🧪 推导 3：SHM 中位移、速度、加速度的相位关系

**推导目标**：严格证明 $v$ 领先 $x$ 为 $\pi/2$，$a$ 领先 $v$ 为 $\pi/2$（即 $a$ 与 $x$ 反相，相差 $\pi$）。

**推导过程**：

由 $x = A\cos(\omega t + \phi)$，利用三角函数的导数关系：

$$
v = \frac{dx}{dt} = -A\omega\sin(\omega t + \phi)
$$

利用 $\sin\theta = \cos(\theta - \pi/2)$：
$$
v = -A\omega\cos\!\left(\omega t + \phi - \frac{\pi}{2}\right) = A\omega\cos\!\left(\omega t + \phi + \frac{\pi}{2}\right)
$$

因此 $v$ 的相位领先 $x$ 为 $\pi/2$（$90^\circ$）。

再求导：
$$
a = \frac{dv}{dt} = -A\omega^2\cos(\omega t + \phi) = A\omega^2\cos(\omega t + \phi + \pi)
$$

因此 $a$ 领先 $v$ 为 $\pi/2$，即 $a$ 与 $x$ 反相（相差 $\pi$，即 $180^\circ$）。

**相位关系的物理含义**：

| 时刻 | $x$ | $v$ | $a$ | 物块状态 |
|:--|:--|:--|:--|:--|
| $\omega t + \phi = 0$ | $+A$（最大） | $0$ | $-A\omega^2$（最大反向） | 在右端，瞬间静止，向左加速 |
| $\omega t + \phi = \pi/4$ | $+A/\sqrt{2}$ | $-A\omega/\sqrt{2}$ | $-A\omega^2/\sqrt{2}$ | 向左运动，仍在减速 |
| $\omega t + \phi = \pi/2$ | $0$ | $-A\omega$（最大向左） | $0$ | 过平衡位置向左，加速度为零 |
| $\omega t + \phi = \pi$ | $-A$ | $0$ | $+A\omega^2$（最大向右） | 在左端，瞬间静止，向右加速 |

> 💡 **记忆口诀**：「速度领先位移 90 度，加速度又领先速度 90 度」——因此加速度始终与位移反相。这可以通过圆周运动的投影直观理解：圆周上点的 $x$ 坐标、速度 $x$ 分量、加速度 $x$ 分量恰好相差 $90^\circ$。

---

#### 7.3.2c 🧪 推导 4：SHM 的平均动能与平均势能

**推导目标**：证明在一个完整周期内，SHM 的平均动能等于平均势能，各为总能量的一半。

**推导过程**：

动能的时间函数：$K(t) = \frac{1}{2}kA^2\sin^2(\omega t + \phi)$（取 $\phi = 0$ 简化，不影响平均值）

一个周期内的平均值：
$$
\bar{K} = \frac{1}{T}\int_0^T \frac{1}{2}kA^2\sin^2(\omega t)\,dt
$$

利用 $\int_0^T \sin^2(\omega t)\,dt = \frac{T}{2}$（因为 $\sin^2$ 在一个周期内的平均值是 $1/2$）：

$$
\bar{K} = \frac{1}{T} \cdot \frac{1}{2}kA^2 \cdot \frac{T}{2} = \frac{1}{4}kA^2 = \frac{1}{2}E
$$

同理 $\bar{U} = \frac{1}{4}kA^2 = \frac{1}{2}E$。

因此：
$$
\boxed{\bar{K} = \bar{U} = \frac{1}{2}E = \frac{1}{4}kA^2}
$$

> 💡 **维里定理在 SHM 中的体现**：对于势能 $U \propto x^2$ 的系统，平均动能等于平均势能。这是更普遍的维里定理（Virial Theorem）的一个特例。

---

#### 7.3.3 🧪 例题 1：从初始条件求运动方程

**题目**：一个 $m = 0.25\ \text{kg}$ 的物块连接在 $k = 16\ \text{N/m}$ 的弹簧上。在 $t = 0$ 时，物块被拉到 $x_0 = +0.12\ \text{m}$ 处并从静止释放。求：
(a) 角频率 $\omega$ 和周期 $T$
(b) 振幅 $A$
(c) 运动方程 $x(t)$
(d) $t = 0.50\ \text{s}$ 时的位移和速度

**题目分析**：

> **已知**：$m = 0.25\ \text{kg}$，$k = 16\ \text{N/m}$，$x_0 = +0.12\ \text{m}$，$v_0 = 0$
>
> **求**：$\omega$、$T$、$A$、$x(t)$、$x(0.50)$、$v(0.50)$

**解答**：

**(a)** $\omega = \sqrt{\dfrac{k}{m}} = \sqrt{\dfrac{16}{0.25}} = \sqrt{64} = \mathbf{8.0\ \text{rad/s}}$

$T = \dfrac{2\pi}{\omega} = \dfrac{2\pi}{8.0} \approx \mathbf{0.785\ \text{s}}$

**(b)** 由 $v_0 = 0$ → $A = |x_0| = \mathbf{0.12\ \text{m}}$

**(c)** $x_0 = A\cos\phi$，且 $x_0 = +A$ → $\cos\phi = 1$ → $\phi = 0$

$$
x(t) = A\cos(\omega t + \phi) = \mathbf{0.12\cos(8.0t)\ \text{m}}
$$

$v(t) = -A\omega\sin(\omega t) = \mathbf{-0.96\sin(8.0t)\ \text{m/s}}$

**(d)** $x(0.50) = 0.12\cos(8.0 \times 0.50) = 0.12\cos(4.0)\ \text{rad}$

$\cos(4.0\ \text{rad}) \approx -0.6536$

$x(0.50) \approx 0.12 \times (-0.6536) \approx \mathbf{-0.0784\ \text{m}}$

$v(0.50) = -0.96\sin(4.0) \approx -0.96 \times (-0.7568) \approx \mathbf{+0.727\ \text{m/s}}$

> 💡 $t = 0.50\ \text{s}$ 时物块在平衡位置左侧 $7.84\ \text{cm}$ 处，正向右运动（$v > 0$）。这比 $T$ 的一半（$0.393\ \text{s}$）稍晚，物块已过最左端并开始返回。

---

#### 7.3.4 🧪 例题 2：从速度-位移关系解题

**题目**：一个做 SHM 的物体振幅 $A = 0.080\ \text{m}$，角频率 $\omega = 10\ \text{rad/s}$。求：
(a) 最大速度 $v_{\max}$
(b) 当位移 $x = 0.040\ \text{m}$ 时的速度大小
(c) 当速度 $v = 0.40\ \text{m/s}$ 时的位移大小
(d) 加速度为零时物体的位置

**题目分析**：

> 用 $v = \pm\omega\sqrt{A^2 - x^2}$ 求速度，用 $a = -\omega^2 x$ 求加速度。

**解答**：

**(a)** $v_{\max} = A\omega = 0.080 \times 10 = \mathbf{0.80\ \text{m/s}}$

**(b)** $|v| = \omega\sqrt{A^2 - x^2} = 10\sqrt{0.080^2 - 0.040^2} = 10\sqrt{0.0064 - 0.0016}$

$= 10\sqrt{0.0048} \approx 10 \times 0.0693 \approx \mathbf{0.693\ \text{m/s}}$

**(c)** 由 $v^2 = \omega^2(A^2 - x^2)$ → $x^2 = A^2 - \dfrac{v^2}{\omega^2}$

$x^2 = 0.0064 - \dfrac{0.40^2}{100} = 0.0064 - 0.0016 = 0.0048$

$|x| = \sqrt{0.0048} \approx \mathbf{0.0693\ \text{m}}$（在平衡位置两侧均可）

**(d)** $a = 0$ 当 $x = 0$——即在**平衡位置**。此时速度达到最大值 $v_{\max} = 0.80\ \text{m/s}$。

> 💡 **速度-位移对称性**：$x = A/2$ 时 $v \approx 0.866v_{\max}$（$\sqrt{3}/2$ 倍），$x = A/\sqrt{2}$ 时 $v = v_{\max}/\sqrt{2}$。这些「特殊比例」在 AP 选择题中反复出现。

---

#### 7.3.5 🧪 例题 3：$x$-$t$、$v$-$t$、$a$-$t$ 图像的绘制与分析

**题目**：一个 SHM 系统 $A = 0.10\ \text{m}$，$T = 0.50\ \text{s}$，$\phi = 0$。在同一时间轴上画出 $t = 0$ 到 $t = T$ 范围内的 $x(t)$、$v(t)$、$a(t)$ 图像，并标出所有最大值和零点。

**解答**：

$\omega = 2\pi/T = 2\pi/0.50 = 4\pi \approx 12.57\ \text{rad/s}$

$x(t) = 0.10\cos(12.57t)\ \text{m}$

$v(t) = -0.10 \times 12.57 \times \sin(12.57t) \approx -1.257\sin(12.57t)\ \text{m/s}$

$a(t) = -0.10 \times 12.57^2 \times \cos(12.57t) \approx -15.79\cos(12.57t)\ \text{m/s}^2$

| $t$ | $x$(m) | $v$(m/s) | $a$(m/s²) |
|:--|:--:|:--:|:--:|
| $0$ | $+0.10$ | $0$ | $-15.79$ |
| $T/4 = 0.125\ \text{s}$ | $0$ | $-1.257$ | $0$ |
| $T/2 = 0.25\ \text{s}$ | $-0.10$ | $0$ | $+15.79$ |
| $3T/4 = 0.375\ \text{s}$ | $0$ | $+1.257$ | $0$ |
| $T = 0.50\ \text{s}$ | $+0.10$ | $0$ | $-15.79$ |

> 💡 注意 $v$ 在 $x=0$ 时达到极值，$a$ 在 $x=\pm A$ 时达到极值。$a$-$t$ 图是 $x$-$t$ 图「上下翻转」的镜像——因为 $a = -\omega^2 x$。

---

#### 7.3.6 🧪 例题 4：非零初相位的运动分析

**题目**：一个 SHM 系统 $A = 0.080\ \text{m}$，$\omega = 5.0\ \text{rad/s}$，$\phi = \pi/3\ \text{rad}$。求：
(a) $t = 0$ 时的位置和速度方向
(b) 物块第一次到达 $x = +A$（最大正位移）的时间
(c) 物块第一次到达平衡位置的时间

**解答**：

**(a)** $x(0) = 0.080\cos(\pi/3) = 0.080 \times 0.5 = \mathbf{+0.040\ \text{m}}$

$v(0) = -0.080 \times 5.0 \times \sin(\pi/3) = -0.40 \times 0.866 \approx \mathbf{-0.346\ \text{m/s}}$（向 $-x$ 方向）

**(b)** $x = +A$ 时 $\cos(\omega t + \pi/3) = 1$ → $\omega t + \pi/3 = 0, 2\pi, 4\pi, \ldots$

最小正解：$\omega t + \pi/3 = 2\pi$ → $t = \dfrac{2\pi - \pi/3}{5.0} = \dfrac{5\pi/3}{5.0} \approx \mathbf{1.047\ \text{s}}$

**(c)** 平衡位置 $x = 0$：$\cos(\omega t + \pi/3) = 0$ → $\omega t + \pi/3 = \pi/2, 3\pi/2, \ldots$

最小正解（从 $\pi/3$ 减小到 $\pi/2$ 需要负时间，下一个是 $3\pi/2$）：
$\omega t + \pi/3 = 3\pi/2$ → $t = \dfrac{3\pi/2 - \pi/3}{5.0} = \dfrac{7\pi/6}{5.0} \approx \mathbf{0.733\ \text{s}}$

---

#### 7.3.7 🧪 例题 5：两个 SHM 的相位比较

**题目**：两个相同频率的 SHM 的位移方程分别为 $x_1 = 0.06\cos(10t)\ \text{m}$ 和 $x_2 = 0.06\cos(10t + \pi/4)\ \text{m}$。求：
(a) 两个振动的相位差
(b) 当 $x_1$ 到达最大正位移时 $x_2$ 的位置
(c) $x_2$ 领先还是落后于 $x_1$？

**解答**：

**(a)** 相位差 $\Delta\phi = \phi_2 - \phi_1 = \pi/4 - 0 = \mathbf{\pi/4\ \text{rad} = 45^\circ}$。

**(b)** $x_1$ 在 $+A$ 时：$10t = 0, 2\pi, 4\pi, \ldots$

取 $10t = 0$：$x_2 = 0.06\cos(0 + \pi/4) = 0.06 \times 0.707 \approx \mathbf{0.0424\ \text{m}}$

**(c)** $x_2$ 在 $t=0$ 时已经处于 $\pi/4$ 的相位——$x_2$ **领先** $x_1$ 为 $45^\circ$。

> 💡 在 $t=0$ 时，$x_1$ 在 $+A$（相位 0），$x_2$ 已经从 $+A$ 走过 $45^\circ$（即 $T/8$），正向平衡位置运动。相位差决定了两个振动的时序关系。

---

### 本节总结

SHM 运动学的核心公式链：

1. **$x = A\cos(\omega t + \phi)$** — 位移
2. **$v = -A\omega\sin(\omega t + \phi) = \pm\omega\sqrt{A^2 - x^2}$** — 速度
3. **$a = -A\omega^2\cos(\omega t + \phi) = -\omega^2 x$** — 加速度
4. **$A = \sqrt{x_0^2 + (v_0/\omega)^2}$** — 由初始条件确定振幅
5. **相位关系**：$v$ 领先 $x$ 为 $\pi/2$，$a$ 与 $x$ 反相（相差 $\pi$）

# 7.4 简谐振子的能量（Energy of the Simple Harmonic Oscillator）

## Part A：基础层（AP Physics 1 必备）

### 一、SHM 的能量守恒

> 简谐运动中的能量在动能和势能之间周期性地转化，但**总机械能守恒**（无阻尼时）。这是 SHM 区别于其他振动的又一标志性特征。
>
> $$
> \boxed{E_{\text{total}} = K + U = \frac{1}{2}mv^2 + \frac{1}{2}kx^2 = \frac{1}{2}kA^2}
> $$

SHM 的能量守恒是 AP 物理中最优美的结论之一——总能量只依赖于振幅 $A$ 和劲度系数 $k$，与质量 $m$ 无关！无论质量多大，只要振幅相同、弹簧相同，总能量就相同。

### 二、动能与势能的时间演化

| 能量形式 | 表达式 | 范围 |
|:--|:--|:--|
| 势能 | $U(t) = \frac{1}{2}kx^2 = \frac{1}{2}kA^2\cos^2(\omega t + \phi)$ | $0 \to \frac{1}{2}kA^2$ |
| 动能 | $K(t) = \frac{1}{2}mv^2 = \frac{1}{2}kA^2\sin^2(\omega t + \phi)$ | $0 \to \frac{1}{2}kA^2$ |
| 总能量 | $E = K + U = \frac{1}{2}kA^2$ | 恒定 |

### 三、能量在振动中的流动

> 能量在 SHM 中以两倍于振动频率的频率在动能和势能之间振荡——每半个周期，能量完成一次从势能到动能再回到势能的轮转。

| 位置 | $x$ | $v$ | $U$ | $K$ |
|:--|:--:|:--:|:--:|:--:|
| 最大位移处（$x = \pm A$） | $\pm A$ | $0$ | $\frac{1}{2}kA^2$（最大） | $0$ |
| 平衡位置（$x = 0$） | $0$ | $\pm A\omega$ | $0$ | $\frac{1}{2}kA^2$（最大） |
| $x = A/\sqrt{2}$ | $\pm A/\sqrt{2}$ | $\pm A\omega/\sqrt{2}$ | $\frac{1}{4}kA^2$ | $\frac{1}{4}kA^2$（相等！） |

### 四、能量法——AP 物理的捷径

> 🎯 在 SHM 问题中，**能量法往往比运动学方法更快**。已知 $x$ 求 $v$ 时，直接用 $v = \pm\omega\sqrt{A^2 - x^2}$（等价于能量守恒 $K + U = E$），无需先求 $t$。

### 五、能量-位移抛物线

$U(x) = \frac{1}{2}kx^2$ 是一条开口向上的抛物线。总能量 $E = \frac{1}{2}kA^2$ 是一条水平线。两条线的交点决定振动的转折点（$x = \pm A$），两线之间的垂直距离就是动能：

$$
K(x) = E - U(x) = \frac{1}{2}k(A^2 - x^2)
$$

---

#### 7.4.1 🧪 推导 1：从 $K$ 和 $U$ 出发证明总能量 $E = \frac{1}{2}kA^2$

**推导目标**：严格证明 SHM 中 $K + U = \frac{1}{2}kA^2$ 是常数。

**推导过程**（代数法 — AP Physics 1）：

动能：
$$
K = \frac{1}{2}mv^2 = \frac{1}{2}m[-A\omega\sin(\omega t + \phi)]^2 = \frac{1}{2}mA^2\omega^2\sin^2(\omega t + \phi)
$$

势能：
$$
U = \frac{1}{2}kx^2 = \frac{1}{2}k[A\cos(\omega t + \phi)]^2 = \frac{1}{2}kA^2\cos^2(\omega t + \phi)
$$

总能量：
$$
E = K + U = \frac{1}{2}mA^2\omega^2\sin^2(\omega t + \phi) + \frac{1}{2}kA^2\cos^2(\omega t + \phi)
$$

由 $\omega^2 = k/m$ → $m\omega^2 = k$，代入：
$$
E = \frac{1}{2}kA^2\sin^2(\omega t + \phi) + \frac{1}{2}kA^2\cos^2(\omega t + \phi)
$$

$$
E = \frac{1}{2}kA^2[\sin^2(\omega t + \phi) + \cos^2(\omega t + \phi)]
$$

$$
\boxed{E = \frac{1}{2}kA^2}
$$

> 💡 **关键替换**：$m\omega^2 = k$ 是连接动能系数与势能系数的桥梁。正是因为 $\omega^2 = k/m$，$\sin^2$ 和 $\cos^2$ 前面的系数才会相同，恒等式 $\sin^2 + \cos^2 = 1$ 才能消去时间依赖。

**从 $v$-$x$ 关系验证**（无需三角函数）：

$$
K + U = \frac{1}{2}mv^2 + \frac{1}{2}kx^2 = \frac{1}{2}m\omega^2(A^2 - x^2) + \frac{1}{2}kx^2
$$

由 $m\omega^2 = k$：
$$
= \frac{1}{2}k(A^2 - x^2) + \frac{1}{2}kx^2 = \frac{1}{2}kA^2
$$

---

#### 7.4.2 🧪 推导 2：能量法中 $v = \pm\omega\sqrt{A^2 - x^2}$ 的两种导出方式

**推导目标**：分别从能量守恒和三角函数恒等式两种途径导出速度-位移关系。

**推导过程**：

**途径一：能量守恒法**（最直接）。

由 $E = \frac{1}{2}mv^2 + \frac{1}{2}kx^2 = \frac{1}{2}kA^2$：

$$
\frac{1}{2}mv^2 = \frac{1}{2}kA^2 - \frac{1}{2}kx^2 = \frac{1}{2}k(A^2 - x^2)
$$

乘以 $2/m$：
$$
v^2 = \frac{k}{m}(A^2 - x^2) = \omega^2(A^2 - x^2)
$$

$$
\boxed{v = \pm\omega\sqrt{A^2 - x^2}}
$$

**途径二：三角函数法**。

由 $x = A\cos(\omega t + \phi)$ → $\cos(\omega t + \phi) = x/A$

由 $v = -A\omega\sin(\omega t + \phi)$，且 $\sin(\omega t + \phi) = \pm\sqrt{1 - \cos^2(\omega t + \phi)}$：

$$
v = -A\omega \cdot \left(\pm\sqrt{1 - \frac{x^2}{A^2}}\right) = \mp \omega\sqrt{A^2 - x^2}
$$

两种途径结果一致。

> 💡 **正负号的含义**：$+$ 表示物块向 $+x$ 方向运动，$-$ 表示向 $-x$ 方向运动。这个符号是两种可能运动方向的体现——在给定 $x$ 处，物块可以向左或向右运动。

---

#### 7.4.2b 🧪 推导 3：从总能量公式导出 $k$ 与振动参数的关系

**推导目标**：证明弹簧劲度系数 $k$ 可以通过测量振幅、质量和最大速度来确定——$k = mv_{\max}^2/A^2$。

**推导过程**：

由总能量守恒：$E = \frac{1}{2}kA^2$

在平衡位置（$x=0$），全部能量为动能：$E = \frac{1}{2}mv_{\max}^2$

两者相等：
$$
\frac{1}{2}kA^2 = \frac{1}{2}mv_{\max}^2
$$

消去 $\frac{1}{2}$：
$$
kA^2 = mv_{\max}^2
$$

$$
\boxed{k = \frac{mv_{\max}^2}{A^2}}
$$

也可写为 $v_{\max} = A\omega = A\sqrt{k/m}$，代入验证一致 ✓。

**实验意义**：在实验中测量 $m$（用天平）、$A$（用尺子）和 $v_{\max}$（用光电门），即可确定 $k$——无需直接测量力。这在弹簧劲度系数难以直接测量的场合（如微型弹簧、生物力学中的肌腱弹性）尤其有用。

---

#### 7.4.2c 🧪 推导 4：能量-位移抛物线——$U(x)$ 与 $E$ 的几何解释

**推导目标**：建立势能抛物线 $U(x) = \frac{1}{2}kx^2$ 的几何图像，阐明 $K(x)$ 和转折点 $x = \pm A$ 的几何含义。

**推导过程**：

势能函数 $U(x) = \frac{1}{2}kx^2$ 是一条开口向上的抛物线，顶点在 $(0, 0)$。

总能量 $E = \frac{1}{2}kA^2$ 是一条水平直线，与 $U(x)$ 相交于 $x = \pm A$。

动能是两线之间的竖直距离：
$$
K(x) = E - U(x) = \frac{1}{2}k(A^2 - x^2)
$$

**几何含义**：
- $x = \pm A$（交点）：$U = E$，$K = 0$——转折点，物块瞬间静止
- $x = 0$（抛物线顶点）：$U = 0$，$K = E$——平衡位置，速度最大
- 抛物线内的区域是「允许区域」（$|x| \leq A$），抛物线外的区域是「禁区」
- 若粒子在抛物线外（$E < U(x)$），动能将为负——在经典力学中不可能

> 💡 **势能抛物线是 SHM 的几何本质**：任何 $U(x) \propto x^2$ 的系统都做 SHM，周期与振幅无关。若 $U(x)$ 不是纯二次函数，振动将是非简谐的——周期依赖于振幅。

---

#### 7.4.3 🧪 例题 1：用能量法求振动参数

**题目**：一个 $m = 0.60\ \text{kg}$ 的物块在 $k = 54\ \text{N/m}$ 的弹簧上做 SHM，振幅 $A = 0.15\ \text{m}$。求：
(a) 系统的总机械能
(b) 物块通过 $x = 0.075\ \text{m}$（$A/2$）时的速度大小
(c) 动能和势能相等时的位移

**题目分析**：

> 能量法：$E = \frac{1}{2}kA^2$，$v = \omega\sqrt{A^2 - x^2}$。

**解答**：

**(a)** $E = \frac{1}{2}kA^2 = \frac{1}{2} \times 54 \times (0.15)^2 = 27 \times 0.0225 = \mathbf{0.608\ \text{J}}$

**(b)** $\omega = \sqrt{k/m} = \sqrt{54/0.60} = \sqrt{90} \approx 9.49\ \text{rad/s}$

$|v| = \omega\sqrt{A^2 - x^2} = 9.49\sqrt{0.0225 - 0.005625} = 9.49\sqrt{0.016875}$

$\approx 9.49 \times 0.1299 \approx \mathbf{1.23\ \text{m/s}}$

$v_{\max} = A\omega = 0.15 \times 9.49 \approx 1.42\ \text{m/s}$，$x = A/2$ 时 $v = \sqrt{3}/2 \cdot v_{\max} \approx 1.23\ \text{m/s}$ ✓

**(c)** $K = U$ → $\frac{1}{2}mv^2 = \frac{1}{2}kx^2$

由能量守恒 $E = K + U = 2U$ → $\frac{1}{2}kA^2 = kx^2$

$$
|x| = \frac{A}{\sqrt{2}} \approx \frac{0.15}{1.414} \approx \mathbf{0.106\ \text{m}}
$$

> 💡 $K = U$ 时 $x = A/\sqrt{2}$ 是一个**与 $\omega$ 和 $m$ 无关**的普适结论——仅由 $E = K + U$ 和 $K = U$ 两个条件推出，适用于任何 SHM 系统。

---

#### 7.4.4 🧪 例题 2：竖直弹簧振子的能量分析

**题目**：一个 $m = 0.80\ \text{kg}$ 的物块悬挂在 $k = 200\ \text{N/m}$ 的竖直弹簧上。物块从平衡位置被拉下 $0.10\ \text{m}$ 后从静止释放。求：
(a) 平衡位置弹簧的伸长量
(b) 以平衡位置为零势面的总机械能
(c) 物块在最低点（释放点）上方 $0.15\ \text{m}$ 处时的速度（该点在平衡位置上方 $0.05\ \text{m}$）

**题目分析**：

> 竖直弹簧振子：以平衡位置为坐标原点和弹性势能零点 + 重力势能零点，则总势能仍为 $\frac{1}{2}kx^2$，能量公式不变。

**解答**：

**(a)** 平衡位置：$k\Delta y_0 = mg$

$$
\Delta y_0 = \frac{mg}{k} = \frac{0.80 \times 9.8}{200} = \frac{7.84}{200} = \mathbf{0.0392\ \text{m} = 3.92\ \text{cm}}
$$

**(b)** 以平衡位置为参考，$A = 0.10\ \text{m}$：

$$
E = \frac{1}{2}kA^2 = \frac{1}{2} \times 200 \times 0.10^2 = \mathbf{1.0\ \text{J}}
$$

> 💡 注意：总能量 $1.0\ \text{J}$ 是弹性势能的变化量 + 重力势能变化量的总和。以平衡位置为参考时，这两个变化量合并为 $\frac{1}{2}kx^2$ 的形式——这就是竖直弹簧振子的优雅之处。

**(c)** $x = +0.05\ \text{m}$（平衡位置上方，取向上为正）：

由 $E = \frac{1}{2}mv^2 + \frac{1}{2}kx^2$：
$$
1.0 = \frac{1}{2} \times 0.80 \times v^2 + \frac{1}{2} \times 200 \times (0.05)^2
$$
$$
1.0 = 0.40v^2 + 0.25
$$
$$
0.40v^2 = 0.75 \quad \Rightarrow \quad v^2 = 1.875
$$
$$
v = \pm\sqrt{1.875} \approx \mathbf{\pm 1.37\ \text{m/s}}
$$

> 💡 **竖直弹簧振子的能量简化**：以平衡位置为参考时，重力被「吸收」进 $\frac{1}{2}kx^2$ 中，能量公式与水平弹簧振子完全相同。这极大简化了计算——你不需要分开处理重力和弹簧力。

---

#### 7.4.5 🧪 例题 3：从能量分布求位移和速度

**题目**：一个 $m = 0.50\ \text{kg}$、$k = 32\ \text{N/m}$ 的 SHM 系统，总能量 $E = 0.36\ \text{J}$。求：
(a) 振幅 $A$
(b) 当动能为势能的 3 倍时，位移是多少？
(c) 此时速度是多少？

**解答**：

**(a)** $A = \sqrt{\dfrac{2E}{k}} = \sqrt{\dfrac{2 \times 0.36}{32}} = \sqrt{0.0225} = \mathbf{0.15\ \text{m}}$

**(b)** $K = 3U$，$E = K + U = 4U$ → $U = E/4$

$\frac{1}{2}kx^2 = \frac{1}{4}E$ → $x^2 = \dfrac{E}{2k} = \dfrac{0.36}{64} = 0.005625$

$|x| = \mathbf{0.075\ \text{m}} = A/2$

**(c)** $K = 3U = 3 \times E/4 = 3 \times 0.09 = 0.27\ \text{J}$

$v = \sqrt{\dfrac{2K}{m}} = \sqrt{\dfrac{0.54}{0.50}} = \sqrt{1.08} \approx \mathbf{1.04\ \text{m/s}}$

验证：$\omega = \sqrt{32/0.50} = 8.0\ \text{rad/s}$，$|v| = \omega\sqrt{A^2 - x^2} = 8.0\sqrt{0.0225 - 0.005625} = 8.0 \times 0.1299 \approx 1.04\ \text{m/s}$ ✓

---

#### 7.4.6 🧪 例题 4：从 $v$-$x$ 数据反推 $k$ 和 $m$

**题目**：一个做 SHM 的物块——在 $x_1 = 0.060\ \text{m}$ 时速度为 $v_1 = 0.80\ \text{m/s}$，在 $x_2 = 0.100\ \text{m}$ 时速度为 $v_2 = 0.40\ \text{m/s}$。振幅 $A = 0.120\ \text{m}$。求：
(a) 角频率 $\omega$
(b) 最大速度 $v_{\max}$

**解答**：

**(a)** 由 $v^2 = \omega^2(A^2 - x^2)$，代入两组数据：

$0.80^2 = \omega^2(0.120^2 - 0.060^2)$ → $0.64 = \omega^2(0.0144 - 0.0036) = \omega^2 \times 0.0108$

$\omega^2 = \dfrac{0.64}{0.0108} \approx 59.26$ → $\omega \approx \mathbf{7.70\ \text{rad/s}}$

用第二组验证：$0.40^2 = 59.26 \times (0.0144 - 0.0100) = 59.26 \times 0.0044 = 0.261$，$\sqrt{0.261} \approx 0.511\ \text{m/s}$——与 $0.40$ 有偏差，可能因数据误差。

**(b)** $v_{\max} = A\omega = 0.120 \times 7.70 \approx \mathbf{0.924\ \text{m/s}}$

> 💡 利用多个 $v$-$x$ 数据点求 $\omega$ 是实验物理中的常用方法——通过 $v^2$ 对 $x^2$ 作图，斜率为 $-\omega^2$，截距为 $\omega^2 A^2$。

---

#### 7.4.7 🧪 例题 5：弹簧分割后的能量守恒

**题目**：一个 $m = 0.40\ \text{kg}$ 的物块连接在 $k = 36\ \text{N/m}$ 的弹簧上，以振幅 $A = 0.10\ \text{m}$ 做 SHM。在物块恰好经过平衡位置时，弹簧被瞬间截去一半（$k$ 变为 $72\ \text{N/m}$）。求：
(a) 截断瞬间物块的动能
(b) 截断后新的振幅
(c) 截断后新的周期

**解答**：

**(a)** 平衡位置时 $U = 0$，$K = E_{\text{before}} = \frac{1}{2}kA^2 = \frac{1}{2} \times 36 \times 0.01 = \mathbf{0.18\ \text{J}}$

**(b)** 截断瞬间 $x = 0$、$v$ 不变 → 动能不变。新系统的总能量仍为 $0.18\ \text{J}$。

$E = \frac{1}{2}k'A'^2$ → $A' = \sqrt{\dfrac{2E}{k'}} = \sqrt{\dfrac{0.36}{72}} = \sqrt{0.005} \approx \mathbf{0.0707\ \text{m}}$

振幅从 $0.10\ \text{m}$ 减小到约 $0.071\ \text{m}$，因为新弹簧更硬，同样能量下变形更小。

**(c)** $T' = 2\pi\sqrt{\dfrac{m}{k'}} = 2\pi\sqrt{\dfrac{0.40}{72}} \approx 2\pi \times 0.0745 \approx \mathbf{0.468\ \text{s}}$

原周期 $T = 2\pi\sqrt{0.40/36} \approx 0.662\ \text{s}$，缩短了约 $29\%$。

> 💡 **弹簧在平衡位置被截断**是特殊情况：此时 $x=0$、$v = v_{\max}$，动能保持连续性。若在非平衡位置截断，则需同时考虑弹性势能的突变。

---

### 本节总结

SHM 的能量核心公式：

1. **$E = \frac{1}{2}kA^2$** — 总能量仅由 $k$ 和 $A$ 决定
2. **$K = \frac{1}{2}k(A^2 - x^2)$** — 动能随位移变化
3. **$U = \frac{1}{2}kx^2$** — 势能随位移变化
4. **$v = \pm\omega\sqrt{A^2 - x^2}$** — 能量守恒的动力学等价物
5. **$K = U$ 时 $x = A/\sqrt{2}$** — 普适结论

# 7.5 单摆与物理摆（Simple and Physical Pendulum）

## Part A：基础层（AP Physics 1 必备）

### 一、单摆——重力驱动的 SHM

> **单摆（Simple Pendulum）** 由一个质点（摆锤）通过轻绳（或轻杆）悬挂在固定点上构成。在小角度摆动下，单摆做近似简谐运动。恢复力来自重力的切向分量。
>
> 单摆的周期（小角度近似）：
> $$
> \boxed{T = 2\pi\sqrt{\frac{L}{g}}}
> $$

单摆是物理学史上最重要的实验工具之一。伽利略用单摆研究落体运动，惠更斯用单摆制造了第一台精确的摆钟，傅科用单摆证明了地球的自转。单摆之所以重要，是因为它的周期只依赖于摆长 $L$ 和重力加速度 $g$——这使得它成为测量 $g$ 的标准方法。

### 二、小角度近似的关键性

> ⚠️ 单摆只在**小角度**（$\theta_{\max} \lesssim 15^\circ$ 即约 $0.26\ \text{rad}$）时近似为 SHM。当摆角较大时，运动仍然是周期性的但不再是简谐运动，周期随振幅增大而增大。

小角度近似的数学基础：$\sin\theta \approx \theta$（当 $\theta \ll 1$，以弧度计）。

| $\theta$ | $\theta$ (rad) | $\sin\theta$ | 相对误差 |
|:--:|:--:|:--:|:--:|
| $5^\circ$ | $0.0873$ | $0.0872$ | $0.1\%$ |
| $10^\circ$ | $0.1745$ | $0.1736$ | $0.5\%$ |
| $15^\circ$ | $0.2618$ | $0.2588$ | $1.1\%$ |
| $30^\circ$ | $0.5236$ | $0.5000$ | $4.7\%$ |
| $60^\circ$ | $1.0472$ | $0.8660$ | $20.9\%$ |

### 三、单摆的能量

单摆的能量在动能和重力势能之间转化。以最低点为零势面：

- 最高点（$\theta = \theta_{\max}$）：$E = mgL(1 - \cos\theta_{\max})$
- 最低点（$\theta = 0$）：$E = \frac{1}{2}mv_{\max}^2$

小角度近似下：$1 - \cos\theta_{\max} \approx \frac{1}{2}\theta_{\max}^2$，$E \approx \frac{1}{2}mgL\theta_{\max}^2$。

### 四、🟣 物理摆（Physical Pendulum）— AP Physics C 独家

> **物理摆（Physical Pendulum）** 是任意形状的刚体绕固定水平轴在重力作用下的摆动。与单摆不同，物理摆的质量分布不可忽略，必须用转动动力学处理。

物理摆的周期：
$$
\boxed{T = 2\pi\sqrt{\frac{I}{mgd}}}
$$

其中 $I$ 是刚体对转轴的转动惯量，$d$ 是从转轴到质心的距离。

**单摆是物理摆的特例**：质点摆锤 → $I = mL^2$，$d = L$ → $T = 2\pi\sqrt{mL^2/(mgL)} = 2\pi\sqrt{L/g}$ ✓

---

#### 7.5.1 🧪 推导 1：单摆周期公式 $T = 2\pi\sqrt{L/g}$ 的推导

**推导目标**：从小角度近似下的恢复力出发，导出单摆的角频率和周期。

**推导过程**：

**第一步**：分析单摆的受力与力矩。

设摆长 $L$，摆角 $\theta$（以竖直向下为零）。重力 $mg$ 的切向分量为 $F_t = -mg\sin\theta$（负号：力使 $\theta$ 减小）。

切向加速度 $a_t = L\alpha = L\dfrac{d^2\theta}{dt^2}$。由牛顿第二定律 $F_t = ma_t$：

$$
-mg\sin\theta = mL\frac{d^2\theta}{dt^2}
$$

**第二步**：小角度近似 $\sin\theta \approx \theta$（$\theta$ 以弧度计）：

$$
\frac{d^2\theta}{dt^2} + \frac{g}{L}\theta = 0
$$

**第三步**：与标准 SHM 微分方程 $\dfrac{d^2x}{dt^2} + \omega^2 x = 0$ 对比：

$$
\omega^2 = \frac{g}{L} \quad \Rightarrow \quad \omega = \sqrt{\frac{g}{L}}
$$

$$
\boxed{T = \frac{2\pi}{\omega} = 2\pi\sqrt{\frac{L}{g}}}
$$

> 💡 **单摆周期的关键特征**：(1) 与摆锤质量无关——伽利略的著名发现；(2) 与振幅无关（小角度）——等时性；(3) 只取决于 $L$ 和 $g$——因此可以用来精确测量 $g$。

**力矩法验证**（转动视角）：

重力对悬点的力矩 $\tau = -mgL\sin\theta$。由 $\tau = I\alpha$，$I = mL^2$：

$$
-mgL\sin\theta = mL^2\frac{d^2\theta}{dt^2}
$$

约去 $mL$：$\dfrac{d^2\theta}{dt^2} + \dfrac{g}{L}\sin\theta = 0$，小角度近似后得相同结果。

---

#### 7.5.2 🧪 推导 2：物理摆周期公式 $T = 2\pi\sqrt{I/(mgd)}$ 的推导

**推导目标**：从转动动力学出发，导出任意形状刚体做小角度摆动的周期公式。

**推导过程**：

**第一步**：建立转动动力学方程。

设刚体绕水平轴 $O$ 旋转，质心距转轴 $d$。摆角 $\theta$ 时，重力对转轴的力矩为：

$$
\tau = -mgd\sin\theta
$$

（负号：力矩使 $\theta$ 减小，指向平衡位置。）

由 $\tau = I\alpha = I\dfrac{d^2\theta}{dt^2}$（$I$ 为绕 $O$ 轴的转动惯量）：

$$
I\frac{d^2\theta}{dt^2} = -mgd\sin\theta
$$

**第二步**：小角度近似 $\sin\theta \approx \theta$：

$$
\frac{d^2\theta}{dt^2} + \frac{mgd}{I}\theta = 0
$$

与 SHM 标准形式对比：$\omega^2 = \dfrac{mgd}{I}$

$$
\boxed{T = 2\pi\sqrt{\frac{I}{mgd}}}
$$

**第三步**：验证——单摆作为特例。

单摆（质点摆锤）：$I = mL^2$，$d = L$：
$$
T = 2\pi\sqrt{\frac{mL^2}{mgL}} = 2\pi\sqrt{\frac{L}{g}}
$$

与单摆周期公式一致 ✓

**物理摆的应用示例**：一根均匀细杆（$M$，$L$）绕一端摆动。

$I = \frac{1}{3}ML^2$，$d = L/2$：
$$
T = 2\pi\sqrt{\frac{\frac{1}{3}ML^2}{Mg \cdot L/2}} = 2\pi\sqrt{\frac{2L}{3g}}
$$

> 💡 均匀细杆绕一端摆动的周期是 $\sqrt{2/3}$ 倍于同长度单摆的周期——因为杆的质量分布在内侧，有效摆长更短。

---

#### 7.5.2b 🧪 推导 3：大角度单摆——非简谐效应的定量分析

**推导目标**：推导大角度单摆的精确运动方程，并展示其周期如何随振幅增大而增大。

**推导过程**：

单摆的精确转动方程（不做小角度近似）：

$$
\frac{d^2\theta}{dt^2} + \frac{g}{L}\sin\theta = 0
$$

这不再是线性微分方程——$\sin\theta$ 不是 $\theta$ 的线性函数。

将 $\sin\theta$ 做泰勒展开：$\sin\theta = \theta - \dfrac{\theta^3}{6} + \dfrac{\theta^5}{120} - \cdots$

取到 $\theta^3$ 项：
$$
\frac{d^2\theta}{dt^2} + \frac{g}{L}\left(\theta - \frac{\theta^3}{6}\right) = 0
$$

这个非线性方程导致周期随振幅增大。精确周期（椭圆积分）的级数展开为：

$$
\boxed{T = 2\pi\sqrt{\frac{L}{g}}\left[1 + \frac{1}{16}\theta_{\max}^2 + \frac{11}{3072}\theta_{\max}^4 + \cdots\right]}
$$

其中 $\theta_{\max}$ 以弧度计。

| $\theta_{\max}$ | 修正因子 | 周期比（$T/T_0$） |
|:--:|:--|:--:|
| $5^\circ$（$0.087\ \text{rad}$） | $1 + 0.00048$ | $1.0005$ |
| $10^\circ$（$0.175\ \text{rad}$） | $1 + 0.00191$ | $1.002$ |
| $30^\circ$（$0.524\ \text{rad}$） | $1 + 0.0171$ | $1.017$ |
| $60^\circ$（$1.047\ \text{rad}$） | $1 + 0.0686$ | $1.069$ |
| $90^\circ$（$1.571\ \text{rad}$） | $1 + 0.154$ | $1.154$ |

> 💡 即使 $\theta_{\max} = 30^\circ$，周期也仅比小角度近似长约 $1.7\%$——所以在大多数实际场合（如钟摆），小角度近似已足够精确。只有在大振幅（$>45^\circ$）的精密实验中才需要考虑修正。

---

#### 7.5.2c 🧪 推导 4：可逆摆（Kater's Pendulum）的等效摆长

**推导目标**：证明物理摆存在一个「等效单摆长度」$L_{\text{eq}} = I/(md)$，使得物理摆的周期等于该长度单摆的周期。

**推导过程**：

物理摆周期：
$$
T = 2\pi\sqrt{\frac{I}{mgd}}
$$

令 $L_{\text{eq}} = \dfrac{I}{md}$，则：
$$
T = 2\pi\sqrt{\frac{L_{\text{eq}}}{g}}
$$

形式上与单摆周期完全相同。$L_{\text{eq}}$ 称为**等效摆长**。

**均匀细杆绕端点**：$I = \frac{1}{3}ML^2$，$d = L/2$

$$
L_{\text{eq}} = \frac{\frac{1}{3}ML^2}{M \cdot L/2} = \frac{2}{3}L
$$

这意味着绕端点摆动的均匀杆「感觉」像一根长度为 $2L/3$ 的单摆。

**打击中心（Center of Percussion）**：在杆上距转轴 $L_{\text{eq}} = 2L/3$ 处施加一个冲量，转轴处不会感受到反冲力——这就是棒球棒「甜点」的物理原理。

> 💡 等效摆长概念统一了单摆和物理摆——任何物理摆都可以用一个等效单摆来替代。这在工程设计中极为有用——你不需要重新计算每个复杂摆的周期，只需找到它的 $L_{\text{eq}}$。

---

#### 7.5.3 🧪 例题 1：单摆周期的实验分析

**题目**：一个单摆在地球表面（$g = 9.8\ \text{m/s}^2$）的周期为 $T_E = 2.0\ \text{s}$。求：
(a) 摆长 $L$
(b) 同一个摆在月球表面（$g_M = 1.6\ \text{m/s}^2$）的周期
(c) 若要使月球上的周期与地球上相同，摆长应如何调整？

**题目分析**：

> **已知**：$T_E = 2.0\ \text{s}$，$g_E = 9.8\ \text{m/s}^2$
>
> **求**：$L$、$T_M$、$L_M$

**解答**：

**(a)** $L = \dfrac{g_E T_E^2}{4\pi^2} = \dfrac{9.8 \times 4.0}{4\pi^2} = \dfrac{39.2}{39.48} \approx \mathbf{0.993\ \text{m}}$

**(b)** $T_M = 2\pi\sqrt{\dfrac{L}{g_M}} = 2\pi\sqrt{\dfrac{0.993}{1.6}} \approx 2\pi \times 0.788 \approx \mathbf{4.95\ \text{s}}$

月球上周期约是地球上的 $2.47$ 倍——因为 $\sqrt{g_E/g_M} = \sqrt{9.8/1.6} \approx 2.47$。

**(c)** $T_M = T_E$ 要求 $L_M/g_M = L_E/g_E$：
$$
L_M = L_E \cdot \frac{g_M}{g_E} = 0.993 \times \frac{1.6}{9.8} \approx \mathbf{0.162\ \text{m}}
$$

> 💡 月球上 $g$ 约为地球的 $1/6$，要在月球上获得相同周期，摆长需缩短到原来的 $1/6$。

---

#### 7.5.4 🧪 例题 2：物理摆——均匀杆的周期

**题目**：一根均匀细杆（$M = 0.50\ \text{kg}$，$L = 0.80\ \text{m}$）可绕通过一端且垂直于杆的水平轴自由摆动。求：
(a) 绕转轴的转动惯量
(b) 小角度摆动的周期
(c) 若在杆的另一端附加一个 $m = 0.30\ \text{kg}$ 的质点，周期变为多少？

**题目分析**：

> 物理摆 $T = 2\pi\sqrt{I/(mgd)}$，需要求绕转轴的 $I$ 和质心到转轴的距离 $d$。

**解答**：

**(a)** $I = \frac{1}{3}ML^2 = \frac{1}{3} \times 0.50 \times 0.80^2 \approx \mathbf{0.1067\ \text{kg·m}^2}$

$d = L/2 = 0.40\ \text{m}$

**(b)** $T = 2\pi\sqrt{\dfrac{I}{Mgd}} = 2\pi\sqrt{\dfrac{0.1067}{0.50 \times 9.8 \times 0.40}}$

$= 2\pi\sqrt{\dfrac{0.1067}{1.96}} \approx 2\pi\sqrt{0.0544} \approx \mathbf{1.47\ \text{s}}$

**(c)** 附加质点后：

系统总质量 $M_{\text{tot}} = 0.50 + 0.30 = 0.80\ \text{kg}$

新质心位置（以转轴为原点）：
$$
d' = \frac{M \cdot L/2 + m \cdot L}{M + m} = \frac{0.50 \times 0.40 + 0.30 \times 0.80}{0.80} = \frac{0.20 + 0.24}{0.80} = 0.55\ \text{m}
$$

新转动惯量：$I' = \frac{1}{3}ML^2 + mL^2 = 0.1067 + 0.30 \times 0.64 = 0.1067 + 0.192 = 0.2987\ \text{kg·m}^2$

$$
T' = 2\pi\sqrt{\frac{I'}{M_{\text{tot}}gd'}} = 2\pi\sqrt{\frac{0.2987}{0.80 \times 9.8 \times 0.55}} \approx 2\pi\sqrt{\frac{0.2987}{4.312}} \approx \mathbf{1.65\ \text{s}}
$$

> 💡 附加质量在远端同时增大了 $I$ 和 $d$，且增大了总质量。由于 $T \propto \sqrt{I/(Md)}$，各因素的综合效果是周期略有增加。

---

#### 7.5.5 🧪 例题 3：单摆的能量与速度

**题目**：一个 $L = 1.5\ \text{m}$ 的单摆被拉到与竖直方向成 $\theta_0 = 20^\circ$ 后释放。摆锤质量 $m = 0.30\ \text{kg}$。求：
(a) 小角度近似的周期（并评估 $20^\circ$ 的误差）
(b) 摆锤在最低点的速度
(c) 摆锤在 $\theta = 10^\circ$ 时的速度

**解答**：

**(a)** $T \approx 2\pi\sqrt{1.5/9.8} \approx 2.46\ \text{s}$。

$\theta_0 = 20^\circ \approx 0.349\ \text{rad}$，修正项约 $(\theta_0/4)^2 = 0.0076$，误差约 $0.76\%$。

**(b)** $h_{\max} = L(1 - \cos 20^\circ) = 1.5 \times 0.0603 \approx 0.0905\ \text{m}$

$v_{\max} = \sqrt{2gh_{\max}} \approx \sqrt{2 \times 9.8 \times 0.0905} \approx \mathbf{1.33\ \text{m/s}}$

**(c)** $h = L(\cos 10^\circ - \cos 20^\circ) = 1.5 \times (0.9848 - 0.9397) = 0.0677\ \text{m}$

$v = \sqrt{2g(h_{\max} - h)} = \sqrt{2 \times 9.8 \times (0.0905 - 0.0677)} \approx \mathbf{0.668\ \text{m/s}}$

---

#### 7.5.6 🧪 例题 4：傅科摆——地球自转的证明

**题目**：傅科在 1851 年在巴黎先贤祠悬挂了一个 $L = 67\ \text{m}$ 的单摆，摆锤质量 $28\ \text{kg}$。求：
(a) 该傅科摆在地球表面（$g = 9.81\ \text{m/s}^2$）的周期
(b) 若摆锤的振幅为 $3.0\ \text{m}$（水平位移），最大角位移是多少度？
(c) 该角度下非简谐修正有多大？是否可忽略？

**解答**：

**(a)** $T = 2\pi\sqrt{\dfrac{67}{9.81}} \approx 2\pi\sqrt{6.83} \approx \mathbf{16.4\ \text{s}}$

**(b)** $\theta_{\max} = \arcsin(3.0/67) \approx \arcsin(0.0448) \approx \mathbf{2.57^\circ}$

**(c)** $\theta_{\max} \approx 0.0448\ \text{rad}$，修正项 $\theta_{\max}^2/16 \approx 0.000125$——仅约 $0.0125\%$ 的修正，完全可忽略。

> 💡 傅科摆是物理学史上最著名的演示实验之一。摆动平面以每小时约 $11^\circ$ 的速率旋转（在巴黎纬度），直接证明了地球的自转——无需观测星空，仅凭地面实验就能确认哥白尼是正确的。

---

#### 7.5.7 🧪 例题 5：三线摆——测量转动惯量

**题目**：一个均匀圆盘（$M = 2.0\ \text{kg}$，$R = 0.15\ \text{m}$）用三根等长 $L = 0.50\ \text{m}$ 的细线悬挂，线在盘上的连接点距盘中心 $r = 0.10\ \text{m}$。当盘绕其中心轴做小角度扭转摆动时，周期为 $T = 1.80\ \text{s}$。用此数据求圆盘的转动惯量，并与理论值 $I = \frac{1}{2}MR^2$ 比较。

**题目分析**：

> 三线摆中，恢复力矩来自悬线倾斜产生的重力矩。扭转角 $\theta$ 和盘的上升高度之间有几何关系。

**解答**：

三线摆的周期公式为 $T = 2\pi\sqrt{\dfrac{IL}{Mgr^2}}$，其中 $I$ 为绕垂直轴的转动惯量。

解出 $I$：
$$
I = \frac{Mgr^2 T^2}{4\pi^2 L} = \frac{2.0 \times 9.8 \times 0.10^2 \times 1.80^2}{4\pi^2 \times 0.50}
$$

$$
= \frac{2.0 \times 9.8 \times 0.01 \times 3.24}{4 \times 9.87 \times 0.50} \approx \frac{0.635}{19.74} \approx \mathbf{0.0322\ \text{kg·m}^2}
$$

理论值：$I_{\text{theory}} = \frac{1}{2}MR^2 = \frac{1}{2} \times 2.0 \times 0.0225 = \mathbf{0.0225\ \text{kg·m}^2}$

偏差约 $43\%$——较大，可能因为连接点不完全在盘边缘处，或盘并非理想均匀。

> 💡 三线摆是实验室测量转动惯量的标准方法——无需知道材料的密度分布，只需测量摆动周期即可反推出 $I$。这在复杂形状物体的转动惯量测量中尤为有用。

---

### 本节总结

单摆与物理摆的核心公式：

| 系统 | 周期 | $\omega$ | 条件 |
|:--|:--|:--|:--|
| 单摆 | $T = 2\pi\sqrt{L/g}$ | $\sqrt{g/L}$ | 小角度 |
| 物理摆 | $T = 2\pi\sqrt{I/(mgd)}$ | $\sqrt{mgd/I}$ | 小角度 |

---

# 🟣 AP Physics C 微积分扩展

## C.1 SHM 微分方程的严格求解

SHM 的标准微分方程：

$$
\frac{d^2x}{dt^2} + \omega^2 x = 0
$$

**特征方程法**：设 $x = e^{rt}$，代入得 $r^2 e^{rt} + \omega^2 e^{rt} = 0$ → $r^2 + \omega^2 = 0$ → $r = \pm i\omega$。

通解：
$$
x(t) = C_1 e^{i\omega t} + C_2 e^{-i\omega t} = C_1\cos(\omega t) + C_2\sin(\omega t)
$$

使用三角恒等式可改写为 $x = A\cos(\omega t + \phi)$，其中 $A = \sqrt{C_1^2 + C_2^2}$，$\phi = \arctan(-C_2/C_1)$。

**解的物理意义**：两个积分常数（$C_1$、$C_2$ 或 $A$、$\phi$）由两个初始条件（$x_0$、$v_0$）唯一确定——这是二阶微分方程的通性。

## C.2 阻尼振动（Damped Oscillations）

当存在与速度成正比的阻尼力 $F_d = -bv$ 时：

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0
$$

标准化：$\dfrac{d^2x}{dt^2} + 2\beta\dfrac{dx}{dt} + \omega_0^2 x = 0$，其中 $\beta = \dfrac{b}{2m}$，$\omega_0 = \sqrt{\dfrac{k}{m}}$。

**三种阻尼状态**：

| 状态 | 条件 | 解的形式 | 物理表现 |
|:--|:--|:--|:--|
| **欠阻尼** | $\beta < \omega_0$ | $x(t) = A_0 e^{-\beta t}\cos(\omega_1 t + \phi)$ | 振幅指数衰减，仍能振荡 |
| **临界阻尼** | $\beta = \omega_0$ | $x(t) = (A + Bt)e^{-\beta t}$ | 最快回到平衡，不振荡 |
| **过阻尼** | $\beta > \omega_0$ | $x(t) = e^{-\beta t}(C_1 e^{\gamma t} + C_2 e^{-\gamma t})$ | 缓慢回到平衡，不振荡 |

欠阻尼角频率：$\omega_1 = \sqrt{\omega_0^2 - \beta^2}$（小于自然频率 $\omega_0$）。

**品质因子**：$Q = \dfrac{\omega_0}{2\beta}$——$Q$ 越大，阻尼越小，振动持续越久。

## C.3 受迫振动与共振（Forced Oscillations & Resonance）

外力 $F(t) = F_0\cos(\omega t)$ 驱动下的稳态解：

$$
x(t) = A(\omega)\cos(\omega t - \delta)
$$

其中振幅：
$$
A(\omega) = \frac{F_0/m}{\sqrt{(\omega_0^2 - \omega^2)^2 + (2\beta\omega)^2}}
$$

**共振频率**：使振幅最大的驱动频率 $\omega_r = \sqrt{\omega_0^2 - 2\beta^2}$。

**共振的物理后果**：
- 轻阻尼（$\beta \ll \omega_0$）：$\omega_r \approx \omega_0$，振幅极大 → 可能导致结构破坏（塔科马海峡大桥）
- 重阻尼（$\beta \gg \omega_0$）：共振峰不明显，振幅始终较小

**相位滞后**：$\tan\delta = \dfrac{2\beta\omega}{\omega_0^2 - \omega^2}$
- $\omega \ll \omega_0$：$\delta \approx 0$（位移与驱动力同相）
- $\omega = \omega_0$：$\delta = \pi/2$（位移落后驱动力 $90^\circ$）
- $\omega \gg \omega_0$：$\delta \approx \pi$（位移与驱动力反相）

## C.4 大角度单摆——非简谐效应

大角度单摆的精确周期（椭圆积分展开）：

$$
T = 2\pi\sqrt{\frac{L}{g}}\left[1 + \frac{1}{16}\theta_{\max}^2 + \frac{11}{3072}\theta_{\max}^4 + \frac{173}{737280}\theta_{\max}^6 + \cdots\right]
$$

$\theta_{\max} = 30^\circ$ 时，周期仅比小角度近似长约 $1.7\%$。$\theta_{\max} = 90^\circ$ 时，周期长约 $15.4\%$。

## C.5 耦合振子简介

SHM 的标准微分方程：

$$
\frac{d^2x}{dt^2} + \omega^2 x = 0
$$

特征方程 $r^2 + \omega^2 = 0$ → $r = \pm i\omega$。通解：

$$
x(t) = C_1\cos(\omega t) + C_2\sin(\omega t)
$$

使用三角恒等式可改写为 $x = A\cos(\omega t + \phi)$，其中 $A = \sqrt{C_1^2 + C_2^2}$。

## C.2 阻尼振动（Damped Oscillations）

$$
\frac{d^2x}{dt^2} + 2\beta\frac{dx}{dt} + \omega_0^2 x = 0
$$

欠阻尼（$\beta < \omega_0$）：$x(t) = A_0 e^{-\beta t}\cos(\omega_1 t + \phi)$，$\omega_1 = \sqrt{\omega_0^2 - \beta^2}$

## C.3 受迫振动与共振（Forced Oscillations & Resonance）

$$
\frac{d^2x}{dt^2} + 2\beta\frac{dx}{dt} + \omega_0^2 x = F_0\cos(\omega t)
$$

共振频率 $\omega_r = \sqrt{\omega_0^2 - 2\beta^2}$，共振时振幅最大。

## C.4 大角度单摆——非简谐效应

大角度单摆的精确周期（椭圆积分）：

$$
T = 2\pi\sqrt{\frac{L}{g}}\left[1 + \frac{1}{16}\theta_{\max}^2 + \frac{11}{3072}\theta_{\max}^4 + \cdots\right]
$$

$\theta_{\max} = 30^\circ$ 时，周期仅比小角度近似长约 $1.7\%$。

---

# Ch7 综合例题

## 综合题 1：弹簧振子的全分析

**题目**：$m = 0.40\ \text{kg}$ 的物块在 $k = 25\ \text{N/m}$ 的弹簧上做 SHM。$t = 0$ 时，$x_0 = -0.080\ \text{m}$，$v_0 = +0.60\ \text{m/s}$。求：
(a) $\omega$、$T$、$f$
(b) 振幅 $A$ 和初相位 $\phi$
(c) $x(t)$ 和 $v(t)$
(d) 总机械能
(e) $x = +0.040\ \text{m}$ 时的速度

**解答**：

**(a)** $\omega = \sqrt{25/0.40} \approx 7.91\ \text{rad/s}$，$T \approx 0.795\ \text{s}$，$f \approx 1.26\ \text{Hz}$

**(b)** $A = \sqrt{(-0.080)^2 + (0.60/7.91)^2} \approx \sqrt{0.0064 + 0.00575} \approx 0.110\ \text{m}$

$\tan\phi = -v_0/(\omega x_0) = -0.60/(7.91 \times (-0.080)) \approx 0.948$ → $\phi \approx 0.759\ \text{rad}$ 或 $\phi + \pi$。

由 $x_0 = A\cos\phi$ 且 $x_0 < 0$ → $\cos\phi < 0$ → $\phi \approx 0.759 + \pi \approx 3.90\ \text{rad}$（或 $-2.38\ \text{rad}$）。

**(c)** $x(t) \approx 0.110\cos(7.91t + 3.90)\ \text{m}$，$v(t) \approx -0.870\sin(7.91t + 3.90)\ \text{m/s}$

**(d)** $E = \frac{1}{2}kA^2 \approx 0.151\ \text{J}$

**(e)** $|v| = \omega\sqrt{A^2 - x^2} \approx 7.91\sqrt{0.0121 - 0.0016} \approx 0.811\ \text{m/s}$

## 综合题 2：单摆的能量与速度

**题目**：一个 $L = 1.5\ \text{m}$ 的单摆被拉到与竖直方向成 $\theta_0 = 20^\circ$ 后释放。摆锤质量 $m = 0.30\ \text{kg}$。求：
(a) 小角度近似的周期（并评估 $20^\circ$ 的误差）
(b) 摆锤在最低点的速度
(c) 摆锤在 $\theta = 10^\circ$ 时的速度

**解答**：

**(a)** $T \approx 2\pi\sqrt{1.5/9.8} \approx 2.46\ \text{s}$。

$\theta_0 = 20^\circ \approx 0.349\ \text{rad}$，修正项约 $(\theta_0/4)^2 = 0.0076$，误差约 $0.76\%$。

**(b)** $h_{\max} = L(1 - \cos 20^\circ) = 1.5 \times 0.0603 \approx 0.0905\ \text{m}$

$v_{\max} = \sqrt{2gh_{\max}} \approx \sqrt{2 \times 9.8 \times 0.0905} \approx \mathbf{1.33\ \text{m/s}}$

**(c)** $h = L(\cos 10^\circ - \cos 20^\circ) = 1.5 \times (0.9848 - 0.9397) = 0.0677\ \text{m}$

$v = \sqrt{2g(h_{\max} - h)} = \sqrt{2 \times 9.8 \times (0.0905 - 0.0677)} \approx \mathbf{0.668\ \text{m/s}}$

## 综合题 3：两弹簧串联-并联混合系统

**题目**：两根弹簧 $k_1 = 100\ \text{N/m}$ 和 $k_2 = 200\ \text{N/m}$ 以以下方式连接 $m = 2.0\ \text{kg}$ 的物块：
(a) 两弹簧并联后连接物块
(b) 两弹簧串联后连接物块
(c) $k_1$ 和 $k_2$ 先串联再与另一根 $k_3 = 150\ \text{N/m}$ 并联
求各种情况下的周期。

**解答**：

**(a)** $k_{\text{eff}} = 100 + 200 = 300\ \text{N/m}$，$T = 2\pi\sqrt{2.0/300} \approx \mathbf{0.513\ \text{s}}$

**(b)** $k_{\text{eff}} = \left(\frac{1}{100} + \frac{1}{200}\right)^{-1} = 66.7\ \text{N/m}$，$T = 2\pi\sqrt{2.0/66.7} \approx \mathbf{1.088\ \text{s}}$

**(c)** 串联部分 $k_{12} = 66.7\ \text{N/m}$，并联：$k_{\text{eff}} = 66.7 + 150 = 216.7\ \text{N/m}$

$T = 2\pi\sqrt{2.0/216.7} \approx \mathbf{0.603\ \text{s}}$

## 综合题 4：阻尼振动的对数衰减率

**题目**：（🟣 C 版）一个阻尼振子（$m = 0.50\ \text{kg}$，$k = 32\ \text{N/m}$，阻尼系数 $b = 1.5\ \text{kg/s}$）做欠阻尼振动。相邻两次同方向经过平衡位置的时间间隔为 $T_d = 0.80\ \text{s}$。求：
(a) 无阻尼时的自然角频率 $\omega_0$
(b) 阻尼因子 $\beta = b/(2m)$
(c) 阻尼角频率 $\omega_1 = \sqrt{\omega_0^2 - \beta^2}$
(d) 振幅在 5 个周期后衰减到初始的百分之几

**解答**：

**(a)** $\omega_0 = \sqrt{k/m} = \sqrt{32/0.50} = \mathbf{8.0\ \text{rad/s}}$

**(b)** $\beta = b/(2m) = 1.5/1.0 = \mathbf{1.5\ \text{s}^{-1}}$

**(c)** $\omega_1 = \sqrt{8.0^2 - 1.5^2} = \sqrt{64 - 2.25} \approx \mathbf{7.86\ \text{rad/s}}$，$T_d = 2\pi/7.86 \approx 0.80\ \text{s}$ ✓

**(d)** $A(t) = A_0 e^{-\beta t}$，5 个周期：$t = 5T_d = 4.0\ \text{s}$

$A/A_0 = e^{-1.5 \times 4.0} = e^{-6.0} \approx \mathbf{0.0025 = 0.25\%}$

## 综合题 5：共振频率的确定

**题目**：（🟣 C 版）一个受迫振子（$m = 0.50\ \text{kg}$，$k = 32\ \text{N/m}$，$\beta = 1.5\ \text{s}^{-1}$）受外力 $F(t) = F_0\cos(\omega t)$ 驱动。求：
(a) 自然频率 $f_0$
(b) 共振角频率 $\omega_r = \sqrt{\omega_0^2 - 2\beta^2}$
(c) 共振时驱动力的周期

**解答**：

**(a)** $f_0 = \dfrac{\omega_0}{2\pi} = \dfrac{8.0}{2\pi} \approx \mathbf{1.27\ \text{Hz}}$

**(b)** $\omega_r = \sqrt{64 - 2 \times 2.25} = \sqrt{59.5} \approx \mathbf{7.71\ \text{rad/s}}$

**(c)** $T_r = \dfrac{2\pi}{\omega_r} = \dfrac{2\pi}{7.71} \approx \mathbf{0.815\ \text{s}}$

> 💡 共振频率 $\omega_r$ 略小于自然频率 $\omega_0$——阻尼使共振峰向低频方向偏移。对于轻阻尼（$\beta \ll \omega_0$），$\omega_r \approx \omega_0$。

## 综合题 6：两个质量耦合的 SHM

**题目**：两个物块 $m_1 = 2.0\ \text{kg}$ 和 $m_2 = 1.0\ \text{kg}$ 由一根 $k = 120\ \text{N/m}$ 的弹簧连接，放在光滑水平面上。初始时弹簧被压缩 $0.15\ \text{m}$ 后同时释放两物块。求：
(a) 每个物块的振幅（以质心为参考）
(b) 每个物块的振动角频率
(c) 振动周期

**题目分析**：

> 双体 SHM：两物块以质心为中心做相对振动。等效约化质量 $\mu = m_1 m_2/(m_1 + m_2)$。

**解答**：

**(a)** 质心位置（从 $m_1$ 量起）：$x_{cm} = \dfrac{m_2 L}{m_1 + m_2}$，其中 $L$ 为弹簧原长。两物块到质心的距离之比等于质量反比：

$m_1$ 距质心 $d_1 = \dfrac{m_2}{m_1 + m_2} \times \text{弹簧原长}$

初始压缩 $0.15\ \text{m}$ 由两物块按质量反比分担：

$A_1 = 0.15 \times \dfrac{m_2}{m_1 + m_2} = 0.15 \times \dfrac{1.0}{3.0} = \mathbf{0.050\ \text{m}}$

$A_2 = 0.15 \times \dfrac{m_1}{m_1 + m_2} = 0.15 \times \dfrac{2.0}{3.0} = \mathbf{0.100\ \text{m}}$

**(b)** 等效约化质量 $\mu = \dfrac{m_1 m_2}{m_1 + m_2} = \dfrac{2.0 \times 1.0}{3.0} = \dfrac{2}{3}\ \text{kg} \approx 0.667\ \text{kg}$

每个物块绕质心的振动角频率相同：
$$
\omega = \sqrt{\frac{k}{\mu}} = \sqrt{\frac{120}{0.667}} = \sqrt{180} \approx \mathbf{13.4\ \text{rad/s}}
$$

**(c)** $T = \dfrac{2\pi}{\omega} = \dfrac{2\pi}{13.4} \approx \mathbf{0.469\ \text{s}}$

> 💡 **约化质量** $\mu$ 是双体 SHM 的核心概念。两个物体绕质心的振动等价于一个质量为 $\mu$ 的物体连接在同一弹簧上的 SHM。当 $m_1 = m_2$ 时 $\mu = m/2$，$\omega = \sqrt{2k/m}$——比单物块快 $\sqrt{2}$ 倍。

## 综合题 7：SHM 与圆周运动投影的数值验证

**题目**：一个质点以 $v = 3.0\ \text{m/s}$ 做半径 $R = 0.20\ \text{m}$ 的匀速圆周运动。求：
(a) 其 $x$ 轴投影 SHM 的 $A$、$\omega$、$T$
(b) 当圆上质点转过的角度 $\theta = 60^\circ$ 时，SHM 投影的 $x$、$v$、$a$
(c) 用 SHM 公式验证 (b) 的结果（取 $\phi = 0$）

**解答**：

**(a)** $A = R = 0.20\ \text{m}$，$\omega = v/R = 3.0/0.20 = 15\ \text{rad/s}$，$T = 2\pi/15 \approx 0.419\ \text{s}$

**(b)** $\theta = 60^\circ = \pi/3\ \text{rad}$：

$x = R\cos\theta = 0.20 \times 0.5 = \mathbf{0.10\ \text{m}}$

$v_x = -v\sin\theta = -3.0 \times 0.866 = \mathbf{-2.60\ \text{m/s}}$

$a_x = -\dfrac{v^2}{R}\cos\theta = -\dfrac{9.0}{0.20} \times 0.5 = \mathbf{-22.5\ \text{m/s}^2}$

**(c)** SHM 公式验证：取 $\omega t = \theta = \pi/3$

$x = A\cos(\omega t) = 0.20 \times 0.5 = 0.10\ \text{m}$ ✓

$v = -A\omega\sin(\omega t) = -0.20 \times 15 \times 0.866 = -2.60\ \text{m/s}$ ✓

$a = -A\omega^2\cos(\omega t) = -0.20 \times 225 \times 0.5 = -22.5\ \text{m/s}^2$ ✓

> 💡 SHM 的参考圆法不仅是理解工具——它在数值上精确等价。任何 SHM 问题都可以通过想象一个对应的圆周运动来直观地解决。

---

## ⚠️ 常见误区辨析

### 误区 1：混淆角频率 $\omega$ 与角速度

> $\omega$ 在 SHM 中是**角频率**（相位变化率，单位 rad/s），不是物体的角速度。对于弹簧振子，物体做直线往复运动，根本不存在「角速度」——$\omega$ 只是一个数学参数。只有在参考圆模型中，$\omega$ 才对应圆周运动的角速度。

### 误区 2：认为 $T = 2\pi\sqrt{m/k}$ 对所有振动都成立

> 这个公式仅适用于弹簧-质量系统的 SHM。单摆的周期是 $T = 2\pi\sqrt{L/g}$，物理摆是 $T = 2\pi\sqrt{I/(mgd)}$。虽然形式相似（都是 $2\pi\sqrt{\text{惯性/恢复}}$），但物理内容完全不同。

### 误区 3：竖直弹簧振子的周期与水平弹簧振子不同

> 错！重力只改变平衡位置，不改变 $\omega$ 和 $T$。竖直弹簧振子的 $\omega = \sqrt{k/m}$ 与水平完全相同。恒定外力不会改变 SHM 的频率——这是 SHM 最深刻的性质之一。

### 误区 4：在最大位移处速度为零所以加速度也为零

> 错！在 $x = \pm A$ 处 $v = 0$ 但 $a = \mp A\omega^2$（加速度达到最大值）。速度为零是因为物块在瞬间改变了运动方向——这恰恰需要最大的加速度来实现。$a$ 与 $x$ 反相而非同相。

### 误区 5：忘记 $\phi$ 由初始条件决定

> 振幅 $A$ 和初相位 $\phi$ 都需要从 $x_0$ 和 $v_0$ 确定。常见的错误是只由 $x_0$ 确定 $A$（$A = |x_0|$），但这不是普遍成立的——只有当 $v_0 = 0$ 时振幅才等于初始位移。一般情况下 $A = \sqrt{x_0^2 + (v_0/\omega)^2}$。

### 误区 6：认为动能和势能相等的位置是 $x = A/2$

> 错！$K = U$ 要求 $\frac{1}{2}mv^2 = \frac{1}{2}kx^2$，由 $E = K + U = 2U = kx^2$ 和 $E = \frac{1}{2}kA^2$ 得 $x = A/\sqrt{2} \approx 0.707A$，不是 $A/2$。$x = A/2$ 时 $K = 3U$，动能是势能的三倍。

### 误区 7：混淆单摆的角位移 $\theta$ 与 SHM 的相位 $\omega t + \phi$

> 在单摆中 $\theta(t) = \theta_{\max}\cos(\omega t + \phi)$，这里的 $\theta(t)$ 是角位移（物理量），$\omega t + \phi$ 是相位（数学参数）。单摆的 $\theta$ 既是描述摆位置的物理变量，又在数学形式上遵循 SHM 的余弦函数——但角位移和相位是两个不同的概念。

### 误区 8：大角度单摆仍是 SHM

> 当 $\theta_{\max} > 15^\circ$ 时，$\sin\theta \neq \theta$，恢复力不再是线性的，周期开始随振幅增大而变化。严格来说，大角度单摆是「非线性振动」而非 SHM。AP Physics 1 考试中除非特别说明，单摆问题均假定小角度近似成立。

---

> **📚 第七章核心回顾**：
>
> 1. **SHM 定义**：$F = -kx$，$a = -\omega^2 x$
> 2. **弹簧周期**：$T = 2\pi\sqrt{m/k}$，$\omega = \sqrt{k/m}$
> 3. **运动学**：$x = A\cos(\omega t + \phi)$，$v = -A\omega\sin(\omega t + \phi)$，$a = -\omega^2 x$
> 4. **能量**：$E = \frac{1}{2}kA^2 = \frac{1}{2}mv^2 + \frac{1}{2}kx^2$
> 5. **单摆**：$T = 2\pi\sqrt{L/g}$（小角度）
> 6. **物理摆**：$T = 2\pi\sqrt{I/(mgd)}$（C 版）
>
> 振动是宇宙的韵律——从原子的量子振动到星系的引力振荡，SHM 是理解这一切的数学钥匙。