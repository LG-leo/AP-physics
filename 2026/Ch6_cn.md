<!-- markdownlint-disable MD033 MD041 -->

<div align="center">

# 📚 AP Physics — 旋转系统的能量与动量

> **Energy & Momentum of Rotating Systems — 完整综合版**
>
> 覆盖 AP Physics 1（代数）+ AP Physics C（微积分）全难度层级

[![AP Physics](https://img.shields.io/badge/AP-Physics-001845?style=for-the-badge&logo=apache&logoColor=white)](https://ap.collegeboard.org/)
[![Physics 1](https://img.shields.io/badge/AP%20Physics-1-FF6B35?style=flat-square)]()
[![Physics C](https://img.shields.io/badge/AP%20Physics-C-004E89?style=flat-square)]()

</div>

---

## 📑 目录

- [6.1 转动动能](#61-转动动能rotational-kinetic-energy)
- [6.2 力矩与功](#62-力矩与功work-and-torque)
- [6.3 角动量与角冲量](#63-角动量与角冲量angular-momentum-and-angular-impulse)
- [6.4 角动量守恒](#64-角动量守恒conservation-of-angular-momentum)
- [6.5 滚动](#65-滚动rolling)
- [6.6 卫星轨道运动](#66-卫星轨道运动satellite-orbital-motion)
- [综合例题](#ch6-综合例题)

---

# 6.1 转动动能（Rotational Kinetic Energy）

## Part A：基础层（AP Physics 1 必备）

### 一、转动动能的物理本质

> **转动动能（Rotational Kinetic Energy）** 是刚体因绕轴旋转而具有的动能，等于物体上所有质量元的平动动能之和。转动动能与平动动能形式完全对应——将质量 $m$ 替换为转动惯量 $I$，将线速度 $v$ 替换为角速度 $\omega$。
>
> $$
> \boxed{K_{\text{rot}} = \frac{1}{2}I\omega^2}
> $$

转动动能是第六章的「能量入口」。在 AP 物理考试中，涉及转动的问题几乎总可以通过能量守恒来简化——这正是转动动能的核心价值。掌握了 $K_{\text{rot}} = \frac{1}{2}I\omega^2$，你就打开了用能量方法解决转动问题的大门。

### 二、平动与转动动能的对应

| 平动 | 转动 | 对应关系 |
|:--|:--|:--|
| $K_{\text{trans}} = \frac{1}{2}mv^2$ | $K_{\text{rot}} = \frac{1}{2}I\omega^2$ | $m \leftrightarrow I$，$v \leftrightarrow \omega$ |
| 动能取决于质量和速度 | 动能取决于转动惯量和角速度 | — |
| 单位：$\text{J}$（焦耳） | 单位：$\text{J}$（焦耳） | 相同 |

### 三、总动能 = 平动动能 + 转动动能

对于同时进行平动和转动的刚体（如滚动的球），总动能为两部分之和：

$$
\boxed{K_{\text{total}} = \frac{1}{2}Mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2}
$$

> ⚠️ **关键注意**：转动动能必须用**绕质心的转动惯量** $I_{cm}$ 来计算，除非物体绕固定轴旋转。这是初学者最容易混淆的地方——滚动中的转动是对质心的，不是对地面接触点的！

### 四、转动动能的物理直觉

- **$I$ 越大** → 同样 $\omega$ 下转动动能越大（更难加速，但也储存更多能量）
- **$\omega$ 以平方出现** → 角速度翻倍，转动动能变为 4 倍
- **飞轮储能**正是利用 $K \propto I\omega^2$ 的特性——大 $I$ + 高 $\omega$ = 巨大储能

### 五、转动动能与平动动能的深度比较

#### 5.1 公式结构的对称性

转动动能公式 $K_{\text{rot}} = \frac{1}{2}I\omega^2$ 与平动动能 $K_{\text{trans}} = \frac{1}{2}mv^2$ 之间的对应并非巧合。它们都源自同一个基本公式 $K = \frac{1}{2} \times (\text{惯量}) \times (\text{速度})^2$：

| 运动类型 | 惯量 | 速度 | 动能 |
|:--|:--|:--|:--|
| 平动 | $m$（质量）— 抵抗平动加速 | $v$（线速度） | $\frac{1}{2}mv^2$ |
| 转动 | $I$（转动惯量）— 抵抗转动加速 | $\omega$（角速度） | $\frac{1}{2}I\omega^2$ |

#### 5.2 为什么 $I$ 不是简单的 $m$

质量 $m$ 是物体固有的标量——无论物体如何运动，$m$ 不变。但转动惯量 $I$ 依赖于**转轴的位置**和**质量的分布**。同一个物体绕不同轴旋转有不同的 $I$。这意味着：

- 同一物体以同样的 $\omega$ 绕不同轴旋转，转动动能不同
- 改变姿势（如滑冰运动员收臂）可以改变 $I$ 从而改变 $K_{\text{rot}}$（在 $L$ 守恒时）
- 工程设计可以通过调整质量分布来优化转动动能存储（飞轮）或最小化转动惯量（赛车车轮）

#### 5.3 转动动能的三种等价视角

| 视角 | 公式 | 何时使用 |
|:--|:--|:--|
| **角速度视角** | $K = \frac{1}{2}I\omega^2$ | 已知 $\omega$ 和 $I$ |
| **角动量视角** | $K = \dfrac{L^2}{2I}$ | $L$ 守恒时分析动能变化 |
| **质量元视角** | $K = \sum \frac{1}{2}m_i v_i^2$ | 从第一性原理理解 |

#### 5.4 转动动能的微观解释

从微观角度看，刚体转动时每个质量元 $dm$ 都在做圆周运动。距轴 $r$ 处的质量元以速率 $v = r\omega$ 运动。其动能为 $\frac{1}{2}dm \cdot r^2\omega^2$。将所有质量元的动能相加：

$$
K_{\text{rot}} = \int \frac{1}{2} r^2\omega^2 dm = \frac{1}{2}\omega^2 \int r^2 dm = \frac{1}{2}I\omega^2
$$

> 🧠 **核心理解**：转动动能不是「另一种」能量——它本质上就是平动动能的总和，只不过用 $I$ 和 $\omega$ 重新包装了。认识到这一点，能量守恒定律在转动问题中的应用就变得自然而非神秘。

### 六、转动动能在自然界和工程中的应用

#### 6.1 飞轮储能（Flywheel Energy Storage）

飞轮是人类最早的能量储存装置之一。现代飞轮储能系统（FESS）使用碳纤维复合材料飞轮在真空中以超过 $50000\ \text{rpm}$ 旋转，能量密度可达 $100$–$200\ \text{Wh/kg}$，与某些化学电池相当。飞轮储能的优势是几乎无限次的充放电循环和极高的功率密度。

能量储存公式：$E = \frac{1}{2}I\omega^2$。要提高储能：
- 增大 $I$：增加飞轮质量或增大半径（但 $I \propto R^2$，增大半径更有效）
- 增大 $\omega$：$\omega$ 以平方出现，提高转速是更高效的增能手段

#### 6.2 陀螺仪中的转动动能

陀螺仪利用高速旋转的转子储存转动动能和角动量。其稳定性（抗干扰能力）来自角动量守恒——要改变陀螺仪转轴的方向，需要施加巨大的力矩。这一原理被用于：

- 飞机和航天器的姿态控制系统
- 智能手机中的微机电陀螺仪（MEMS gyroscopes）
- 哈勃太空望远镜的精确指向

#### 6.3 生物力学中的转动动能

人体的许多运动涉及转动动能：
- **投掷**：手臂绕肩关节旋转，动能 = $\frac{1}{2}I_{\text{arm}}\omega^2$
- **踢球**：腿绕髋关节旋转
- **空翻和转体**：体操运动员通过改变身体姿态（改变 $I$）控制转速

---

#### 6.1.1 🧪 推导 1：从质点系动能导出 $K_{\text{rot}} = \frac{1}{2}I\omega^2$

**推导目标**：证明刚体绕固定轴旋转的总动能等于 $\frac{1}{2}I\omega^2$。

**推导过程**：

将刚体视为 $N$ 个质量元 $\Delta m_i$ 的集合。第 $i$ 个质量元距转轴 $r_i$，其线速度 $v_i = r_i\omega$（所有质量元 $\omega$ 相同）。该质量元的动能为：

$$
K_i = \frac{1}{2}\Delta m_i v_i^2 = \frac{1}{2}\Delta m_i (r_i\omega)^2 = \frac{1}{2}\Delta m_i r_i^2 \omega^2
$$

总动能 = 所有质量元动能之和：

$$
K_{\text{rot}} = \sum_i K_i = \sum_i \frac{1}{2}\Delta m_i r_i^2 \omega^2
$$

由于 $\omega^2$ 对所有质量元相同，可以提出：

$$
K_{\text{rot}} = \frac{1}{2}\left(\sum_i \Delta m_i r_i^2\right)\omega^2
$$

括号内恰好是刚体对转轴的转动惯量 $I = \sum_i \Delta m_i r_i^2$，因此：

$$
\boxed{K_{\text{rot}} = \frac{1}{2}I\omega^2}
$$

> 💡 **核心洞察**：转动动能公式并非新的物理定律，而是对每一个微小质量元使用 $\frac{1}{2}mv^2$ 然后求和的结果。$I = \sum mr^2$ 的出现正是这个求和过程的自然产物。你可以把转动动能理解为「把刚体上每一小块的平动动能加起来」。

---

#### 6.1.2 🧪 推导 2：转动动能与角动量的关系 $K = \dfrac{L^2}{2I}$

**推导目标**：证明转动动能可以用角动量 $L = I\omega$ 表示为 $K = \dfrac{L^2}{2I}$，这与平动中的 $K = \dfrac{p^2}{2m}$ 完全对应。

**推导过程**：

由转动动能定义出发：

$$
K = \frac{1}{2}I\omega^2
$$

将 $\omega = \dfrac{L}{I}$（由 $L = I\omega$ 解出）代入：

$$
K = \frac{1}{2}I\left(\frac{L}{I}\right)^2 = \frac{1}{2}I \cdot \frac{L^2}{I^2} = \frac{L^2}{2I}
$$

因此：
$$
\boxed{K = \frac{L^2}{2I}}
$$

**与平动的对应**：

| | 平动 | 转动 |
|:--|:--|:--|
| 动量/角动量 | $p = mv$ | $L = I\omega$ |
| 动能形式 1 | $K = \frac{1}{2}mv^2$ | $K = \frac{1}{2}I\omega^2$ |
| 动能形式 2 | $K = \dfrac{p^2}{2m}$ | $K = \dfrac{L^2}{2I}$ |

> 💡 **应用价值**：在角动量守恒问题中（$L$ 不变，$I$ 变化），$K = L^2/(2I)$ 直接告诉你当转动惯量减小时动能增大——这解释了花样滑冰运动员收臂时转速加快且动能增加的深层原因：肌肉做了功！

---

#### 6.1.2b 🧪 推导 3：转动动能的微积分严格推导（🟣 C 版深化）

**推导目标**：用积分方法严格证明连续质量分布刚体的转动动能 $K = \frac{1}{2}I\omega^2$。

**推导过程**：

对于连续质量分布的刚体，将 $I = \sum m_i r_i^2$ 替换为积分 $I = \int r^2 dm$。刚体上每个质量元 $dm$ 的动能为：

$$
dK = \frac{1}{2} v^2 dm = \frac{1}{2} (r\omega)^2 dm = \frac{1}{2} r^2 \omega^2 dm
$$

其中 $\omega$ 对所有质量元相同（刚体绕固定轴旋转）。总动能为：

$$
K = \int dK = \int \frac{1}{2} r^2 \omega^2 dm = \frac{1}{2} \omega^2 \int r^2 dm
$$

由转动惯量的积分定义 $I = \int r^2 dm$，得：

$$
\boxed{K = \frac{1}{2}I\omega^2}
$$

**实例验证**：均匀细杆绕端点以 $\omega$ 旋转，$I = \frac{1}{3}ML^2$。距端点 $x$ 处 $dm = \frac{M}{L}dx$，$v = x\omega$：

$$
K = \int_0^L \frac{1}{2} \left(\frac{M}{L}dx\right) (x\omega)^2 = \frac{M\omega^2}{2L} \int_0^L x^2 dx = \frac{M\omega^2}{2L} \cdot \frac{L^3}{3} = \frac{1}{6}ML^2\omega^2
$$

而 $\frac{1}{2}I\omega^2 = \frac{1}{2} \cdot \frac{1}{3}ML^2 \cdot \omega^2 = \frac{1}{6}ML^2\omega^2$，两者一致 ✓。

> 💡 这个推导展示了「先积分再乘 $\frac{1}{2}\omega^2$」和「先求 $I$ 再乘 $\frac{1}{2}\omega^2$」的等价性——这正是 $I$ 作为「加权平均 $r^2$」的物理意义所在。

---

#### 6.1.2c 🧪 推导 4：转动动能与功-能定理的关联证明

**推导目标**：证明合外力矩做的功等于转动动能的变化量——旋转功-能定理 $\int \tau\,d\theta = \Delta(\frac{1}{2}I\omega^2)$。

**推导过程**：

由 $\tau = I\alpha = I\dfrac{d\omega}{dt}$，利用链式法则：

$$
\tau = I\frac{d\omega}{dt} = I\frac{d\omega}{d\theta}\frac{d\theta}{dt} = I\omega\frac{d\omega}{d\theta}
$$

因此：

$$
\tau\,d\theta = I\omega\,d\omega
$$

两边积分：

$$
\int_{\theta_1}^{\theta_2} \tau\,d\theta = \int_{\omega_1}^{\omega_2} I\omega\,d\omega = \frac{1}{2}I\omega_2^2 - \frac{1}{2}I\omega_1^2
$$

即：

$$
\boxed{W_{\text{net}} = \Delta K_{\text{rot}}}
$$

> 💡 这个推导的妙处在于使用了链式法则 $\frac{d\omega}{dt} = \omega\frac{d\omega}{d\theta}$——这是连接力矩（动力学）与角位移（运动学）的数学桥梁。完全对应平动中 $F dx = mv\,dv$ → $W = \Delta(\frac{1}{2}mv^2)$。

---

#### 6.1.3 🧪 例题 1：飞轮储能计算

**题目**：一个实心圆柱形飞轮质量 $M = 100\ \text{kg}$，半径 $R = 0.50\ \text{m}$，以 $3000\ \text{rpm}$ 绕其中心轴旋转。求：
(a) 飞轮的转动惯量
(b) 飞轮的转动动能
(c) 若飞轮用于为村庄供电，需要提供 $1.0 \times 10^5\ \text{J}$ 的能量，飞轮的角速度降至多少？

**题目分析**：

> **已知**：$M = 100\ \text{kg}$，$R = 0.50\ \text{m}$，$\omega_0 = 3000\ \text{rpm}$，$I = \frac{1}{2}MR^2$（实心圆柱）
>
> **求**：$I$、$K$、释放 $10^5\ \text{J}$ 后的 $\omega$
>
> **策略**：先转换单位，再套用转动动能公式，用能量差求末角速度。

**解答**：

**(a)** 转动惯量：
$$
I = \frac{1}{2}MR^2 = \frac{1}{2} \times 100 \times (0.50)^2 = \mathbf{12.5\ \text{kg·m}^2}
$$

**(b)** 转换角速度：
$$
\omega_0 = 3000\ \frac{\text{rev}}{\text{min}} \times \frac{2\pi\ \text{rad}}{1\ \text{rev}} \times \frac{1\ \text{min}}{60\ \text{s}} = 100\pi \approx 314.2\ \text{rad/s}
$$

转动动能：
$$
K_0 = \frac{1}{2}I\omega_0^2 = \frac{1}{2} \times 12.5 \times (314.2)^2 \approx \mathbf{6.17 \times 10^5\ \text{J}}
$$

**(c)** 释放能量后剩余动能：$K_f = K_0 - 1.0 \times 10^5 = 5.17 \times 10^5\ \text{J}$

由 $K_f = \frac{1}{2}I\omega_f^2$：
$$
\omega_f = \sqrt{\frac{2K_f}{I}} = \sqrt{\frac{2 \times 5.17 \times 10^5}{12.5}} \approx \mathbf{287.6\ \text{rad/s} \approx 2746\ \text{rpm}}
$$

> 💡 **飞轮储能的实际意义**：$6.17 \times 10^5\ \text{J}$ 约等于 $0.17\ \text{kWh}$——足够一只 10W 的 LED 灯泡点亮约 17 小时。现代飞轮储能系统使用碳纤维飞轮以数万 rpm 旋转，能量密度可与化学电池媲美。

---

#### 6.1.4 🧪 例题 2：转动动能与平动动能的比较

**题目**：一个均匀实心球（$I = \frac{2}{5}MR^2$）以速度 $v$ 在水平面上无滑动滚动。求：
(a) 平动动能占总动能的比例
(b) 转动动能占总动能的比例
(c) 若球沿斜面滚下高度 $h$，求底部速度（用能量法）

**题目分析**：

> **已知**：$I = \frac{2}{5}MR^2$，无滑动滚动 → $v = R\omega$
>
> **求**：动能分配比例，滚下斜面的末速度
>
> **策略**：用 $v = R\omega$ 将 $\omega$ 替换为 $v/R$，然后比较两部分动能。

**解答**：

**(a)** 总动能：
$$
K_{\text{total}} = \frac{1}{2}Mv^2 + \frac{1}{2}I\omega^2 = \frac{1}{2}Mv^2 + \frac{1}{2} \cdot \frac{2}{5}MR^2 \cdot \left(\frac{v}{R}\right)^2
$$
$$
= \frac{1}{2}Mv^2 + \frac{1}{5}Mv^2 = \frac{7}{10}Mv^2
$$

平动动能占比：
$$
\frac{K_{\text{trans}}}{K_{\text{total}}} = \frac{\frac{1}{2}Mv^2}{\frac{7}{10}Mv^2} = \frac{5}{7} \approx \mathbf{71.4\%}
$$

**(b)** 转动动能占比：
$$
\frac{K_{\text{rot}}}{K_{\text{total}}} = \frac{\frac{1}{5}Mv^2}{\frac{7}{10}Mv^2} = \frac{2}{7} \approx \mathbf{28.6\%}
$$

**(c)** 能量守恒（从高度 $h$ 滚下，无滑动）：
$$
Mgh = \frac{7}{10}Mv^2 \quad \Rightarrow \quad v = \sqrt{\frac{10}{7}gh}
$$

> 💡 **对比纯滑动**（无摩擦斜面）：$v = \sqrt{2gh}$。滚动速度是纯滑动的 $\sqrt{\frac{10}{7} \div 2} = \sqrt{\frac{5}{7}} \approx 0.845$ 倍——因为一部分重力势能转化为了转动动能而非全部转化为平动动能。

---

#### 6.1.5 🧪 例题 3：两个滑轮的转动动能比较

**题目**：两个滑轮质量相同（$M = 5.0\ \text{kg}$）、半径相同（$R = 0.20\ \text{m}$），但一个是实心圆盘（$I = \frac{1}{2}MR^2$），另一个是自行车轮式（质量全部集中在边缘，$I = MR^2$）。两者都以 $\omega = 30\ \text{rad/s}$ 旋转。求：
(a) 各自的转动动能
(b) 若要使两者都从静止加速到 $30\ \text{rad/s}$，哪个需要的功更多？多多少？

**题目分析**：

> **已知**：$M = 5.0\ \text{kg}$，$R = 0.20\ \text{m}$，$\omega = 30\ \text{rad/s}$
>
> **求**：$K_{\text{disk}}$、$K_{\text{ring}}$，功的差异
>
> **策略**：分别计算 $I$，再用 $K = \frac{1}{2}I\omega^2$。

**解答**：

**(a)** 实心圆盘：

$$
I_{\text{disk}} = \frac{1}{2}MR^2 = \frac{1}{2} \times 5.0 \times (0.20)^2 = 0.10\ \text{kg·m}^2
$$

$$
K_{\text{disk}} = \frac{1}{2} \times 0.10 \times 30^2 = \mathbf{45\ \text{J}}
$$

自行车轮式（薄圆环）：

$$
I_{\text{ring}} = MR^2 = 5.0 \times (0.20)^2 = 0.20\ \text{kg·m}^2
$$

$$
K_{\text{ring}} = \frac{1}{2} \times 0.20 \times 30^2 = \mathbf{90\ \text{J}}
$$

**(b)** 由功-能定理，所需功 = 末动能（从静止开始）：

$$
\Delta W = K_{\text{ring}} - K_{\text{disk}} = 90 - 45 = \mathbf{45\ \text{J}}
$$

> 💡 **洞察**：圆环的转动惯量是圆盘的 2 倍（质量在边缘 vs 均匀分布），以相同角速度旋转时转动动能也是 2 倍。要让圆环加速到相同转速，电机需要多做一倍的功——这也是为什么高性能车轮追求轻量化边缘（减少 $I$）。

---

#### 6.1.6 🧪 例题 4：三物体系统的动能分配

**题目**：如图，一根轻杆两端分别固定 $m_1 = 2.0\ \text{kg}$ 和 $m_2 = 3.0\ \text{kg}$ 的质点，杆长 $L = 0.80\ \text{m}$，绕通过杆上距 $m_1$ 为 $0.30\ \text{m}$ 的点的垂直轴以 $\omega = 4.0\ \text{rad/s}$ 旋转。求：
(a) 系统对转轴的转动惯量
(b) 系统的转动动能
(c) $m_1$ 和 $m_2$ 各自动能占系统总动能的百分比

**题目分析**：

> **已知**：$m_1 = 2.0\ \text{kg}$（距轴 $r_1 = 0.30\ \text{m}$），$m_2 = 3.0\ \text{kg}$（距轴 $r_2 = 0.50\ \text{m}$），$\omega = 4.0\ \text{rad/s}$
>
> **求**：$I$、$K$、动能分配
>
> **策略**：$I = \sum m_i r_i^2$，$K = \frac{1}{2}I\omega^2$，各质点 $K_i = \frac{1}{2}m_i(r_i\omega)^2$。

**解答**：

**(a)** 转动惯量：
$$
I = m_1 r_1^2 + m_2 r_2^2 = 2.0 \times (0.30)^2 + 3.0 \times (0.50)^2
$$
$$
= 2.0 \times 0.09 + 3.0 \times 0.25 = 0.18 + 0.75 = \mathbf{0.93\ \text{kg·m}^2}
$$

**(b)** 转动动能：
$$
K = \frac{1}{2}I\omega^2 = \frac{1}{2} \times 0.93 \times 16 = \mathbf{7.44\ \text{J}}
$$

**(c)** 各质点动能：
$$
K_1 = \frac{1}{2}m_1(r_1\omega)^2 = \frac{1}{2} \times 2.0 \times (0.30 \times 4.0)^2 = 1.0 \times 1.44 = 1.44\ \text{J}
$$
$$
K_2 = \frac{1}{2}m_2(r_2\omega)^2 = \frac{1}{2} \times 3.0 \times (0.50 \times 4.0)^2 = 1.5 \times 4.0 = 6.00\ \text{J}
$$

占比：
- $m_1$：$\dfrac{1.44}{7.44} \times 100\% \approx \mathbf{19.4\%}$
- $m_2$：$\dfrac{6.00}{7.44} \times 100\% \approx \mathbf{80.6\%}$

> 💡 **质量分布的影响**：$m_2$ 虽然质量只有 $m_1$ 的 1.5 倍，但由于 $r_2/r_1 = 5/3$，$r_2^2/r_1^2 = 25/9 \approx 2.78$——距离平方的放大效应使 $m_2$ 占据了超过 80% 的动能。这再次验证了 $K \propto r^2$ 对外围质量的极度敏感性。

---

### 本节总结

转动动能的三个等价表达式构成了能量分析的工具箱：

1. **$K = \frac{1}{2}I\omega^2$** — 最基本的定义，适用于绕固定轴旋转
2. **$K = \dfrac{L^2}{2I}$** — 角动量守恒问题中的最优形式
3. **$K_{\text{total}} = \frac{1}{2}Mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2$** — 滚动问题的能量守恒公式

### ⚠️ 常见误区辨析

> ❌ **误区 1**：「转动动能和平动动能是两个独立的物理量，它们不会互相转化。」
>
> ✅ **正确**：在滚动中，静摩擦力可以将平动动能「重定向」为转动动能（反之亦然）。滚动刚体在斜面上时，重力势能同时转化为平动和转动动能——两者的比例由形状因子 $\beta = I/MR^2$ 决定。

> ❌ **误区 2**：「$K = L^2/(2I)$ 在任何情况下都成立。」
>
> ✅ **正确**：这个等式仅在 $L = I\omega$ 成立时有效。如果 $\vec{L}$ 与 $\vec{\omega}$ 方向不同（非对称轴旋转），$K \neq L^2/(2I)$。但 AP 物理范围内转轴都是对称轴，该公式始终有效。

> ❌ **误区 3**：「转动动能比平动动能更难计算。」
>
> ✅ **正确**：转动动能的计算只需两步——确定 $I$ 和 $\omega$，代入 $K = \frac{1}{2}I\omega^2$。困难通常出在确定 $I$（选择正确的公式和转轴），而非动能公式本身。
2. **$K = \dfrac{L^2}{2I}$** — 角动量守恒问题中的最优形式
3. **$K_{\text{total}} = \frac{1}{2}Mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2$** — 滚动问题的能量守恒公式

# 6.2 力矩与功（Work and Torque）

## Part A：基础层（AP Physics 1 必备）

### 一、旋转功的物理本质

> 在平动中，力沿位移方向做功：$W = Fd\cos\theta$。在转动中，**力矩沿角位移方向做功**。当一个恒定力矩 $\tau$ 使物体转过角 $\Delta\theta$ 时，力矩做的功为：
>
> $$
> \boxed{W = \tau \Delta\theta}
> $$

旋转功是能量在转动世界中的「货币」。每次你转动扳手、拧开瓶盖或使飞轮加速，力矩都在做旋转功。这个公式的简洁性背后是深刻的物理对应——$F \leftrightarrow \tau$，$d \leftrightarrow \theta$。

> 📐 **旋转功的三种等价定义** — 同一个物理量，三个不同视角：
>
> | 视角 | 表达式 | 物理含义 | 何时使用 |
> |:--|:--|:--|:--|
> | **力×弧长视角** | $W = F \cdot s = F \cdot r\Delta\theta$ | 力沿圆弧路径做的功 | 已知力和作用半径时 |
> | **力矩×角位移视角** | $W = \tau\Delta\theta$ | 力矩直接在角位移上做功 | 已知力矩和转角时（最常用） |
> | **能量变化视角** | $W = \Delta K_{\text{rot}} = \Delta(\frac{1}{2}I\omega^2)$ | 功等于转动动能的变化 | 能量守恒问题中 |
>
> 🧠 **统一理解**：这三种表达描述的是同一个过程——力通过力矩使物体转动，将能量从一种形式转化为转动动能。选择哪种表达取决于已知条件：有力臂用第一种，有力矩用第二种，有能量信息用第三种。

### 二、平动功与旋转功的对应

| 平动 | 转动 | 对应 |
|:--|:--|:--|
| $W = Fd\cos\theta$ | $W = \tau\Delta\theta$ | 力 → 力矩，位移 → 角位移 |
| $P = Fv$ | $P = \tau\omega$ | 功率：力×速度 → 力矩×角速度 |
| 功改变平动动能 | 功改变转动动能 | 功-能定理 |

### 三、旋转功-能定理

$$
\boxed{W_{\text{net}} = \Delta K_{\text{rot}} = \frac{1}{2}I\omega_f^2 - \frac{1}{2}I\omega_i^2}
$$

> 🎯 在能量守恒问题中，旋转功可以来自重力（力矩做功）、摩擦力（力矩做功）或外加力矩。如果系统中没有非保守力矩做功，则转动动能 + 势能守恒。

### 四、功率的旋转形式

力矩做功的功率（做功速率）为：

$$
\boxed{P = \frac{dW}{dt} = \tau \frac{d\theta}{dt} = \tau\omega}
$$

> 💡 这与 $P = Fv$ 完美对应。发动机的「扭矩 × 转速 = 功率」正是这个公式的工程应用。

### 五、旋转功的深入理解

#### 5.1 力矩做功与力做功的类比链

旋转功和力做功之间存在一套完整的类比体系，掌握这套体系可以让你在转动和平动之间自如切换：

| 概念 | 平动 | 转动 | 类比关系 |
|:--|:--|:--|:--|
| 功的微分形式 | $dW = F\,dx$ | $dW = \tau\,d\theta$ | $F \leftrightarrow \tau$，$dx \leftrightarrow d\theta$ |
| 功的积分形式 | $W = \int F\,dx$ | $W = \int \tau\,d\theta$ | $\tau$-$\theta$ 图下面积 |
| 功率 | $P = Fv$ | $P = \tau\omega$ | 发动机的扭矩×转速 |
| 功-能定理 | $W = \Delta(\frac{1}{2}mv^2)$ | $W = \Delta(\frac{1}{2}I\omega^2)$ | 功改变动能 |

#### 5.2 旋转功的几何解释——$\tau$-$\theta$ 图

在 $\tau$-$\theta$ 坐标图中，力矩曲线下的面积等于力矩做的功。对于恒定力矩，这是一个矩形面积 $\tau \times \Delta\theta$。对于变力矩（如扭转弹簧 $\tau = -k\theta$），曲线下的面积需要用积分计算。这完全类似于 $F$-$x$ 图中力曲线下的面积等于力做的功。

#### 5.3 力矩做功的正负

- **力矩方向与角位移方向相同** → 正功（增加转动动能，如电机驱动飞轮加速）
- **力矩方向与角位移方向相反** → 负功（减少转动动能，如刹车制动）
- **力矩垂直于角位移** → 不做功（在二维平面问题中不会出现此情况）

#### 5.4 日常生活中旋转功的实例

- **拧螺丝**：螺丝刀施加力矩转过 $\theta$，做功 $W = \tau\theta$。力矩越大或转的圈数越多，做的功越多。
- **骑自行车**：脚踏力通过曲柄产生力矩，力矩做功驱动后轮。功率 $P = \tau\omega$ 决定了骑行速度。
- **开门**：推门时力对铰链产生力矩，力矩做功转化为门的转动动能——$W = \tau\Delta\theta = \Delta(\frac{1}{2}I\omega^2)$。
- **风力发电机**：风力使叶片旋转，力矩做功驱动发电机将机械能转化为电能。

#### 5.5 旋转功与保守力

当力矩由保守力产生时，力矩做的功可以表示为势能的减少：
- 重力矩：$W_g = -\Delta U_g$
- 扭转弹簧力矩：$W_{\text{spring}} = -\Delta U_{\text{spring}} = -\Delta(\frac{1}{2}k\theta^2)$

这类似于平动中 $W_g = -\Delta(mgy)$ 和 $W_{\text{spring}} = -\Delta(\frac{1}{2}kx^2)$。保守力矩的存在意味着我们可以定义「转动势能」并将能量守恒扩展到转动系统。

---

#### 6.2.1 🧪 推导 1：从功的平动定义导出 $W = \tau\Delta\theta$

**推导目标**：证明恒定力矩在角位移 $\Delta\theta$ 上做的功等于 $\tau\Delta\theta$。

**推导过程**：

考虑一个力 $F$ 作用在距转轴 $r$ 处，力的方向始终沿切线方向（$\theta = 90^\circ$，力矩 $\tau = rF$）。当物体转过小角位移 $d\theta$ 时，力作用点沿圆弧运动的弧长为 $ds = r\,d\theta$。

力做的微功为：

$$
dW = F\,ds = F \cdot r\,d\theta = (rF)\,d\theta = \tau\,d\theta
$$

对恒定力矩 $\tau$，从 $\theta_1$ 到 $\theta_2$ 积分：

$$
W = \int_{\theta_1}^{\theta_2} \tau\,d\theta = \tau(\theta_2 - \theta_1) = \tau\Delta\theta
$$

因此：
$$
\boxed{W = \tau\Delta\theta}
$$

> 💡 **物理图像**：力矩做的功 = 力矩 × 转过的角度。这就像力做的功 = 力 × 位移。注意这里要求 $\tau$ 恒定（或 $\theta$ 很小时力矩近似恒定），对于变力矩需要用积分（AP Physics C 范围）。

**验证 — 从功-能定理角度**：

由 $\tau = I\alpha$ 和转动运动学 $\omega^2 = \omega_0^2 + 2\alpha\Delta\theta$：

$$
W = \tau\Delta\theta = I\alpha\Delta\theta = I \cdot \frac{\omega^2 - \omega_0^2}{2} = \frac{1}{2}I\omega^2 - \frac{1}{2}I\omega_0^2 = \Delta K_{\text{rot}}
$$

这正是旋转功-能定理。

---

#### 6.2.2 🧪 推导 2：导出功率的旋转形式 $P = \tau\omega$

**推导目标**：证明力矩做功的瞬时功率等于力矩与角速度的乘积。

**推导过程**：

功率是功对时间的导数：

$$
P = \frac{dW}{dt}
$$

将 $dW = \tau\,d\theta$ 代入：

$$
P = \frac{\tau\,d\theta}{dt} = \tau\frac{d\theta}{dt} = \tau\omega
$$

因此：
$$
\boxed{P = \tau\omega}
$$

**从平动功率推导**（交叉验证）：

平动功率 $P = Fv$。对于旋转中力作用在距轴 $r$ 处的情况：

$$
P = Fv = F(r\omega) = (rF)\omega = \tau\omega
$$

两种方法得到一致结果。

> 💡 **工程应用**：汽车发动机的功率 = 扭矩 × 转速。这就是为什么柴油机（高扭矩、低转速）和汽油机（低扭矩、高转速）可以输出相同的功率——$\tau$ 和 $\omega$ 的乘积决定 $P$。

---

#### 6.2.2b 🧪 推导 3：变力矩做功的积分形式（🟣 C 版）

**推导目标**：证明当力矩 $\tau$ 随角度变化时，旋转功需用积分 $W = \int \tau(\theta)\,d\theta$ 计算。

**推导过程**：

将角位移 $\theta_1 \to \theta_2$ 分割为 $N$ 个小角位移 $\Delta\theta_i$。在每一个微小角位移中，力矩 $\tau_i$ 近似恒定，做功 $\Delta W_i = \tau_i\Delta\theta_i$。

总功为各段功之和：

$$
W \approx \sum_i \tau_i \Delta\theta_i
$$

取极限 $N \to \infty$，$\Delta\theta_i \to d\theta$：

$$
\boxed{W = \int_{\theta_1}^{\theta_2} \tau(\theta)\,d\theta}
$$

这正好是 $\tau$-$\theta$ 曲线下的面积——与平动中 $W = \int F(x)\,dx$ 为 $F$-$x$ 曲线下面积完全对应。

**应用示例——扭转弹簧**：

扭转弹簧产生的力矩 $\tau = -k\theta$（$k$ 为扭转劲度系数，类似 $F = -kx$）。将弹簧从平衡位置扭转 $\theta_0$ 所需的功（克服弹性力矩）：

$$
W = \int_0^{\theta_0} k\theta\,d\theta = \frac{1}{2}k\theta_0^2
$$

这与平动弹簧 $W = \frac{1}{2}kx^2$ 完全对应。扭转弹簧储存的弹性势能为 $U = \frac{1}{2}k\theta^2$。

---

#### 6.2.2c 🧪 推导 4：重力矩做功与势能变化的关系

**推导目标**：证明重力矩做的功等于重力势能的减少量——$W_g = -\Delta U_g$。

**推导过程**：

考虑一个不规则形状的刚体，质心距转轴 $d$。当刚体从角位置 $\theta_1$ 转到 $\theta_2$ 时，质心的竖直高度变化为 $\Delta y = d(\cos\theta_1 - \cos\theta_2)$。

重力对转轴的力矩为 $\tau_g = -Mgd\sin\theta$（以 $\theta$ 从竖直方向量起，负号表示力矩使 $\theta$ 减小）。

重力矩做的功：

$$
W_g = \int_{\theta_1}^{\theta_2} \tau_g\,d\theta = \int_{\theta_1}^{\theta_2} (-Mgd\sin\theta)\,d\theta
$$

$$
= Mgd\left[\cos\theta\right]_{\theta_1}^{\theta_2} = Mgd(\cos\theta_2 - \cos\theta_1)
$$

而重力势能变化：$\Delta U_g = Mg\Delta y = Mgd(\cos\theta_2 - \cos\theta_1)$

因此：
$$
\boxed{W_g = -\Delta U_g}
$$

> 💡 **深刻含义**：重力矩做功的结果与「将所有质量集中在质心计算」完全一致。这证明了在处理重力矩问题时，可以简单地将重力画在质心上——均匀重力场中，重力矩等价于质心处集中重力的力矩。

---

#### 6.2.3 🧪 例题 1：电机加速飞轮

**题目**：一个电机对飞轮（$I = 0.80\ \text{kg·m}^2$）施加恒定的 $5.0\ \text{N·m}$ 力矩。飞轮从静止开始旋转。求：
(a) 飞轮的角加速度
(b) 飞轮转过 $20\ \text{rad}$ 时力矩做的功
(c) 此时的角速度

**题目分析**：

> **已知**：$I = 0.80\ \text{kg·m}^2$，$\tau = 5.0\ \text{N·m}$，$\omega_0 = 0$，$\Delta\theta = 20\ \text{rad}$
>
> **求**：$\alpha$、$W$、$\omega$
>
> **策略**：用 $\tau = I\alpha$ 求角加速度 → 用 $W = \tau\Delta\theta$ 求功 → 用功-能定理求末角速度。

**解答**：

**(a)** $\alpha = \dfrac{\tau}{I} = \dfrac{5.0}{0.80} = \mathbf{6.25\ \text{rad/s}^2}$

**(b)** $W = \tau\Delta\theta = 5.0 \times 20 = \mathbf{100\ \text{J}}$

**(c)** 由功-能定理 $W = \Delta K = \frac{1}{2}I\omega^2 - 0$：

$$
\omega = \sqrt{\frac{2W}{I}} = \sqrt{\frac{2 \times 100}{0.80}} = \sqrt{250} \approx \mathbf{15.8\ \text{rad/s}}
$$

**交叉验证**（用运动学）：由 $\omega^2 = 2\alpha\Delta\theta$：
$$
\omega^2 = 2 \times 6.25 \times 20 = 250 \quad \Rightarrow \quad \omega \approx 15.8\ \text{rad/s} \checkmark
$$

> 💡 **能量视角 vs 运动学视角**：两种方法得到相同答案，说明旋转功-能定理与转动运动学自洽。在更复杂的问题中（如力矩不恒定），能量法往往比运动学法更简洁。

---

#### 6.2.4 🧪 例题 2：重力对下落物体-滑轮系统做的功

**题目**：一个半径 $R = 0.15\ \text{m}$ 的滑轮（$I = 0.045\ \text{kg·m}^2$）上绕有轻绳，绳端悬挂 $m = 3.0\ \text{kg}$ 的重物。重物从静止释放并下落 $h = 2.0\ \text{m}$。用能量法求重物落地时的速度。

**题目分析**：

> **已知**：$I = 0.045\ \text{kg·m}^2$，$R = 0.15\ \text{m}$，$m = 3.0\ \text{kg}$，$h = 2.0\ \text{m}$
>
> **求**：$v$
>
> **策略**：能量守恒——重力势能 → 重物平动动能 + 滑轮转动动能。用 $v = R\omega$ 关联。

**解答**：

能量守恒（系统 = 重物 + 滑轮 + 地球）：

初始能量（以落地位置为零势面）：$E_i = mgh$

末能量：$E_f = \frac{1}{2}mv^2 + \frac{1}{2}I\omega^2$

由 $v = R\omega$（绳不打滑）→ $\omega = v/R$：

$$
mgh = \frac{1}{2}mv^2 + \frac{1}{2}I\left(\frac{v}{R}\right)^2
$$

$$
mgh = \frac{1}{2}v^2\left(m + \frac{I}{R^2}\right)
$$

$$
v^2 = \frac{2mgh}{m + I/R^2} = \frac{2 \times 3.0 \times 9.8 \times 2.0}{3.0 + 0.045/(0.15)^2}
$$

$$
= \frac{117.6}{3.0 + 2.0} = \frac{117.6}{5.0} = 23.52
$$

$$
v = \mathbf{4.85\ \text{m/s}}
$$

> 💡 **滑轮质量的「等效平动质量」**：分母中 $I/R^2 = 2.0\ \text{kg}$ 是滑轮对系统平动惯性的等效贡献。没有滑轮时 $v = \sqrt{2gh} = \sqrt{39.2} \approx 6.26\ \text{m/s}$，有滑轮时 $v = 4.85\ \text{m/s}$——能量「分流」了一部分用于转动滑轮。

---

#### 6.2.5 🧪 例题 3：扭转弹簧中的功与能

**题目**：一个扭转弹簧的劲度系数 $k = 3.0\ \text{N·m/rad}$。将一个转动惯量 $I = 0.50\ \text{kg·m}^2$ 的圆盘从平衡位置扭转 $\theta_0 = 0.80\ \text{rad}$ 后释放。求：
(a) 弹簧中储存的势能
(b) 释放后圆盘通过平衡位置时的角速度
(c) 圆盘的最大转动动能

**题目分析**：

> **已知**：$k = 3.0\ \text{N·m/rad}$，$I = 0.50\ \text{kg·m}^2$，$\theta_0 = 0.80\ \text{rad}$
>
> **求**：$U$、$\omega_{\max}$、$K_{\max}$
>
> **策略**：扭转弹簧势能 $U = \frac{1}{2}k\theta^2$，能量守恒。

**解答**：

**(a)** 弹簧势能：
$$
U = \frac{1}{2}k\theta_0^2 = \frac{1}{2} \times 3.0 \times (0.80)^2 = \mathbf{0.96\ \text{J}}
$$

**(b)** 在平衡位置，全部势能转化为转动动能：
$$
\frac{1}{2}I\omega^2 = 0.96 \quad \Rightarrow \quad \omega = \sqrt{\frac{2 \times 0.96}{0.50}} = \sqrt{3.84} \approx \mathbf{1.96\ \text{rad/s}}
$$

**(c)** 最大转动动能 = 初始势能 = $\mathbf{0.96\ \text{J}}$

> 💡 **扭转弹簧 vs 平动弹簧**：$\frac{1}{2}k\theta^2$ ↔ $\frac{1}{2}kx^2$，$\tau = -k\theta$ ↔ $F = -kx$。所有平动简谐运动的结果都可以「翻译」为转动简谐运动——周期 $T = 2\pi\sqrt{I/k}$（对应 $T = 2\pi\sqrt{m/k}$）。

---

#### 6.2.6 🧪 例题 4：恒定功率加速飞轮

**题目**：一台电机以恒定功率 $P = 500\ \text{W}$ 驱动一个 $I = 4.0\ \text{kg·m}^2$ 的飞轮从静止开始加速。忽略摩擦。求：
(a) $t = 3.0\ \text{s}$ 时飞轮的角速度
(b) 在此期间电机做的总功
(c) $t = 3.0\ \text{s}$ 时飞轮的转动动能

**题目分析**：

> **已知**：$P = 500\ \text{W}$（恒定），$I = 4.0\ \text{kg·m}^2$，$\omega_0 = 0$，$t = 3.0\ \text{s}$
>
> **求**：$\omega(3.0)$、$W$、$K(3.0)$
>
> **策略**：恒功率 → $W = Pt$ → $W = \Delta K = \frac{1}{2}I\omega^2$ → 解出 $\omega$。

**解答**：

**(a)** 由 $P = \tau\omega$ 和 $\tau = I\alpha = I\frac{d\omega}{dt}$：
$$
P = I\omega\frac{d\omega}{dt}
$$

分离变量：$\omega\,d\omega = \frac{P}{I}dt$

积分：$\int_0^\omega \omega\,d\omega = \frac{P}{I}\int_0^t dt$ → $\frac{\omega^2}{2} = \frac{P}{I}t$

$$
\omega = \sqrt{\frac{2Pt}{I}} = \sqrt{\frac{2 \times 500 \times 3.0}{4.0}} = \sqrt{750} \approx \mathbf{27.4\ \text{rad/s}}
$$

**(b)** $W = Pt = 500 \times 3.0 = \mathbf{1500\ \text{J}}$

**(c)** $K = \frac{1}{2}I\omega^2 = \frac{1}{2} \times 4.0 \times (27.4)^2 \approx \mathbf{1500\ \text{J}}$ ✓

> 💡 **恒功率 vs 恒力矩**：恒力矩下 $\omega$ 随时间线性增长（$\omega = \alpha t$）；恒功率下 $\omega \propto \sqrt{t}$——因为随着转速增加，同样功率产生的力矩 $\tau = P/\omega$ 越来越小，加速越来越慢。这解释了为什么汽车在高速时加速变慢。

---

### 本节总结

旋转功的三个核心公式：

1. **$W = \tau\Delta\theta$** — 恒定力矩的功（$\tau$ 恒定）
2. **$P = \tau\omega$** — 力矩做功的瞬时功率
3. **$W_{\text{net}} = \Delta K_{\text{rot}}$** — 旋转功-能定理

🟣 **AP Physics C 扩展**：当 $\tau$ 不恒定时，$W = \int \tau\,d\theta$。

### ⚠️ 常见误区辨析

> ❌ **误区 1**：「力矩做的功可以写成焦耳（J），因为 $\text{N·m} = \text{J}$。」
>
> ✅ **正确**：力矩的单位必须写为 $\text{N·m}$ 而非 $\text{J}$。虽然量纲相同，但力矩是矢量（叉积），功是标量（点积）。在 AP 考试中写错单位会被扣分。

> ❌ **误区 2**：「$P = \tau\omega$ 只对恒定力矩成立。」
>
> ✅ **正确**：$P = \tau\omega$ 是瞬时功率公式，对每个时刻都成立——即使 $\tau$ 和 $\omega$ 随时间变化。恒定力矩的功 $W = \tau\Delta\theta$ 才是仅在 $\tau$ 恒定时成立的公式。

> ❌ **误区 3**：「静摩擦力做负功使滚动减速。」
>
> ✅ **正确**：纯滚动中静摩擦力不做功（接触点瞬时速度为零）。静摩擦力将平动动能「转换」为转动动能，不消耗总能量。

# 6.3 角动量与角冲量（Angular Momentum and Angular Impulse）

## Part A：基础层（AP Physics 1 必备）

### 一、角动量的物理本质

> **角动量（Angular Momentum，符号 $\vec{L}$）** 是描述物体旋转运动状态的矢量物理量——它是转动中的「动量」。正如动量 $\vec{p} = m\vec{v}$ 描述平动运动的量，角动量 $\vec{L} = I\vec{\omega}$ 描述转动运动的量。
>
> 对于绕固定轴旋转的刚体：
> $$
> \boxed{L = I\omega}
> $$
>
> 对于质点（绕某参考点）：
> $$
> \boxed{\vec{L} = \vec{r} \times \vec{p} = \vec{r} \times m\vec{v}}
> $$

角动量是第六章的灵魂概念。如果说第五章的核心是力矩（转动中的力），那么第六章的核心就是角动量（转动中的动量）。力矩与角动量的关系 $\vec{\tau} = d\vec{L}/dt$ 是转动动力学最普遍的方程，比 $\tau = I\alpha$ 更基本。

> 📐 **角动量的三种等价定义** — 同一个物理量，三种表达方式：
>
> | 视角 | 表达式 | 物理含义 | 适用场景 |
> |:--|:--|:--|:--|
> | **刚体转动视角** | $L = I\omega$ | 转动惯量×角速度——转动中的「动量」 | 刚体绕固定轴旋转 |
> | **质点叉积视角** | $\vec{L} = \vec{r} \times \vec{p} = \vec{r} \times m\vec{v}$ | 位置矢量与动量的叉积——最普遍定义 | 任意质点对任意参考点 |
> | **几何视角** | $L = rmv\sin\theta = r_\perp p = r p_\perp$ | 动量臂×动量 或 矢径×垂直动量分量 | 快速计算角动量大小 |
>
> 🧠 **统一理解**：三种定义等价但适用于不同情境。$L = I\omega$ 是工程计算中最常用的形式；$\vec{L} = \vec{r} \times \vec{p}$ 是理论物理的出发点；几何形式 $L = r_\perp mv$ 提供了最直观的物理图像——角动量衡量的是物体「绕参考点旋转的趋势强度」。

> 📝 **Step-by-Step：如何确定角动量的方向**
>
> 1. **确定旋转平面**：物体在哪个平面内运动或旋转？
> 2. **使用右手定则**：右手四指沿旋转方向弯曲（或从 $\vec{r}$ 弯向 $\vec{v}$）
> 3. **大拇指指向**：大拇指所指即为 $\vec{L}$ 的方向
> 4. **标记方向**：出纸面用 $\odot$，入纸面用 $\otimes$
> 5. **检查一致性**：$\vec{L}$、$\vec{\omega}$、$\vec{\tau}$ 三者方向关系需自洽

### 二、角动量的关键性质

| 性质 | 说明 |
|:--|:--|
| **矢量** | 方向由右手定则确定（同角速度方向） |
| **单位** | $\text{kg·m}^2\text{/s}$ |
| **对转轴的依赖性** | 同一物体对不同转轴有不同的 $L$ |
| **叠加性** | 系统的总角动量 = 各部分角动量的矢量和 |

### 三、角冲量（Angular Impulse）

力矩对时间的积分称为**角冲量**：

$$
\boxed{\text{角冲量} = \int \tau\,dt = \Delta L}
$$

当力矩恒定时：

$$
\boxed{\tau\Delta t = \Delta L = L_f - L_i}
$$

> 🎯 这与平动中的冲量-动量定理 $\vec{F}\Delta t = \Delta \vec{p}$ 完全对应。角冲量 = 力矩 × 时间 = 角动量的变化量。

### 四、$\vec{\tau} = d\vec{L}/dt$ — 转动动力学的最普遍形式

$$
\boxed{\vec{\tau}_{\text{net}} = \frac{d\vec{L}}{dt}}
$$

这是旋转牛顿第二定律的最一般形式，它在以下情况下都成立：
- $I$ 恒定：退化为 $\tau = I\alpha$
- $I$ 变化（如滑冰运动员收臂）：$\tau = I\frac{d\omega}{dt} + \omega\frac{dI}{dt}$

### 五、角动量的深度理解

#### 5.1 角动量的矢量性质

角动量 $\vec{L}$ 是矢量，其方向由右手定则确定：右手四指沿旋转方向弯曲，大拇指所指即为 $\vec{L}$ 的方向。在 AP 物理中，角动量的方向通常用 $\odot$（出纸面）和 $\otimes$（入纸面）表示。

> ⚠️ **角动量的方向不一定与角速度方向相同**。对于非对称轴旋转，$\vec{L}$ 可能与 $\vec{\omega}$ 有夹角。但在 AP 物理范围内，转轴始终是对称轴，$\vec{L} \parallel \vec{\omega}$。

#### 5.2 角动量的物理直觉

- **$I$ 大、$\omega$ 大** → 角动量大 → 更难改变旋转状态
- **角动量是旋转的「运动量」**——正如动量是平动的「运动量」
- 要改变角动量的大小或方向，需要施加力矩（$\vec{\tau} = d\vec{L}/dt$）

#### 5.3 角动量与动量的系统类比

| 特征 | 平动 | 转动 |
|:--|:--|:--|
| 运动的量 | $\vec{p} = m\vec{v}$ | $\vec{L} = I\vec{\omega}$（刚体） |
| 基本方程 | $\vec{F} = d\vec{p}/dt$ | $\vec{\tau} = d\vec{L}/dt$ |
| 守恒条件 | $\Sigma\vec{F}_{\text{ext}} = 0$ | $\Sigma\vec{\tau}_{\text{ext}} = 0$ |
| 守恒量的变化方式 | $m$ 可变（火箭） | $I$ 可变（滑冰） |
| 冲量 | $\int\vec{F}dt = \Delta\vec{p}$ | $\int\vec{\tau}dt = \Delta\vec{L}$ |

#### 5.4 角动量为什么重要？

角动量是物理学中最重要的守恒量之一，其应用远超出经典力学：

- **天体物理**：行星轨道、星系旋转、中子星（脉冲星）、黑洞吸积盘
- **量子力学**：电子自旋角动量、轨道角动量、原子光谱
- **工程**：陀螺仪导航、卫星姿态控制、飞轮储能
- **生物力学**：猫从高处落下总能四脚着地——它们通过扭转身体不同部分来「重新分配」角动量

#### 5.5 角冲量的直观理解

角冲量 $\int\tau\,dt$ 是力矩在时间上的累积效果。一个大力矩作用很短时间、或一个小力矩作用很长时间，可以产生相同的角冲量——即相同的角动量变化。这解释了：

- 为什么锤子猛击能产生巨大旋转效果（大力矩 × 短时间）
- 为什么缓慢拧动扳手也能拧紧螺丝（小力矩 × 长时间）
- 碰撞问题中角动量守恒如此有用——碰撞时间极短，外力矩的角冲量可忽略

---

#### 6.3.1 🧪 推导 1：从 $\vec{L} = \vec{r} \times \vec{p}$ 推导质点的角动量

**推导目标**：证明质点绕参考点 $O$ 的角动量大小为 $L = rmv\sin\theta = rp_\perp = r_\perp p$。

**推导过程**：

质点的角动量定义为位置矢量与动量的叉积：

$$
\vec{L} = \vec{r} \times \vec{p} = \vec{r} \times m\vec{v}
$$

叉积的大小：

$$
|\vec{L}| = |\vec{r}||\vec{p}|\sin\theta = rmv\sin\theta
$$

其中 $\theta$ 是 $\vec{r}$ 与 $\vec{v}$（即 $\vec{p}$）之间的夹角。

三种等价表达：

**(a)** 基本形式：$L = rmv\sin\theta = rp\sin\theta$

**(b)** 垂直动量形式：定义 $p_\perp = mv\sin\theta = mv_\perp$（垂直于 $\vec{r}$ 的动量分量）：
$$
L = rp_\perp
$$

**(c)** 力臂形式（动量臂）：定义 $r_\perp = r\sin\theta$（从参考点到动量方向的垂直距离）：
$$
L = r_\perp p = r_\perp mv
$$

因此：
$$
\boxed{L = rmv\sin\theta = rp_\perp = r_\perp p}
$$

> 💡 **几何直觉**：$r_\perp$ 是从参考点向速度矢量方向作垂线的长度——也称为「动量臂」。这与力矩中的力臂 $r_\perp$ 概念完全类似：力矩 = 力臂 × 力，角动量 = 动量臂 × 动量。

**特殊情况**：
- 质点做圆周运动（$\vec{v} \perp \vec{r}$，$\theta = 90^\circ$）：$L = rmv = mr^2\omega = I\omega$
- 质点沿直线远离参考点（$\theta = 0^\circ$）：$L = 0$

---

#### 6.3.2 🧪 推导 2：从 $\vec{\tau} = d\vec{L}/dt$ 导出角冲量-角动量定理

**推导目标**：证明合外力矩的角冲量等于角动量的变化量。

**推导过程**：

由 $\vec{\tau}_{\text{net}} = \dfrac{d\vec{L}}{dt}$，分离变量：

$$
d\vec{L} = \vec{\tau}_{\text{net}}\,dt
$$

从初始时刻 $t_i$ 到末时刻 $t_f$ 积分：

$$
\int_{\vec{L}_i}^{\vec{L}_f} d\vec{L} = \int_{t_i}^{t_f} \vec{\tau}_{\text{net}}\,dt
$$

$$
\boxed{\Delta\vec{L} = \vec{L}_f - \vec{L}_i = \int_{t_i}^{t_f} \vec{\tau}_{\text{net}}\,dt}
$$

对于恒定合力矩：

$$
\boxed{\Delta\vec{L} = \vec{\tau}_{\text{net}}\Delta t}
$$

> 💡 **与平动对比**：

| 平动 | 转动 |
|:--|:--|
| $\vec{F} = d\vec{p}/dt$ | $\vec{\tau} = d\vec{L}/dt$ |
| $\Delta\vec{p} = \int \vec{F}\,dt$ | $\Delta\vec{L} = \int \vec{\tau}\,dt$ |
| $\Delta\vec{p} = \vec{F}\Delta t$（恒力） | $\Delta\vec{L} = \vec{\tau}\Delta t$（恒力矩） |

---

#### 6.3.2b 🧪 推导 3：刚体角动量的矢量形式 $\vec{L} = I\vec{\omega}$ 的推导

**推导目标**：证明对于绕固定轴旋转的刚体，总角动量矢量 $\vec{L} = I\vec{\omega}$，且 $\vec{L}$ 与 $\vec{\omega}$ 方向相同。

**推导过程**：

将刚体视为 $N$ 个质点的集合。第 $i$ 个质点的位置矢量为 $\vec{r}_i$，速度 $\vec{v}_i = \vec{\omega} \times \vec{r}_i$（纯转动）。

该质点的角动量：$\vec{L}_i = \vec{r}_i \times m_i\vec{v}_i = m_i \vec{r}_i \times (\vec{\omega} \times \vec{r}_i)$

使用矢量恒等式 $\vec{A} \times (\vec{B} \times \vec{C}) = \vec{B}(\vec{A}\cdot\vec{C}) - \vec{C}(\vec{A}\cdot\vec{B})$：

$$
\vec{L}_i = m_i\left[\vec{\omega}(\vec{r}_i\cdot\vec{r}_i) - \vec{r}_i(\vec{r}_i\cdot\vec{\omega})\right] = m_i\left[r_i^2\vec{\omega} - \vec{r}_i(\vec{r}_i\cdot\vec{\omega})\right]
$$

对于绕固定轴（设为 $z$ 轴）的旋转，$\vec{\omega} = \omega\hat{k}$，$\vec{r}_i = (x_i, y_i, z_i)$，$\vec{r}_i\cdot\vec{\omega} = z_i\omega$。

沿 $z$ 轴（转轴方向）的角动量分量：

$$
L_{i,z} = m_i\left[r_i^2\omega - z_i(z_i\omega)\right] = m_i(x_i^2 + y_i^2)\omega = m_i r_{i,\perp}^2\omega
$$

其中 $r_{i,\perp} = \sqrt{x_i^2 + y_i^2}$ 是质点到转轴的垂直距离。

总角动量的 $z$ 分量：

$$
L_z = \sum_i L_{i,z} = \left(\sum_i m_i r_{i,\perp}^2\right)\omega = I\omega
$$

因此对于绕对称轴旋转的刚体：
$$
\boxed{\vec{L} = I\vec{\omega}}
$$

> 💡 **一般情况注意**：对于非对称轴旋转，$\vec{L}$ 与 $\vec{\omega}$ 方向可能不同（$\vec{L}$ 不是简单的 $I\vec{\omega}$），此时转动惯量需用张量（惯性张量）描述。但 AP 物理范围内，转轴都是对称轴，$\vec{L} \parallel \vec{\omega}$ 始终成立。

---

#### 6.3.2c 🧪 推导 4：角动量定理的微分与积分形式统一

**推导目标**：展示 $\vec{\tau} = d\vec{L}/dt$ 如何统一描述 $I$ 恒定和 $I$ 变化两种情况。

**推导过程**：

由乘积法则对 $\vec{L} = I\vec{\omega}$ 求导：

$$
\vec{\tau} = \frac{d}{dt}(I\vec{\omega}) = I\frac{d\vec{\omega}}{dt} + \vec{\omega}\frac{dI}{dt}
$$

**情况 1**：$I$ 恒定 → $\frac{dI}{dt} = 0$，$\vec{\tau} = I\vec{\alpha}$（第五章的标准形式）

**情况 2**：$\tau_{\text{ext}} = 0$ 且 $I$ 变化 → $I\frac{d\omega}{dt} + \omega\frac{dI}{dt} = 0$

这等价于 $\frac{d}{dt}(I\omega) = 0$，即 $I\omega = \text{常数}$——角动量守恒。

**情况 3**：既有外力矩，$I$ 又在变化：
$$
\vec{\tau} = I\vec{\alpha} + \vec{\omega}\frac{dI}{dt}
$$

角加速度不仅来自力矩（$I\alpha$），还来自转动惯量的变化（$\omega\frac{dI}{dt}$）。例如：滑冰运动员边收臂（$\frac{dI}{dt} < 0$）边用冰刀施加力矩（$\tau \neq 0$），角加速度由两项共同决定。

> 💡 **统一视角**：$\vec{\tau} = d\vec{L}/dt$ 是转动动力学的「终极方程」，$\tau = I\alpha$ 只是其 $I$ 恒定时的特例。在 AP Physics C 中，你必须理解这个层次关系。

---

#### 6.3.3 🧪 例题 1：质点的角动量计算

**题目**：一个 $m = 2.0\ \text{kg}$ 的质点以 $v = 8.0\ \text{m/s}$ 的速度沿直线运动。在某一时刻，该质点的位置相对于参考点 $O$ 的矢径大小为 $r = 3.0\ \text{m}$，矢径与速度方向的夹角为 $30^\circ$。求质点对 $O$ 点的角动量大小。

**题目分析**：

> **已知**：$m = 2.0\ \text{kg}$，$v = 8.0\ \text{m/s}$，$r = 3.0\ \text{m}$，$\theta = 30^\circ$
>
> **求**：$L$
>
> **策略**：直接用 $L = rmv\sin\theta$。

**解答**：

$$
L = rmv\sin\theta = 3.0 \times 2.0 \times 8.0 \times \sin 30^\circ = 48 \times 0.5 = \mathbf{24\ \text{kg·m}^2\text{/s}}
$$

**验证（动量臂法）**：$r_\perp = r\sin 30^\circ = 3.0 \times 0.5 = 1.5\ \text{m}$

$L = r_\perp mv = 1.5 \times 2.0 \times 8.0 = 24\ \text{kg·m}^2\text{/s}$ ✓

> 💡 角动量的方向：用右手定则，四指从 $\vec{r}$ 弯向 $\vec{v}$，大拇指方向即为 $\vec{L}$ 方向（垂直纸面向外或向内）。

---

#### 6.3.4 🧪 例题 2：力矩产生的角动量变化

**题目**：一个飞轮（$I = 2.5\ \text{kg·m}^2$）初始以 $\omega_i = 10\ \text{rad/s}$ 旋转。对其施加恒定的 $8.0\ \text{N·m}$ 制动力矩（与旋转方向相反），持续 $3.0\ \text{s}$。求：
(a) 角冲量的大小
(b) 飞轮的末角速度
(c) 若要使飞轮完全停止，还需要多长时间？

**题目分析**：

> **已知**：$I = 2.5\ \text{kg·m}^2$，$\omega_i = 10\ \text{rad/s}$，$\tau = -8.0\ \text{N·m}$（制动），$\Delta t = 3.0\ \text{s}$
>
> **求**：角冲量、$\omega_f$、附加制动时间
>
> **策略**：用角冲量-角动量定理 $\tau\Delta t = \Delta L = I(\omega_f - \omega_i)$。

**解答**：

**(a)** 角冲量大小：$|\tau\Delta t| = 8.0 \times 3.0 = \mathbf{24\ \text{N·m·s}}$

**(b)** 由 $\tau\Delta t = I\omega_f - I\omega_i$：

$$
-8.0 \times 3.0 = 2.5\omega_f - 2.5 \times 10
$$

$$
-24 = 2.5\omega_f - 25
$$

$$
2.5\omega_f = 1 \quad \Rightarrow \quad \omega_f = \mathbf{0.40\ \text{rad/s}}
$$

**(c)** 从当前 $\omega_f = 0.40\ \text{rad/s}$ 制动到 $0$：
$$
\tau\Delta t' = 0 - I\omega_f
$$
$$
-8.0 \times \Delta t' = -2.5 \times 0.40
$$
$$
\Delta t' = \frac{1.0}{8.0} = \mathbf{0.125\ \text{s}}
$$

> 💡 **角冲量的直观理解**：$3.0\ \text{s}$ 内制动力矩提供了 $-24\ \text{kg·m}^2\text{/s}$ 的角动量变化，使角速度从 $10$ 降至 $0.40\ \text{rad/s}$。角冲量的单位 $\text{N·m·s}$ 等价于 $\text{kg·m}^2\text{/s}$（角动量单位）。

---

#### 6.3.5 🧪 例题 3：行星轨道的角动量

**题目**：地球绕太阳的轨道可近似为半径 $r = 1.50 \times 10^{11}\ \text{m}$ 的圆。地球质量 $m = 5.97 \times 10^{24}\ \text{kg}$，轨道速度 $v = 2.98 \times 10^4\ \text{m/s}$。求：
(a) 地球对太阳的轨道角动量大小
(b) 若将地球突然移到 $r' = 2.0 \times 10^{11}\ \text{m}$ 的圆轨道（保持角动量守恒），新轨道速度是多少？
(c) 比较新旧轨道的转动动能

**题目分析**：

> 地球对太阳的角动量 = $rmv$（$\vec{r} \perp \vec{v}$）。

**解答**：

**(a)** $L = rmv = 1.50 \times 10^{11} \times 5.97 \times 10^{24} \times 2.98 \times 10^4$
$$
\approx \mathbf{2.67 \times 10^{40}\ \text{kg·m}^2\text{/s}}
$$

**(b)** 角动量守恒：$rmv = r'mv'$ → $v' = v \cdot \frac{r}{r'} = 2.98 \times 10^4 \times \frac{1.50}{2.00} = \mathbf{2.24 \times 10^4\ \text{m/s}}$

**(c)** $K = \frac{1}{2}mv^2$：
- 旧轨道：$K = \frac{1}{2} \times 5.97 \times 10^{24} \times (2.98 \times 10^4)^2 \approx 2.65 \times 10^{33}\ \text{J}$
- 新轨道：$K' = \frac{1}{2} \times 5.97 \times 10^{24} \times (2.24 \times 10^4)^2 \approx 1.49 \times 10^{33}\ \text{J}$

> 💡 轨道越高，速度越慢，动能越小。用 $K = L^2/(2I)$ 理解：$L$ 守恒，$I = mr^2$ 增大，$K \propto 1/I$ 减小。但注意实际轨道转移需要外力矩（火箭推力），所以角动量不守恒——这里仅为示意。

---

#### 6.3.6 🧪 例题 4：碰撞中的角冲量

**题目**：一个 $m = 0.10\ \text{kg}$ 的小球以 $v = 20\ \text{m/s}$ 的速度水平飞来，击中一根可绕上端旋转的竖直细杆的中点，并以 $v/2$ 反弹。杆长 $L = 1.0\ \text{m}$，质量 $M = 2.0\ \text{kg}$。碰撞时间 $\Delta t = 0.010\ \text{s}$。求碰撞期间杆对球的平均力矩大小。

**题目分析**：

> 球对杆上端的角动量变化 = 力矩 × 时间（角冲量）。先求球的角动量变化，再求平均力矩。

**解答**：

球的初角动量（对杆上端，$r = L/2 = 0.50\ \text{m}$）：
$$
L_i = rmv = 0.50 \times 0.10 \times 20 = 1.0\ \text{kg·m}^2\text{/s}
$$

末角动量（反弹，$v_f = -10\ \text{m/s}$）：
$$
L_f = rm(-v/2) = 0.50 \times 0.10 \times (-10) = -0.50\ \text{kg·m}^2\text{/s}
$$

角动量变化：$\Delta L_{\text{ball}} = L_f - L_i = -0.50 - 1.0 = -1.50\ \text{kg·m}^2\text{/s}$

由杆对球的角冲量 = 球的角动量变化（杆对球的力矩与球的角动量变化方向相反）：
$$
\tau_{\text{avg}} \cdot \Delta t = |\Delta L_{\text{ball}}|
$$
$$
\tau_{\text{avg}} = \frac{1.50}{0.010} = \mathbf{150\ \text{N·m}}
$$

> 💡 碰撞中的力矩可以极其巨大——$150\ \text{N·m}$ 相当于一个 $75\ \text{kg}$ 的人站在 $0.20\ \text{m}$ 扳手上的效果。这就是为什么碰撞（锤击、撞击）能产生远大于静力的转动力矩。

---

### 本节总结

角动量和角冲量是第六章的理论基石：

1. **$L = I\omega$**（刚体）或 **$L = rmv\sin\theta$**（质点）
2. **$\vec{\tau} = d\vec{L}/dt$** — 转动动力学最普遍形式
3. **角冲量 = $\int\tau\,dt = \Delta L$** — 与冲量-动量定理完全对应

### ⚠️ 常见误区辨析

> ❌ **误区 1**：「角动量就是旋转的动量，只对旋转的物体有意义。」
>
> ✅ **正确**：角动量可以在任何运动中对任意参考点定义。沿直线运动的质点对不在其运动直线上的点也有角动量——$L = rmv\sin\theta$。角动量不等于「自旋」。

> ❌ **误区 2**：「角冲量的单位很特殊。」
>
> ✅ **正确**：角冲量的单位 $\text{N·m·s}$ 等价于 $\text{kg·m}^2\text{/s}$（角动量单位）。量纲上 $[\tau t] = [L]$ 是必然的——因为 $\vec{\tau} = d\vec{L}/dt$。

> ❌ **误区 3**：「$\tau = I\alpha$ 和 $\tau = dL/dt$ 是两种不同的物理定律。」
>
> ✅ **正确**：$\tau = I\alpha$ 是 $\tau = dL/dt$ 在 $I$ 恒定时的特例。后者是更基本的方程。AP Physics C 明确要求区分这两种情况。

# 6.4 角动量守恒（Conservation of Angular Momentum）

## Part A：基础层（AP Physics 1 必备）

### 一、角动量守恒定律

> 当系统所受的**合外力矩为零**（$\Sigma \vec{\tau}_{\text{ext}} = 0$）时，系统的总角动量保持不变：
>
> $$
> \boxed{\vec{L}_i = \vec{L}_f}
> $$
>
> 即：
> $$
> \boxed{I_i\omega_i = I_f\omega_f}
> $$

角动量守恒是物理学中最优美、应用最广泛的守恒定律之一。从天体物理中星系的旋转到花样滑冰运动员的旋转，从量子力学中的粒子自旋到直升机尾桨的设计，角动量守恒无处不在。它比动量守恒更「微妙」——因为角动量依赖于参考点的选择，但一旦确定系统和外力矩为零，它就铁面无私地守恒。

> 📐 **角动量守恒的三种等价表述** — 同一原理，三种形式：
>
> | 视角 | 表达式 | 物理含义 | 典型应用 |
> |:--|:--|:--|:--|
> | **矢量守恒形式** | $\vec{L}_i = \vec{L}_f$ | 总角动量矢量不变（大小和方向都不变） | 陀螺仪定轴性、行星轨道平面不变 |
> | **$I\omega$ 乘积形式** | $I_i\omega_i = I_f\omega_f$ | $I$ 和 $\omega$ 反向变化，乘积恒定 | 滑冰收臂、跳水展体、中子星坍缩 |
> | **微分形式** | $\frac{d\vec{L}}{dt} = 0$（当 $\Sigma\vec{\tau}_{\text{ext}} = 0$） | 角动量的时间变化率为零 | 判断是否守恒、理论推导 |
>
> 🧠 **统一理解**：这三种形式在数学上完全等价，但在解题中各有优势。矢量形式强调方向守恒，$I\omega$ 形式适合定量计算，微分形式适合判断守恒条件是否满足。

> 📝 **Step-by-Step：角动量守恒问题的通用解题流程**
>
> 1. **定义系统**：明确哪些物体属于系统
> 2. **选择参考点/转轴**：角动量必须对同一个点或轴计算
> 3. **检查外力矩**：$\Sigma\vec{\tau}_{\text{ext}} = 0$ 是否成立？如果碰撞时间极短，外力矩的角冲量可忽略
> 4. **写出初末角动量**：$L_i = L_f$，注意 $I$ 可能变化
> 5. **关联运动学量**：如有滚动，用 $v = R\omega$；如有绳连接，用 $a = R\alpha$
> 6. **解出未知量**：代数求解
> 7. **验证合理性**：$\omega$ 是否在物理合理范围内？动能是否守恒（弹性碰撞）或不守恒（非弹性碰撞）？

### 二、角动量守恒的三种典型情形

| 情形 | $I$ 变化 | $\omega$ 变化 | 实例 |
|:--|:--:|:--:|:--|
| **转动惯量改变** | 减小 | 增大 | 滑冰运动员收臂加速旋转 |
| **转动惯量改变** | 增大 | 减小 | 跳水运动员展体减速 |
| **系统重新分布** | 部分转移 | — | 直升机尾桨抵消机身旋转 |

### 三、角动量守恒的条件

> ⚠️ **角动量守恒的条件是合外力矩为零，而非合力为零！**

- 合力为零但合力矩不为零 → 角动量不守恒（如力偶）
- 合力矩为零但合力不为零 → 角动量守恒（如行星绕太阳，引力过参考点）

### 四、与动量守恒的对比

| | 动量守恒 | 角动量守恒 |
|:--|:--|:--|
| 条件 | $\Sigma \vec{F}_{\text{ext}} = 0$ | $\Sigma \vec{\tau}_{\text{ext}} = 0$ |
| 守恒量 | $\vec{p} = m\vec{v}$ | $\vec{L} = I\vec{\omega}$ |
| $m$ 可变时 | $\vec{p}$ 守恒（如火箭） | $I$ 可变时 $L$ 守恒（如滑冰） |

### 五、角动量守恒的深度理解

#### 5.1 为什么角动量守恒如此普遍？

角动量守恒源于空间的**旋转对称性**——这是诺特定理（Noether's Theorem）的深刻结论。简单来说：物理定律在所有方向上都是相同的（空间各向同性），导致角动量必然守恒。这一原理在经典力学、量子力学和相对论中都成立。

#### 5.2 角动量守恒 vs 动量守恒 vs 能量守恒

| 守恒定律 | 守恒条件 | 被什么破坏 | 适用范围 |
|:--|:--|:--|:--|
| 能量 | 无耗散力做功 | 摩擦力、空气阻力 | 孤立系统 |
| 动量 | $\Sigma\vec{F}_{\text{ext}} = 0$ | 外力 | 任何孤立系统 |
| 角动量 | $\Sigma\vec{\tau}_{\text{ext}} = 0$ | 外力矩 | 任何孤立系统 |

> ⚠️ 在碰撞问题中：动量始终守恒（碰撞内力不产生净外力），角动量也守恒（内力矩抵消），但动能只有在弹性碰撞中才守恒。

#### 5.3 角动量守恒的三种实现机制

**(a) $I$ 和 $\omega$ 反向变化（最常见）**：
运动员收臂 → $I$ 减小 → $\omega$ 增大 → $L = I\omega$ 不变。这是角动量守恒最直观的体现。

**(b) 旋转方向的改变**：
跳水运动员在空中可以翻转身体朝向——$\vec{L}$ 的方向不变（守恒），但身体各部分相对位置改变，产生不同的视觉效果。猫从高处落下总能用脚着地也是这个原理。

**(c) 多体系统中的角动量重新分配**：
直升机主旋翼旋转时，机身会产生反向旋转趋势（角动量守恒）。尾桨的作用就是提供抵消力矩——或者用两个反向旋转的主旋翼（如 CH-47 支努干）。

#### 5.4 角动量守恒在天体物理中的关键作用

- **太阳系的形成**：原始星云缓慢旋转，在引力收缩过程中 $I$ 减小、$\omega$ 增大，形成旋转的原始太阳和行星盘。
- **脉冲星**：恒星核坍缩时半径缩小百万倍，$I \propto R^2$ 缩小万亿倍，$\omega$ 增大万亿倍——从 27 天一圈变为每秒数百圈。
- **星系旋臂**：星系的自转是角动量守恒的结果。旋臂结构来自引力扰动和差速旋转。
- **黑洞吸积盘**：物质落入黑洞时角动量守恒，形成高速旋转的吸积盘——其内缘温度可达数百万度，发出 X 射线。

#### 5.5 常见误区辨析

> ❌ **误区 1**：「角动量守恒要求合力为零。」
>
> ✅ **正确**：角动量守恒要求**合外力矩为零**。行星受太阳引力（合力不为零），但引力过太阳中心（力臂为零），力矩为零，因此角动量守恒。

> ❌ **误区 2**：「角动量守恒时动能也守恒。」
>
> ✅ **正确**：角动量守恒时 $L = I\omega$ 不变，但 $K = L^2/(2I)$ 在 $I$ 改变时会变化。运动员收臂时动能增大——肌肉做功提供了额外能量。

> ❌ **误区 3**：「角动量守恒只在转动问题中有用。」
>
> ✅ **正确**：开普勒第二定律（行星面积速度恒定）正是角动量守恒的直接推论——而行星运动是「平动」（沿轨道运行），不是绕自身轴的旋转。

---

#### 6.4.1 🧪 推导 1：从 $\vec{\tau}_{\text{ext}} = d\vec{L}/dt$ 导出角动量守恒

**推导目标**：证明当合外力矩为零时系统角动量守恒。

**推导过程**：

由 $\vec{\tau}_{\text{ext}} = \dfrac{d\vec{L}_{\text{sys}}}{dt}$（系统角动量的时间变化率等于合外力矩）。

若 $\Sigma \vec{\tau}_{\text{ext}} = 0$，则：

$$
\frac{d\vec{L}_{\text{sys}}}{dt} = 0
$$

这意味着 $\vec{L}_{\text{sys}}$ 不随时间变化——即角动量守恒：

$$
\boxed{\vec{L}_{\text{sys}} = \text{常数}}
$$

对于绕固定轴旋转的单个刚体：

$$
L_i = L_f \quad \Rightarrow \quad I_i\omega_i = I_f\omega_f
$$

**守恒的微观机制**：即使 $I$ 和 $\omega$ 各自可以变化（如滑冰运动员收臂），只要没有外力矩，$I\omega$ 的乘积保持不变。内部力——如运动员的肌肉力——不改变系统的总角动量，因为它们不产生净外力矩。

> 💡 **关键理解**：内部力可以改变 $I$ 的分布（从而改变 $\omega$），但不能改变 $L$。这就像内部力可以改变系统的动能分配但不会改变总动量——内力的力矩之和恒为零（牛顿第三定律保证）。

---

#### 6.4.2 🧪 推导 2：花样滑冰旋转的定量分析

**推导目标**：建立滑冰运动员收臂时角速度变化的定量模型，推导 $\omega_f = \omega_i \cdot \dfrac{I_i}{I_f}$。

**推导过程**：

将滑冰运动员简化为两个模型：

**初始状态**（手臂展开）：转动惯量 $I_i = I_{\text{身体}} + 2mR_1^2$，其中 $m$ 是单只手臂的质量，$R_1$ 是手臂质心到转轴的距离。

**末状态**（手臂收回）：转动惯量 $I_f = I_{\text{身体}} + 2mR_2^2$，其中 $R_2 \ll R_1$。

由角动量守恒（冰面摩擦力矩可忽略）：

$$
I_i\omega_i = I_f\omega_f
$$

$$
\boxed{\omega_f = \omega_i \cdot \frac{I_i}{I_f}}
$$

由于 $I_i > I_f$（手臂展开时转动惯量更大），所以 $\omega_f > \omega_i$——转速增大。

**动能变化**：初动能 $K_i = \frac{1}{2}I_i\omega_i^2$，末动能 $K_f = \frac{1}{2}I_f\omega_f^2$。

利用 $\omega_f = \dfrac{I_i}{I_f}\omega_i$：

$$
K_f = \frac{1}{2}I_f\left(\frac{I_i}{I_f}\omega_i\right)^2 = \frac{I_i}{I_f} \cdot \frac{1}{2}I_i\omega_i^2 = \frac{I_i}{I_f}K_i
$$

因为 $I_i > I_f$，所以 $K_f > K_i$——动能**增大**了！

> 💡 **能量从哪来？** 运动员收臂时肌肉做正功（克服离心力），这个功转化为转动动能的增加。角动量守恒保证了 $I\omega$ 不变，而动能 $K = L^2/(2I)$ 随 $I$ 减小而增大——肌肉做功是能量来源。

---

#### 6.4.2b 🧪 推导 3：开普勒第二定律——角动量守恒的几何证明

**推导目标**：从角动量守恒出发，严格证明行星与太阳的连线在相等时间内扫过相等的面积。

**推导过程**：

行星对太阳的角动量 $\vec{L} = \vec{r} \times m\vec{v}$。引力始终指向太阳（中心力），对太阳的力矩 $\vec{\tau} = \vec{r} \times \vec{F} = 0$（$\vec{r} \parallel \vec{F}$），因此角动量守恒。

在 $dt$ 时间内，行星的位移为 $d\vec{r} = \vec{v}\,dt$。矢径扫过的三角形面积为：

$$
dA = \frac{1}{2}|\vec{r} \times d\vec{r}| = \frac{1}{2}|\vec{r} \times \vec{v}|\,dt
$$

而 $|\vec{r} \times \vec{v}| = \dfrac{|\vec{L}|}{m}$（由 $\vec{L} = \vec{r} \times m\vec{v}$），所以：

$$
\frac{dA}{dt} = \frac{|\vec{L}|}{2m} = \text{常数}
$$

因此：
$$
\boxed{\frac{dA}{dt} = \text{常数}}
$$

> 💡 **面积速度恒定**是角动量守恒的直接几何表现。行星在近日点速度大（$r$ 小 → $v$ 大）、在远日点速度小（$r$ 大 → $v$ 小），恰好使 $r \times v$ 保持恒定。这并非巧合——正是角动量守恒迫使行星按此方式运动。

---

#### 6.4.2c 🧪 推导 4：非弹性转动碰撞中的角动量守恒

**推导目标**：证明在完全非弹性转动碰撞中（如两个圆盘碰撞后粘在一起），角动量守恒但动能不守恒。

**推导过程**：

设圆盘 1（$I_1$、$\omega_1$）与静止圆盘 2（$I_2$、$\omega_2 = 0$）同轴碰撞后粘在一起。

**碰撞前**：$L_i = I_1\omega_1$，$K_i = \frac{1}{2}I_1\omega_1^2$

**碰撞中**：内力矩不改变系统总角动量（作用力-反作用力对同一轴的力矩抵消）

**碰撞后**：$L_f = (I_1 + I_2)\omega_f$

角动量守恒：
$$
I_1\omega_1 = (I_1 + I_2)\omega_f \quad \Rightarrow \quad \omega_f = \frac{I_1}{I_1 + I_2}\omega_1
$$

末动能：
$$
K_f = \frac{1}{2}(I_1 + I_2)\omega_f^2 = \frac{1}{2}(I_1 + I_2)\left(\frac{I_1}{I_1 + I_2}\omega_1\right)^2 = \frac{I_1}{I_1 + I_2} \cdot \frac{1}{2}I_1\omega_1^2 = \frac{I_1}{I_1 + I_2}K_i
$$

动能损失：
$$
\boxed{\Delta K = K_f - K_i = -\frac{I_2}{I_1 + I_2}K_i < 0}
$$

> 💡 **类比**：这与平动中的完全非弹性碰撞 $m_1v_1 = (m_1+m_2)v_f$ 完全对应。转动碰撞中「粘在一起」导致动能损失，损失的能量转化为热和声——如同两辆汽车碰撞后一起滑行。

---

#### 6.4.2d 🧪 推导 5：碰撞中的角动量守恒——冲量近似证明

**推导目标**：严格证明在碰撞时间极短的条件下，即使存在外力矩，系统角动量仍近似守恒。

**推导过程**：

考虑碰撞过程中系统受到外力矩 $\tau_{\text{ext}}$（如重力对支点的力矩）。角动量变化为：

$$
\Delta L = \int_{t_i}^{t_f} \tau_{\text{ext}}\,dt
$$

碰撞时间 $\Delta t = t_f - t_i$ 通常极短（$\sim 10^{-3}\ \text{s}$ 量级）。对于典型外力矩（如重力矩 $\sim MgL$），若 $\tau_{\text{ext}}$ 在碰撞期间近似恒定：

$$
|\Delta L| = |\tau_{\text{ext}}|\Delta t
$$

而碰撞内力矩极大（$\sim 10^2$–$10^4\ \text{N·m}$），内力矩的角冲量主导角动量在系统内部的重新分配。外力矩的角冲量相比之下可忽略：

$$
\frac{|\tau_{\text{ext}}\Delta t|}{|L_{\text{sys}}|} \ll 1
$$

**数值验证**：子弹击中杆，碰撞时间 $\Delta t \approx 0.001\ \text{s}$，重力矩 $\tau_g \approx MgL/2 \approx 10\ \text{N·m}$，角冲量 $\approx 0.01\ \text{N·m·s}$。子弹角动量 $\approx 15\ \text{kg·m}^2\text{/s}$。相对误差 $\approx 0.07\%$——完全可以忽略。

因此：
$$
\boxed{\Delta L_{\text{sys}} \approx 0 \quad \text{（碰撞期间角动量近似守恒）}}
$$

> 💡 **冲量近似的精髓**：碰撞时间极短 → 外力矩的角冲量 $\tau_{\text{ext}}\Delta t \to 0$ → 角动量守恒。但碰撞后（长时间尺度），外力矩的累积效果不可忽略——这就是为什么弹道摆碰后能量守恒阶段不能忽略重力。

---

#### 6.4.7 🧪 例题 5：旋转木马——人从边缘走向中心

**题目**：一个半径 $R = 3.0\ \text{m}$、质量 $M = 200\ \text{kg}$ 的圆形旋转平台（$I = \frac{1}{2}MR^2$）以 $\omega_i = 2.0\ \text{rad/s}$ 旋转。一个 $m = 60\ \text{kg}$ 的人最初站在平台边缘，然后走向平台中心。求：
(a) 人走到距中心 $r = 0.50\ \text{m}$ 处时平台的角速度
(b) 系统动能变化了多少？能量从哪里来？
(c) 若人走到中心（$r = 0$），角速度是多少？

**题目分析**：

> **已知**：$M = 200\ \text{kg}$，$R = 3.0\ \text{m}$，$\omega_i = 2.0\ \text{rad/s}$，$m = 60\ \text{kg}$
>
> **求**：$\omega_f$（$r = 0.50\ \text{m}$ 和 $r = 0$），$\Delta K$
>
> **策略**：角动量守恒（无外力矩）。人视为质点，$I_{\text{person}} = mr^2$。

**解答**：

平台转动惯量：$I_{\text{platform}} = \frac{1}{2}MR^2 = \frac{1}{2} \times 200 \times 9.0 = 900\ \text{kg·m}^2$

**(a)** 初始人 $r_i = R = 3.0\ \text{m}$：
$$
I_i = 900 + 60 \times 9.0 = 900 + 540 = 1440\ \text{kg·m}^2
$$

末态人 $r_f = 0.50\ \text{m}$：
$$
I_f = 900 + 60 \times 0.25 = 900 + 15 = 915\ \text{kg·m}^2
$$

角动量守恒：$I_i\omega_i = I_f\omega_f$
$$
\omega_f = 2.0 \times \frac{1440}{915} \approx \mathbf{3.15\ \text{rad/s}}
$$

**(b)** $K_i = \frac{1}{2} \times 1440 \times 4.0 = 2880\ \text{J}$

$K_f = \frac{1}{2} \times 915 \times (3.15)^2 \approx 4540\ \text{J}$

$\Delta K \approx \mathbf{+1660\ \text{J}}$——动能增大了！能量来自人走向中心时**克服离心力做的功**（肌肉做功转化为转动动能）。

**(c)** 人在中心（$r = 0$）：$I_f = 900\ \text{kg·m}^2$
$$
\omega_f = 2.0 \times \frac{1440}{900} = \mathbf{3.20\ \text{rad/s}}
$$

> 💡 **有趣的事实**：即使人走到了正中心，角速度也只是增加了 $60\%$——因为平台本身的转动惯量（$900$）远大于人的贡献（$540 \to 0$）。如果平台更轻，效果会更显著。

---

#### 6.4.8 🧪 例题 6：转动碰撞中的角动量守恒——不同轴碰撞

**题目**：一根长 $L = 1.2\ \text{m}$、质量 $M = 3.0\ \text{kg}$ 的均匀细杆静止在光滑水平面上。一个 $m = 0.10\ \text{kg}$ 的油灰球以 $v = 25\ \text{m/s}$ 的速度垂直击中杆的一端并粘住。求：
(a) 碰撞后系统质心的速度
(b) 碰撞后系统绕质心的角速度
(c) 碰撞中损失的动能百分比

**题目分析**：

> 碰撞后：杆+油灰系统既有平动（质心运动）又有转动（绕质心）。先用动量守恒求质心速度，再用角动量守恒（对质心）求角速度。

**解答**：

**(a)** 动量守恒（水平方向无外力）：
$$
mv = (M + m)v_{cm}
$$
$$
v_{cm} = \frac{0.10 \times 25}{3.0 + 0.10} = \frac{2.5}{3.10} \approx \mathbf{0.806\ \text{m/s}}
$$

**(b)** 系统质心位置（从杆中心算起，向油灰一侧为正）：

杆中心为原点。油灰粘在杆一端，距杆中心 $L/2 = 0.60\ \text{m}$。

质心距杆中心：$x_{cm} = \frac{M \cdot 0 + m \cdot (L/2)}{M + m} = \frac{0.10 \times 0.60}{3.10} \approx 0.0194\ \text{m}$

碰撞前油灰对系统质心的角动量：

油灰距系统质心：$r_\perp = 0.60 - 0.0194 = 0.5806\ \text{m}$（近似为 $L/2$）

$$
L_i = m v r_\perp \approx 0.10 \times 25 \times 0.5806 \approx 1.4515\ \text{kg·m}^2\text{/s}
$$

系统绕质心的转动惯量（平行轴定理）：

杆绕质心：$I_{\text{rod,cm}} = \frac{1}{12}ML^2 = \frac{1}{12} \times 3.0 \times 1.44 = 0.36\ \text{kg·m}^2$

杆对系统质心：$I_{\text{rod}} = 0.36 + 3.0 \times (0.0194)^2 \approx 0.361\ \text{kg·m}^2$

油灰对系统质心：$I_{\text{putty}} = 0.10 \times (0.5806)^2 \approx 0.0337\ \text{kg·m}^2$

$$
I_{\text{total}} \approx 0.361 + 0.0337 = 0.3947\ \text{kg·m}^2
$$

角动量守恒（对系统质心）：
$$
\omega = \frac{L_i}{I_{\text{total}}} = \frac{1.4515}{0.3947} \approx \mathbf{3.68\ \text{rad/s}}
$$

**(c)** 初动能：$K_i = \frac{1}{2}mv^2 = \frac{1}{2} \times 0.10 \times 625 = 31.25\ \text{J}$

末动能：$K_f = \frac{1}{2}(M+m)v_{cm}^2 + \frac{1}{2}I_{\text{total}}\omega^2$
$$
= \frac{1}{2} \times 3.10 \times 0.650 + \frac{1}{2} \times 0.3947 \times 13.54 \approx 1.008 + 2.672 = 3.68\ \text{J}
$$

损失：$\Delta K = 3.68 - 31.25 = -27.57\ \text{J}$，约 $\mathbf{88.2\%}$ 损失！

> 💡 **完全非弹性碰撞的巨大能量损失**：油灰粘在杆上，类似两车碰撞后一起滑行——$88\%$ 的能量转化为热和变形能。仅有约 $12\%$ 的初始动能保留为机械能。

---

#### 6.4.3 🧪 例题 1：旋转平台上的角动量守恒

**题目**：一个学生手持两个 $2.0\ \text{kg}$ 的哑铃站在可自由旋转的平台上，初始角速度 $\omega_i = 3.0\ \text{rad/s}$。学生+平台（不含哑铃）的转动惯量为 $6.0\ \text{kg·m}^2$。哑铃初始距转轴 $0.80\ \text{m}$，学生将哑铃收到距转轴 $0.20\ \text{m}$ 处。求：
(a) 初始总转动惯量
(b) 末总转动惯量
(c) 末角速度

**题目分析**：

> **已知**：$m_{\text{dumbbell}} = 2.0\ \text{kg} \times 2$，$I_{\text{student}} = 6.0\ \text{kg·m}^2$，$r_i = 0.80\ \text{m}$，$r_f = 0.20\ \text{m}$，$\omega_i = 3.0\ \text{rad/s}$
>
> **求**：$I_i$、$I_f$、$\omega_f$
>
> **策略**：哑铃视为质点，$I_{\text{dumbbells}} = 2 \times mr^2$。用角动量守恒。

**解答**：

**(a)** 初始总转动惯量：
$$
I_i = I_{\text{student}} + 2mr_i^2 = 6.0 + 2 \times 2.0 \times (0.80)^2 = 6.0 + 2.56 = \mathbf{8.56\ \text{kg·m}^2}
$$

**(b)** 末总转动惯量：
$$
I_f = I_{\text{student}} + 2mr_f^2 = 6.0 + 2 \times 2.0 \times (0.20)^2 = 6.0 + 0.16 = \mathbf{6.16\ \text{kg·m}^2}
$$

**(c)** 角动量守恒 $I_i\omega_i = I_f\omega_f$：
$$
\omega_f = \omega_i \cdot \frac{I_i}{I_f} = 3.0 \times \frac{8.56}{6.16} \approx \mathbf{4.17\ \text{rad/s}}
$$

> 💡 **角速度增大了约 39%**——哑铃从 $0.80\ \text{m}$ 收到 $0.20\ \text{m}$（距离缩小到 $1/4$），哑铃对 $I$ 的贡献从 $2.56$ 降到 $0.16$（缩小到 $1/16$，因为 $I \propto r^2$）。

---

#### 6.4.4 🧪 例题 2：圆盘与人——系统角动量守恒

**题目**：一个半径 $2.0\ \text{m}$、质量 $100\ \text{kg}$ 的均匀圆盘（$I = \frac{1}{2}MR^2$）可绕中心轴自由旋转，初始静止。一个 $m = 60\ \text{kg}$ 的人从圆盘边缘以相对于圆盘 $v_{\text{rel}} = 2.0\ \text{m/s}$ 的切向速度沿边缘行走。求圆盘的角速度。

**题目分析**：

> **已知**：$M = 100\ \text{kg}$，$R = 2.0\ \text{m}$，$m = 60\ \text{kg}$，$v_{\text{rel}} = 2.0\ \text{m/s}$
>
> **求**：圆盘角速度 $\omega_{\text{disk}}$
>
> **策略**：系统初始角动量为零 → 末总角动量也为零。圆盘角动量 + 人角动量 = 0。

**解答**：

设圆盘角速度为 $\omega_d$（逆时针为正）。

人的绝对速度 $v = v_{\text{rel}} + \omega_d R$（相对于地面的速度 = 相对速度 + 牵连速度）。

人的角动量（视为质点）：$L_{\text{person}} = mRv = mR(v_{\text{rel}} + \omega_d R)$

圆盘的角动量：$L_{\text{disk}} = I\omega_d = \frac{1}{2}MR^2\omega_d$

角动量守恒（初始为零）：
$$
L_{\text{person}} + L_{\text{disk}} = 0
$$

$$
mR(v_{\text{rel}} + \omega_d R) + \frac{1}{2}MR^2\omega_d = 0
$$

$$
mRv_{\text{rel}} + mR^2\omega_d + \frac{1}{2}MR^2\omega_d = 0
$$

$$
mRv_{\text{rel}} = -\left(mR^2 + \frac{1}{2}MR^2\right)\omega_d
$$

$$
\omega_d = -\frac{mRv_{\text{rel}}}{R^2(m + \frac{1}{2}M)} = -\frac{60 \times 2.0 \times 2.0}{4.0 \times (60 + 50)} = -\frac{240}{4.0 \times 110} = -\frac{240}{440} \approx \mathbf{-0.545\ \text{rad/s}}
$$

> 💡 **负号的含义**：圆盘以 $0.545\ \text{rad/s}$ 沿与人行走**相反**的方向旋转。这是角动量守恒的直接体现——人获得顺时针角动量，圆盘必须获得逆时针角动量使总量保持为零。

---

#### 6.4.5 🧪 例题 3：两个圆盘的非弹性转动碰撞

**题目**：圆盘 A（$I_A = 0.60\ \text{kg·m}^2$）以 $\omega_A = 12\ \text{rad/s}$ 绕固定轴旋转。圆盘 B（$I_B = 0.40\ \text{kg·m}^2$）初始静止在同一轴上。两圆盘碰撞后粘在一起。求：
(a) 碰撞后的角速度
(b) 碰撞中损失的动能
(c) 损失的能量去哪了

**题目分析**：

> 同轴碰撞 → 角动量守恒，完全非弹性 → 粘在一起。

**解答**：

**(a)** 角动量守恒：
$$
I_A\omega_A = (I_A + I_B)\omega_f
$$
$$
\omega_f = \frac{0.60 \times 12}{0.60 + 0.40} = \frac{7.2}{1.0} = \mathbf{7.2\ \text{rad/s}}
$$

**(b)** 初动能：$K_i = \frac{1}{2} \times 0.60 \times 12^2 = 43.2\ \text{J}$

末动能：$K_f = \frac{1}{2} \times 1.0 \times 7.2^2 = 25.92\ \text{J}$

损失：$\Delta K = 25.92 - 43.2 = \mathbf{-17.28\ \text{J}}$（损失 $40\%$）

**(c)** 能量转化为热能和声能——两盘接触面之间的摩擦将机械能耗散。

> 💡 损失比例 = $\frac{I_B}{I_A + I_B} = 0.40$，恰好等于 $B$ 的转动惯量占比。这类似于平动中 $m_2/(m_1+m_2)$ 的能量损失比例。

---

#### 6.4.6 🧪 例题 4：中子星的自转加速——天体物理中的角动量守恒

**题目**：一颗恒星（类似太阳）以 $\omega_i = 2.7 \times 10^{-6}\ \text{rad/s}$（约 27 天一圈）自转，半径 $R_i = 7.0 \times 10^8\ \text{m}$，质量 $M = 2.0 \times 10^{30}\ \text{kg}$。当它坍缩为中子星时，半径变为 $R_f = 1.0 \times 10^4\ \text{m}$（密度均匀的球，$I = \frac{2}{5}MR^2$）。假设角动量守恒，求中子星的自转周期。

**题目分析**：

> $I \propto R^2$，$R$ 缩小 $7 \times 10^4$ 倍，$I$ 缩小 $(7 \times 10^4)^2$ 倍，$\omega$ 增大同样倍数。

**解答**：

角动量守恒：$I_i\omega_i = I_f\omega_f$

由于 $I \propto R^2$：
$$
\frac{\omega_f}{\omega_i} = \frac{I_i}{I_f} = \frac{R_i^2}{R_f^2} = \left(\frac{7.0 \times 10^8}{1.0 \times 10^4}\right)^2 = (7.0 \times 10^4)^2 = 4.9 \times 10^9
$$

$$
\omega_f = 2.7 \times 10^{-6} \times 4.9 \times 10^9 \approx 1.32 \times 10^4\ \text{rad/s}
$$

周期：$T_f = \dfrac{2\pi}{\omega_f} = \dfrac{2\pi}{1.32 \times 10^4} \approx \mathbf{4.75 \times 10^{-4}\ \text{s} \approx 0.48\ \text{ms}}$

> 💡 恒星从 27 天一圈变为每秒旋转约 2100 圈！这就是脉冲星——快速旋转的中子星发出极其规律的电磁脉冲，被誉为「宇宙中最精确的时钟」。角动量守恒是天体物理中最强大的工具之一。

---

### 本节总结

角动量守恒是第六章最核心的考点：

1. **条件**：$\Sigma \vec{\tau}_{\text{ext}} = 0$
2. **$I_i\omega_i = I_f\omega_f$** — $I$ 和 $\omega$ 反向变化
3. **守恒时动能可以变化** — 内部力做功改变 $I$ 分布，$K = L^2/(2I)$
4. **角动量是矢量** — 方向由右手定则确定，守恒包括方向不变

### ⚠️ 常见误区辨析

> ❌ **误区 1**：「角动量守恒意味着系统的角速度不变。」
>
> ✅ **正确**：角动量守恒意味着 $L = I\omega$ 不变。$I$ 可以变化（改变姿态、质量分布），$\omega$ 随之反向变化。滑冰运动员收臂时 $\omega$ 增大正是角动量守恒的结果——而非违反。

> ❌ **误区 2**：「内力矩不能改变总角动量，所以内部力对旋转没有影响。」
>
> ✅ **正确**：内力矩确实不能改变总角动量，但内部力可以重新分配系统内各部分的角动量。猫在空中扭转身体、直升机尾桨抵消机身旋转，都是内部力重新分配角动量的例子。

> ❌ **误区 3**：「碰撞中角动量守恒自动成立。」
>
> ✅ **正确**：只有外力矩的角冲量可忽略时角动量才守恒。典型的碰撞时间极短（毫秒级），外力矩（如重力、轴摩擦力）的角冲量 $\tau\Delta t$ 通常可以忽略——但你需要**明确声明**这一近似。

# 6.5 滚动（Rolling）

## Part A：基础层（AP Physics 1 必备）

### 一、纯滚动的物理本质

> **纯滚动（Rolling Without Slipping）** 是指物体在表面上滚动时，接触点相对于表面瞬时静止——没有滑动。纯滚动是平动和转动完美耦合的运动形式，是第六章能量方法的「综合考场」。
>
> 纯滚动的运动学条件：
> $$
> \boxed{v_{cm} = R\omega,\quad a_{cm} = R\alpha}
> $$

纯滚动将第五章和第六章的所有概念串联在一起：转动运动学（$v = R\omega$）、转动动能（$\frac{1}{2}I\omega^2$）、力矩（摩擦力提供力矩）、角动量——都在纯滚动中得到了统一应用。

### 二、纯滚动的能量

纯滚动刚体的总动能：

$$
\boxed{K = \frac{1}{2}Mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2 = \frac{1}{2}Mv_{cm}^2\left(1 + \frac{I_{cm}}{MR^2}\right)}
$$

令 $\beta = \dfrac{I_{cm}}{MR^2}$（形状因子）：

$$
K = \frac{1}{2}Mv_{cm}^2(1 + \beta)
$$

| 形状 | $\beta$ | $K_{\text{total}}$ |
|:--|:--:|:--|
| 实心球 | $\frac{2}{5}$ | $\frac{7}{10}Mv^2$ |
| 实心圆柱 | $\frac{1}{2}$ | $\frac{3}{4}Mv^2$ |
| 薄球壳 | $\frac{2}{3}$ | $\frac{5}{6}Mv^2$ |
| 薄圆环 | $1$ | $Mv^2$ |

### 三、摩擦力在纯滚动中的角色

> ⚠️ **关键误区**：纯滚动中**静摩擦力不做功**！因为接触点瞬时速度为零（$v_{\text{contact}} = v_{cm} - R\omega = 0$），$P = f \cdot v_{\text{contact}} = 0$。

- 静摩擦力提供力矩使物体旋转，但不消耗能量
- 若出现滑动（$v_{cm} \neq R\omega$），则动摩擦力做负功，消耗机械能
- 在斜面上纯滚动时，静摩擦力沿斜面**向上**（阻止滑动），大小由动力学方程确定

### 四、滚动的三种视角

| 视角 | 描述 | 适用场景 |
|:--|:--|:--|
| **质心平动 + 绕质心转动** | $K = \frac{1}{2}Mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2$ | 能量分析 |
| **绕接触点的纯转动**（瞬时） | $K = \frac{1}{2}I_{\text{contact}}\omega^2$ | 瞬时分析（$I_{\text{contact}} = I_{cm} + MR^2$） |
| **动力学** | $F = Ma_{cm}$ + $\tau = I\alpha$ + $a_{cm} = R\alpha$ | 求力和加速度 |

> 📝 **Step-by-Step：纯滚动问题的标准解题框架**
>
> 纯滚动问题是第六章最常见的综合题型。以下是经过验证的五步解题法：
>
> **第 1 步：确认纯滚动条件**
> - 检查 $v_{cm} = R\omega$ 是否成立（运动学锁）
> - 检查 $\mu_s$ 是否足够大以维持纯滚动：$\mu_s \geq \frac{\beta}{1+\beta}\tan\theta$（斜面）
>
> **第 2 步：选择方法**
> - **能量法**（推荐首选）：$E_i = E_f$，静摩擦力不做功，机械能守恒
> - **动力学法**：$F = Ma_{cm}$ + $\tau = I\alpha$ + $a_{cm} = R\alpha$ 联立
> - **绕接触点法**（瞬时纯转动）：$K = \frac{1}{2}I_{\text{contact}}\omega^2$
>
> **第 3 步：写出能量方程（能量法）或动力学方程（动力学法）**
> - 能量法：$Mgh = \frac{1}{2}Mv_{cm}^2(1 + \beta)$
> - 动力学法：$Mg\sin\theta - f = Ma$，$fR = I\alpha$
>
> **第 4 步：代入形状因子 $\beta = I/MR^2$**
> - 实心球 $\beta = 2/5$，实心圆柱 $\beta = 1/2$，薄球壳 $\beta = 2/3$，薄圆环 $\beta = 1$
>
> **第 5 步：解出未知量并验证**
> - 检查 $v_{cm}$ 是否小于纯滑动速度 $\sqrt{2gh}$
> - 检查静摩擦力是否在允许范围内

### 五、纯滚动的深度理解

#### 5.1 为什么纯滚动是「完美的运动」？

纯滚动之所以重要，是因为它是静摩擦力「零功但关键」的最美体现。静摩擦力不做功（接触点瞬时静止），但它是**转动和平动之间的能量转换器**：

- 在下坡滚动中：静摩擦力将一部分重力势能「引导」为转动动能，而非全部变为平动动能
- 在水平滚动中：如果物体已经有转动，静摩擦力可以将转动动能转化为平动动能
- 保龄球的滑动→滚动过渡：动摩擦力消耗能量直到纯滚动条件满足，之后静摩擦力维持纯滚动而不消耗能量

#### 5.2 纯滚动 vs 纯滑动

| 特征 | 纯滑动 | 纯滚动 |
|:--|:--|:--|
| 接触点速度 | $v_{\text{contact}} \neq 0$ | $v_{\text{contact}} = 0$ |
| 摩擦力类型 | 动摩擦 | 静摩擦 |
| 摩擦力做功？ | 是（消耗机械能） | 否（能量守恒） |
| 运动学约束 | 无 | $v_{cm} = R\omega$ |
| 效率 | 低（能量被摩擦消耗） | 高（能量不损失） |

#### 5.3 滚动阻力的来源

在实际滚动中（如汽车轮胎），仍然存在「滚动阻力」——但它不是来自静摩擦力。滚动阻力主要来自：

1. **材料滞后损耗**：轮胎和地面变形后不能完全恢复，消耗能量
2. **表面粗糙度**：微观不平导致持续的小碰撞
3. **塑性变形**：软地面（如沙地）被永久压出痕迹

滚动阻力通常远小于滑动摩擦力——这就是为什么轮子的发明是人类最伟大的技术突破之一。

#### 5.4 形状因子 $\beta$ 的物理意义

$\beta = I/(MR^2)$ 是决定滚动行为的关键参数。它表示转动动能占平动动能的比率（当 $v = R\omega$ 时）：

$$
\frac{K_{\text{rot}}}{K_{\text{trans}}} = \frac{\frac{1}{2}I\omega^2}{\frac{1}{2}Mv^2} = \frac{I}{MR^2} = \beta
$$

- $\beta = 0$（质点）：无转动，全部能量用于平动——加速度最大
- $\beta = 2/5$（实心球）：$28.6\%$ 能量用于转动——滚得较快
- $\beta = 1$（薄圆环）：$50\%$ 能量用于转动——滚得最慢

> 🏆 **「滚下斜面比赛」的排名**：质点 > 实心球 > 实心圆柱 > 薄球壳 > 薄圆环。转动惯量越小的物体滚得越快——因为它们将更少的能量「浪费」在转动上。

#### 5.5 滚动在自然界和工程中的应用

- **汽车轮胎**：轮胎的设计需要在滚动阻力（能耗）、抓地力（安全）和耐磨性之间取得平衡
- **球类运动**：保龄球、高尔夫球、台球的旋转（spin）改变了球的运动轨迹——这是马格努斯效应
- **轴承**：滚珠轴承用滚动取代滑动，大幅减少摩擦（从 $\mu_k \approx 0.3$–$0.5$ 降至滚动阻力系数 $\approx 0.001$–$0.005$）
- **生物运动**：人类行走本质上是「倒立摆」的滚动运动——脚跟着地时接触点瞬时静止

---

#### 6.5.1 🧪 推导 1：纯滚动总动能的两种等价表达

**推导目标**：证明 $K = \frac{1}{2}Mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2$ 和 $K = \frac{1}{2}I_{\text{contact}}\omega^2$ 等价。

**推导过程**：

**方法一**（质心平动 + 绕质心转动）：

$$
K = K_{\text{trans}} + K_{\text{rot}} = \frac{1}{2}Mv_{cm}^2 + \frac{1}{2}I_{cm}\omega^2
$$

代入 $v_{cm} = R\omega$：

$$
K = \frac{1}{2}MR^2\omega^2 + \frac{1}{2}I_{cm}\omega^2 = \frac{1}{2}(MR^2 + I_{cm})\omega^2
$$

**方法二**（绕接触点的纯转动）：

由平行轴定理，绕地面接触点的转动惯量为 $I_{\text{contact}} = I_{cm} + MR^2$。在纯滚动的瞬时，接触点速度为零，因此物体绕接触点的运动是纯转动：

$$
K = \frac{1}{2}I_{\text{contact}}\omega^2 = \frac{1}{2}(I_{cm} + MR^2)\omega^2
$$

两种方法结果一致：
$$
\boxed{K = \frac{1}{2}(I_{cm} + MR^2)\omega^2 = \frac{1}{2}Mv_{cm}^2\left(1 + \frac{I_{cm}}{MR^2}\right)}
$$

> 💡 **视角切换的威力**：方法一适合逐项分析平动和转动分量；方法二适合快速计算总动能。在选择题中，方法二通常更快。

---

#### 6.5.2 🧪 推导 2：斜面纯滚动的加速度与摩擦力

**推导目标**：推导任意形状刚体沿斜面纯滚动的加速度 $a = \dfrac{g\sin\theta}{1 + \beta}$ 和静摩擦力 $f = \dfrac{\beta}{1 + \beta}Mg\sin\theta$。

**推导过程**：

设斜面倾角 $\theta$，刚体质量 $M$，半径 $R$，$I_{cm} = \beta MR^2$。

**平动方程**（沿斜面向下为正）：
$$
Mg\sin\theta - f = Ma \tag{1}
$$

**转动方程**（绕质心，$f$ 产生力矩使物体顺时针转）：
$$
fR = I_{cm}\alpha = \beta MR^2 \cdot \frac{a}{R} = \beta MRa
$$

$$
f = \beta Ma \tag{2}
$$

将 (2) 代入 (1)：
$$
Mg\sin\theta - \beta Ma = Ma
$$
$$
Mg\sin\theta = Ma(1 + \beta)
$$

$$
\boxed{a = \frac{g\sin\theta}{1 + \beta}}
$$

代入 (2) 得摩擦力：
$$
\boxed{f = \frac{\beta}{1 + \beta}Mg\sin\theta}
$$

**纯滚动的摩擦条件**：
$$
f \leq \mu_s N = \mu_s Mg\cos\theta
$$
$$
\frac{\beta}{1 + \beta}Mg\sin\theta \leq \mu_s Mg\cos\theta
$$
$$
\boxed{\mu_s \geq \frac{\beta}{1 + \beta}\tan\theta}
$$

> 💡 **极端情况验证**：(a) $\beta = 0$（质点）→ $a = g\sin\theta$，$f = 0$ → 纯滑动，无转动；(b) $\beta = 1$（薄圆环）→ $a = \frac{1}{2}g\sin\theta$，$f = \frac{1}{2}Mg\sin\theta$ → 加速度是纯滑动的一半。

---

#### 6.5.2b 🧪 推导 3：纯滚动中静摩擦力不做功的严格证明

**推导目标**：证明纯滚动中静摩擦力的瞬时功率为零——$P_f = 0$。

**推导过程**：

功率 = 力 · 力作用点的速度。静摩擦力 $f$ 作用在接触点。在纯滚动中，接触点相对于地面的瞬时速度为零：

$$
v_{\text{contact}} = v_{cm} - R\omega = 0
$$

因此：
$$
P_f = f \cdot v_{\text{contact}} = f \cdot 0 = 0
$$

**能量角度验证**：物体沿斜面滚下 $h$，重力势能减少 $Mgh$。静摩擦力不做功 → 总机械能守恒 → $Mgh = \frac{1}{2}Mv_{cm}^2(1 + \beta)$，与之前能量法结果一致。

**静摩擦力的双重作用**：

1. **平动角度**：$f$ 是阻力——它减小了质心加速度（$a < g\sin\theta$）
2. **转动角度**：$f$ 是驱动力——它产生力矩 $fR$ 使物体旋转

$$
\boxed{\text{静摩擦力将平动能量「重定向」为转动能量——不消耗能量，只是重新分配}}
$$

> 💡 这是纯滚动最精妙之处：静摩擦力扮演了能量「转换器」而非「消耗者」的角色。动摩擦力则会消耗能量（$P = f_k v_{\text{contact}} \neq 0$），因此纯滚动的能量效率远高于滑动。

---

#### 6.5.2c 🧪 推导 4：滚动刚体在水平面上受拉力时的动力学分析

**推导目标**：推导一个绕有轻绳的线轴在水平面上被水平力拉动时的加速度和摩擦条件。这是区分「绳子从上方拉」和「绳子从下方拉」两种情况的经典问题。

**推导过程**：

设线轴质量 $M$，外半径 $R$，转动惯量 $I = \beta MR^2$。水平力 $F$ 作用在半径为 $r$ 的内轴上（$r < R$），方向水平向右。摩擦力 $f$ 方向暂时未知（可能是静摩擦）。

**平动**：$F - f = Ma$（设 $a$ 向右为正）

**转动**（绕质心）：$Fr + fR = I\alpha$（摩擦力方向待定，假设 $f$ 向右则力矩同向）

由纯滚动 $a = R\alpha$，且 $\alpha$ 应为顺时针（对应向右滚动）。若绳从上方拉，$F$ 产生顺时针力矩；若从下方拉，$F$ 产生逆时针力矩。

这里先讨论绳从上方拉（$F$ 在轴的上方，产生顺时针力矩）。

转动方程（设顺时针为正方向）：$Fr - fR = I\alpha = \beta MR^2 \cdot \frac{a}{R} = \beta MRa$

联立：
$$
F - f = Ma,\quad Fr - fR = \beta MRa
$$

消去 $a$，解得：
$$
\boxed{f = F \cdot \frac{\beta R - r}{R(1 + \beta)}}
$$

**关键分析**：
- 若 $\beta R > r$：$f > 0$，摩擦力方向与假设一致（向右即向后，阻止滑动）
- 若 $\beta R = r$：$f = 0$，无需摩擦力也能纯滚动
- 若 $\beta R < r$：$f < 0$，摩擦力方向与假设相反（向前，驱动滚动）

> 💡 这个推导展示了摩擦力方向取决于系统参数的微妙关系——不是简单的「摩擦总与运动方向相反」。

---

#### 6.5.2d 🧪 推导 5：能量法与动力学法的等价性证明

**推导目标**：证明纯滚动问题中能量法（$Mgh = \frac{1}{2}Mv^2(1+\beta)$）与动力学法（$a = g\sin\theta/(1+\beta)$）给出相同结果。

**推导过程**：

**能量法**：从静止滚下高度 $h$，沿斜面距离 $d = h/\sin\theta$，末速度 $v$：

$$
Mgh = \frac{1}{2}Mv^2(1+\beta) \quad \Rightarrow \quad v^2 = \frac{2gh}{1+\beta}
$$

**动力学法**：匀加速 $a = g\sin\theta/(1+\beta)$，距离 $d$：

$$
v^2 = 2ad = 2 \cdot \frac{g\sin\theta}{1+\beta} \cdot \frac{h}{\sin\theta} = \frac{2gh}{1+\beta}
$$

两种方法得到完全相同的 $v^2$ 表达式 ✓。

**更深刻的验证**——从动力学推导能量守恒：

将 $a = g\sin\theta/(1+\beta)$ 代入运动学公式，两边同乘 $\frac{1}{2}M(1+\beta)$：

$$
\frac{1}{2}M(1+\beta)v^2 = \frac{1}{2}M(1+\beta) \cdot \frac{2gh}{1+\beta} = Mgh
$$

这正是能量守恒表达式。

> 💡 **方法论洞察**：能量法和动力学法在纯滚动问题中数学等价。能量法更简洁（一个方程解决），动力学法能给出更多信息（摩擦力大小、加速度过程）。AP 考试中优先使用能量法——步骤少、不易出错。

---

#### 6.5.7 🧪 例题 5：线轴在水平面上被拉动——摩擦力方向判断

**题目**：一个线轴（外半径 $R = 0.12\ \text{m}$，内轴半径 $r = 0.040\ \text{m}$，质量 $M = 0.80\ \text{kg}$，$I = \frac{1}{2}MR^2$）放在水平桌面上。用水平力 $F = 3.0\ \text{N}$ 拉绕在内轴上的轻绳。分别求绳从上方拉和从下方拉时：
(a) 线轴的加速度
(b) 摩擦力的大小和方向
(c) 判断是否为纯滚动

**题目分析**：

> **已知**：$R = 0.12\ \text{m}$，$r = 0.040\ \text{m}$，$M = 0.80\ \text{kg}$，$\beta = 0.5$，$F = 3.0\ \text{N}$
>
> **求**：$a$、$f$（大小和方向）
>
> **策略**：联立平动和转动方程，用推导 4 的结果分析。

**解答**：

由推导 4 的公式 $f = F \cdot \dfrac{\beta R - r}{R(1+\beta)}$：

$\beta R = 0.5 \times 0.12 = 0.060\ \text{m}$，$r = 0.040\ \text{m}$

因为 $\beta R > r$，$f > 0$（摩擦力方向与 $F$ 同向——即摩擦力向后，阻止滑动）。

**(a)** 由 $F - f = Ma$ 和 $f = \beta Ma$：
$$
a = \frac{F}{M(1+\beta)} = \frac{3.0}{0.80 \times 1.5} = \mathbf{2.5\ \text{m/s}^2}
$$

**(b)** $f = \beta Ma = 0.5 \times 0.80 \times 2.5 = \mathbf{1.0\ \text{N}}$，方向与 $F$ 相同（向后，即摩擦力阻止平动但驱动转动）。

**(c)** 需要静摩擦系数满足 $\mu_s \geq f/N = 1.0/(0.80 \times 9.8) \approx 0.128$ 才能维持纯滚动。

> 💡 **绳从下方拉的情况**：$F$ 产生逆时针力矩，摩擦力方向将相反（向前）。此时 $f = F \cdot \dfrac{-\beta R - r}{R(1+\beta)} < 0$，摩擦力向前驱动平动。

---

#### 6.5.8 🧪 例题 6：球滚上斜坡——最大高度与能量分配

**题目**：一个薄球壳（$M = 0.30\ \text{kg}$，$R = 0.040\ \text{m}$，$I = \frac{2}{3}MR^2$）以 $v_0 = 4.0\ \text{m/s}$ 的初速度在水平面上纯滚动，然后滚上倾角 $\theta = 25^\circ$ 的斜面（继续保持纯滚动）。求：
(a) 球沿斜面上升的最大垂直高度
(b) 球在斜面上滚动的最大距离
(c) 若斜面完全光滑（无摩擦），球能上升多高？

**题目分析**：

> **已知**：$M = 0.30\ \text{kg}$，$\beta = 2/3$，$v_0 = 4.0\ \text{m/s}$，$\theta = 25^\circ$
>
> **求**：$h_{\max}$，$d_{\max}$，光滑斜面时的 $h_{\max}$
>
> **策略**：能量守恒（静摩擦力不做功）。光滑斜面意味着无转动——球只滑不转。

**解答**：

**(a)** 能量守恒：$\frac{1}{2}Mv_0^2(1+\beta) = Mgh_{\max}$

$$
h_{\max} = \frac{v_0^2(1+\beta)}{2g} = \frac{16 \times (1 + 2/3)}{19.6} = \frac{16 \times 5/3}{19.6} = \frac{80/3}{19.6} \approx \mathbf{1.36\ \text{m}}
$$

**(b)** $d_{\max} = h_{\max}/\sin 25^\circ = 1.36 / 0.423 \approx \mathbf{3.22\ \text{m}}$

**(c)** 光滑斜面（无摩擦 → 无转动 → $\beta = 0$）：
$$
h_{\max}^{\text{no rot}} = \frac{v_0^2}{2g} = \frac{16}{19.6} \approx 0.816\ \text{m}
$$

> 💡 **带转动的球上升更高**！$h_{\max}^{\text{rolling}} / h_{\max}^{\text{sliding}} = 1 + \beta = 5/3 \approx 1.67$。薄球壳因为有 $2/3$ 的能量在转动中，初始总动能是纯平动的 $5/3$ 倍，因此能上升 $5/3$ 倍的高度——但这一切都转化为重力势能。

---

#### 6.5.3 🧪 例题 1：不同物体滚下斜面的比赛

**题目**：一个实心球（$I = \frac{2}{5}MR^2$）、一个实心圆柱（$I = \frac{1}{2}MR^2$）和一个薄圆环（$I = MR^2$）同时从同一斜面顶端从静止释放，沿斜面纯滚动。三者到达底部的时间之比是多少？

**题目分析**：

> **已知**：三个物体的 $\beta$ 分别为 $\frac{2}{5}$、$\frac{1}{2}$、$1$，从静止出发
>
> **求**：时间比
>
> **策略**：先用 $a = g\sin\theta/(1+\beta)$ 求各自加速度，再用 $t = \sqrt{2L/a}$（匀加速，$L$ 为斜面长度）求时间比。

**解答**：

加速度：
- 实心球：$a_1 = \dfrac{g\sin\theta}{1 + 0.4} = \dfrac{g\sin\theta}{1.4}$
- 实心圆柱：$a_2 = \dfrac{g\sin\theta}{1 + 0.5} = \dfrac{g\sin\theta}{1.5}$
- 薄圆环：$a_3 = \dfrac{g\sin\theta}{1 + 1} = \dfrac{g\sin\theta}{2}$

由 $L = \frac{1}{2}at^2$ → $t = \sqrt{2L/a}$：
$$
t \propto \frac{1}{\sqrt{a}}
$$

$$
t_1 : t_2 : t_3 = \frac{1}{\sqrt{a_1}} : \frac{1}{\sqrt{a_2}} : \frac{1}{\sqrt{a_3}} = \sqrt{1.4} : \sqrt{1.5} : \sqrt{2}
$$

$$
\approx 1.183 : 1.225 : 1.414 \approx \mathbf{1 : 1.035 : 1.195}
$$

> 💡 **结论**：实心球最快，薄圆环最慢。如果将实心球的时间归一化为 1，则圆柱慢约 3.5%，圆环慢约 19.5%。$\beta$ 越小（质量越集中），滚动越快——能量中分配给转动的比例越小，平动速度就越大。

---

#### 6.5.4 🧪 例题 2：滚动的能量法应用

**题目**：一个实心球（$M = 2.0\ \text{kg}$，$R = 0.10\ \text{m}$，$I = \frac{2}{5}MR^2$）以 $v_0 = 5.0\ \text{m/s}$ 的初速度沿水平面纯滚动，然后滚上一个倾角 $\theta = 30^\circ$ 的斜面（仍保持纯滚动）。求球沿斜面上升的最大高度。

**题目分析**：

> **已知**：$M = 2.0\ \text{kg}$，$v_0 = 5.0\ \text{m/s}$，$\theta = 30^\circ$，$\beta = 0.4$
>
> **求**：$h_{\max}$
>
> **策略**：能量守恒——初始总动能全部转化为重力势能（静摩擦力不做功）。

**解答**：

初始总动能：
$$
K_i = \frac{1}{2}Mv_0^2 + \frac{1}{2}I\omega_0^2 = \frac{1}{2}Mv_0^2 + \frac{1}{2} \cdot \frac{2}{5}MR^2 \cdot \left(\frac{v_0}{R}\right)^2
$$

$$
= \frac{1}{2}Mv_0^2 + \frac{1}{5}Mv_0^2 = \frac{7}{10}Mv_0^2
$$

能量守恒 $K_i = Mgh_{\max}$：
$$
\frac{7}{10}Mv_0^2 = Mgh_{\max}
$$

$$
h_{\max} = \frac{7v_0^2}{10g} = \frac{7 \times 25}{10 \times 9.8} = \frac{175}{98} \approx \mathbf{1.79\ \text{m}}
$$

沿斜面上升距离：$d = \dfrac{h_{\max}}{\sin 30^\circ} = \dfrac{1.79}{0.5} = \mathbf{3.57\ \text{m}}$

> 💡 **对比纯滑动**（无摩擦，无转动）：$h_{\max} = \dfrac{v_0^2}{2g} = \dfrac{25}{19.6} \approx 1.28\ \text{m}$。纯滚动上升得**更高**——因为初始总能量中多了转动动能（$\frac{7}{10}$ vs $\frac{1}{2}$），而所有这些能量都转化为重力势能。

---

#### 6.5.5 🧪 例题 3：保龄球的纯滚动过渡

**题目**：一个保龄球（$M = 7.0\ \text{kg}$，$R = 0.11\ \text{m}$，$I = \frac{2}{5}MR^2$）以 $v_0 = 8.0\ \text{m/s}$ 的初速度沿水平球道滑动（初始无旋转）。球道与球之间的动摩擦系数 $\mu_k = 0.12$。求球从滑动过渡到纯滚动所经过的距离。

**题目分析**：

> 初始：$v_0 = 8.0\ \text{m/s}$，$\omega_0 = 0$。摩擦力使平动减速、转动加速。当 $v = R\omega$ 时开始纯滚动。

**解答**：

动摩擦力 $f_k = \mu_k Mg = 0.12 \times 7.0 \times 9.8 = 8.23\ \text{N}$（方向与速度相反）

平动：$a = -\dfrac{f_k}{M} = -\dfrac{8.23}{7.0} = -1.176\ \text{m/s}^2$

$v(t) = v_0 + at = 8.0 - 1.176t$

转动：$\alpha = \dfrac{\tau}{I} = \dfrac{f_k R}{\frac{2}{5}MR^2} = \dfrac{5f_k}{2MR} = \dfrac{5 \times 8.23}{2 \times 7.0 \times 0.11} = 26.7\ \text{rad/s}^2$

$\omega(t) = \alpha t = 26.7t$

纯滚动条件 $v = R\omega$：
$$
8.0 - 1.176t = 0.11 \times 26.7t
$$
$$
8.0 - 1.176t = 2.937t
$$
$$
8.0 = 4.113t \quad \Rightarrow \quad t = 1.945\ \text{s}
$$

距离：
$$
d = v_0 t + \frac{1}{2}at^2 = 8.0 \times 1.945 + \frac{1}{2} \times (-1.176) \times (1.945)^2
$$
$$
= 15.56 - 2.22 \approx \mathbf{13.3\ \text{m}}
$$

> 💡 保龄球在约 13 m 后进入纯滚动状态。进入纯滚动后，静摩擦力取代动摩擦力，不再消耗能量，球以恒定速度继续前进——这就是为什么保龄球道足够长以便球进入纯滚动。

---

#### 6.5.6 🧪 例题 4：滚动的角动量分析

**题目**：一个实心球以速度 $v$ 在水平面上纯滚动。求球对以下参考点的角动量：
(a) 对质心
(b) 对地面接触点
(c) 验证 $L_{\text{contact}} = I_{\text{contact}}\omega$

**题目分析**：

> 角动量对质心：$L_{cm} = I_{cm}\omega$。对接触点：需要考虑质心运动贡献的角动量。

**解答**：

**(a)** 对质心：$L_{cm} = I_{cm}\omega = \frac{2}{5}MR^2\omega$（沿旋转轴方向）

**(b)** 对接触点：将球的总角动量视为质心角动量 + 质心运动对接触点的角动量。质心在接触点上方 $R$ 处，以 $v$ 向右运动：
$$
\vec{L}_{\text{contact}} = \vec{L}_{cm} + \vec{r}_{cm} \times M\vec{v}_{cm}
$$

$\vec{r}_{cm}$ 从接触点指向质心（向上），$M\vec{v}_{cm}$ 水平向右，叉积方向垂直纸面向外（与 $\vec{\omega}$ 同向）：
$$
L_{\text{contact}} = I_{cm}\omega + RMv = \frac{2}{5}MR^2\omega + MRv
$$

由 $v = R\omega$：
$$
L_{\text{contact}} = \frac{2}{5}MR^2\omega + MR^2\omega = \frac{7}{5}MR^2\omega
$$

**(c)** 绕接触点的转动惯量由平行轴定理：$I_{\text{contact}} = I_{cm} + MR^2 = \frac{2}{5}MR^2 + MR^2 = \frac{7}{5}MR^2$

$$
I_{\text{contact}}\omega = \frac{7}{5}MR^2\omega = L_{\text{contact}} \quad \checkmark
$$

> 💡 绕接触点的纯转动视角给出了与「质心平动+绕质心转动」视角完全一致的角动量——这验证了平行轴定理和角动量的可加性。

---

### 本节总结

纯滚动是平动与转动的完美结合：

1. **运动学锁**：$v_{cm} = R\omega$，$a_{cm} = R\alpha$
2. **能量**：$K = \frac{1}{2}Mv_{cm}^2(1 + \beta)$，静摩擦力不做功
3. **斜面加速度**：$a = \dfrac{g\sin\theta}{1 + \beta}$，$\beta$ 越小越快
4. **摩擦条件**：$\mu_s \geq \dfrac{\beta}{1 + \beta}\tan\theta$

### ⚠️ 常见误区辨析

> ❌ **误区 1**：「纯滚动中摩擦力做负功。」
>
> ✅ **正确**：纯滚动中静摩擦力不做功——接触点瞬时速度为零，$P = f \cdot v_{\text{contact}} = 0$。摩擦力提供力矩但不消耗能量。动摩擦力才做功消耗能量。

> ❌ **误区 2**：「滚动比滑动慢，所以滚动是低效的运动方式。」
>
> ✅ **正确**：滚动虽然加速度较小（能量分流到转动），但它几乎不损失机械能——滚下斜面后可以滚上另一个斜面到几乎相同高度。滑动虽然加速度大，但动摩擦力消耗能量，滑上另一个斜面的高度远低于起始高度。论「效率」，滚动远优于滑动。

> ❌ **误区 3**：「任何情况下只要 $v = R\omega$ 就是纯滚动。」
>
> ✅ **正确**：$v = R\omega$ 是纯滚动的必要条件，但不是充分条件。还需要静摩擦力足够大（$\mu_s \geq \frac{\beta}{1+\beta}\tan\theta$）来维持纯滚动。如果静摩擦力不够，物体会开始滑动。

# 6.6 卫星轨道运动（Satellite Orbital Motion）

## Part A：基础层（AP Physics 1 必备）

### 一、卫星轨道的物理本质

> 卫星绕地球做近似圆周运动时，地球引力提供向心力。卫星轨道运动是第六章的「天体应用」——它将引力、圆周运动、角动量和能量完美统一在一个系统中。
>
> 对于圆轨道：
> $$
> \boxed{\frac{GMm}{r^2} = \frac{mv^2}{r}}
> $$

卫星问题本质上是引力提供向心力的圆周运动问题。但卫星的独特之处在于——引力始终指向力心（地球中心），因此引力对地心的力矩为零，**卫星对地心的角动量守恒**。这一事实导致了开普勒第二定律（面积定律）——行星与太阳的连线在相等时间内扫过相等的面积。

### 二、圆轨道核心公式

由 $\dfrac{GMm}{r^2} = \dfrac{mv^2}{r}$ 导出：

| 物理量 | 公式 | $\propto$ 关系 |
|:--|:--|:--|
| 轨道速度 | $v = \sqrt{\dfrac{GM}{r}}$ | $v \propto r^{-1/2}$ |
| 轨道周期 | $T = \dfrac{2\pi r}{v} = 2\pi\sqrt{\dfrac{r^3}{GM}}$ | $T \propto r^{3/2}$（开普勒第三定律） |
| 角速度 | $\omega = \dfrac{v}{r} = \sqrt{\dfrac{GM}{r^3}}$ | $\omega \propto r^{-3/2}$ |

### 三、轨道能量（🟣 AP Physics C 内容）

卫星的机械能 = 动能 + 引力势能：

$$
\boxed{E = \frac{1}{2}mv^2 - \frac{GMm}{r}}
$$

对于圆轨道，利用 $v^2 = \dfrac{GM}{r}$：

$$
\boxed{E = -\frac{GMm}{2r}}
$$

> 💡 **负总能量**意味着卫星被引力束缚——需要外界提供正能量才能逃逸。$E < 0$ 对应椭圆或圆轨道（束缚轨道），$E \geq 0$ 对应抛物线或双曲线轨道（逃逸轨道）。

### 四、开普勒定律

| 定律 | 内容 | 物理本质 |
|:--|:--|:--|
| **第一定律** | 行星沿椭圆轨道运动，太阳在焦点 | 平方反比引力的结果 |
| **第二定律** | 面积速度恒定 | **角动量守恒** |
| **第三定律** | $T^2 \propto a^3$（$a$ 为半长轴） | $F \propto 1/r^2$ 的结果 |

### 五、卫星轨道运动的深度理解

#### 5.1 为什么卫星不需要「持续推力」？

这是初学者最常问的问题。答案是：**卫星已经具有足够的速度**。引力垂直指向地球中心，始终改变速度的方向而不改变速度的大小（圆轨道中）。引力提供了恰好需要的向心力，使卫星「不断向地球下落但永远落不到地面」——这就是轨道的本质。

> 🧠 **关键直觉**：卫星不是在「飞」，而是在「不停地掉向地球但总是错过」。牛顿的炮弹思想实验：从高山上以足够大的速度水平发射一颗炮弹，地球的曲率使地面「弯离」炮弹的下落轨迹——炮弹就进入了轨道。

#### 5.2 不同轨道的能量特征

| 轨道类型 | 偏心率 $e$ | 总能量 $E$ | 是否束缚 |
|:--|:--:|:--|:--:|
| 圆 | $e = 0$ | $E = -\dfrac{GMm}{2a} < 0$ | 束缚 |
| 椭圆 | $0 < e < 1$ | $E = -\dfrac{GMm}{2a} < 0$ | 束缚 |
| 抛物线 | $e = 1$ | $E = 0$ | 刚好逃逸 |
| 双曲线 | $e > 1$ | $E > 0$ | 非束缚（飞越） |

> 💡 轨道能量 $E$ 只依赖于半长轴 $a$——与偏心率无关。两个轨道只要半长轴相同，总能量就相同。这就是为什么开普勒第三定律 $T^2 \propto a^3$ 对椭圆轨道也适用。

#### 5.3 轨道速度的反直觉结论

**轨道越高，速度越慢。** 这与许多人的直觉相反——我们会觉得「飞得更高需要更快」。实际上：

- 近地轨道（LEO，~400 km）：$v \approx 7.7\ \text{km/s}$，周期约 90 分钟
- 中地球轨道（GPS，~20200 km）：$v \approx 3.9\ \text{km/s}$，周期约 12 小时
- 地球同步轨道（GEO，~35800 km）：$v \approx 3.1\ \text{km/s}$，周期 24 小时
- 月球轨道（~384000 km）：$v \approx 1.0\ \text{km/s}$，周期约 27 天

> 🧠 **理解方式**：越高轨道引力越弱 → 需要更小的向心力 → 速度可以更慢。或者从能量角度：从低轨道转移到高轨道需要**加速两次**——但末速度比初速度**更小**！这是因为动能的一部分转化为了势能。

#### 5.4 轨道转移与火箭方程

将卫星从低轨道送到高轨道需要的能量来自火箭发动机。霍曼转移轨道是最省燃料的两脉冲方案（共面圆轨道之间）：

1. 第一次加速：从圆轨道进入椭圆转移轨道
2. 沿椭圆轨道滑行半个周期到达远地点
3. 第二次加速：从椭圆轨道进入目标圆轨道

有趣的是，两次加速后的末速度比初速度**更小**——虽然发动机做了正功，但动能的一部分转化为了引力势能。这体现了引力场中能量守恒的非直观特性。

#### 5.5 卫星轨道的实际应用

- **GPS 卫星**：24 颗卫星分布在中地球轨道（~20200 km），每颗卫星携带高精度原子钟。定位需要至少 4 颗卫星的信号。
- **地球同步卫星（GEO）**：轨道周期 = 地球自转周期，从地面看卫星「固定」在空中——通信、气象、电视广播。
- **极轨卫星**：轨道经过两极，地球在卫星下方自转——可以扫描全球（气象、遥感、侦察）。
- **国际空间站（ISS）**：近地轨道约 400 km，速度约 7.66 km/s，约 90 分钟绕地球一圈。
- **星链（Starlink）**：数千颗小卫星在约 550 km 的低轨道，提供全球互联网覆盖。

#### 5.6 角动量守恒与开普勒定律

开普勒第二定律（面积定律）是角动量守恒的直接推论。引力始终指向太阳（中心力），对太阳的力矩恒为零，因此行星对太阳的角动量守恒。面积速度 $\dfrac{dA}{dt} = \dfrac{L}{2m} = \text{常数}$ 正是角动量守恒的几何表述。

这意味着：
- 行星在近日点运动得快（$r$ 小，$v$ 大）
- 行星在远日点运动得慢（$r$ 大，$v$ 小）
- 两者的乘积 $rv$ 通过角动量 $L = mrv$ 联系在一起

---

#### 6.6.1 🧪 推导 1：从引力=向心力导出圆轨道速度

**推导目标**：证明圆轨道卫星的速度为 $v = \sqrt{GM/r}$，并由此推导开普勒第三定律。

**推导过程**：

卫星在圆轨道上，引力全部用于提供向心力：

$$
\frac{GMm}{r^2} = \frac{mv^2}{r}
$$

两边约去 $m$，乘以 $r$：

$$
\frac{GM}{r} = v^2
$$

$$
\boxed{v = \sqrt{\frac{GM}{r}}}
$$

**导出开普勒第三定律**：

周期 $T = \dfrac{2\pi r}{v} = 2\pi r \cdot \sqrt{\dfrac{r}{GM}} = 2\pi\sqrt{\dfrac{r^3}{GM}}$

平方：
$$
T^2 = \frac{4\pi^2}{GM}r^3
$$

$$
\boxed{T^2 \propto r^3}
$$

> 💡 **$v \propto 1/\sqrt{r}$ 的反直觉结论**：轨道越高，速度越慢！近地卫星（如国际空间站，$r \approx R_E + 400\ \text{km}$）的速度约 $7.7\ \text{km/s}$，而地球同步卫星（$r \approx 42000\ \text{km}$）的速度仅约 $3.1\ \text{km/s}$。

---

#### 6.6.2 🧪 推导 2：圆轨道机械能 $E = -GMm/(2r)$ 的推导

**推导目标**：证明圆轨道卫星的总机械能为负，且等于引力势能的一半。

**推导过程**（🟣 AP Physics C）：

卫星机械能 = 动能 + 引力势能（取无穷远为零势能）：

$$
E = K + U = \frac{1}{2}mv^2 - \frac{GMm}{r}
$$

对于圆轨道，代入 $v^2 = \dfrac{GM}{r}$：

$$
E = \frac{1}{2}m \cdot \frac{GM}{r} - \frac{GMm}{r} = -\frac{GMm}{2r}
$$

因此：
$$
\boxed{E = -\frac{GMm}{2r}}
$$

并且：
$$
\boxed{K = -E,\quad U = 2E}
$$

即圆轨道中：动能 = $-E$（正数），势能 = $2E$（负数，绝对值是动能的两倍）。

> 💡 **维里定理（Virial Theorem）**：对于平方反比力（引力、静电力）束缚的系统，平均动能与平均势能满足 $\langle K \rangle = -\frac{1}{2}\langle U \rangle$。圆轨道是其特例。

**轨道转移的能量变化**：从 $r_1$ 到 $r_2$（$r_2 > r_1$）：
$$
\Delta E = E_2 - E_1 = -\frac{GMm}{2}\left(\frac{1}{r_2} - \frac{1}{r_1}\right) = \frac{GMm}{2}\left(\frac{1}{r_1} - \frac{1}{r_2}\right) > 0
$$

需要提供正能量才能将卫星送入更高轨道。

---

#### 6.6.2b 🧪 推导 3：逃逸速度的推导

**推导目标**：从能量守恒出发推导地球表面的逃逸速度 $v_e = \sqrt{2GM/R_E}$。

**推导过程**：

逃逸的物理含义：物体具有足够的动能克服地球引力束缚，到达无穷远（$r \to \infty$）时速度恰好为零。

能量守恒（初始在地球表面，末态在无穷远）：

$$
E_i = \frac{1}{2}mv_e^2 - \frac{GMm}{R_E},\quad E_f = 0 \quad (\text{无穷远}, K = 0, U = 0)
$$

$$
\frac{1}{2}mv_e^2 - \frac{GMm}{R_E} = 0
$$

$$
\boxed{v_e = \sqrt{\frac{2GM}{R_E}}}
$$

**与圆轨道速度的关系**：地球表面圆轨道速度 $v_{\text{orbit}} = \sqrt{GM/R_E}$（第一宇宙速度），因此：

$$
\boxed{v_e = \sqrt{2}\,v_{\text{orbit}}}
$$

**数值计算**：
$$
v_{\text{orbit}} = \sqrt{\frac{6.67 \times 10^{-11} \times 5.97 \times 10^{24}}{6.37 \times 10^6}} \approx 7.91 \times 10^3\ \text{m/s}
$$

$$
v_e = \sqrt{2} \times 7.91 \times 10^3 \approx \mathbf{1.12 \times 10^4\ \text{m/s} = 11.2\ \text{km/s}}
$$

> 💡 逃逸速度不依赖于物体的质量——无论是一颗卫星还是一粒尘埃，从地球表面逃逸都需要 $11.2\ \text{km/s}$。气体分子的热运动速度若超过逃逸速度，就会逃逸到太空中——这解释了为什么月球没有大气层（月球逃逸速度仅 $2.4\ \text{km/s}$）。

---

#### 6.6.2c 🧪 推导 4：椭圆轨道的总能量（🟣 C 版深化）

**推导目标**：证明椭圆轨道（半长轴 $a$）的总能量与圆轨道形式相同：$E = -\dfrac{GMm}{2a}$。

**推导过程**：

椭圆轨道的总能量在轨道上各点守恒。在近地点（$r_p$）和远地点（$r_a$），速度垂直于矢径：

能量守恒：
$$
\frac{1}{2}mv_p^2 - \frac{GMm}{r_p} = \frac{1}{2}mv_a^2 - \frac{GMm}{r_a} = E
$$

角动量守恒（近地点和远地点）：
$$
mr_p v_p = mr_a v_a \quad \Rightarrow \quad v_a = \frac{r_p}{r_a}v_p
$$

利用椭圆几何关系 $r_p + r_a = 2a$（$a$ 为半长轴）和上述两个守恒定律，可以导出：

$$
\boxed{E = -\frac{GMm}{2a}}
$$

> 💡 **深刻结论**：椭圆轨道的总能量只依赖于半长轴 $a$——与偏心率无关！一个圆轨道和一个扁椭圆轨道只要 $a$ 相同，总能量就相同。轨道周期也仅依赖于 $a$（开普勒第三定律 $T^2 \propto a^3$）。

---

#### 6.6.3 🧪 例题 1：地球同步卫星

**题目**：求地球同步卫星（周期 $T = 24\ \text{h}$）的轨道半径和轨道速度。已知地球质量 $M_E = 5.97 \times 10^{24}\ \text{kg}$，$G = 6.67 \times 10^{-11}\ \text{N·m}^2/\text{kg}^2$。

**题目分析**：

> **已知**：$T = 24\ \text{h} = 86400\ \text{s}$，$M_E = 5.97 \times 10^{24}\ \text{kg}$
>
> **求**：$r$、$v$
>
> **策略**：由 $T^2 = \frac{4\pi^2}{GM}r^3$ 解出 $r$，再用 $v = \sqrt{GM/r}$。

**解答**：

由开普勒第三定律：

$$
r^3 = \frac{GMT^2}{4\pi^2} = \frac{6.67 \times 10^{-11} \times 5.97 \times 10^{24} \times (86400)^2}{4\pi^2}
$$

$$
= \frac{6.67 \times 5.97 \times 7.465 \times 10^{-11+24+9}}{39.48}
$$

$$
\approx 7.54 \times 10^{22}
$$

$$
r = \sqrt[3]{7.54 \times 10^{22}} \approx \mathbf{4.22 \times 10^7\ \text{m}}
$$

距地面高度：$h = r - R_E = 4.22 \times 10^7 - 6.37 \times 10^6 \approx \mathbf{3.58 \times 10^7\ \text{m} \approx 35800\ \text{km}}$

轨道速度：
$$
v = \sqrt{\frac{GM}{r}} = \sqrt{\frac{6.67 \times 10^{-11} \times 5.97 \times 10^{24}}{4.22 \times 10^7}} \approx \mathbf{3.07 \times 10^3\ \text{m/s} = 3.07\ \text{km/s}}
$$

> 💡 地球同步卫星在赤道上方约 35800 km 处，以 3.07 km/s 绕行。其轨道周期与地球自转周期相同，因此从地面看卫星似乎「固定」在天空中——这就是通信卫星和气象卫星的理想轨道。

---

#### 6.6.4 🧪 例题 2：从低轨道转移到高轨道（C 难度）

**题目**：一个 $m = 1000\ \text{kg}$ 的卫星从半径为 $r_1 = 7.0 \times 10^6\ \text{m}$ 的圆轨道转移到半径为 $r_2 = 1.4 \times 10^7\ \text{m}$ 的圆轨道。求转移所需的最小能量。已知 $M_E = 5.97 \times 10^{24}\ \text{kg}$，$G = 6.67 \times 10^{-11}$。

**题目分析**：

> **已知**：$m = 1000\ \text{kg}$，$r_1$、$r_2$
>
> **求**：$\Delta E$
>
> **策略**：用圆轨道能量公式 $E = -GMm/(2r)$，计算两轨道的能量差。

**解答**：

初始轨道能量：
$$
E_1 = -\frac{GMm}{2r_1} = -\frac{6.67 \times 10^{-11} \times 5.97 \times 10^{24} \times 1000}{2 \times 7.0 \times 10^6}
$$

$$
= -\frac{3.98 \times 10^{17}}{1.4 \times 10^7} \approx -2.84 \times 10^{10}\ \text{J}
$$

末轨道能量：
$$
E_2 = -\frac{GMm}{2r_2} = -\frac{3.98 \times 10^{17}}{2 \times 1.4 \times 10^7} \approx -1.42 \times 10^{10}\ \text{J}
$$

所需能量：
$$
\Delta E = E_2 - E_1 = (-1.42 \times 10^{10}) - (-2.84 \times 10^{10}) = \mathbf{1.42 \times 10^{10}\ \text{J}}
$$

> 💡 这相当于约 3370 kg TNT 当量的能量——将卫星送入更高轨道需要巨大的能量，这就是为什么火箭需要如此多的燃料。

---

#### 6.6.5 🧪 例题 3：不同轨道高度的速度与周期比较

**题目**：两颗卫星分别在地球表面附近（$r_1 = R_E = 6.37 \times 10^6\ \text{m}$）和 GPS 卫星轨道（$r_2 = 2.66 \times 10^7\ \text{m}$，约 $4.18R_E$）上做圆轨道运动。求：
(a) 两颗卫星的速度之比
(b) 两颗卫星的周期之比
(c) 哪颗卫星的总能量更大（负得更少）

**题目分析**：

> 用 $v \propto r^{-1/2}$ 和 $T \propto r^{3/2}$。

**解答**：

**(a)** $\dfrac{v_1}{v_2} = \sqrt{\dfrac{r_2}{r_1}} = \sqrt{\dfrac{2.66 \times 10^7}{6.37 \times 10^6}} = \sqrt{4.18} \approx \mathbf{2.04}$

近地卫星速度是 GPS 卫星的约 2 倍。

**(b)** $\dfrac{T_2}{T_1} = \left(\dfrac{r_2}{r_1}\right)^{3/2} = (4.18)^{3/2} \approx \mathbf{8.55}$

GPS 卫星周期约是近地卫星的 8.55 倍。近地卫星周期约 84 分钟，GPS 卫星周期约 $84 \times 8.55 \approx 718\ \text{min} \approx 12\ \text{h}$（实际 GPS 卫星周期确实约 12 小时）。

**(c)** $E = -\dfrac{GMm}{2r}$，$r_2 > r_1$ → $|E_2| < |E_1|$ → $E_2 > E_1$（负得更少）。

GPS 卫星的总能量更高（更接近零），因此需要更多能量才能到达该轨道。

---

#### 6.6.6 🧪 例题 4：霍曼转移轨道（C 难度）

**题目**：一颗卫星从半径为 $r_1$ 的圆轨道通过霍曼转移（半椭圆轨道）转移到半径为 $r_2$ 的共面圆轨道（$r_2 > r_1$）。霍曼转移轨道是一个以 $r_1$ 为近地点、$r_2$ 为远地点的椭圆。求转移轨道所需的总速度增量 $\Delta v_{\text{total}}$。

**题目分析**：

> 霍曼转移轨道的半长轴 $a = (r_1 + r_2)/2$。用能量和角动量求椭圆轨道在两端的的速度。

**解答**：

转移轨道的总能量 $E = -\dfrac{GMm}{2a} = -\dfrac{GMm}{r_1 + r_2}$

在近地点 $r_1$ 处的速度（由能量守恒）：
$$
\frac{1}{2}mv_1^2 - \frac{GMm}{r_1} = -\frac{GMm}{r_1 + r_2}
$$
$$
v_1 = \sqrt{2GM\left(\frac{1}{r_1} - \frac{1}{r_1 + r_2}\right)} = \sqrt{\frac{2GM}{r_1} \cdot \frac{r_2}{r_1 + r_2}}
$$

初始圆轨道速度 $v_{c1} = \sqrt{GM/r_1}$，第一次加速增量：
$$
\Delta v_1 = v_1 - v_{c1}
$$

在远地点 $r_2$ 处的速度（同理）：
$$
v_2 = \sqrt{\frac{2GM}{r_2} \cdot \frac{r_1}{r_1 + r_2}}
$$

目标圆轨道速度 $v_{c2} = \sqrt{GM/r_2}$，第二次加速增量：
$$
\Delta v_2 = v_{c2} - v_2
$$

总速度增量：$\Delta v_{\text{total}} = \Delta v_1 + \Delta v_2$

> 💡 霍曼转移是燃料最优的两脉冲轨道转移方案（在共面圆轨道之间）。这是航天器轨道设计的基石——从阿波罗登月到火星探测器，都使用了霍曼转移或其变体。

---

#### 6.6.2d 🧪 推导 5：轨道能量与半长轴的关系——维里定理应用

**推导目标**：证明对于任何平方反比力场中的束缚轨道（椭圆），总机械能 $E = -GMm/(2a)$，仅依赖于半长轴 $a$，与偏心率无关。

**推导过程**：

对于椭圆轨道，能量在轨道上各点守恒。在近地点 $r_p$ 和远地点 $r_a$：

$$
E = \frac{1}{2}mv_p^2 - \frac{GMm}{r_p} = \frac{1}{2}mv_a^2 - \frac{GMm}{r_a}
$$

角动量守恒（近地点和远地点 $\vec{r} \perp \vec{v}$）：
$$
mr_p v_p = mr_a v_a \quad \Rightarrow \quad v_a = \frac{r_p}{r_a}v_p
$$

利用椭圆几何关系 $r_p + r_a = 2a$，联立能量守恒和角动量守恒方程，消去 $v_p$ 和 $v_a$：

由角动量守恒：$v_a = \frac{r_p}{r_a}v_p$

能量守恒：
$$
\frac{1}{2}mv_p^2 - \frac{GMm}{r_p} = \frac{1}{2}m\left(\frac{r_p}{r_a}v_p\right)^2 - \frac{GMm}{r_a}
$$

整理：
$$
\frac{1}{2}mv_p^2\left(1 - \frac{r_p^2}{r_a^2}\right) = GMm\left(\frac{1}{r_p} - \frac{1}{r_a}\right)
$$

$$
\frac{1}{2}mv_p^2 \cdot \frac{r_a^2 - r_p^2}{r_a^2} = GMm \cdot \frac{r_a - r_p}{r_p r_a}
$$

$$
\frac{1}{2}mv_p^2 \cdot \frac{(r_a - r_p)(r_a + r_p)}{r_a^2} = GMm \cdot \frac{r_a - r_p}{r_p r_a}
$$

约去 $r_a - r_p$，代入 $r_a + r_p = 2a$：
$$
\frac{1}{2}mv_p^2 \cdot \frac{2a}{r_a^2} = \frac{GMm}{r_p r_a}
$$

$$
v_p^2 = \frac{GM}{a} \cdot \frac{r_a}{r_p}
$$

类似可得 $v_a^2 = \dfrac{GM}{a} \cdot \dfrac{r_p}{r_a}$。

现在计算总能量（在近地点）：
$$
E = \frac{1}{2}mv_p^2 - \frac{GMm}{r_p} = \frac{1}{2}m \cdot \frac{GM}{a} \cdot \frac{r_a}{r_p} - \frac{GMm}{r_p}
$$

$$
= \frac{GMm}{r_p}\left(\frac{r_a}{2a} - 1\right) = \frac{GMm}{r_p}\left(\frac{r_a - 2a}{2a}\right)
$$

由 $r_a + r_p = 2a$ → $r_a - 2a = -r_p$：
$$
E = \frac{GMm}{r_p}\left(\frac{-r_p}{2a}\right) = -\frac{GMm}{2a}
$$

因此：
$$
\boxed{E = -\frac{GMm}{2a}}
$$

> 💡 **深远意义**：轨道能量**只由半长轴决定**。一个 $a = 10000\ \text{km}$ 的圆轨道和 $a = 10000\ \text{km}$ 的扁椭圆轨道（$e = 0.9$）具有完全相同的总能量和相同的周期（开普勒第三定律 $T^2 \propto a^3$）。偏心率只影响角动量的大小和轨道形状，不影响能量。

---

#### 6.6.7 🧪 例题 5：国际空间站（ISS）的轨道参数

**题目**：国际空间站在高度 $h = 408\ \text{km}$ 的近圆轨道上运行。已知 $R_E = 6371\ \text{km}$，$M_E = 5.97 \times 10^{24}\ \text{kg}$，$G = 6.67 \times 10^{-11}\ \text{N·m}^2/\text{kg}^2$。求：
(a) ISS 的轨道速度
(b) ISS 的轨道周期（分钟）
(c) 宇航员在 ISS 上「失重」——他们的真实重量是多少？（设宇航员 $m = 70\ \text{kg}$）

**题目分析**：

> **已知**：$h = 408\ \text{km}$，$r = R_E + h$
>
> **求**：$v$、$T$、宇航员视重
>
> **策略**：圆轨道基本公式 + 等效原理理解失重。

**解答**：

$r = 6371 + 408 = 6779\ \text{km} = 6.779 \times 10^6\ \text{m}$

**(a)** $v = \sqrt{\dfrac{GM_E}{r}} = \sqrt{\dfrac{6.67 \times 10^{-11} \times 5.97 \times 10^{24}}{6.779 \times 10^6}}$
$$
= \sqrt{\dfrac{3.98 \times 10^{14}}{6.779 \times 10^6}} = \sqrt{5.87 \times 10^7} \approx \mathbf{7.66 \times 10^3\ \text{m/s} = 7.66\ \text{km/s}}
$$

**(b)** $T = \dfrac{2\pi r}{v} = \dfrac{2\pi \times 6.779 \times 10^6}{7.66 \times 10^3} \approx 5560\ \text{s} \approx \mathbf{92.7\ \text{min}}$

（ISS 实际周期约 92.7 分钟，每天绕地球约 15.5 圈）

**(c)** 宇航员在 ISS 上的真实重量（地球引力）：
$$
F_g = \frac{GM_E m}{r^2} = \frac{6.67 \times 10^{-11} \times 5.97 \times 10^{24} \times 70}{(6.779 \times 10^6)^2} \approx \mathbf{606\ \text{N}}
$$

地面上重量：$mg = 70 \times 9.8 = 686\ \text{N}$。ISS 上的引力是地面的约 $88\%$——并不是零！

> 💡 **失重的真相**：宇航员并非「没有重力」，而是处于**自由落体**状态。引力提供了向心力使宇航员与 ISS 一起沿轨道「下落」。宇航员感觉不到重量是因为他们与 ISS 以相同的加速度运动——没有支持力（$N = 0$），这与爱因斯坦等效原理一致。

---

#### 6.6.8 🧪 例题 6：双星系统的轨道运动

**题目**：两颗质量分别为 $M_1 = 3.0 \times 10^{30}\ \text{kg}$ 和 $M_2 = 1.0 \times 10^{30}\ \text{kg}$ 的恒星，相距 $d = 2.0 \times 10^{11}\ \text{m}$，在引力作用下绕共同质心做圆轨道运动。求：
(a) 每颗恒星到质心的距离
(b) 系统的轨道角速度
(c) 系统的总角动量
(d) 系统的总机械能

**题目分析**：

> 双星系统：两颗星都绕质心旋转，角速度相同。引力提供各自的向心力。

**解答**：

**(a)** 质心位置：$r_1 = \dfrac{M_2}{M_1 + M_2}d = \dfrac{1.0}{4.0} \times 2.0 \times 10^{11} = \mathbf{5.0 \times 10^{10}\ \text{m}}$

$r_2 = d - r_1 = \mathbf{1.5 \times 10^{11}\ \text{m}}$

验证：$M_1 r_1 = M_2 r_2$ → $3.0 \times 0.50 = 1.0 \times 1.5$ ✓

**(b)** 对 $M_1$，引力提供向心力：
$$
\frac{GM_1 M_2}{d^2} = M_1 \omega^2 r_1
$$
$$
\omega = \sqrt{\frac{GM_2}{d^2 r_1}} = \sqrt{\frac{6.67 \times 10^{-11} \times 1.0 \times 10^{30}}{(2.0 \times 10^{11})^2 \times 5.0 \times 10^{10}}}
$$
$$
= \sqrt{\frac{6.67 \times 10^{19}}{4.0 \times 10^{22} \times 5.0 \times 10^{10}}} = \sqrt{3.335 \times 10^{-14}} \approx \mathbf{1.83 \times 10^{-7}\ \text{rad/s}}
$$

周期：$T = \dfrac{2\pi}{\omega} \approx 3.44 \times 10^7\ \text{s} \approx \mathbf{398\ \text{天}}$

**(c)** 总角动量（对质心）：
$$
L = M_1 r_1^2 \omega + M_2 r_2^2 \omega = \omega(M_1 r_1^2 + M_2 r_2^2)
$$
$$
= 1.83 \times 10^{-7} \times (3.0 \times 10^{30} \times 2.5 \times 10^{21} + 1.0 \times 10^{30} \times 2.25 \times 10^{22})
$$
$$
= 1.83 \times 10^{-7} \times (7.5 \times 10^{51} + 2.25 \times 10^{52}) \approx \mathbf{5.49 \times 10^{45}\ \text{kg·m}^2\text{/s}}
$$

**(d)** 总机械能：
$$
E = K_1 + K_2 + U = \frac{1}{2}M_1(r_1\omega)^2 + \frac{1}{2}M_2(r_2\omega)^2 - \frac{GM_1 M_2}{d}
$$

计算动能部分：
$$
K = \frac{1}{2}\omega^2(M_1 r_1^2 + M_2 r_2^2) = \frac{1}{2} \times (1.83 \times 10^{-7})^2 \times 3.0 \times 10^{52}
$$
$$
\approx 5.02 \times 10^{38}\ \text{J}
$$

引力势能：
$$
U = -\frac{6.67 \times 10^{-11} \times 3.0 \times 10^{30} \times 1.0 \times 10^{30}}{2.0 \times 10^{11}} \approx -1.00 \times 10^{39}\ \text{J}
$$

$$
E \approx \mathbf{-5.0 \times 10^{38}\ \text{J}}
$$

> 💡 **双星系统的天体物理意义**：通过观测双星的轨道周期和速度，天文学家可以精确测定恒星质量——这是天文学中为数不多的直接「称量」恒星的方法。双星轨道也是验证广义相对论引力波辐射的经典系统（如著名的 Hulse-Taylor 双脉冲星）。

---

### 本节总结

卫星轨道运动的核心公式：

1. **$v = \sqrt{GM/r}$** — 轨道越高，速度越慢
2. **$T^2 \propto r^3$** — 开普勒第三定律
3. **$E = -GMm/(2r)$**（C 版）— 圆轨道总能量为负
4. **角动量守恒** → 开普勒第二定律（面积定律）

### ⚠️ 常见误区辨析

> ❌ **误区 1**：「卫星轨道越高，需要的速度越大。」
>
> ✅ **正确**：轨道越高速度越慢（$v = \sqrt{GM/r}$）。从低轨道到高轨道需要两次加速，但末速度比初速度更小——多余的动能转化为了引力势能。这是引力场中能量守恒的反直觉结果。

> ❌ **误区 2**：「卫星没有重力——它们在太空中是失重的。」
>
> ✅ **正确**：卫星和宇航员并非「没有重力」，而是处于**自由落体**状态。引力提供了向心力使卫星沿轨道曲线运动，宇航员和卫星以相同的加速度下落——这就是「失重感」的来源（等效原理）。

> ❌ **误区 3**：「开普勒定律只对行星绕太阳成立。」
>
> ✅ **正确**：开普勒三定律对任何平方反比中心力场中的束缚轨道都成立（修正后）。卫星绕地球、电子绕原子核（量子力学近似下）都遵循类似规律。开普勒第三定律 $T^2 \propto a^3$ 对所有 $F \propto 1/r^2$ 系统成立。

---

# 🟣 AP Physics C 微积分扩展

## C.1 旋转功的积分形式

当力矩 $\tau$ 不恒定时：

$$
\boxed{W = \int_{\theta_1}^{\theta_2} \tau(\theta)\,d\theta}
$$

**示例**：若 $\tau = k\theta$（力矩与角度成正比，如扭转弹簧），转过 $\theta_0$ 的功为：

$$
W = \int_0^{\theta_0} k\theta\,d\theta = \frac{1}{2}k\theta_0^2
$$

这类似于弹簧 $W = \frac{1}{2}kx^2$。

## C.2 角动量的矢量叉积形式

对于三维运动：
$$
\vec{L} = \vec{r} \times \vec{p} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ x & y & z \\ p_x & p_y & p_z \end{vmatrix}
$$

$\vec{L}$ 垂直于 $\vec{r}$ 和 $\vec{p}$ 确定的平面。

## C.3 轨道能量的详细分析

### 逃逸速度

卫星从地球表面逃逸所需的最小速度：$E = K + U = 0$

$$
\frac{1}{2}mv_e^2 - \frac{GMm}{R_E} = 0 \quad \Rightarrow \quad \boxed{v_e = \sqrt{\frac{2GM}{R_E}}}
$$

地球表面逃逸速度约 $11.2\ \text{km/s}$。注意 $v_e = \sqrt{2}v_{\text{orbit}}$（逃逸速度 = $\sqrt{2}$ × 圆轨道速度）。

### 不同轨道的能量

| 轨道类型 | 偏心率 $e$ | 总能量 $E$ |
|:--|:--|:--|
| 圆 | $e = 0$ | $E = -\dfrac{GMm}{2a}$ |
| 椭圆 | $0 < e < 1$ | $E = -\dfrac{GMm}{2a} < 0$ |
| 抛物线 | $e = 1$ | $E = 0$ |
| 双曲线 | $e > 1$ | $E > 0$ |

其中 $a$ 是半长轴（圆轨道 $a = r$）。

### C.4 非恒定力矩的角动量变化

当刚体的 $I$ 随时间变化时（如收臂），即使 $\tau_{\text{ext}} = 0$，角加速度也非零：

$$
\frac{dL}{dt} = 0 \Rightarrow I\frac{d\omega}{dt} + \omega\frac{dI}{dt} = 0 \Rightarrow \alpha = -\frac{\omega}{I}\frac{dI}{dt}
$$

若 $I$ 减小（$dI/dt < 0$），则 $\alpha > 0$——即使没有外力矩，角速度也在增大。

### C.5 转动惯量变化的功

当 $I$ 变化时，内部力做的功等于转动动能的变化：

$$
W_{\text{internal}} = \Delta K = \frac{L^2}{2}\left(\frac{1}{I_f} - \frac{1}{I_i}\right)
$$

这是滑冰运动员收臂时肌肉做功的定量表达。

---

# 🎯 Ch6 解题大师指南（Step-by-Step Master Guide）

> **学习目标**：掌握第六章所有题型的通用解题策略。以下流程涵盖了 AP Physics 1 和 C 级别考试中 95% 以上的转动问题。

---

## 📋 第一步：识别问题类型（5 秒判断法）

阅读题目后，快速判断属于以下哪种类型：

| 类型 | 关键词/信号 | 首选方法 | 典型公式 |
|:--|:--|:--|:--|
| **类型 A：纯转动能量** | 「绕固定轴旋转」「飞轮」「角速度从…变为…」 | 能量守恒或功-能定理 | $K = \frac{1}{2}I\omega^2$，$W = \tau\Delta\theta$ |
| **类型 B：角动量守恒** | 「收臂」「展体」「坍缩」「无外力矩」「碰撞」 | 角动量守恒 | $I_i\omega_i = I_f\omega_f$ |
| **类型 C：纯滚动** | 「无滑动滚动」「滚下斜面」「保龄球」 | 能量守恒 + $v = R\omega$ | $K = \frac{1}{2}Mv^2(1+\beta)$ |
| **类型 D：卫星/轨道** | 「圆轨道」「周期」「轨道半径」 | 引力=向心力 | $v = \sqrt{GM/r}$，$T^2 \propto r^3$ |
| **类型 E：转动碰撞** | 「击中」「嵌入」「粘在一起」「碰撞」 | 角动量守恒（碰时）+ 能量守恒（碰后） | $L_i = L_f$，$K = L^2/(2I)$ |
| **类型 F：综合滑轮系统** | 「滑轮有质量」「绳绕在滑轮上」「重物下落」 | 能量守恒或动力学联立 | $mgh = \frac{1}{2}mv^2 + \frac{1}{2}I\omega^2$ |

---

## 📋 第二步：选择解题路线（决策树）

```mermaid
graph TD
    A[开始读题] --> B{系统是否受外力矩?}
    B -->|否| C[角动量守恒路线]
    B -->|是| D{是否有非保守力做功?}
    D -->|否| E[机械能守恒路线]
    D -->|是| F[功-能定理路线]
    C --> G{是否为碰撞?}
    G -->|是| H[碰撞时 L 守恒 + 碰后 E 守恒]
    G -->|否| I[I_i ω_i = I_f ω_f]
    E --> J{是否纯滚动?}
    J -->|是| K[K = ½Mv²(1+β), v=Rω]
    J -->|否| L[½Iω² + Mgh = constant]
    F --> M[W_net = τΔθ = ΔK_rot]
```

---

## 📋 第三步：执行解题——六类题型的标准操作流程

### 类型 A：纯转动能量 — SOP

**Step 1**：确定转轴，写出或计算 $I$

**Step 2**：确认 $\omega$ 的单位（必须为 rad/s）

**Step 3**：写出能量方程
- 只有转动：$\frac{1}{2}I\omega_i^2 + W_{\text{ext}} = \frac{1}{2}I\omega_f^2$
- 有重力：$\frac{1}{2}I\omega^2 + Mg y_{\text{cm}} = \text{常数}$

**Step 4**：代入数据求解

> 🔑 **关键技巧**：当 $\omega$ 以 rpm 给出时，立即转换为 rad/s：$\omega = \text{rpm} \times \frac{2\pi}{60}$

---

### 类型 B：角动量守恒 — SOP

**Step 1**：定义系统，确认 $\Sigma\vec{\tau}_{\text{ext}} = 0$

**Step 2**：写出 $I_i\omega_i = I_f\omega_f$

**Step 3**：分析 $I$ 如何变化（谁在动？距离变了吗？）

**Step 4**：解出 $\omega_f$

**Step 5**（可选）：计算动能变化 $\Delta K = \frac{L^2}{2}(\frac{1}{I_f} - \frac{1}{I_i})$

> 🔑 **关键技巧**：用 $K = L^2/(2I)$ 直接判断动能增减——$I$ 减小则 $K$ 增大（肌肉做功）

---

### 类型 C：纯滚动 — SOP

**Step 1**：确认纯滚动条件 $v_{cm} = R\omega$（题目明确说「无滑动」或「纯滚动」）

**Step 2**：确定形状因子 $\beta = I/MR^2$

**Step 3**：选择能量法（推荐）或动力学法
- **能量法**（首选）：$Mgh = \frac{1}{2}Mv_{cm}^2(1+\beta)$
- **动力学法**：联立 $Mg\sin\theta - f = Ma$、$fR = I\alpha$、$a = R\alpha$

**Step 4**：解出 $v_{cm}$ 或 $a$

**Step 5**：如有需要，求静摩擦力 $f = \frac{\beta}{1+\beta}Mg\sin\theta$

> 🔑 **关键技巧**：滚下斜面的「比赛排名」——$\beta$ 越小滚得越快：实心球 > 实心圆柱 > 薄球壳 > 薄圆环

---

### 类型 D：卫星轨道 — SOP

**Step 1**：确认是圆轨道（$F_g = F_c$）

**Step 2**：用 $\frac{GMm}{r^2} = \frac{mv^2}{r}$ 导出 $v = \sqrt{GM/r}$

**Step 3**：如需周期，用 $T = \frac{2\pi r}{v} = 2\pi\sqrt{r^3/(GM)}$

**Step 4**：如需能量（C 版），用 $E = -\frac{GMm}{2r}$

> 🔑 **关键技巧**：$v \propto 1/\sqrt{r}$——轨道越高，速度越慢！（反直觉但正确）

---

### 类型 E：转动碰撞 — SOP

**Step 1**：碰撞期间角动量守恒（外力矩的角冲量可忽略）

**Step 2**：$L_i = L_f$，写出碰撞前后的角动量
- 质点：$L = rmv\sin\theta$
- 刚体：$L = I\omega$

**Step 3**：解出碰后角速度 $\omega_f$

**Step 4**：碰后能量守恒（如有摆起/下落）
- $\frac{1}{2}I_{\text{total}}\omega_f^2 = M_{\text{total}} g \Delta y_{\text{cm}}$

**Step 5**：计算动能损失（如需要）：$\Delta K = K_f - K_i$

> 🔑 **关键技巧**：完全非弹性转动碰撞的动能损失比例 = $I_{\text{target}}/(I_{\text{projectile}} + I_{\text{target}})$

---

### 类型 F：滑轮系统 — SOP

**Step 1**：识别约束关系（绳长不变 → $a_1$、$a_2$、$\alpha$ 之间有几何关系）

**Step 2**：选择方法
- **能量法**（如求末速度）：$\Delta U_g + \Delta K_{\text{trans}} + \Delta K_{\text{rot}} = 0$
- **动力学法**（如求加速度）：对每个物体写 $F=ma$，对滑轮写 $\tau = I\alpha$

**Step 3**：联立求解

> 🔑 **关键技巧**：滑轮转动惯量的「等效平动质量」= $I/R^2$——这告诉你滑轮「吃掉了」多少加速度

---

## 📋 第四步：验证答案（10 秒合理性检查）

| 检查项 | 合理范围 | 红旗信号 |
|:--|:--|:--|
| 角速度 | $0 < \omega < 10^4\ \text{rad/s}$（日常） | 负值、无穷大、$>10^6$（除中子星外） |
| 滚动速度 | $v < \sqrt{2gh}$（滚动慢于自由滑动） | $v > \sqrt{2gh}$（违反能量守恒） |
| 角动量 | $L$ 方向用右手定则验证 | 方向与旋转方向不一致 |
| 动能 | $K_f \leq K_i$（非弹性过程） | 非弹性碰撞后 $K$ 反而增大 |
| 卫星速度 | 近地 $\sim 7.9\ \text{km/s}$，同步 $\sim 3.1\ \text{km/s}$ | $v > 11.2\ \text{km/s}$（逃逸了！） |

---

## 📋 第五步：AP 考试特别提醒

1. **单位陷阱**：力矩用 N·m（不是 J！），角动量用 kg·m²/s
2. **方向标记**：角动量方向用 ⊗（入纸面）和 ⊙（出纸面），不要漏掉
3. **公式引用**：AP Physics 1 给出 $I$ 公式，AP Physics C 需要自己积分
4. **近似声明**：碰撞问题中必须声明「碰撞时间极短，外力矩的角冲量可忽略」
5. **文字解释**：FRQ 答题需要文字说明，不能只列公式

---

# Ch6 综合例题

## 综合题 1：弹道摆——角动量守恒 + 能量

**题目**：一个 $m = 0.050\ \text{kg}$ 的子弹以 $v_0 = 300\ \text{m/s}$ 水平射入并嵌入一个静止的均匀细杆下端。杆质量 $M = 2.0\ \text{kg}$，长度 $L = 1.0\ \text{m}$，可绕上端自由旋转。求杆摆起的最大角度。

**解答**：

**第一步**：碰撞瞬间角动量守恒（对杆上端）。子弹角动量 = 系统末角动量。

子弹对杆上端的角动量（碰撞前）：
$$
L_i = mv_0L = 0.050 \times 300 \times 1.0 = 15\ \text{kg·m}^2\text{/s}
$$

系统末转动惯量（杆绕端点 $I = \frac{1}{3}ML^2$ + 子弹 $mL^2$）：
$$
I_f = \frac{1}{3}ML^2 + mL^2 = \frac{1}{3} \times 2.0 \times 1.0^2 + 0.050 \times 1.0^2 = 0.667 + 0.050 = 0.717\ \text{kg·m}^2
$$

末角速度：
$$
\omega_f = \frac{L_i}{I_f} = \frac{15}{0.717} \approx 20.92\ \text{rad/s}
$$

**第二步**：碰后能量守恒（转动动能 → 重力势能）。

杆质心上升 $h_{\text{rod}} = \frac{L}{2}(1 - \cos\theta)$，子弹上升 $h_{\text{bullet}} = L(1 - \cos\theta)$。

$$
\frac{1}{2}I_f\omega_f^2 = Mg \cdot \frac{L}{2}(1 - \cos\theta) + mgL(1 - \cos\theta)
$$

$$
\frac{1}{2} \times 0.717 \times (20.92)^2 = (2.0 \times 9.8 \times 0.5 + 0.050 \times 9.8 \times 1.0)(1 - \cos\theta)
$$

$$
157.0 = (9.8 + 0.49)(1 - \cos\theta) = 10.29(1 - \cos\theta)
$$

$$
1 - \cos\theta = 15.25 \quad \rightarrow \quad \text{不可能！}
$$

> ⚠️ 弹道摆问题中，若子弹动能过大，杆会转过最高点继续旋转。此处 $\omega_f$ 过大，杆会完成整圈旋转——$1 - \cos\theta$ 不能超过 2，实际 $\theta_{\max}$ 将是 $360^\circ$（完整一圈）。

---

## 综合题 2：滚下斜面的能量分配

**题目**：一个实心球从高度 $h = 2.0\ \text{m}$ 的斜面顶端从静止纯滚动到底部。求：
(a) 底部平动速度
(b) 平动动能与转动动能之比
(c) 若球不是滚动而是无摩擦滑动，底部速度是多少？

**解答**：

**(a)** 能量守恒：$Mgh = \frac{7}{10}Mv^2$

$$
v = \sqrt{\frac{10}{7}gh} = \sqrt{\frac{10}{7} \times 9.8 \times 2.0} = \sqrt{28} \approx \mathbf{5.29\ \text{m/s}}
$$

**(b)** $\dfrac{K_{\text{trans}}}{K_{\text{rot}}} = \dfrac{\frac{1}{2}Mv^2}{\frac{1}{5}Mv^2} = \dfrac{5}{2} = \mathbf{2.5}$

**(c)** 纯滑动：$v_{\text{slide}} = \sqrt{2gh} = \sqrt{2 \times 9.8 \times 2.0} = \sqrt{39.2} \approx \mathbf{6.26\ \text{m/s}}$

滚动速度/滑动速度 = $5.29 / 6.26 \approx 0.845$

---

## 综合题 3：飞轮制动——角冲量与功的综合应用

**题目**：一个飞轮（$I = 3.0\ \text{kg·m}^2$）以 $\omega_0 = 40\ \text{rad/s}$ 旋转。制动器对飞轮施加恒定的 $\tau = -12\ \text{N·m}$ 力矩。求：
(a) 飞轮停止所需的时间
(b) 制动过程中力矩做的功
(c) 制动过程中的角冲量大小
(d) 验证功-能定理和角冲量-角动量定理的一致性

**解答**：

**(a)** $\alpha = \tau/I = -12/3.0 = -4.0\ \text{rad/s}^2$

$t = \dfrac{0 - 40}{-4.0} = \mathbf{10.0\ \text{s}}$

**(b)** 制动过程中的角位移：$\theta = \frac{1}{2}(\omega_0 + 0)t = \frac{1}{2} \times 40 \times 10 = 200\ \text{rad}$

$W = \tau\theta = (-12) \times 200 = \mathbf{-2400\ \text{J}}$

**(c)** 角冲量 = $|\tau t| = 12 \times 10 = \mathbf{120\ \text{N·m·s}}$

**(d)** 功-能定理：$W = \Delta K = 0 - \frac{1}{2} \times 3.0 \times 40^2 = -2400\ \text{J}$ ✓

角冲量-角动量定理：$\tau t = \Delta L = 0 - 3.0 \times 40 = -120\ \text{kg·m}^2\text{/s}$ ✓

---

## 综合题 4：两个滑轮的角动量守恒碰撞

**题目**：滑轮 A（$I_A = 2.0\ \text{kg·m}^2$）以 $\omega_A = 15\ \text{rad/s}$ 逆时针旋转，滑轮 B（$I_B = 3.0\ \text{kg·m}^2$）以 $\omega_B = 10\ \text{rad/s}$ 顺时针旋转。两滑轮突然啮合在一起（同轴）。求：
(a) 啮合后的角速度（大小和方向）
(b) 碰撞中的动能损失
(c) 损失的动能占初始总动能的百分比

**解答**：

**(a)** 取逆时针为正：$L_A = 2.0 \times 15 = 30$，$L_B = 3.0 \times (-10) = -30$

$L_{\text{total}} = 30 + (-30) = 0$ → $\omega_f = \mathbf{0}$！

**(b)** $K_i = \frac{1}{2} \times 2.0 \times 15^2 + \frac{1}{2} \times 3.0 \times 10^2 = 225 + 150 = 375\ \text{J}$

$K_f = 0$ → $\Delta K = \mathbf{-375\ \text{J}}$（全部损失！）

**(c)** 损失 100%。两滑轮的角动量大小相等方向相反，碰撞后完全停止。

---

## 综合题 5：翻滚过山车的能量分析

**题目**：一个实心球（$M = 0.050\ \text{kg}$，$R = 0.015\ \text{m}$，$I = \frac{2}{5}MR^2$）在半径为 $r_{\text{track}} = 0.30\ \text{m}$ 的环形轨道内纯滚动。球从高度 $h = 1.2\ \text{m}$ 处从静止释放。球能否通过最高点而不脱离轨道？

**解答**：

能量守恒（释放点→轨道最高点，最高点高度 $= 2r_{\text{track}} = 0.60\ \text{m}$）：
$$
Mgh = Mg(2r_{\text{track}}) + \frac{7}{10}Mv^2
$$
$$
v^2 = \frac{10}{7}g(h - 2r_{\text{track}}) = \frac{10}{7} \times 9.8 \times (1.2 - 0.60) = 8.40
$$
$$
v = \mathbf{2.90\ \text{m/s}}
$$

最高点处：$Mg + N = \dfrac{Mv^2}{r_{\text{track}}}$ → $N = M\left(\dfrac{v^2}{r_{\text{track}}} - g\right)$

$N = 0.050 \times (28.0 - 9.8) = \mathbf{0.91\ \text{N} > 0}$ → 球能通过 ✓

---

## 综合题 6：斜面上滚动的摩擦力方向判断

**题目**：一个线轴（外径 $R = 0.10\ \text{m}$，内轴 $r = 0.04\ \text{m}$，$I = \frac{1}{2}MR^2$）放在 $\theta = 30^\circ$ 的斜面上。绳绕在内轴上沿斜面向上拉。求摩擦力方向。

**解答**：

设沿斜面向上为正。$F - Mg\sin\theta - f = Ma$，$Fr - fR = I\alpha = \frac{1}{2}MRa$

联立得：$f = F \cdot \dfrac{\beta R - r}{R(1+\beta)}$

$r/R = 0.4$，$\beta = 0.5$，$\beta R = 0.5R > 0.4R = r$ → $f > 0$

摩擦力沿斜面向下（阻止滑动，提供转动力矩）。

---

## 综合题 7：卫星轨道转移的角动量分析

**题目**：一颗 $m = 500\ \text{kg}$ 的卫星在 $r = 7.0 \times 10^6\ \text{m}$ 圆轨道上。发动机沿切线方向点火，速度瞬间增加 $10\%$。求新轨道的近地点和远地点。

**解答**：

点火前：$v_0 = \sqrt{GM/r}$，$E_0 = -\dfrac{GMm}{2r}$，$L_0 = mrv_0$

点火后：$v_1 = 1.10v_0$，$E_1 = \frac{1}{2}m(1.10v_0)^2 - \dfrac{GMm}{r}$

新轨道半长轴：$a = -\dfrac{GMm}{2E_1}$

$E_1 = 1.21 \cdot \frac{1}{2}mv_0^2 - GMm/r = 1.21 \cdot \frac{GMm}{2r} - \frac{GMm}{r} = \frac{GMm}{r}(0.605 - 1) = -0.395\dfrac{GMm}{r}$

$a = -\dfrac{GMm}{2 \times (-0.395GMm/r)} = \dfrac{r}{0.79} \approx 1.266r \approx 8.86 \times 10^6\ \text{m}$

用角动量和能量求偏心率 $e$：$e = \sqrt{1 + \dfrac{2EL^2}{G^2M^2m^3}}$

计算得 $r_{\min} = r$（点火点为近地点），$r_{\max} = a(1+e) \approx$ 远地点。

---

## 综合题 8：陀螺仪的进动（C 难度）

**题目**：陀螺转子（$I = 0.020\ \text{kg·m}^2$）以 $\omega = 200\ \text{rad/s}$ 自转。质心距支点 $d = 0.050\ \text{m}$，$M = 1.5\ \text{kg}$。求进动角速度 $\Omega$。

**解答**：

$\tau = Mgd = 0.735\ \text{N·m}$，$L = I\omega = 4.0\ \text{kg·m}^2\text{/s}$

$\Omega = \dfrac{\tau}{L} = 0.184\ \text{rad/s}$，周期 $T = 34.2\ \text{s}$

---

## 综合题 9：复合滑轮系统

**题目**：两个同轴滑轮——实心圆盘（$M_1 = 4.0\ \text{kg}$，$R_1 = 0.20\ \text{m}$）和薄圆环（$M_2 = 2.0\ \text{kg}$，$R_2 = 0.10\ \text{m}$）。绳绕 $R_1$ 连 $m_1 = 6.0\ \text{kg}$（桌面），绳绕 $R_2$ 连 $m_2 = 3.0\ \text{kg}$（悬挂）。求系统加速度。

**解答**：

$I_{\text{total}} = \frac{1}{2}M_1R_1^2 + M_2R_2^2 = 0.08 + 0.02 = 0.10\ \text{kg·m}^2$

$a_1 = R_1\alpha$，$a_2 = R_2\alpha = 0.5a_1$

$T_1 = m_1a_1 = 6.0a_1$，$T_2 = m_2(g - a_2) = 3.0(9.8 - 0.5a_1)$

$(T_2R_2 - T_1R_1) = I\alpha = I a_1/R_1$

$(29.4 - 1.5a_1)0.10 - 6.0a_1 \times 0.20 = 0.10 a_1/0.20$

$2.94 - 0.15a_1 - 1.20a_1 = 0.50a_1$ → $a_1 = \mathbf{1.59\ \text{m/s}^2}$

---

## 综合题 10：质心运动与转动的叠加

**题目**：均匀细杆（$M = 1.0\ \text{kg}$，$L = 0.60\ \text{m}$）静止在光滑水平面上。$m = 0.050\ \text{kg}$ 油灰以 $v = 12\ \text{m/s}$ 垂直击中杆一端并粘住。求碰后质心速度和角速度。

**解答**：

动量守恒：$mv = (M+m)v_{cm}$ → $v_{cm} = 0.571\ \text{m/s}$

碰撞对初始质心的角动量：$L_i = mvr_\perp$，$r_\perp = \frac{M}{M+m} \cdot \frac{L}{2} \approx 0.286\ \text{m}$

$L_i = 0.050 \times 12 \times 0.286 \approx 0.171\ \text{kg·m}^2\text{/s}$

碰后 $I$（对系统质心）$\approx 0.0343\ \text{kg·m}^2$

$\omega = \dfrac{L_i}{I} \approx \mathbf{4.99\ \text{rad/s}}$

---

## 综合题 11：开普勒定律验证

**题目**：火星 $T = 687$ 天，$a = 2.28 \times 10^{11}\ \text{m}$。验证 $T^2 \propto a^3$ 并求太阳质量。

**解答**：

$\dfrac{T_M^2}{T_E^2} = 3.54$，$\dfrac{a_M^3}{a_E^3} = 3.51$ → 验证 ✓

$M = \dfrac{4\pi^2 a^3}{GT^2} \approx \mathbf{1.99 \times 10^{30}\ \text{kg}}$

---

## 综合题 12：飞轮储能工程设计

**题目**：设计储存 $1.0\ \text{MJ}$ 的钢制飞轮（$\rho = 7800\ \text{kg/m}^3$，实心圆柱，$R = 0.40\ \text{m}$，$\omega_{\max} = 500\ \text{rad/s}$）。求厚度。

**解答**：

$I = \dfrac{2E}{\omega_{\max}^2} = 8.0\ \text{kg·m}^2$，$M = \dfrac{2I}{R^2} = 100\ \text{kg}$

$h = \dfrac{M}{\rho\pi R^2} \approx \mathbf{2.55\ \text{cm}}$

---

## 综合题 13：滑动到滚动的能量损失

**题目**：实心球（$M = 0.50\ \text{kg}$，$R = 0.040\ \text{m}$）以 $v_0 = 3.0\ \text{m/s}$、$\omega_0 = 0$ 沿 $\mu_k = 0.25$ 水平面滑动。求过渡到纯滚动损失的能量。

**解答**：

纯滚动条件建立时间 $t = \dfrac{2v_0}{7\mu_k g} \approx 0.350\ \text{s}$

$v_f = v_0 - \mu_k g t \approx 2.14\ \text{m/s}$

$K_i = 2.25\ \text{J}$，$K_f = \frac{7}{10}Mv_f^2 \approx 1.60\ \text{J}$

$\Delta K = \mathbf{-0.65\ \text{J}}$（约 29%）

---

## 综合题 14：有质量滑轮系统

**题目**：滑轮（$I$，$R$）两侧悬 $m_1 > m_2$。释放后瞬间求角加速度。

**解答**：

$m_1g - T_1 = m_1a$，$T_2 - m_2g = m_2a$，$(T_1 - T_2)R = I\alpha$，$a = R\alpha$

$$
\alpha = \frac{(m_1 - m_2)gR}{I + (m_1 + m_2)R^2}
$$

---

## 综合题 15：双星系统角动量

**题目**：$M_1 = 2.0 \times 10^{30}\ \text{kg}$，$M_2 = 1.0 \times 10^{30}\ \text{kg}$，间距 $d = 1.0 \times 10^{12}\ \text{m}$ 绕共同质心做圆轨道。求周期和总角动量。

**解答**：

$r_1 = \frac{M_2}{M_1+M_2}d \approx 3.33 \times 10^{11}\ \text{m}$，$r_2 \approx 6.67 \times 10^{11}\ \text{m}$

$\omega = \sqrt{\dfrac{GM_2}{d^2 r_1}} \approx 1.41 \times 10^{-9}\ \text{rad/s}$，$T \approx \mathbf{141\ \text{年}}$

$L \approx \mathbf{9.4 \times 10^{44}\ \text{kg·m}^2\text{/s}}$

---

> **📚 第六章核心回顾**：
>
> 1. **转动动能**：$K_{\text{rot}} = \frac{1}{2}I\omega^2 = \dfrac{L^2}{2I}$
> 2. **旋转功**：$W = \tau\Delta\theta$，$P = \tau\omega$
> 3. **角动量**：$L = I\omega = rmv\sin\theta$
> 4. **角动量守恒**：$\Sigma\tau_{\text{ext}} = 0 \Rightarrow I_i\omega_i = I_f\omega_f$
> 5. **纯滚动**：$v_{cm} = R\omega$，$K = \frac{1}{2}Mv_{cm}^2(1 + \beta)$
> 6. **卫星轨道**：$v = \sqrt{GM/r}$，$T^2 \propto r^3$，$E = -\dfrac{GMm}{2r}$（C 版）
>
> 第六章将能量和动量两大守恒定律扩展到转动世界——这是力学体系的最终完整形态。

## 综合题 1：弹道摆——角动量守恒 + 能量

**题目**：一个 $m = 0.050\ \text{kg}$ 的子弹以 $v_0 = 300\ \text{m/s}$ 水平射入并嵌入一个静止的均匀细杆下端。杆质量 $M = 2.0\ \text{kg}$，长度 $L = 1.0\ \text{m}$，可绕上端自由旋转。求杆摆起的最大角度。

**解答**：

**第一步**：碰撞瞬间角动量守恒（对杆上端）。子弹角动量 = 系统末角动量。

子弹对杆上端的角动量（碰撞前）：
$$
L_i = mv_0L = 0.050 \times 300 \times 1.0 = 15\ \text{kg·m}^2\text{/s}
$$

系统末转动惯量（杆绕端点 $I = \frac{1}{3}ML^2$ + 子弹 $mL^2$）：
$$
I_f = \frac{1}{3}ML^2 + mL^2 = \frac{1}{3} \times 2.0 \times 1.0^2 + 0.050 \times 1.0^2 = 0.667 + 0.050 = 0.717\ \text{kg·m}^2
$$

末角速度：
$$
\omega_f = \frac{L_i}{I_f} = \frac{15}{0.717} \approx 20.92\ \text{rad/s}
$$

**第二步**：碰后能量守恒（转动动能 → 重力势能）。

杆质心上升 $h_{\text{rod}} = \frac{L}{2}(1 - \cos\theta)$，子弹上升 $h_{\text{bullet}} = L(1 - \cos\theta)$。

$$
\frac{1}{2}I_f\omega_f^2 = Mg \cdot \frac{L}{2}(1 - \cos\theta) + mgL(1 - \cos\theta)
$$

$$
\frac{1}{2} \times 0.717 \times (20.92)^2 = (2.0 \times 9.8 \times 0.5 + 0.050 \times 9.8 \times 1.0)(1 - \cos\theta)
$$

$$
157.0 = (9.8 + 0.49)(1 - \cos\theta) = 10.29(1 - \cos\theta)
$$

$$
1 - \cos\theta = 15.25 \quad \rightarrow \quad \text{不可能！}
$$

> ⚠️ 弹道摆问题中，若子弹动能过大，杆会转过最高点继续旋转。此处 $\omega_f$ 过大，杆会完成整圈旋转——$1 - \cos\theta$ 不能超过 2，实际 $\theta_{\max}$ 将是 $360^\circ$（完整一圈）。

---

## 综合题 2：滚下斜面的能量分配

**题目**：一个实心球从高度 $h = 2.0\ \text{m}$ 的斜面顶端从静止纯滚动到底部。求：
(a) 底部平动速度
(b) 平动动能与转动动能之比
(c) 若球不是滚动而是无摩擦滑动，底部速度是多少？

**解答**：

**(a)** 能量守恒：$Mgh = \frac{7}{10}Mv^2$

$$
v = \sqrt{\frac{10}{7}gh} = \sqrt{\frac{10}{7} \times 9.8 \times 2.0} = \sqrt{28} \approx \mathbf{5.29\ \text{m/s}}
$$

**(b)** $\dfrac{K_{\text{trans}}}{K_{\text{rot}}} = \dfrac{\frac{1}{2}Mv^2}{\frac{1}{5}Mv^2} = \dfrac{5}{2} = \mathbf{2.5}$

**(c)** 纯滑动：$v_{\text{slide}} = \sqrt{2gh} = \sqrt{2 \times 9.8 \times 2.0} = \sqrt{39.2} \approx \mathbf{6.26\ \text{m/s}}$

滚动速度/滑动速度 = $5.29 / 6.26 \approx 0.845$

---

## 综合题 3：飞轮制动——角冲量与功的综合应用

**题目**：一个飞轮（$I = 3.0\ \text{kg·m}^2$）以 $\omega_0 = 40\ \text{rad/s}$ 旋转。制动器对飞轮施加恒定的 $\tau = -12\ \text{N·m}$ 力矩。求：
(a) 飞轮停止所需的时间
(b) 制动过程中力矩做的功
(c) 制动过程中的角冲量大小
(d) 验证功-能定理和角冲量-角动量定理的一致性

**解答**：

**(a)** $\alpha = \tau/I = -12/3.0 = -4.0\ \text{rad/s}^2$

$t = \dfrac{0 - 40}{-4.0} = \mathbf{10.0\ \text{s}}$

**(b)** 制动过程中的角位移：$\theta = \frac{1}{2}(\omega_0 + 0)t = \frac{1}{2} \times 40 \times 10 = 200\ \text{rad}$

$W = \tau\theta = (-12) \times 200 = \mathbf{-2400\ \text{J}}$（负功，减少动能）

**(c)** 角冲量 = $|\tau t| = 12 \times 10 = \mathbf{120\ \text{N·m·s}}$

**(d)** 功-能定理：$W = \Delta K = 0 - \frac{1}{2} \times 3.0 \times 40^2 = -2400\ \text{J}$ ✓

角冲量-角动量定理：$\tau t = \Delta L = 0 - 3.0 \times 40 = -120\ \text{kg·m}^2\text{/s}$ ✓

两者数值一致：$|W| = |\tau|\theta = 2400\ \text{J}$，$|\Delta L| = |\tau|t = 120\ \text{kg·m}^2\text{/s}$。注意功和角动量变化的关系：$\Delta K = \frac{L_f^2 - L_i^2}{2I}$。

---

## 综合题 4：两个滑轮的角动量守恒碰撞

**题目**：滑轮 A（$I_A = 2.0\ \text{kg·m}^2$）以 $\omega_A = 15\ \text{rad/s}$ 逆时针旋转，滑轮 B（$I_B = 3.0\ \text{kg·m}^2$）以 $\omega_B = 10\ \text{rad/s}$ 顺时针旋转。两滑轮突然啮合在一起（同轴）。求：
(a) 啮合后的角速度（大小和方向）
(b) 碰撞中的动能损失
(c) 损失的动能占初始总动能的百分比

**解答**：

**(a)** 取逆时针为正：$L_A = 2.0 \times 15 = 30$，$L_B = 3.0 \times (-10) = -30$

$L_{\text{total}} = 30 + (-30) = 0$ → $\omega_f = \mathbf{0}$！

**(b)** $K_i = \frac{1}{2} \times 2.0 \times 15^2 + \frac{1}{2} \times 3.0 \times 10^2 = 225 + 150 = 375\ \text{J}$

$K_f = 0$ → $\Delta K = \mathbf{-375\ \text{J}}$（全部损失！）

**(c)** 损失 100%。两滑轮的角动量大小相等方向相反，碰撞后完全停止——所有动能转化为热。这类似两个动量等大反向的物体发生完全非弹性碰撞后静止。

---

> **📚 第六章核心回顾**：

**题目**：一个 $m = 0.050\ \text{kg}$ 的子弹以 $v_0 = 300\ \text{m/s}$ 水平射入并嵌入一个静止的均匀细杆下端。杆质量 $M = 2.0\ \text{kg}$，长度 $L = 1.0\ \text{m}$，可绕上端自由旋转。求杆摆起的最大角度。

**解答**：

**第一步**：碰撞瞬间角动量守恒（对杆上端）。子弹角动量 = 系统末角动量。

子弹对杆上端的角动量（碰撞前）：
$$
L_i = mv_0L = 0.050 \times 300 \times 1.0 = 15\ \text{kg·m}^2\text{/s}
$$

系统末转动惯量（杆绕端点 $I = \frac{1}{3}ML^2$ + 子弹 $mL^2$）：
$$
I_f = \frac{1}{3}ML^2 + mL^2 = \frac{1}{3} \times 2.0 \times 1.0^2 + 0.050 \times 1.0^2 = 0.667 + 0.050 = 0.717\ \text{kg·m}^2
$$

末角速度：
$$
\omega_f = \frac{L_i}{I_f} = \frac{15}{0.717} \approx 20.92\ \text{rad/s}
$$

**第二步**：碰后能量守恒（转动动能 → 重力势能）。

杆质心上升 $h_{\text{rod}} = \frac{L}{2}(1 - \cos\theta)$，子弹上升 $h_{\text{bullet}} = L(1 - \cos\theta)$。

$$
\frac{1}{2}I_f\omega_f^2 = Mg \cdot \frac{L}{2}(1 - \cos\theta) + mgL(1 - \cos\theta)
$$

$$
\frac{1}{2} \times 0.717 \times (20.92)^2 = (2.0 \times 9.8 \times 0.5 + 0.050 \times 9.8 \times 1.0)(1 - \cos\theta)
$$

$$
157.0 = (9.8 + 0.49)(1 - \cos\theta) = 10.29(1 - \cos\theta)
$$

$$
1 - \cos\theta = 15.25 \quad \rightarrow \quad \text{不可能！}
$$

> ⚠️ 弹道摆问题中，若子弹动能过大，杆会转过最高点继续旋转。此处 $\omega_f$ 过大，杆会完成整圈旋转——$1 - \cos\theta$ 不能超过 2，实际 $\theta_{\max}$ 将是 $360^\circ$（完整一圈）。

---

## 综合题 2：滚下斜面的能量分配

**题目**：一个实心球从高度 $h = 2.0\ \text{m}$ 的斜面顶端从静止纯滚动到底部。求：
(a) 底部平动速度
(b) 平动动能与转动动能之比
(c) 若球不是滚动而是无摩擦滑动，底部速度是多少？

**解答**：

**(a)** 能量守恒：$Mgh = \frac{7}{10}Mv^2$

$$
v = \sqrt{\frac{10}{7}gh} = \sqrt{\frac{10}{7} \times 9.8 \times 2.0} = \sqrt{28} \approx \mathbf{5.29\ \text{m/s}}
$$

**(b)** $\dfrac{K_{\text{trans}}}{K_{\text{rot}}} = \dfrac{\frac{1}{2}Mv^2}{\frac{1}{5}Mv^2} = \dfrac{5}{2} = \mathbf{2.5}$

**(c)** 纯滑动：$v_{\text{slide}} = \sqrt{2gh} = \sqrt{2 \times 9.8 \times 2.0} = \sqrt{39.2} \approx \mathbf{6.26\ \text{m/s}}$

滚动速度/滑动速度 = $5.29 / 6.26 \approx 0.845$

---

> **📚 第六章核心回顾**：
>
> 1. **转动动能**：$K_{\text{rot}} = \frac{1}{2}I\omega^2 = \dfrac{L^2}{2I}$
> 2. **旋转功**：$W = \tau\Delta\theta$，$P = \tau\omega$
> 3. **角动量**：$L = I\omega = rmv\sin\theta$
> 4. **角动量守恒**：$\Sigma\tau_{\text{ext}} = 0 \Rightarrow I_i\omega_i = I_f\omega_f$
> 5. **纯滚动**：$v_{cm} = R\omega$，$K = \frac{1}{2}Mv_{cm}^2(1 + \beta)$
> 6. **卫星轨道**：$v = \sqrt{GM/r}$，$T^2 \propto r^3$，$E = -\dfrac{GMm}{2r}$（C 版）
>
> 第六章将能量和动量两大守恒定律扩展到转动世界——这是力学体系的最终完整形态。