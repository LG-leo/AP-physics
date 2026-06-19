<!-- markdownlint-disable MD033 MD041 -->

<div align="center">

# 📚 AP Physics — 运动学 1.1：标量与矢量

> **Scalars vs. Vectors — 完整综合版**
>
> 覆盖 AP Physics 1 & 2（代数）+ AP Physics C（微积分）全难度层级

[![AP Physics](https://img.shields.io/badge/AP-Physics-001845?style=for-the-badge&logo=apache&logoColor=white)](https://ap.collegeboard.org/)
[![Physics 1](https://img.shields.io/badge/AP%20Physics-1-FF6B35?style=flat-square)]()
[![Physics C](https://img.shields.io/badge/AP%20Physics-C-004E89?style=flat-square)]()
[![GitHub](https://img.shields.io/badge/maintained%20with-❤️-ff69b4?style=flat-square)]()

</div>

---

## 📑 目录

- [Part A：基础层（AP Physics 1 & 2 必备）](#part-a基础层ap-physics-1--2-必备)
  - [一、核心概念——标量与矢量的本质区别](#一核心概念标量与矢量的本质区别)
  - [二、距离 vs 位移](#二距离-vs-位移distance-vs-displacement)
  - [三、速率 vs 速度](#三速率-vs-速度speed-vs-velocity)
  - [四、一维运动中的正方向约定](#四一维运动中的正方向约定)
  - [五、矢量分解与合成](#五矢量分解与合成)
- [Part B：AP 难度层](#part-bap-难度层概念陷阱--深度理解)
  - [六、AP 考试真正的概念陷阱](#六ap-考试真正考的概念陷阱)
  - [七、AP Physics C 的微积分深度](#七ap-physics-c-的微积分深度)
  - [八、难度分级总结](#八ap-考试难度分级总结)
  - [九、AP 级别综合练习](#九ap-级别综合练习)
  - [十、考点频率统计](#十本节-ap-考点频率统计)

---

# Part A：基础层（AP Physics 1 & 2 必备）

---

## 一、核心概念——标量与矢量的本质区别

### 1.1 定义对比

| 对比项 | 标量（Scalar） | 矢量（Vector） |
|:--|:--|:--|
| **定义** | 只有 **大小**（magnitude）的物理量 | 既有 **大小** 又有 **方向**（direction）的物理量 |
| **数学表示** | 一个实数（带单位） | 箭头符号 $\vec{v}$ 或加粗 $\mathbf{v}$，或分量形式 $\langle v_x, v_y \rangle$ |
| **运算规则** | 普通代数运算（$2+3=5$） | 遵循 **矢量加法**（平行四边形法则、分量加法） |
| **能否为负** | ❌ 标量（如速率、距离）不能为负 | ✅ 一维中用正负号表示方向 |

### 1.2 常见物理量分类

| 标量（Scalar） | 矢量（Vector） |
|:--|:--|
| 距离（distance）、速率（speed） | 位移（displacement）、速度（velocity） |
| 时间（time）、质量（mass） | 加速度（acceleration）、力（force） |
| 能量（energy）、功（work） | 动量（momentum）、冲量（impulse） |
| 功率（power）、温度（temperature） | 电场强度（electric field）、磁场强度（magnetic field） |
| 电荷量（charge）、电势（potential） | 重力（gravity）、摩擦力（friction） |

---

## 二、距离 vs 位移（Distance vs. Displacement）

### 2.1 定义对比

| | **距离（Distance）** | **位移（Displacement）** |
|:--|:--|:--|
| 类别 | **标量** | **矢量** |
| 含义 | 物体运动路径的 **总长度** | 从起点指向终点的 **有向线段** |
| 关心什么 | "走了多远"（不管方向） | "从哪到哪，多远 + 什么方向" |
| 能否为零 | 只有物体没动时才为零 | 可以为零——走一圈回到原点，位移 $=0$，但距离 $\neq 0$ |
| 符号 | $d$ 或 $s$（纯数值） | $\Delta \vec{x}$ 或 $\vec{d}$ |
| 单位 | 米（m） | 米（m） |

### 2.2 🧪 经典基础例题

**题目**：小明从家出发向东走 3 m，然后向北走 4 m。

- **距离**（总路径长）$= 3 + 4 = \mathbf{7\ m}$ ✅
- **位移**（起点→终点的直线距离）$= \sqrt{3^2 + 4^2} = \mathbf{5\ m}$，方向为 **东偏北 $53^\circ$**（$\theta = \tan^{-1}\frac{4}{3}$）✅

---

## 三、速率 vs 速度（Speed vs. Velocity）

### 3.1 定义对比

| | **速率（Speed）** | **速度（Velocity）** |
|:--|:--|:--|
| 类别 | **标量** | **矢量** |
| 含义 | "有多快"（只问快慢） | "有多快 + 往哪去" |
| 公式 | $v = \dfrac{\text{距离}}{\text{时间}}$ | $\vec{v} = \dfrac{\Delta \vec{x}}{\Delta t}$ |
| AP 符号 | $v$（没有箭头） | $\vec{v}$ 或 $v_x$（带正负号的一维表示） |
| 能否为负 | ❌ 速率永远是 **非负** 的 | ✅ 可以 **为负**——表示与正方向相反 |

### 3.2 关键理解

在一维运动中，我们 **先选一个正方向**（比如向右为正），那么：

- 物体 **向右** 运动 → 速度为 $+5\ \text{m/s}$
- 物体 **向左** 运动 → 速度为 $-5\ \text{m/s}$

**速率都是 $5\ \text{m/s}$**，但速度方向不同！

---

## 四、一维运动中的正方向约定

### 4.1 标准做法

在一维（直线）运动中，我们用 **正负号** 代表方向：

```
          ← 负方向          正方向 →
    ─────┼────┼────┼────┼────┼────
         -2   -1    0    1    2
```

- 选取一个方向为 **正方向**（通常是向右或向上）
- 与正方向相同 → **正值**
- 与正方向相反 → **负值**

### 4.2 🧪 基础例题

一个物体从 $x=2\ \text{m}$ 运动到 $x=-3\ \text{m}$，若正方向向右：

- 位移 $\Delta x = x_f - x_i = -3 - 2 = \mathbf{-5\ m}$（向左移动了 5 m）
- 如果用了 2 秒，则平均速度 $\bar{v}= \dfrac{-5}{2} = \mathbf{-2.5\ m/s}$

---

## 五、矢量分解与合成

### 5.1 分量分解

将矢量 $\vec{v}$ 分解为互相垂直的分量（设 $\theta$ 为与 $x$ 轴正方向的夹角）：

```
        ↑
        |  v_y = v·sinθ
        |  ↗
        | /
    θ   |/→ v_x = v·cosθ
    ────┴────────→
```

- $v_x = v \cos\theta$
- $v_y = v \sin\theta$

### 5.2 矢量合成

- $v = \sqrt{v_x^2 + v_y^2}$
- $\theta = \tan^{-1}\left(\dfrac{v_y}{v_x}\right)$

### 5.3 一维矢量加法

> 直接代数相加，注意正负号！

**例**：物体受到向右 5 N 和向左 3 N 的力

- 设向右为正
- 合力 $F_{net} = 5 + (-3) = \mathbf{2\ N}$（向右）

### 5.4 🧪 推导：矢量分解与合成的几何基础

矢量加法有两种等价的方法——**图解法**（平行四边形法则）和 **解析法**（分量加法）。下面证明它们的等价性。

#### 平行四边形法则

对于两个矢量 $\vec{a}$ 和 $\vec{b}$，其合矢量 $\vec{c} = \vec{a} + \vec{b}$ 是以 $\vec{a}$ 和 $\vec{b}$ 为邻边的平行四边形的对角线。

#### 从平行四边形法则→分量加法的推导

设 $\vec{a} = a_x\hat{i} + a_y\hat{j}$，$\vec{b} = b_x\hat{i} + b_y\hat{j}$，其夹角为 $\phi$。

根据平行四边形法则，合矢量的大小为：

$$
c = \sqrt{a^2 + b^2 + 2ab\cos\phi}
$$

根据分量加法：

$$
\vec{c} = (a_x + b_x)\hat{i} + (a_y + b_y)\hat{j}
$$

其大小为：

$$
|c| = \sqrt{(a_x + b_x)^2 + (a_y + b_y)^2}
$$

由于 $a_x = a\cos\theta_a$，$a_y = a\sin\theta_a$，$b_x = b\cos\theta_b$，$b_y = b\sin\theta_b$，代入展开：

$$
|c| = \sqrt{a^2 + b^2 + 2ab(\cos\theta_a\cos\theta_b + \sin\theta_a\sin\theta_b)} = \sqrt{a^2 + b^2 + 2ab\cos(\theta_a - \theta_b)}
$$

其中 $\phi = \theta_a - \theta_b$ 正是两矢量的夹角。两种方法得到完全相同的结果！✅

> 💡 **核心结论**：平行四边形法则和分量加法是 **完全等价** 的——解析法本质上是将几何问题转化为代数计算，更适合编程和数值计算。

### 5.5 🧪 例题：多个矢量的连续相加

**题目**：某物体依次受到三个力的作用：$\vec{F}_1 = 3\hat{i} + 4\hat{j}\ \text{N}$，$\vec{F}_2 = -2\hat{i} + \hat{j}\ \text{N}$，$\vec{F}_3 = \hat{i} - 3\hat{j}\ \text{N}$。求合力的大小和方向。

**解答**：

**(1)** 分量法相加：

$$
\vec{F}_{net} = \vec{F}_1 + \vec{F}_2 + \vec{F}_3 = (3 - 2 + 1)\hat{i} + (4 + 1 - 3)\hat{j} = 2\hat{i} + 2\hat{j}\ \text{N}
$$

**(2)** 合力大小：

$$
|\vec{F}_{net}| = \sqrt{2^2 + 2^2} = \sqrt{8} = 2\sqrt{2} \approx \mathbf{2.83\ N}
$$

**(3)** 合力方向（与 $x$ 轴正方向夹角）：

$$
\theta = \tan^{-1}\left(\frac{2}{2}\right) = \tan^{-1}(1) = \mathbf{45^\circ}
$$

> ⭐ **无论有多少个矢量相加，只需将它们的 $x$ 分量和 $y$ 分量分别求和即可！**

---

# Part B：AP 难度层（概念陷阱 + 深度理解）

---

## 六、AP 考试真正考的概念陷阱

### 🎯 陷阱 1：看似简单的情境辨析

**真题风格**：

> A person walks 10 m east, then 10 m north, then 10 m west.
>
> **Question**: Which of the following is true about the person's motion?
>
> A) Distance = 30 m, Displacement = 10 m north
> B) Distance = 30 m, Displacement = 10 m east
> C) Distance = 10 m, Displacement = 30 m
> D) Distance = 30 m, Displacement = 0 m

**答案**：A ✅

- 距离 $= 10+10+10 = 30$ m
- 位移 $=$ 从起点 $(0,0)$ 到终点 $(0,10) =$ **10 m 向北**
- ❌ 常见错误：有人觉得走了一圈回到原点，但这里是回到 $x=0,\ y=10$，**没有回原点**！

> 💡 **AP 难度精髓**：他们不会让你算简单的来回直线，而是设一个 **让你误以为回到原点** 的路径！

---

### 🎯 陷阱 2：速率 vs 速度的深层理解

**AP Physics 1 必考概念题**：

> An object moves in a **circular path** at **constant speed**.
>
> Which of the following statements is correct?
>
> A) Both speed and velocity are constant.
> B) Speed is constant, so acceleration is zero.
> C) **Velocity changes because direction changes, so there is acceleration.**
> D) Acceleration is zero because speed is constant.

**答案**：C ✅

> ⚠️ 这就是 AP 最喜欢的设计——**用"匀速"这个词误导你**！"匀速圆周运动"中的"匀速"是指速率 constant，但 velocity 每一瞬间方向都在变，所以 **velocity is NOT constant**，因此 **一定有加速度**（向心加速度）！

---

### 🎯 陷阱 3：正负号的真正含义

AP 不会只问你"正负号表示什么"，它会在 **计算中设坑**：

> A ball is thrown **upward** from the ground with initial speed $v_0$.

**AP 学生的常见错误**：

```
❌ 设向上为正，重力加速度 g = 9.8 m/s²（忘了加负号！）
```

**正确做法**：

```
✅ 设向上为正，则 a = -g = -9.8 m/s²
   v(t) = v₀ - gt
   y(t) = v₀t - ½gt²
```

**换个方向呢？**

```
✅ 设向下为正，则 a = +g = +9.8 m/s²
   但此时 v₀ 就是负的了（因为向上抛，与正方向相反）
   v(t) = -v₀ + gt
```

> ⭐ **AP C 级别的理解**：正方向的选择不会改变物理结果，只是改变了方程中正负号的写法。两种选法算出来的 **最终答案（大小和实际方向）是一样的**。

---

### 🎯 陷阱 4：平均速率 vs 平均速度

AP 考试特别爱考这个区别！

| | **平均速率（Average Speed）** | **平均速度（Average Velocity）** |
|:--|:--|:--|
| 公式 | $\bar{v}_{\text{avg speed}} = \dfrac{\text{总距离}}{\text{总时间}}$ | $\vec{\bar{v}} = \dfrac{\text{总位移}}{\text{总时间}}$ |
| 类别 | **标量** | **矢量** |

**🧪 经典 AP 陷阱题**：

> A runner runs 100 m east in 10 s, then turns around and runs 60 m west in 10 s.
>
> (a) Average speed?
> (b) Average velocity?

**解答**：

- 总距离 $= 100 + 60 = 160$ m，总时间 $= 10 + 10 = 20$ s
- (a) **平均速率** $= \dfrac{160}{20} = \mathbf{8\ m/s}$ ✅
- 总位移 $= 100 - 60 = 40$ m（向东）
- (b) **平均速度** $= \dfrac{40}{20} = \mathbf{2\ m/s\ east}$ ✅

> ⚠️ 看到没有？平均速率是 **8 m/s**，平均速度只有 **2 m/s**！这两个值可以差很大！

---

## 七、AP Physics C 的微积分深度

### 7.1 矢量在微积分框架下的意义

AP Physics C 要求你从 **代数视角** 升级到 **微积分视角**：

| 概念 | 代数理解（AP 1） | **微积分理解（AP C）** |
|:--|:--|:--|
| **位置** | 一个坐标值 $x$ | 位置矢量 $\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j} + z(t)\hat{k}$ |
| **位移** | $\Delta \vec{x} = \vec{x}_f - \vec{x}_i$ | $\Delta \vec{r} = \displaystyle\int_{t_i}^{t_f} \vec{v}(t)\ dt$ |
| **速度** | $\vec{v} = \dfrac{\Delta\vec{x}}{\Delta t}$ | $\vec{v}(t) = \dfrac{d\vec{r}}{dt} = \dot{x}\hat{i} + \dot{y}\hat{j} + \dot{z}\hat{k}$ |
| **加速度** | $\vec{a} = \dfrac{\Delta\vec{v}}{\Delta t}$ | $\vec{a}(t) = \dfrac{d\vec{v}}{dt} = \dfrac{d^2\vec{r}}{dt^2}$ |
| **速率** | $v = \|\vec{v}\|$（几何意义） | $v = \|\vec{v}(t)\| = \sqrt{\dot{x}^2 + \dot{y}^2 + \dot{z}^2}$（函数求模） |

### 7.2 核心微积分关系图

```
位置矢量 ──求导──▶ 速度矢量 ──求导──▶ 加速度矢量
 →r(t)          →v(t)          →a(t)
   │               │               │
   ◀──积分────    ◀──积分────
```

### 7.3 🧪 AP Physics C 真题难度示例

> The position of a particle is given by $\vec{r}(t) = (3t^2 - 2t)\hat{i} + (4t)\hat{j}$ meters.
>
> **(a)** Find the velocity vector $\vec{v}(t)$.
> **(b)** Find the **speed** at $t = 2$ s.
> **(c)** Find the acceleration vector.

**解答**：

**(a)**

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (6t - 2)\hat{i} + 4\hat{j}\ \text{m/s}
$$

**(b) ⚠️ 重点！** speed = |velocity|，不是某个分量！

$$
\vec{v}(2) = (12-2)\hat{i} + 4\hat{j} = 10\hat{i} + 4\hat{j}
$$

$$
\text{speed} = |\vec{v}(2)| = \sqrt{10^2 + 4^2} = \sqrt{116} \approx 10.77\ \text{m/s}
$$

> ⚠️ **AP C 常见失分点**：题目问 speed，很多学生直接给了 $10$ 或 $4$，忘了求模！

**(c)**

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = 6\hat{i} + 0\hat{j} = 6\hat{i}\ \text{m/s}^2
$$

> 注意加速度是 **常数**，而且只有 $x$ 方向！这说明虽然粒子在二维空间运动，但 $y$ 方向速度恒定，只有 $x$ 方向在加速。

### 7.4 📐 矢量点积与夹角的微积分应用

**AP Physics C 中，经常需要求速度与加速度之间的夹角**：

$$
\vec{v} \cdot \vec{a} = |\vec{v}||\vec{a}|\cos\theta \quad\Rightarrow\quad \cos\theta = \frac{\vec{v} \cdot \vec{a}}{|\vec{v}||\vec{a}|}
$$

**🧪 示例**：接上题，求 $t=1$ s 时 $\vec{v}$ 与 $\vec{a}$ 的夹角。

$$
\vec{v}(1) = (6-2)\hat{i} + 4\hat{j} = 4\hat{i} + 4\hat{j}
$$
$$
\vec{a} = 6\hat{i} + 0\hat{j}
$$
$$
\vec{v}\cdot\vec{a} = 4\times6 + 4\times0 = 24
$$
$$
|\vec{v}| = \sqrt{4^2+4^2} = \sqrt{32} = 4\sqrt{2}, \quad |\vec{a}| = 6
$$
$$
\cos\theta = \frac{24}{4\sqrt{2} \times 6} = \frac{24}{24\sqrt{2}} = \frac{1}{\sqrt{2}}
$$
$$
\theta = 45^\circ
$$

> 当 $\vec{v} \cdot \vec{a} > 0$ 时，速度与加速度方向夹角小于 $90^\circ$，物体在 **加速**；
> 当 $\vec{v} \cdot \vec{a} < 0$ 时，夹角大于 $90^\circ$，物体在 **减速**；
> 当 $\vec{v} \cdot \vec{a} = 0$ 时，两者垂直，速率不变（如匀速圆周运动）。

---

## 八、AP 考试难度分级总结

| 层次 | 对应考试 | 核心要求 | 典型题特征 |
|:--|:--|:--|:--|
| **Level 1：基础记忆** | 学校期中 | 知道标量和矢量的定义、常见分类 | 直接问"下列哪个是矢量？" |
| **Level 2：概念辨析** | **AP Physics 1 & 2** 🎯 | 能在情境中区分距离/位移、速率/速度；识别常见陷阱 | 路程折返问题、匀速圆周运动、平均速率 vs 平均速度 |
| **Level 3：微积分应用** | **AP Physics C** 🎯 | 对矢量函数求导/积分；用点积分析运动 | $\vec{r}(t)$ 求 $\vec{v}$、$\vec{a}$；求 speed 随时间变化；矢量夹角判断加速/减速 |

---

## 九、AP 级别综合练习

### 🟢 AP Physics 1 风格

> A car travels along a straight road. Its position as a function of time is given by $x(t) = 4t - t^2$ (meters, seconds).
>
> (a) At what time(s) does the car change direction?
> (b) What is the **displacement** of the car from $t=0$ to $t=4$ s?
> (c) What is the **distance traveled** from $t=0$ to $t=4$ s?
> (d) What is the **average speed** and **average velocity** over this interval?

**解答思路**：

- (a) 方向改变时 $v=0$，$v(t)=dx/dt=4-2t=0$ → $t=2$ s ✅
- (b) 位移 $= x(4) - x(0) = (16-16) - (0) = \mathbf{0\ m}$ ✅
- (c) 分两段算：
  - $0\rightarrow2$ s：$x(2)-x(0) = (8-4)-0 = 4$ m（正向）
  - $2\rightarrow4$ s：$x(4)-x(2) = 0-4 = -4$ m，绝对值 $4$ m（反向）
  - 距离 $= 4 + 4 = \mathbf{8\ m}$ ✅
- (d) 平均速度 $= 0/4 = \mathbf{0\ m/s}$，平均速率 $= 8/4 = \mathbf{2\ m/s}$ ✅

> ⚠️ **AP 陷阱**：位移为 0，但距离不为 0！平均速度为 0，但平均速率不为 0！

---

### 🔵 AP Physics C 风格

> A particle moves in the $xy$-plane with velocity $\vec{v}(t) = 3\hat{i} + 4t\hat{j}$ m/s.
> At $t=0$, the particle is at the origin.
>
> (a) Find the position vector $\vec{r}(t)$.
> (b) Find the acceleration vector $\vec{a}(t)$.
> (c) Find the magnitude of the acceleration at $t=2$ s.
> (d) Find the angle between the velocity and acceleration vectors at $t=1$ s.
> (e) Is the particle speeding up or slowing down at $t=1$ s? Justify.

**解答**：

**(a)**

$$
\vec{r}(t) = \int \vec{v}(t)\ dt = \int (3\hat{i} + 4t\hat{j})\ dt = 3t\hat{i} + 2t^2\hat{j} + \vec{C}
$$

代入 $\vec{r}(0)=\vec{0}$ 得 $\vec{C}=\vec{0}$，所以：

$$
\vec{r}(t) = 3t\hat{i} + 2t^2\hat{j}\ \text{m}
$$

**(b)**

$$
\vec{a}(t) = \dfrac{d\vec{v}}{dt} = 0\hat{i} + 4\hat{j} = 4\hat{j}\ \text{m/s}^2 \quad (\text{常数加速度！})
$$

**(c)**

$$
|\vec{a}| = \sqrt{0^2+4^2} = \mathbf{4\ m/s^2} \quad \checkmark \ (\text{与 } t \text{ 无关})
$$

**(d)** 在 $t=1$：

$$
\vec{v}(1) = 3\hat{i} + 4(1)\hat{j} = 3\hat{i} + 4\hat{j}
$$
$$
\vec{a} = 4\hat{j}
$$
$$
\vec{v}\cdot\vec{a} = 3\times0 + 4\times4 = 16
$$
$$
|\vec{v}| = \sqrt{3^2+4^2} = 5,\quad |\vec{a}| = 4
$$
$$
\cos\theta = \frac{16}{5\times4} = \frac{16}{20} = 0.8
$$
$$
\theta = \cos^{-1}(0.8) \approx \mathbf{36.9^\circ}
$$

**(e)** $\vec{v}\cdot\vec{a} = 16 > 0$，所以 $\theta < 90^\circ$，粒子在 **speeding up** ✅

> ⭐ **AP C FRQ 评分标准**：只说 speeding up 不够，要用点积或分量分析来 justify！

---

## 十、本节 AP 考点频率统计

| 考点 | AP 1 频率 | AP C 频率 | 说明 |
|:--|:--:|:--:|:--|
| 距离 vs 位移辨析 | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | AP 1 选择题最爱 |
| 速率 vs 速度辨析 | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | 匀速圆周运动必考 |
| 平均速率 vs 平均速度 | ⭐⭐⭐⭐ | ⭐⭐⭐ | FRQ 中也可能出现 |
| 正负号约定 | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | 一维运动基础 |
| 矢量分解与合成 | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | 贯穿所有力学题 |
| 矢量函数的求导/积分 | — | ⭐⭐⭐⭐⭐ | AP C 核心技能 |
| 点积判断加速/减速 | — | ⭐⭐⭐⭐ | FRQ 高频考点 |

---

<div align="center">

**📖 AP Physics — Kinematics 1.1: Scalars vs. Vectors**

*Made with ❤️ for AP Physics learners*

</div>

---
---

---

# 1.2 位移、速度与加速度（Displacement, Velocity & Acceleration）

---

## Part A：基础层（AP Physics 1 & 2 必备）

---

### 一、平均速度与瞬时速度

#### 1.2.1 平均速度（Average Velocity）

**定义**：位移与发生这段位移所用时间之比。

$$
\boxed{\vec{\bar{v}} = \frac{\Delta \vec{x}}{\Delta t} = \frac{\vec{x}_f - \vec{x}_i}{t_f - t_i}}
$$

| 项目 | 说明 |
|:--|:--|
| 类别 | **矢量** —— 方向与位移方向相同 |
| 物理含义 | 描述一段时间内 **整体运动快慢和方向** |
| 单位 | m/s（米每秒） |
| 与路径无关 | 只关心起点和终点，不关心中间怎么走的 |

> ⚠️ **注意**：平均速度不是速度的平均值！$\vec{\bar{v}} \neq \dfrac{\vec{v}_i + \vec{v}_f}{2}$（只有在 **匀加速直线运动** 中这个等式才成立！）

#### 1.2.2 瞬时速度（Instantaneous Velocity）

**定义**：物体在 **某一时刻** 或 **某一位置** 的速度。

$$
\boxed{\vec{v}(t) = \lim_{\Delta t \to 0} \frac{\Delta \vec{x}}{\Delta t}}
$$

| 项目 | 说明 |
|:--|:--|
| 类别 | **矢量** —— 方向为物体在该点的运动方向 |
| 物理含义 | 描述物体在 **某个瞬间** 运动的快慢和方向 |
| 直观理解 | 汽车速度表上显示的就是瞬时速率（标量形式） |

#### 1.2.3 平均速率（Average Speed）—— 再强调一次！

$$
\boxed{\bar{v}_{\text{speed}} = \frac{\text{总距离}}{\text{总时间}}}
$$

> **平均速率 $\neq$ 平均速度的大小！**
>
> 只有物体沿 **单一方向直线运动** 且 **不折返** 时，平均速率才等于平均速度的大小。

**🧪 示例**：绕操场跑一圈 400 m，用时 80 s
- 平均速率 $= 400 / 80 = 5\ \text{m/s}$
- 平均速度 $= 0 / 80 = 0\ \text{m/s}$（回到起点，位移为 0）
- 平均速度的大小 $= 0 \neq 5$ ✅

---

### 二、平均加速度与瞬时加速度

#### 2.1 平均加速度（Average Acceleration）

**定义**：速度变化量与发生这一变化所用时间之比。

$$
\boxed{\vec{\bar{a}} = \frac{\Delta \vec{v}}{\Delta t} = \frac{\vec{v}_f - \vec{v}_i}{t_f - t_i}}
$$

| 项目 | 说明 |
|:--|:--|
| 类别 | **矢量** —— 方向与速度变化量 $\Delta \vec{v}$ 的方向相同 |
| 物理含义 | 描述一段时间内 **速度变化的平均快慢** |
| 单位 | m/s²（米每二次方秒） |

> ⚠️ **注意**：加速度的方向 **不一定** 是速度方向！加速时 $\vec{a}$ 与 $\vec{v}$ 同向，减速时反向。

#### 2.2 瞬时加速度（Instantaneous Acceleration）

**定义**：物体在 **某一时刻** 的加速度。

$$
\boxed{\vec{a}(t) = \lim_{\Delta t \to 0} \frac{\Delta \vec{v}}{\Delta t}}
$$

| 项目 | 说明 |
|:--|:--|
| 类别 | **矢量** |
| 物理含义 | 描述物体在 **某个瞬间** 速度变化的快慢 |

#### 2.3 关键理解：加速度的方向

加速度的方向 **由 $\Delta \vec{v}$ 决定**，不是由 $\vec{v}$ 本身决定！

| 运动状态 | $\vec{v}$ 方向 | $\vec{a}$ 方向 | $\Delta \vec{v}$ 方向 |
|:--|:--|:--|:--|
| 向东加速 | → 东 | → 东 | → 东 |
| 向东减速 | → 东 | ← 西 | ← 西 |
| 向西加速 | ← 西 | ← 西 | ← 西 |
| 向西减速 | ← 西 | → 东 | → 东 |

> 💡 **记忆口诀**：加速时 $\vec{a}$ 与 $\vec{v}$ **同向**，减速时 $\vec{a}$ 与 $\vec{v}$ **反向**。

---

### 三、匀加速直线运动三大公式

#### 3.1 适用条件

> 物体沿 **直线** 运动，且 **加速度为常数**（大小和方向都不变）。

#### 3.2 三大核心公式

设 $t=0$ 时初速度为 $v_0$，位置为 $x_0$，加速度 $a$ 为常数：

| 编号 | 公式 | 含义 | 不含的变量 |
|:--:|:--|:--|:--:|
| **①** | $v = v_0 + at$ | **速度-时间关系** | $\Delta x$ |
| **②** | $\Delta x = v_0 t + \dfrac{1}{2}at^2$ | **位置-时间关系** | $v$ |
| **③** | $v^2 = v_0^2 + 2a\Delta x$ | **速度-位移关系** | $t$ |

其中 $\Delta x = x - x_0$。

#### 3.3 🧪 经典基础例题

**题目**：一辆汽车从静止开始以 $2\ \text{m/s}^2$ 的加速度匀加速行驶 5 秒。求：
(a) 第 5 秒末的速度
(b) 前 5 秒内的位移

**解答**：

已知 $v_0 = 0$，$a = 2\ \text{m/s}^2$，$t = 5\ \text{s}$

**(a)** 用公式 ①：
$$v = v_0 + at = 0 + 2 \times 5 = \mathbf{10\ m/s}$$

**(b)** 用公式 ②：
$$\Delta x = v_0 t + \frac{1}{2}at^2 = 0 + \frac{1}{2} \times 2 \times 5^2 = \mathbf{25\ m}$$

#### 3.4 公式的选择策略 🎯

| 已知条件 | 要求 | 选哪个公式 |
|:--|:--|:--:|
| $v_0,\ a,\ t$ | $v$ | ① $v = v_0 + at$ |
| $v_0,\ a,\ t$ | $\Delta x$ | ② $\Delta x = v_0 t + \frac{1}{2}at^2$ |
| $v_0,\ a,\ \Delta x$ | $v$ | ③ $v^2 = v_0^2 + 2a\Delta x$ |
| $v_0,\ v,\ a$ | $\Delta x$ | ③ 变形 $\Delta x = \dfrac{v^2-v_0^2}{2a}$ |
| $v_0,\ v,\ t$ | $\Delta x$ | $\Delta x = \dfrac{v_0+v}{2}\cdot t$（由 ① 和 ② 推导） |

#### 3.5 🧪 推导：三大匀加速公式的相互推导

三大公式并非独立，而是可以从匀加速的定义出发，逐次推导出来。

> **出发点**：加速度恒定 $a = \text{constant}$，且 $a = \dfrac{dv}{dt}$（微积分定义）。

##### 从定义推导公式 ①（速度-时间关系）

由加速度定义 $a = \dfrac{dv}{dt}$，对时间积分：

$$
\int_{v_0}^{v} dv = \int_{0}^{t} a\ dt = a \int_{0}^{t} dt
$$

$$
v - v_0 = at \quad\Rightarrow\quad \boxed{v = v_0 + at}
$$

✅ 这就是公式 ①。

##### 从公式 ① 推导公式 ②（位置-时间关系）

由速度定义 $v = \dfrac{dx}{dt}$，代入公式 ①：

$$
\frac{dx}{dt} = v_0 + at
$$

对时间积分：

$$
\int_{x_0}^{x} dx = \int_{0}^{t} (v_0 + at)\ dt
$$

$$
x - x_0 = v_0 t + \frac{1}{2}at^2 \quad\Rightarrow\quad \boxed{\Delta x = v_0 t + \frac{1}{2}at^2}
$$

✅ 这就是公式 ②。

##### 从公式 ① 和 ② 推导公式 ③（速度-位移关系）

由公式 ① 解出 $t = \dfrac{v - v_0}{a}$，代入公式 ②：

$$
\Delta x = v_0\left(\frac{v - v_0}{a}\right) + \frac{1}{2}a\left(\frac{v - v_0}{a}\right)^2
$$

$$
\Delta x = \frac{v_0(v - v_0)}{a} + \frac{(v - v_0)^2}{2a}
$$

通分：

$$
\Delta x = \frac{2v_0(v - v_0) + (v - v_0)^2}{2a} = \frac{(v - v_0)(2v_0 + v - v_0)}{2a}
$$

$$
\Delta x = \frac{(v - v_0)(v + v_0)}{2a} = \frac{v^2 - v_0^2}{2a}
$$

移项得：

$$
\boxed{v^2 = v_0^2 + 2a\Delta x}
$$

✅ 这就是公式 ③。

> ⭐ **三个公式只需记住任意两个（通常记 ① 和 ②），第三个可以通过代数推导出来！**

#### 3.6 🧪 例题：追及相遇问题

**题目**：一辆轿车以 $20\ \text{m/s}$ 的恒定速度行驶，司机发现前方 $80\ \text{m}$ 处有一辆卡车以 $10\ \text{m/s}$ 的速度同向行驶。轿车司机立即刹车，产生大小为 $2\ \text{m/s}^2$ 的恒定加速度。

(a) 轿车是否会撞上卡车？
(b) 如果会撞上，发生在刹车后多少秒？
(c) 如果不撞，两车最近距离是多少？

**解答**：

设轿车初始位置为 $x=0$，卡车初始位置为 $x=80\ \text{m}$。

轿车：$x_C(t) = 20t - \frac{1}{2} \times 2 \times t^2 = 20t - t^2$（匀减速）
卡车：$x_T(t) = 80 + 10t$（匀速）

**(a)** 两车相撞时位置相等：

$$
20t - t^2 = 80 + 10t
$$

$$
-t^2 + 10t - 80 = 0 \quad\Rightarrow\quad t^2 - 10t + 80 = 0
$$

判别式 $\Delta = 100 - 320 = -220 < 0$，**无实数解** → **不会撞上** ✅

**(b)** 由于无实数解，不会相撞。

**(c)** 两车距离 $d(t) = x_T(t) - x_C(t) = (80 + 10t) - (20t - t^2) = t^2 - 10t + 80$

这是一个开口向上的二次函数，最小值在 $t = -\frac{b}{2a} = \frac{10}{2} = 5\ \text{s}$ 处：

$$
d_{min} = 5^2 - 10 \times 5 + 80 = 25 - 50 + 80 = \mathbf{55\ m}
$$

所以最近距离为 **55 m**，不会相撞。✅

> ⭐ **解题关键**：追及问题列位置相等方程，如果无实数解则不会相撞；最小距离用二次函数求极值或相对速度为零的条件求解。

---

### 四、自由落体运动

#### 4.1 核心要点

> 在 **忽略空气阻力** 的条件下，所有物体在 **同一地点** 以 **相同的重力加速度** $g$ 竖直下落。

- $g \approx 9.8\ \text{m/s}^2$（地表附近，方向竖直向下）
- 自由落体是 **初速度为 0**、**加速度为 $g$ 向下** 的匀加速直线运动

#### 4.2 自由落体公式

设向下为正方向，$v_0 = 0$，$a = g$：

| 公式 | 自由落体形式 |
|:--|:--|
| $v = v_0 + at$ | $v = gt$ |
| $\Delta x = v_0 t + \frac{1}{2}at^2$ | $h = \frac{1}{2}gt^2$ |
| $v^2 = v_0^2 + 2a\Delta x$ | $v^2 = 2gh$ |

#### 4.3 🧪 基础例题

**题目**：从 45 m 高的塔顶释放一个小球（$g = 10\ \text{m/s}^2$）。求：
(a) 落到地面所需时间
(b) 落地时的速度

**解答**：

**(a)** 用 $h = \frac{1}{2}gt^2$：
$$45 = \frac{1}{2} \times 10 \times t^2 \quad\Rightarrow\quad t^2 = 9 \quad\Rightarrow\quad t = \mathbf{3\ s}$$

**(b)** 用 $v = gt$：
$$v = 10 \times 3 = \mathbf{30\ m/s}\ (\text{向下})$$

#### 4.4 🧪 推导：自由落体公式的微积分推导

从牛顿第二定律出发，自由落体只受重力 $F = mg$：

$$
a = \frac{F}{m} = g \quad (\text{方向向下})
$$

设向下为正方向，对加速度积分得速度：

$$
v(t) = \int a\ dt = \int g\ dt = gt + C
$$

代入初始条件 $v(0) = 0$ 得 $C = 0$，所以：

$$
\boxed{v = gt}
$$

对速度积分得位置：

$$
y(t) = \int v(t)\ dt = \int gt\ dt = \frac{1}{2}gt^2 + D
$$

代入初始条件 $y(0) = 0$ 得 $D = 0$，所以：

$$
\boxed{h = \frac{1}{2}gt^2}
$$

从公式 $v^2 = 2gh$ 也可由 $v = gt$ 和 $h = \frac{1}{2}gt^2$ 消去 $t$ 得到：

$$
t = \frac{v}{g} \quad\Rightarrow\quad h = \frac{1}{2}g\left(\frac{v}{g}\right)^2 = \frac{v^2}{2g} \quad\Rightarrow\quad \boxed{v^2 = 2gh}
$$

> 💡 **微积分的优势**：如果重力加速度随高度变化（如 $g(y)$ 非常数），用代数法就无法直接求解，但微积分法仍然适用！

#### 4.5 🧪 例题：竖直上抛运动的完整分析

**题目**：以 $30\ \text{m/s}$ 的初速度竖直向上抛出一小球（$g = 10\ \text{m/s}^2$，忽略空气阻力）。
求：
(a) 到达最高点的时间
(b) 最大高度
(c) 从抛出到落回原处的时间
(d) 落回原处时的速度
(e) 抛出后 $2\ \text{s}$ 和 $5\ \text{s}$ 时的速度和位置

**解答**：

设向上为正方向，$v_0 = +30\ \text{m/s}$，$a = -g = -10\ \text{m/s}^2$。

**(a)** 最高点 $v = 0$：

$$0 = 30 - 10t \quad\Rightarrow\quad t_{up} = \mathbf{3\ s}$$

**(b)** 最大高度：

$$H = v_0 t_{up} - \frac{1}{2}gt_{up}^2 = 30 \times 3 - 5 \times 9 = 90 - 45 = \mathbf{45\ m}$$

**(c)** 落回原处时 $y=0$：

$$0 = 30t - 5t^2 \quad\Rightarrow\quad t(30 - 5t) = 0$$
$$t = 0\ (\text{抛出点}),\quad t = \mathbf{6\ s}\ (\text{落回})$$

> ⭐ 注意 $t_{total} = 2 \times t_{up} = 6\ \text{s}$，即上升时间 = 下降时间（对称性）。

**(d)** 落回原处时的速度：

$$v = v_0 - gt = 30 - 10 \times 6 = -30\ \text{m/s}$$

速度大小为 $30\ \text{m/s}$，方向 **向下**（与初速度相反）。✅

**(e)** $t=2\ \text{s}$（上升阶段）：

$$v(2) = 30 - 20 = 10\ \text{m/s}\ (\text{向上})$$
$$y(2) = 30 \times 2 - 5 \times 4 = 60 - 20 = \mathbf{40\ m}\ (\text{仍在上升})$$

$t=5\ \text{s}$（下降阶段）：

$$v(5) = 30 - 50 = -20\ \text{m/s}\ (\text{向下})$$
$$y(5) = 30 \times 5 - 5 \times 25 = 150 - 125 = \mathbf{25\ m}\ (\text{已过最高点，正在下落})$$

> ⚠️ **AP 常见错误**：$t=5\ \text{s}$ 时小球已经在下降了！很多学生以为 $t=5\ \text{s}$ 还在上升。

---

## Part B：AP 难度层（概念陷阱 + 深度理解）

---

### 五、AP 考试真正的概念陷阱

#### 🎯 陷阱 1：平均速度 vs 平均速率——数值可以差很多

**AP 经典题**：

> A particle moves along a line with velocity $v(t) = 3t^2 - 12t + 9$ m/s for $0 \leq t \leq 4$ s.
> Find the **average speed** and **average velocity** over $[0, 4]$.

**关键**：要先判断物体是否改变了方向！令 $v(t)=0$：
$$3t^2 - 12t + 9 = 0 \quad\Rightarrow\quad t^2 - 4t + 3 = 0 \quad\Rightarrow\quad (t-1)(t-3)=0$$
在 $t=1$ 和 $t=3$ 时方向改变。

然后分段算路径长度（需要积分），再除以总时间。

> ⚠️ **AP 1 不考积分求路径**（那是 AP C 的内容），但会给你分段常数速度让你手算！

#### 🎯 陷阱 2：加速度为负 = 减速？——❌ 大错特错！

**AP 最爱考的概念题**：

> An object moves along the $x$-axis with velocity $v_x = -10\ \text{m/s}$ and acceleration $a_x = -2\ \text{m/s}^2$.
> Is the object speeding up or slowing down?

**分析**：
- $v_x = -10$（向左运动）
- $a_x = -2$（加速度也向左）
- 速度与加速度 **同向**（都是负的）

**答案**：**Speeding up** ✅

> ⭐ **核心理解**：
> - **$\vec{v}$ 与 $\vec{a}$ 同向** → **加速**（无论正负）
> - **$\vec{v}$ 与 $\vec{a}$ 反向** → **减速**
>
> "加速度为负" 只表示方向与正方向相反，**不代表减速**！

#### 🎯 陷阱 3：自由落体中的质量迷思

**AP 经典错误概念**：

> ❌ "重的物体下落更快。"

**正确答案**：在忽略空气阻力时，**所有物体** 无论质量大小，都以相同的加速度 $g$ 下落。

**伽利略比萨斜塔实验**（传说）与现代验证：
- 在真空中，羽毛和铁球同时落地 ✅
- 在地球表面，空气阻力会影响轻质物体，但 **重力加速度本身与质量无关**

> 💡 **AP 考试提示**：如果题目说"忽略空气阻力"，那么所有物体的下落加速度都是 $g$，与质量无关！

#### 🎯 陷阱 4：刹车问题——别忘了检查停止时间！⚠️

**AP 经典坑题**：

> A car is traveling at $20\ \text{m/s}$ when the driver applies brakes, causing a constant deceleration of $4\ \text{m/s}^2$.
> How far does the car travel before stopping?

**错误做法**：直接用公式 ② 代入 $t=5$ s，算 $\Delta x$……

等等！$t=5$ s 是怎么来的？用 $v = v_0 + at$：
$$0 = 20 - 4t \quad\Rightarrow\quad t = 5\ \text{s}$$

这个 **5 s 就是停止时间**，正确代入公式 ③：
$$v^2 = v_0^2 + 2a\Delta x \quad\Rightarrow\quad 0 = 20^2 + 2(-4)\Delta x$$
$$\Delta x = \frac{400}{8} = \mathbf{50\ m}$$

**但**——如果题目问的是 **$t = 7$ s 时的位移** 呢？

> ⚠️ **AP 超级陷阱**：车在 $t=5$ s 时就停了！$t=7$ s 时车已经停了 2 秒，位移 **还是 50 m**，不是用 $t=7$ 代入公式算出来的值！
>
> **必检步骤**：刹车问题一定先算 **停止时间** $t_{stop} = \dfrac{v_0}{|a|}$！

#### 🎯 陷阱 5：上抛运动——最高点 v=0，但 a≠0！

**AP Physics 1 必考概念**：

> A ball is thrown straight upward. At the highest point of its motion:
>
> A) Both velocity and acceleration are zero.
> B) Velocity is zero, acceleration is zero.
> C) **Velocity is zero, acceleration is $g$ downward.**
> D) Velocity is maximum, acceleration is zero.

**答案**：C ✅

> ⭐ **关键理解**：
> - 最高点：$v = 0$（瞬间静止）
> - 最高点：$a = g$ 向下 **≠ 0**（重力始终存在！）
>
> AP 考试超爱考这个！千万别选 B！

---

### 六、AP Physics C 的微积分深度

#### 6.1 从代数到微积分的完整框架

**微分（由位置到速度到加速度）**

$$
\vec{r}(t) \xrightarrow{\ \dfrac{d}{dt}\ } \vec{v}(t) = \frac{d\vec{r}}{dt} \xrightarrow{\ \dfrac{d}{dt}\ } \vec{a}(t) = \frac{d\vec{v}}{dt} = \frac{d^2\vec{r}}{dt^2}
$$

**积分（由加速度到速度到位置）**

$$
\vec{a}(t) \xrightarrow{\ \displaystyle\int dt\ } \vec{v}(t) = \vec{v}_0 + \int_{0}^{t} \vec{a}(\tau)\ d\tau \xrightarrow{\ \displaystyle\int dt\ } \vec{r}(t) = \vec{r}_0 + \int_{0}^{t} \vec{v}(\tau)\ d\tau
$$

#### 6.2 匀加速是微积分框架的特例

当 $\vec{a} = \text{constant}$：

$$
\vec{v}(t) = \vec{v}_0 + \int_0^t \vec{a}\ d\tau = \vec{v}_0 + \vec{a}t
$$

$$
\vec{r}(t) = \vec{r}_0 + \int_0^t (\vec{v}_0 + \vec{a}\tau)\ d\tau = \vec{r}_0 + \vec{v}_0 t + \frac{1}{2}\vec{a}t^2
$$

**看！三大公式中的前两个就是从微积分积分得到的！** ✅

#### 6.3 🧪 AP Physics C 真题难度示例

> The acceleration of a particle moving along the $x$-axis is given by $a(t) = 6t - 4\ \text{m/s}^2$.
> At $t = 0$, the particle is at $x = 2\ \text{m}$ with velocity $v = 3\ \text{m/s}$.
>
> **(a)** Find the velocity function $v(t)$.
> **(b)** Find the position function $x(t)$.
> **(c)** Find the velocity at $t = 2$ s.
> **(d)** Find the displacement from $t = 0$ to $t = 3$ s.

**解答**：

**(a)** 对加速度积分：

$$
v(t) = \int a(t)\ dt = \int (6t - 4)\ dt = 3t^2 - 4t + C
$$

代入 $v(0) = 3$：
$$3 = 0 - 0 + C \quad\Rightarrow\quad C = 3$$

$$
\boxed{v(t) = 3t^2 - 4t + 3\ \text{m/s}}
$$

**(b)** 对速度积分：

$$
x(t) = \int v(t)\ dt = \int (3t^2 - 4t + 3)\ dt = t^3 - 2t^2 + 3t + D
$$

代入 $x(0) = 2$：
$$2 = 0 - 0 + 0 + D \quad\Rightarrow\quad D = 2$$

$$
\boxed{x(t) = t^3 - 2t^2 + 3t + 2\ \text{m}}
$$

**(c)** 代入 $t=2$：

$$
v(2) = 3(4) - 4(2) + 3 = 12 - 8 + 3 = \mathbf{7\ m/s}
$$

**(d)** 位移 $\Delta x = x(3) - x(0)$：

$$
x(3) = 27 - 18 + 9 + 2 = 20
$$
$$
x(0) = 2
$$
$$
\Delta x = 20 - 2 = \mathbf{18\ m}
$$

#### 6.4 变力与牛顿第二定律的连接（AP C 进阶）

AP Physics C 中，常将加速度与力联系起来：

$$
\vec{F}_{net} = m\vec{a} = m\frac{d\vec{v}}{dt} = m\frac{d^2\vec{r}}{dt^2}
$$

当力随时间变化时：

$$
\vec{F}(t) = m\vec{a}(t) \quad\Rightarrow\quad \vec{a}(t) = \frac{\vec{F}(t)}{m}
$$

然后通过积分求速度和位置：

$$
\vec{v}(t) = \vec{v}_0 + \int_0^t \frac{\vec{F}(\tau)}{m}\ d\tau
$$

$$
\vec{r}(t) = \vec{r}_0 + \int_0^t \vec{v}(\tau)\ d\tau
$$

#### 6.5 点积判断加速/减速（AP C 二维运动）

在二维运动中，判断 speeding up 还是 slowing down，用 **速度与加速度的点积**：

$$
\vec{v} \cdot \vec{a} \; \begin{cases}
> 0 & \text{加速 (speeding up)} \\
< 0 & \text{减速 (slowing down)} \\
= 0 & \text{速率不变 (如匀速圆周运动)}
\end{cases}
$$

> 这是 1.1 中提到的点积判断法的 **实际应用场景**！

---

### 七、AP 考试难度分级总结

| 层次 | 对应考试 | 核心要求 | 典型题特征 |
|:--|:--|:--|:--|
| **Level 1：公式应用** | 学校期中 | 记忆三大公式，直接代入计算 | 已知 $v_0, a, t$ 求 $v$ 或 $\Delta x$ |
| **Level 2：概念辨析** | **AP Physics 1 & 2** 🎯 | 区分平均 vs 瞬时、加速 vs 减速、刹车检查、最高点分析 | 上抛最高点 v=0 但 a≠0、刹车停止时间、加速度正负不等于加减速 |
| **Level 3：微积分应用** | **AP Physics C** 🎯 | 对 $a(t)$ 积分求 $v(t)$，再积分求 $x(t)$；反向求导 | $a(t)=6t-4$ 给初值积分求 $x(t)$；从 $x(t)$ 求导得到 $v(t)$ 和 $a(t)$ |

---

### 八、AP 级别综合练习

#### 🟢 AP Physics 1 风格

> A ball is thrown **downward** from a cliff with initial speed $5\ \text{m/s}$.
> The cliff is $60\ \text{m}$ high. ($g = 10\ \text{m/s}^2$)
>
> (a) How long does it take to reach the ground?
> (b) What is the velocity just before hitting the ground?
> (c) How far does it fall in the last second of its motion?

**解答思路**：

设向下为正方向，$v_0 = +5\ \text{m/s}$，$a = +g = 10\ \text{m/s}^2$，$\Delta y = 60\ \text{m}$

**(a)** 用 $\Delta y = v_0 t + \frac{1}{2}gt^2$：
$$60 = 5t + 5t^2 \quad\Rightarrow\quad t^2 + t - 12 = 0$$
$$(t+4)(t-3)=0 \quad\Rightarrow\quad t = \mathbf{3\ s} \quad (t=-4\ \text{舍去})$$

**(b)** 用 $v = v_0 + gt$：
$$v = 5 + 10(3) = \mathbf{35\ m/s}\ (\text{向下})$$

**(c)** "最后 1 秒" = 从 $t=2$ s 到 $t=3$ s：
- $y(2) = 5(2) + \frac{1}{2}(10)(4) = 10 + 20 = 30\ \text{m}$
- $y(3) = 60\ \text{m}$（地面）
- 最后 1 秒下落距离 $= 60 - 30 = \mathbf{30\ m}$ ✅

> ⚠️ **AP 陷阱**：不要直接用 $v_0=5$ 套公式算 1 秒的位移——那是初速度为 5 的前 1 秒，不是最后 1 秒！

#### 🔵 AP Physics C 风格

> A particle moves along the $x$-axis with acceleration $a(t) = 12t^2 - 6\ \text{m/s}^2$.
> At $t = 0$, $x = 1\ \text{m}$ and $v = -4\ \text{m/s}$.
>
> (a) Find $v(t)$ and $x(t)$.
> (b) At what time(s) does the particle come to rest?
> (c) Find the displacement from $t = 0$ to $t = 2$ s.
> (d) Find the total distance traveled from $t = 0$ to $t = 2$ s.

**解答**：

**(a)** 对 $a(t)$ 积分求 $v(t)$：

$$
v(t) = \int (12t^2 - 6)\ dt = 4t^3 - 6t + C
$$

代入 $v(0) = -4$：
$$-4 = 0 - 0 + C \quad\Rightarrow\quad C = -4$$

$$
\boxed{v(t) = 4t^3 - 6t - 4\ \text{m/s}}
$$

对 $v(t)$ 积分求 $x(t)$：

$$
x(t) = \int (4t^3 - 6t - 4)\ dt = t^4 - 3t^2 - 4t + D
$$

代入 $x(0) = 1$：
$$1 = 0 - 0 - 0 + D \quad\Rightarrow\quad D = 1$$

$$
\boxed{x(t) = t^4 - 3t^2 - 4t + 1\ \text{m}}
$$

**(b)** "Come to rest" 即 $v(t) = 0$：

$$4t^3 - 6t - 4 = 0 \quad\Rightarrow\quad 2t^3 - 3t - 2 = 0$$

试 $t=...$ 可以用计算器求根，$t \approx 1.46$ s（只有一个实数解，因为 $4t^3 - 6t - 4$ 是增函数）

**(c)** 位移 $\Delta x = x(2) - x(0)$：

$$
x(2) = 16 - 12 - 8 + 1 = -3
$$
$$
x(0) = 1
$$
$$
\Delta x = -3 - 1 = \mathbf{-4\ m}
$$

**(d)** 总距离需要分两段（$t \approx 1.46$ 为折返点）：

从 $t=0$ 到 $t=1.46$（向左运动）：$\Delta x_1 = x(1.46) - x(0) \approx -6.69 - 1 = -7.69$，距离 $d_1 = 7.69$ m

从 $t=1.46$ 到 $t=2$（向右运动）：$\Delta x_2 = x(2) - x(1.46) \approx -3 - (-6.69) = 3.69$，距离 $d_2 = 3.69$ m

总距离 $d = 7.69 + 3.69 \approx \mathbf{11.38\ m}$ ✅

> ⭐ **AP C 评分重点**：只要思路正确——找到折返点、分区间计算——即使数值是近似值也能拿大部分分数！

---

### 九、本节 AP 考点频率统计

| 考点 | AP 1 频率 | AP C 频率 | 说明 |
|:--|:--:|:--:|:--|
| 平均速度公式 | ⭐⭐⭐⭐ | ⭐⭐⭐ | 基础计算 |
| 匀加速三大公式 | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | AP 1 核心工具 |
| 自由落体/上抛运动 | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | AP 1 必考情境 |
| 刹车停止时间检查 | ⭐⭐⭐⭐ | ⭐⭐⭐ | 陷阱高频点 |
| 最高点 $v=0,\ a\neq0$ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | 概念必考题 |
| $a$ 正负与加减速关系 | ⭐⭐⭐⭐ | ⭐⭐⭐ | 概念辨析 |
| 对 $a(t)$ 积分求 $v(t), x(t)$ | — | ⭐⭐⭐⭐⭐ | AP C 核心技能 |
| 从 $x(t)$ 求导求 $v(t), a(t)$ | — | ⭐⭐⭐⭐⭐ | AP C 核心技能 |
| 带折返的路径长度计算 | — | ⭐⭐⭐⭐ | FRQ 必考 |
| 变力连接 $F=ma$ 积分 | — | ⭐⭐⭐⭐ | AP C 综合题 |

---
---

# 1.3 运动学图像分析（Kinematics Graph Analysis）

---

## Part A：基础层（AP Physics 1 & 2 必备）

---

### 一、位置-时间图（x-t 图）

#### 1.3.1 核心要点

> **x-t 图上某点的斜率 = 该时刻的瞬时速度**

$$
\boxed{v(t) = \text{slope of } x(t) \text{ at time } t = \frac{dx}{dt}}
$$

#### 1.3.2 各种形状的含义

| x-t 图特征 | 对应的运动 | 速度情况 |
|:--|:--|:--|
| ✅ 直线（斜率为正） | 匀速向右运动 | $v$ = 正常数 |
| ✅ 直线（斜率为负） | 匀速向左运动 | $v$ = 负常数 |
| ✅ 直线（斜率为零/水平） | 静止 | $v = 0$ |
| 🔼 曲线向上弯曲（上凸） | 加速运动 | $v$ 在增大 |
| 🔽 曲线向下弯曲（下凹） | 减速运动 | $v$ 在减小 |
| 🔄 抛物线形状 | 匀加速/匀减速直线运动 | $v$ 线性变化 |

#### 1.3.3 🧪 基础示例：读取速度

```
x (m)
↑
6 ┤        ╱
5 ┤      ╱
4 ┤    ╱
3 ┤  ╱
2 ┤╱
1 ┤
0 ┼──────────────────→ t (s)
   0  1  2  3  4  5
```

这是一条过原点的直线，斜率 $= \frac{6-0}{3-0} = 2\ \text{m/s}$

所以物体以 **$2\ \text{m/s}$ 的恒定速度** 向右运动。

#### 1.3.4 平均速度在 x-t 图上的几何意义

$$
\bar{v} = \frac{\Delta x}{\Delta t} = \text{连接起点和终点的割线斜率}
$$

- 瞬时速度 $v(t)$ = 曲线上该点 **切线** 的斜率
- 平均速度 $\bar{v}$ = 曲线上起点到终点 **割线** 的斜率

> 💡 **两者区别**：割线看整体，切线看瞬间。

---

### 二、速度-时间图（v-t 图）

#### 2.1 核心要点

v-t 图是 **AP 物理最重要的图像**，因为它包含两种信息：

$$
\boxed{\text{斜率} = \text{加速度} \quad\quad \text{面积} = \text{位移}}
$$

##### 斜率 ⇒ 加速度

$$
a(t) = \text{slope of } v(t) \text{ at time } t = \frac{dv}{dt}
$$

##### 面积 ⇒ 位移

$$
\Delta x = \text{area under } v(t) \text{ curve} = \int_{t_i}^{t_f} v(t)\ dt
$$

> ⚠️ **注意**：
> - 曲线在 $t$ 轴上方的面积 → **正位移**（向右）
> - 曲线在 $t$ 轴下方的面积 → **负位移**（向左）
> - **总位移** = 上方总面积 − 下方总面积
> - **总路程** = 上方总面积 + 下方总面积（都取绝对值）

#### 2.2 各种形状的含义

| v-t 图特征 | 对应的运动 | 加速度情况 |
|:--|:--|:--|
| ✅ 水平线（$v \neq 0$） | 匀速直线运动 | $a = 0$ |
| ✅ 水平线（$v = 0$） | 静止 | $a = 0$ |
| ✅ 斜线（斜率正） | 匀加速运动 | $a$ = 正常数 |
| ✅ 斜线（斜率负） | 匀减速运动 | $a$ = 负常数 |
| 🔼 曲线向上弯曲 | 加速度在增大 | $a$ 在增加 |
| 🔽 曲线向下弯曲 | 加速度在减小 | $a$ 在减小 |

#### 2.3 🧪 基础示例

```
v (m/s)
↑
6 ┤        ╱
5 ┤      ╱
4 ┤    ╱
3 ┤  ╱
2 ┤╱
1 ┤
0 ┼──────────────────→ t (s)
   0  1  2  3  4  5
```

- **斜率** $= \frac{6-0}{3-0} = 2\ \text{m/s}^2$ → 加速度为 $2\ \text{m/s}^2$
- **面积**（三角形）$= \frac{1}{2} \times 3 \times 6 = 9\ \text{m}$ → 位移为 $9\ \text{m}$

---

### 三、加速度-时间图（a-t 图）

#### 3.1 核心要点

$$
\boxed{\text{面积} = \text{速度变化量}}
$$

$$
\Delta v = \text{area under } a(t) \text{ curve} = \int_{t_i}^{t_f} a(t)\ dt
$$

#### 3.2 各种形状的含义

| a-t 图特征 | 对应的运动 | 速度情况 |
|:--|:--|:--|
| ✅ 水平线（$a \neq 0$） | 匀加速/匀减速 | $v$ 线性变化 |
| ✅ 水平线（$a = 0$） | 匀速或静止 | $v$ 不变 |
| 🔼 斜线 | 加速度均匀变化 | $v$ 呈二次变化 |

#### 3.3 🧪 基础示例

```
a (m/s²)
↑
3 ┤╱╱╱╱╱╱╱╱╱
2 ┤╱╱╱╱╱╱╱╱╱
1 ┤╱╱╱╱╱╱╱╱╱
0 ┼──────────────────→ t (s)
   0  1  2  3  4  5
```

从 $t=0$ 到 $t=4$ s 的 **面积** $= 3 \times 4 = 12$ → 速度变化量 $\Delta v = 12\ \text{m/s}$

如果 $v_0 = 0$，则 $v(4) = 12\ \text{m/s}$

---

### 四、三类图像之间的相互转换

#### 4.1 转换关系总图

```
  x-t 图
    │
    │ 求导（斜率）
    ▼
  v-t 图 ──── 求导（斜率）────▶ a-t 图
    │                            │
    │ 积分（面积）                │ 积分（面积）
    ▼                            ▼
  Δx (位移)                    Δv (速度变化量)
```

#### 4.2 已知 x-t 图 → 画 v-t 图

| 步骤 | 操作 |
|:--|:--|
| **1** | 在 x-t 图上选关键点（转折点、拐点） |
| **2** | 求各段 **斜率**（即速度） |
| **3** | 将斜率值画到 v-t 图上对应时间区间 |

**🧪 示例**：

```
x-t:                      v-t:
x ↑                       v ↑
  |     ╱╲                  |    ╱╲
  |   ╱   ╲    ╱            |  ╱   ╲    ╱
  | ╱      ╲  ╱             |╱      ╲  ╱
  |╱        ╲╱              |        ╲╱
  └───────→ t               └─────────→ t
```

- x-t 斜率从正逐渐减小到 0 → v-t 从正减小到 0
- x-t 斜率变负且绝对值增大 → v-t 负向增大

#### 4.3 已知 v-t 图 → 画 a-t 图

| 步骤 | 操作 |
|:--|:--|
| **1** | 在 v-t 图上求各段 **斜率**（即加速度） |
| **2** | 将斜率值画到 a-t 图上 |

#### 4.4 已知 v-t 图 → 画 x-t 图

| 步骤 | 操作 |
|:--|:--|
| **1** | 选起点位置 $x_0$ |
| **2** | 计算 v-t 图中各段 **面积**（即位移） |
| **3** | 累积位移画到 x-t 图上 |

#### 4.5 🧪 综合转换示例

**题目**：已知某物体的 v-t 图如下，画出对应的 a-t 图和 x-t 图（设 $x_0 = 0$）。

```
v (m/s)
↑
4 ┤        ╱╲
3 ┤      ╱   ╲
2 ┤    ╱      ╲
1 ┤  ╱         ╲
0 ┼╱────────────╲──→ t (s)
   0  1  2  3  4  5
```

**解答**：

**a-t 图**：v-t 斜率为常数（各段直线）⇒ a 为分段常数

- $0 \leq t \leq 2$：斜率 $= \frac{4-0}{2-0} = 2$ ⇒ $a = 2\ \text{m/s}^2$
- $2 \leq t \leq 4$：斜率 $= \frac{0-4}{4-2} = -2$ ⇒ $a = -2\ \text{m/s}^2$
- $t > 4$：斜率 $= 0$ ⇒ $a = 0$

```
a (m/s²)
↑
2 ┤╱╱╱╱╱╱╱╱
1 ┤╱╱╱╱╱╱╱╱
0 ┼──────────────╱╱╱╱╱╱──→ t (s)
  │        ╱╱╱╱
-1┤      ╱╱╱╱
-2┤    ╱╱╱╱
   0  1  2  3  4  5
```

**x-t 图**：计算 v-t 下方面积（累积位移）

- $t=2$：面积 $= \frac{1}{2} \times 2 \times 4 = 4$ m
- $t=4$：面积 $= 4 + \frac{1}{2} \times 2 \times 4 = 8$ m
- $t=5$：面积 $= 8 + 0 = 8$ m（之后静止）

```
x (m)
↑
8 ┤              ═══
6 ┤          ╱
4 ┤      ╱
2 ┤  ╱
0 ┼──────────────────→ t (s)
   0  1  2  3  4  5
```

#### 4.6 🧪 推导：v-t 图面积等于位移的数学证明

**核心思想**：将时间轴分成无数个极短的时间段 $\Delta t_i$，在每个 $\Delta t_i$ 内，速度近似不变（匀速运动），那么位移 $\Delta x_i \approx v(t_i) \Delta t_i$。

当 $\Delta t_i \to 0$ 时，近似变为精确：

$$
\Delta x = \lim_{\Delta t_i \to 0} \sum_i v(t_i) \Delta t_i = \int_{t_i}^{t_f} v(t)\ dt
$$

这正是 **黎曼和 → 定积分** 的过程：

```
v(t)
↑
│    ╱╲
│  ╱   ╲     每个小矩形面积 ≈ v(tᵢ)·Δtᵢ
│╱      ╲    总面积 → 位移
└─────────→ t
  Δtᵢ
```

**几何意义**：v-t 曲线与 $t$ 轴围成的面积等于位移。

> 💡 **类比**：就像用许多小矩形逼近曲线下的面积，当矩形宽度趋近于 0 时，总面积就等于定积分。

#### 4.7 🧪 例题：根据文字描述画运动图像

**题目**：一个物体沿 $x$ 轴运动，其运动过程如下：
- $0 \to 2\ \text{s}$：从原点出发，以 $3\ \text{m/s}$ 匀速向右运动
- $2 \to 4\ \text{s}$：以 $-2\ \text{m/s}^2$ 的加速度匀减速
- $4 \to 6\ \text{s}$：反向以 $1\ \text{m/s}$ 匀速向左运动

画出 (a) x-t 图 (b) v-t 图 (c) a-t 图。

**解答**：

**第一步：写出分段函数**

$x$ 轴正方向向右。

$0 \to 2\ \text{s}$：匀速，$v = 3\ \text{m/s}$，$x(t) = 3t$

$2 \to 4\ \text{s}$：匀减速，$v_0 = 3\ \text{m/s}$，$a = -2\ \text{m/s}^2$
- $v(t) = 3 - 2(t-2) = 7 - 2t$
- $x(2) = 6\ \text{m}$，$x(t) = 6 + 3(t-2) - (t-2)^2$

$4 \to 6\ \text{s}$：匀速向左，$v = -1\ \text{m/s}$，$x(4) = 6 + 3(2) - 4 = 8\ \text{m}$
- $x(t) = 8 - (t-4)$

**第二步：画 v-t 图**

```
v (m/s)
↑
3 ┤══════╲
2 ┤       ╲
1 ┤        ╲
0 ┼─────────╲─────────→ t (s)
  │          ╲
-1┤           ══════
   0  1  2  3  4  5  6
```

- $0 \to 2$：水平线 $v=3$
- $2 \to 4$：斜线，$v$ 从 $3$ 降到 $-1$
- $4 \to 6$：水平线 $v=-1$

**第三步：画 a-t 图**

```
a (m/s²)
↑
1 ┤
0 ┼────────┬───────────→ t (s)
  │        │
-1┤        │
-2┤        ═══════
   0  1  2  3  4  5  6
```

- $0 \to 2$：$a = 0$
- $2 \to 4$：$a = -2\ \text{m/s}^2$
- $4 \to 6$：$a = 0$

**第四步：画 x-t 图**

```
x (m)
↑
8 ┤            ═══
6 ┤      ╱╲
4 ┤    ╱    ╲
2 ┤  ╱        ╲
0 ┼╱──────────────→ t (s)
   0  1  2  3  4  5  6
```

- $0 \to 2$：斜率为 $3$ 的直线
- $2 \to 4$：开口向下的抛物线（斜率逐渐减小到负值）
- $4 \to 6$：斜率为 $-1$ 的直线，位置从 $8\ \text{m}$ 降到 $6\ \text{m}$

> ⭐ **关键能力**：能够从文字描述反推出运动图像，这是 AP Physics 1 图像题的进阶技能！

---

## Part B：AP 难度层（概念陷阱 + 深度理解）

---

### 五、AP 考试真正的概念陷阱

#### 🎯 陷阱 1：v-t 图的面积是位移，不是路程！

> 很多学生知道"面积 = 位移"，但 AP 会问路程——这时要取绝对值！

**🧪 经典题**：

```
v (m/s)
↑
3 ┤╱╱╱╱╱╱╱
2 ┤╱╱╱╱╱╱╱
1 ┤╱╱╱╱╱╱╱
0 ┼─────────────→ t (s)
  │ ╲╱╲╱
-1┤   ╲╱ ╲╱
-2┤     ╲  ╲
   0  1  2  3  4
```

**问**：从 $t=0$ 到 $t=4$ 的 (a) 位移 (b) 路程？

- 位移 $= \text{正面积} - \text{负面积} = \frac{1}{2}\times 3 \times 3 - \frac{1}{2} \times 1 \times 1 = 4.5 - 0.5 = \mathbf{4\ m}$
- 路程 $= \text{正面积} + \text{负面积的绝对值} = 4.5 + 0.5 = \mathbf{5\ m}$

> ⚠️ **AP 陷阱**：题目问 "total distance traveled" 就是路程！问 "displacement" 才是位移！

#### 🎯 陷阱 2：x-t 图的斜率是速度，但曲线弯曲方向代表什么？

| x-t 曲线形状 | 含义 |
|:--|:--|
| 上凸（cup up） | $v$ 在增大（加速） |
| 下凹（cup down） | $v$ 在减小（减速） |

但这只是 **一阶信息**。AP C 会进一步问 **二阶信息**：

- 上凸 ⇒ $v$ 增加 ⇒ $a > 0$
- 下凹 ⇒ $v$ 减小 ⇒ $a < 0$

> 💡 这是通过 **二阶导数** 判断的：x-t 上凸时 $\frac{d^2x}{dt^2} = a > 0$！

#### 🎯 陷阱 3：x-t 图的斜率是速度——但切线和割线要分清！

**AP 必考选择题**：

```
x (m)
↑
  |      ╱
  |    ╱
  |  ╱
  |╱
  └─────────→ t (s)
```

> Which of the following correctly describes the motion?
>
> A) Velocity is constant.
> B) Velocity is increasing.
> C) **Velocity is decreasing.** ✅
> D) Acceleration is zero.

**解析**：x-t 曲线的斜率（切线）随 $t$ 增大而减小 ⇒ 速度在减小 ⇒ 正确答案是 C。

> ⭐ **AP 考点**：不是问曲线本身，而是问 **曲线斜率的变化**！

#### 🎯 陷阱 4：a-t 图的面积是 $\Delta v$，不是 $v$！

**AP 经典错误**：

> 学生看到 a-t 图的面积，直接说"这就是速度"。

**正确答案**：
$$v(t) = v_0 + \text{area under } a(t) \text{ from } 0 \text{ to } t$$

> ⚠️ 面积给出的是 **速度变化量 $\Delta v$**，要加上初速度 $v_0$ 才得到 $v(t)$！

#### 🎯 陷阱 5：图像转换中的"拐点"识别

AP 考试经常给一张图，让你画另一张图——**拐点对应关系** 是关键！

| 原始图 | 特征点 | 转换到目标图 |
|:--|:--|:--|
| x-t 拐点（斜率变化） | v-t 的转折点 |
| x-t 水平切线（$v=0$） | v-t 与 $t$ 轴交点 |
| v-t 拐点（斜率变化） | a-t 的转折点 |
| v-t 与 $t$ 轴交点（$v=0$） | 物体改变方向的位置 |
| v-t 极值点（斜率为 0） | a-t 与 $t$ 轴交点（$a=0$） |

#### 🎯 陷阱 6：AP 经典——哪个图不能表示同一运动？

**AP Physics 1 真题风格**：

> Which of the following sets of graphs could **NOT** represent the motion of the same object?

这种题考的是 **图像之间的一致性**：

- 如果 x-t 是抛物线向上开口 ⇒ v-t 应该是斜率为正的直线 ⇒ a-t 应该是正常数的水平线
- 如果 v-t 是水平线 ⇒ a-t 应该是 0 的水平线，x-t 应该是斜线

> ⚠️ **AP 陷阱**：选项中常常有一组图看起来差不多，但斜率/面积关系对不上！

---

### 六、AP Physics C 的微积分深度

#### 6.1 微积分基本定理在运动学中的统一

AP Physics C 要求你真正理解 **斜率 = 导数，面积 = 积分** 的本质：

##### 微分视角（斜率）

$$
v(t) = \frac{dx}{dt} \quad\longleftrightarrow\quad \text{x-t 图切线斜率}
$$

$$
a(t) = \frac{dv}{dt} = \frac{d^2x}{dt^2} \quad\longleftrightarrow\quad \text{v-t 图切线斜率}
$$

##### 积分视角（面积）

$$
\Delta x = \int_{t_i}^{t_f} v(t)\ dt \quad\longleftrightarrow\quad \text{v-t 曲线下面积}
$$

$$
\Delta v = \int_{t_i}^{t_f} a(t)\ dt \quad\longleftrightarrow\quad \text{a-t 曲线下面积}
$$

#### 6.2 微积分基本定理的运动学表述

$$
\boxed{\frac{d}{dt} \int_{a}^{t} f(\tau)\ d\tau = f(t)}
$$

在运动学中：

$$
\frac{d}{dt} \left[ \int_{0}^{t} v(\tau)\ d\tau \right] = v(t)
$$

这意味着：**面积函数的导数 = 原始函数**——这就是图像转换的数学本质！

#### 6.3 🧪 AP Physics C 真题难度示例

> The velocity of a particle moving along the $x$-axis is given by $v(t) = 3t^2 - 12t + 9$ m/s for $t \geq 0$.
>
> **(a)** Find the acceleration function $a(t)$.
> **(b)** At what time(s) does the particle change direction?
> **(c)** Find the displacement from $t = 0$ to $t = 4$ s.
> **(d)** Find the total distance traveled from $t = 0$ to $t = 4$ s.
> **(e)** Sketch $v(t)$ and $a(t)$ on the same axes for $0 \leq t \leq 4$.

**解答**：

**(a)** 求导：

$$
a(t) = \frac{dv}{dt} = 6t - 12\ \text{m/s}^2
$$

**(b)** 改变方向时 $v(t) = 0$：

$$3t^2 - 12t + 9 = 0 \quad\Rightarrow\quad t^2 - 4t + 3 = 0$$
$$(t-1)(t-3) = 0 \quad\Rightarrow\quad t = \mathbf{1\ s, \ 3\ s}$$

**(c)** 位移 = v-t 曲线下的净面积（积分）：

$$
\Delta x = \int_{0}^{4} (3t^2 - 12t + 9)\ dt
$$

$$
= \left[ t^3 - 6t^2 + 9t \right]_{0}^{4}
$$

$$
= (64 - 96 + 36) - (0) = \mathbf{4\ m}
$$

**(d)** 总路程需要分三段（$0 \to 1$，$1 \to 3$，$3 \to 4$），每段取绝对值：

**区间 [$0$, $1$]：$v \geq 0$**

$$
d_1 = \int_{0}^{1} (3t^2 - 12t + 9)\ dt = \left[ t^3 - 6t^2 + 9t \right]_{0}^{1} = 1 - 6 + 9 = 4\ \text{m}
$$

**区间 [$1$, $3$]：$v \leq 0$**

$$
d_2 = \left| \int_{1}^{3} (3t^2 - 12t + 9)\ dt \right| = \left| \left[ t^3 - 6t^2 + 9t \right]_{1}^{3} \right|
$$

$$
= |(27 - 54 + 27) - (1 - 6 + 9)| = |0 - 4| = 4\ \text{m}
$$

**区间 [$3$, $4$]：$v \geq 0$**

$$
d_3 = \int_{3}^{4} (3t^2 - 12t + 9)\ dt = \left[ t^3 - 6t^2 + 9t \right]_{3}^{4}
$$

$$
= (64 - 96 + 36) - (27 - 54 + 27) = 4 - 0 = 4\ \text{m}
$$

**总路程**：

$$
d = d_1 + d_2 + d_3 = 4 + 4 + 4 = \mathbf{12\ m}
$$

> ⭐ **AP C 核心考点**：位移和路程的区别——位移是积分的代数和，路程是绝对值之和！

**(e)** 图像草图：

```
v, a
↑
9 ┤ v(t) = 3t² - 12t + 9
  │  ╱
6 ┤ ╱    a(t) = 6t - 12
  │╱
3 ┤╱
0 ┼─────┬──────┬──────→ t
  │  1  │  3   │  4
-3┤     │      │
  │     │      │
-6┤     │      │
```

- $v(t)$ 是开口向上的抛物线，在 $t=2$ 处有最小值 $v(2) = -3$ m/s
- $a(t)$ 是斜率为正的直线，在 $t=2$ 时 $a=0$
- 当 $t < 2$ 时 $a < 0$（减速），$t > 2$ 时 $a > 0$（加速）

#### 6.4 高阶应用：从 x-t 图分析加速度方向（AP C）

AP C 会要求你从 x-t 图的 **曲率（二阶导数）** 直接判断加速度方向：

| x-t 曲线 | 一阶导 $v$ | 二阶导 $a$ | 运动状态 |
|:--|:--:|:--:|:--|
| 向上弯曲（上凸） | $v > 0$ | $a > 0$ | 正向加速 |
| 向上弯曲（上凸） | $v < 0$ | $a > 0$ | 负向减速 |
| 向下弯曲（下凹） | $v > 0$ | $a < 0$ | 正向减速 |
| 向下弯曲（下凹） | $v < 0$ | $a < 0$ | 负向加速 |

> 💡 **记忆方法**：上凸 = 加速度为正（像微笑 😊），下凹 = 加速度为负（像皱眉 😞）

---

### 七、AP 考试难度分级总结

| 层次 | 对应考试 | 核心要求 | 典型题特征 |
|:--|:--|:--|:--|
| **Level 1：读数计算** | 学校期中 | 从 x-t 图读斜率求速度；从 v-t 图读斜率求加速度、面积求位移 | "求 $t=2$ 时的速度" |
| **Level 2：图像转换** | **AP Physics 1 & 2** 🎯 | x-t → v-t → a-t 相互转换；判断哪组图不能表示同一运动 | "Which set could NOT represent the same motion?" |
| **Level 3：微积分分析** | **AP Physics C** 🎯 | 用积分精确求面积、用导数求斜率；从 $v(t)$ 函数求总路程（分段积分） | $v(t)=3t^2-12t+9$ 求总路程 |

---

### 八、AP 级别综合练习

#### 🟢 AP Physics 1 风格

> The velocity-time graph of an object moving along the $x$-axis is shown below.

```
v (m/s)
↑
4 ┤    ╱╲
3 ┤  ╱   ╲
2 ┤╱      ╲
1 ┤         ╲
0 ┼───────────╲──→ t (s)
  │            ╲
-1┤             ╲
-2┤              ╲
   0  1  2  3  4  5
```

> (a) What is the acceleration during the first 2 seconds?
> (b) What is the displacement from $t=0$ to $t=4$ s?
> (c) What is the total distance traveled from $t=0$ to $t=4$ s?
> (d) At what time is the object farthest from its starting point?

**解答**：

**(a)** $0 \to 2$ s：斜率 $= \frac{4-0}{2-0} = \mathbf{2\ m/s^2}$ ✅

**(b)** 位移 = v-t 净面积：

- $0 \to 2$：三角形面积 $= \frac{1}{2} \times 2 \times 4 = 4$ m
- $2 \to 3$：三角形面积 $= \frac{1}{2} \times 1 \times 4 = 2$ m（正）
- $3 \to 4$：三角形面积 $= \frac{1}{2} \times 1 \times (-2) = -1$ m（负）

净位移 $= 4 + 2 + (-1) = \mathbf{5\ m}$ ✅

**(c)** 总路程 $= 4 + 2 + 1 = \mathbf{7\ m}$ ✅

**(d)** 物体在 $t=3$ s 时 $v=0$（方向改变），此时离起点最远：$x(3) = 4 + 2 = \mathbf{6\ m}$ ✅

#### 🔵 AP Physics C 风格

> A particle moves along the $x$-axis with acceleration $a(t) = 4t - 6\ \text{m/s}^2$.
> At $t = 0$, $x = 0$ and $v = 8\ \text{m/s}$.
>
> (a) Find $v(t)$ and $x(t)$.
> (b) At what time(s) is the particle at rest?
> (c) Find the displacement and total distance for $0 \leq t \leq 4$.
> (d) Sketch $v(t)$ and indicate on the graph the area that represents displacement.

**解答**：

**(a)** 积分求 $v(t)$：

$$
v(t) = \int (4t - 6)\ dt = 2t^2 - 6t + C
$$

代入 $v(0) = 8$：

$$
8 = 0 - 0 + C \quad\Rightarrow\quad C = 8
$$

$$
\boxed{v(t) = 2t^2 - 6t + 8\ \text{m/s}}
$$

再积分求 $x(t)$：

$$
x(t) = \int (2t^2 - 6t + 8)\ dt = \frac{2}{3}t^3 - 3t^2 + 8t + D
$$

代入 $x(0) = 0$：

$$
0 = 0 + D \quad\Rightarrow\quad D = 0
$$

$$
\boxed{x(t) = \frac{2}{3}t^3 - 3t^2 + 8t\ \text{m}}
$$

**(b)** At rest 即 $v(t) = 0$：

$$2t^2 - 6t + 8 = 0 \quad\Rightarrow\quad t^2 - 3t + 4 = 0$$

判别式 $\Delta = 9 - 16 = -7 < 0$，**无实数解**！

这意味着粒子 **从未停下来**——速度始终为正。✅

**(c)** 位移 $\Delta x = x(4) - x(0)$：

$$
x(4) = \frac{2}{3}(64) - 3(16) + 8(4) = \frac{128}{3} - 48 + 32 = \frac{80}{3} \approx 26.67\ \text{m}
$$

$$
\Delta x = \frac{80}{3} - 0 = \mathbf{\frac{80}{3}\ \text{m} \approx 26.67\ \text{m}}
$$

因为 $v(t) > 0$ 对所有 $t \geq 0$ 成立（判别式 < 0，且开口向上），粒子从不折返，所以 **总路程 = 位移**：

$$
\text{总路程} = \mathbf{\frac{80}{3}\ \text{m} \approx 26.67\ \text{m}}
$$

**(d)** 图像：

```
v (m/s)
↑
8 ┤╱
  │ ╲
6 ┤   ╲
  │     ╲
4 ┤       ╲
  │         ╲
2 ┤           ╲
  │             ╲
0 ┼───────────────╲──→ t (s)
  │                ╲
   0  1  2  3  4  5
```

$v(t) = 2t^2 - 6t + 8$ 是开口向上的抛物线。曲线下全部在 $t$ 轴上方 ⇒ 位移 = 路程。

> ⭐ **AP C 重要判断**：$v(t)$ 是否恒正？看判别式 + 开口方向 + $v(0)$！

---

### 九、本节 AP 考点频率统计

| 考点 | AP 1 频率 | AP C 频率 | 说明 |
|:--|:--:|:--:|:--|
| x-t 图读斜率求速度 | ⭐⭐⭐⭐ | ⭐⭐⭐ | 基础技能 |
| v-t 图读斜率求加速度 | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | 基础技能 |
| v-t 图面积求位移 | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | AP 1 核心技能 |
| v-t 图面积求路程（取绝对值） | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | 陷阱高频点 |
| a-t 图面积求 $\Delta v$ | ⭐⭐⭐ | ⭐⭐⭐⭐ | 需加初速度 |
| 图像转换（x-t ↔ v-t ↔ a-t） | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | AP 1 选择/FRQ 常考 |
| "Which set cannot represent same motion" | ⭐⭐⭐⭐ | ⭐⭐⭐ | AP 1 选择题经典 |
| 从 $v(t)$ 函数求总路程（分段积分） | — | ⭐⭐⭐⭐⭐ | AP C FRQ 必考 |
| 二阶导数判断加速度方向 | — | ⭐⭐⭐⭐ | 从 x-t 曲率直接判断 |
| 判别式判断 $v(t)$ 是否恒正 | — | ⭐⭐⭐ | AP C 解题技巧 |

---
---

# 1.4 参考系与相对运动（Reference Frames & Relative Motion）

---

## Part A：基础层（AP Physics 1 & 2 必备）

---

### 一、什么是参考系

#### 1.4.1 核心概念

> **参考系（Reference Frame）** 是用于描述物体位置和运动的 **坐标系 + 时间度量**。

同一物体的运动，在不同的参考系中观测，结果可能 **完全不同**！

**经典例子**：

| 场景 | 地面参考系观察 | 火车参考系观察 |
|:--|:--|:--|
| 静止在火车上的人 | 以 $v_{train}$ 向前运动 | **静止** |
| 在火车上向前走的人 | 以 $v_{train} + v_{walk}$ 向前运动 | 以 $v_{walk}$ 向前运动 |
| 从火车上丢下的球 | **抛物线** 运动 | **自由落体**（竖直下落） |

> 💡 **核心思想**：运动是 **相对的**，没有绝对静止的参考系。

#### 1.4.2 惯性参考系 vs 非惯性参考系

| 类型 | 定义 | 特点 |
|:--|:--|:--|
| **惯性参考系（Inertial Frame）** | 牛顿定律成立的参考系（静止或匀速直线运动） | 无需虚拟力 |
| **非惯性参考系（Non-inertial Frame）** | 加速运动的参考系 | 需引入虚拟力（如离心力、科里奥利力） |

> ⚠️ **AP Physics 1 只考惯性参考系之间的转换**。非惯性参考系是 AP Physics C 的内容。

---

### 二、相对速度的基本概念

#### 1.4.3 符号约定

为了清晰描述相对运动，我们使用下标约定：

| 符号 | 含义 | 读法 |
|:--|:--|:--|
| $\vec{v}_{A/B}$ | A **相对于** B 的速度 | "A with respect to B" |
| $\vec{v}_{A/G}$ | A 相对于地面的速度 | "A relative to Ground" |

#### 1.4.4 相对速度的矢量加法 —— 核心公式

$$
\boxed{\vec{v}_{A/C} = \vec{v}_{A/B} + \vec{v}_{B/C}}
$$

> **中文解读**：A 相对于 C 的速度 = A 相对于 B 的速度 + B 相对于 C 的速度。

**重要推论**：

$$
\boxed{\vec{v}_{A/B} = -\vec{v}_{B/A}}
$$

> A 相对于 B 的速度，与 B 相对于 A 的速度，大小相等、方向相反。

#### 1.4.5 🧪 基础示例

**题目**：小明以 $2\ \text{m/s}$ 的速度在火车上向东走，火车以 $10\ \text{m/s}$ 的速度向东行驶。求小明相对于地面的速度。

**解答**：

设向东为正方向：

$$
v_{\text{小明/地面}} = v_{\text{小明/火车}} + v_{\text{火车/地面}} = 2 + 10 = \mathbf{12\ m/s\ (向东)}
$$

---

### 三、一维相对运动

#### 1.4.6 沿同一方向

当两个物体沿同一直线运动时，相对速度是 **代数差**：

$$
\boxed{v_{A/B} = v_A - v_B}
$$

（这里 $v_A$ 和 $v_B$ 都是带正负号的代数数值）

| 场景 | $v_A$ | $v_B$ | $v_{A/B}$ | 解释 |
|:--|:--:|:--:|:--:|:--|
| 同向，A 更快 | $+10$ | $+6$ | $+4$ | A 相对于 B 以 4 向前靠近 |
| 同向，B 更快 | $+6$ | $+10$ | $-4$ | A 相对于 B 以 4 向后远离 |
| 相向而行 | $+10$ | $-6$ | $+16$ | A 相对于 B 以 16 快速靠近 |
| 背向而行 | $-10$ | $+6$ | $-16$ | A 相对于 B 以 16 快速远离 |

#### 1.4.7 🧪 一维相对运动例题

**题目**：一辆轿车以 $25\ \text{m/s}$ 向东行驶，一辆卡车以 $15\ \text{m/s}$ 向西行驶。求轿车相对于卡车的速度。

**解答**：

设向东为正方向：

- 轿车：$v_{car} = +25\ \text{m/s}$
- 卡车：$v_{truck} = -15\ \text{m/s}$

$$
v_{car/truck} = v_{car} - v_{truck} = (+25) - (-15) = \mathbf{+40\ m/s\ (向东)}
$$

> 💡 **直观理解**：从卡车司机的角度看，轿车以 $40\ \text{m/s}$ 的速度向东冲过来！

---

### 四、二维相对运动

#### 1.4.8 矢量加法在二维中的应用

当两个物体的运动方向不在同一直线上时，需要用 **矢量加法**（平行四边形法则或分量法）来求相对速度。

$$
\boxed{\vec{v}_{A/C} = \vec{v}_{A/B} + \vec{v}_{B/C}}
$$

这个公式对二维同样成立，只是现在是 **矢量加法**。

#### 1.4.9 解题步骤

| 步骤 | 操作 |
|:--|:--|
| **1** | 确定所有已知速度（大小和方向） |
| **2** | 写出矢量关系式 $\vec{v}_{A/C} = \vec{v}_{A/B} + \vec{v}_{B/C}$ |
| **3** | 将各矢量分解为 $x$ 和 $y$ 分量 |
| **4** | 分别对各分量进行代数加法 |
| **5** | 合成得到结果矢量的大小和方向 |

#### 1.4.10 🧪 经典二维相对运动：横渡河流

**题目**：一艘船在静水中的速度为 $4\ \text{m/s}$（船头指向对岸），河水流速为 $3\ \text{m/s}$ 向东。河宽 $200\ \text{m}$。求：

(a) 船相对于河岸的速度（大小和方向）
(b) 船到达对岸所需时间
(c) 船在下游多远处靠岸

**解答**：

设 $y$ 正方向为垂直河岸指向对岸，$x$ 正方向为下游。

**(a)** 船相对于水的速度：$\vec{v}_{B/W} = 4\ \hat{j}\ \text{m/s}$
水相对于岸的速度：$\vec{v}_{W/G} = 3\ \hat{i}\ \text{m/s}$

$$
\vec{v}_{B/G} = \vec{v}_{B/W} + \vec{v}_{W/G} = 4\hat{j} + 3\hat{i} = 3\hat{i} + 4\hat{j}\ \text{m/s}
$$

**大小**：

$$
|\vec{v}_{B/G}| = \sqrt{3^2 + 4^2} = \mathbf{5\ m/s}
$$

**方向**（与下游方向的夹角）：

$$
\theta = \tan^{-1}\left(\frac{4}{3}\right) \approx \mathbf{53^\circ}\ \text{（指向上游方向的对岸）}
$$

**(b)** 渡河时间只取决于 **垂直河岸方向的分速度**：

$$
t = \frac{\text{河宽}}{v_y} = \frac{200}{4} = \mathbf{50\ s}
$$

**(c)** 下游漂移距离：

$$
\Delta x = v_x \times t = 3 \times 50 = \mathbf{150\ m\ (下游)}
$$

> ⭐ **核心结论**：渡河时间只由 **垂直河岸的分速度** 决定，与水流速度无关！

#### 1.4.11 🧪 推导：伽利略变换的加速度不变性证明

**伽利略变换的核心**：两个以恒定速度相对运动的惯性系中，**加速度保持不变**。

**数学证明**：

设 $S'$ 系相对于 $S$ 系以恒定速度 $\vec{V}$ 运动，两系原点在 $t=0$ 时重合。

**位置变换**：

$$
\vec{r}'(t) = \vec{r}(t) - \vec{V}t
$$

**速度变换**（对时间求导）：

$$
\vec{v}'(t) = \frac{d\vec{r}'}{dt} = \frac{d\vec{r}}{dt} - \vec{V} = \vec{v}(t) - \vec{V}
$$

**加速度变换**（再次求导）：

$$
\vec{a}'(t) = \frac{d\vec{v}'}{dt} = \frac{d\vec{v}}{dt} - \frac{d\vec{V}}{dt} = \vec{a}(t) - 0 = \vec{a}(t)
$$

因为 $\vec{V}$ 是常量，所以 $\dfrac{d\vec{V}}{dt} = 0$。✅

> ⭐ **重要推论**：既然 $\vec{a}' = \vec{a}$，且质量 $m$ 在经典力学中不变，那么 $\vec{F} = m\vec{a}$ 在所有惯性系中形式相同——这就是 **伽利略相对性原理**！

#### 1.4.12 🧪 例题：多参考系复合问题

**题目**：一列火车以 $20\ \text{m/s}$ 向东行驶。火车上一个人以 $2\ \text{m/s}$ 的速度（相对于火车）向东行走。此时地面上另一个人以 $5\ \text{m/s}$ 的速度向东骑自行车。求：

(a) 火车上的人相对于地面的速度
(b) 火车上的人相对于骑自行车人的速度
(c) 骑自行车人相对于火车上的人的速度

**解答**：

设向东为正方向。

**(a)** 已知 $v_{person/train} = +2\ \text{m/s}$，$v_{train/ground} = +20\ \text{m/s}$

$$
v_{person/ground} = v_{person/train} + v_{train/ground} = 2 + 20 = \mathbf{+22\ \text{m/s}\ (向东)}
$$

**(b)** 求 $v_{person/bike}$：

已知 $v_{bike/ground} = +5\ \text{m/s}$

$$
v_{person/bike} = v_{person/ground} - v_{bike/ground} = 22 - 5 = \mathbf{+17\ \text{m/s}\ (向东)}
$$

或者用链式法则：

$$
v_{person/bike} = v_{person/train} + v_{train/ground} + v_{ground/bike}
$$

注意 $v_{ground/bike} = -v_{bike/ground} = -5\ \text{m/s}$：

$$
v_{person/bike} = 2 + 20 + (-5) = \mathbf{+17\ \text{m/s}\ (向东)}
$$

**(c)** 由对称性：

$$
v_{bike/person} = -v_{person/bike} = \mathbf{-17\ \text{m/s}\ (向西)}
$$

> ⭐ **链式法则技巧**：相对速度的链式加法可以串联任意多个中间参考系：
>
> $$
> \vec{v}_{A/Z} = \vec{v}_{A/B} + \vec{v}_{B/C} + \vec{v}_{C/D} + \cdots + \vec{v}_{Y/Z}
> $$
>
> 只要保证相邻下标"首尾相连"即可！

---

## Part B：AP 难度层（概念陷阱 + 深度理解）

---

### 五、AP 考试真正的概念陷阱

#### 🎯 陷阱 1：参考系转换时忘记加矢量

**AP 经典错误**：

> ❌ 直接用代数加法，忽略了方向。

**✅ 正确做法**：相对速度公式是 **矢量公式**，必须注意方向！

**🧪 示例**：

> A boat heading north at $5\ \text{m/s}$ in still water crosses a river flowing east at $3\ \text{m/s}$.

**错误答案**：$5 + 3 = 8\ \text{m/s}$ ❌

**正确答案**：$\sqrt{5^2 + 3^2} = \sqrt{34} \approx 5.83\ \text{m/s}$，方向为 **北偏东 $31^\circ$** ✅

#### 🎯 陷阱 2：渡河问题——最短路径 vs 最短时间

AP 考试常考两种不同的渡河策略！

| 策略 | 条件 | 船头指向 | 结果 |
|:--|:--|:--|:--|
| **最短时间** | 船头直接指向对岸 | 垂直河岸 | 时间最短，但会漂到下游 |
| **最短路径** | 船头朝向上游某角度 | 抵消水流 | 垂直过河，不漂移，但时间更长 |

**🧪 例题**：

> 河宽 $120\ \text{m}$，水流 $4\ \text{m/s}$ 向东，船在静水中速度 $5\ \text{m/s}$。
>
> (a) 最短渡河时间是多少？
> (b) 最短路径（不漂移）渡河，船头应指向什么方向？

**解答 (a)**：

船头垂直指向对岸，$v_y = 5\ \text{m/s}$

$$
t_{min} = \frac{120}{5} = \mathbf{24\ s}
$$

**解答 (b)**：

要垂直过河（不漂移），船头需朝向上游某角度 $\theta$，使得 $x$ 方向分速度抵消水流：

$$
v_{B/W}\sin\theta = v_{water} \quad\Rightarrow\quad 5\sin\theta = 4
$$

$$
\sin\theta = \frac{4}{5} = 0.8 \quad\Rightarrow\quad \theta = \sin^{-1}(0.8) \approx \mathbf{53^\circ}\ \text{（指向上游）}
$$

此时垂直河岸的分速度：

$$
v_y = 5\cos\theta = 5 \times 0.6 = 3\ \text{m/s}
$$

渡河时间：

$$
t = \frac{120}{3} = \mathbf{40\ s}
$$

> ⚠️ **AP 陷阱**：最短时间（24 s）≠ 最短路径（40 s），题目一定要看清楚问的是哪种！

#### 🎯 陷阱 3：雨中走路/跑步问题

**经典 AP 情境**：

> 雨滴竖直下落。一个人是走路快还是跑步快，淋到的雨更少？

**分析**：

- 从 **地面参考系** 看：雨竖直下落，人水平运动
- 从 **人的参考系** 看：雨相对于人不仅有竖直向下的速度，还有 **水平方向的速度**（大小等于人的速度，方向相反）

> ⭐ **AP 结论**：跑得越快，单位时间淋到的雨 **越少**（但跑的路程更短，总淋雨量也更少）。

#### 🎯 陷阱 4：风对飞机的影响——与渡河问题同构

**AP Physics 1 常考题**：

> 飞机的空速（相对于空气的速度）为 $200\ \text{km/h}$ 向北。风从西向东以 $50\ \text{km/h}$ 吹。
>
> (a) 飞机相对于地面的速度？
> (b) 若飞机要向北飞行，机头应指向什么方向？

**解答 (a)**：

$$
\vec{v}_{P/G} = \vec{v}_{P/A} + \vec{v}_{A/G} = 200\hat{j} + 50\hat{i}
$$

大小：$\sqrt{200^2 + 50^2} \approx 206\ \text{km/h}$
方向：北偏东 $\tan^{-1}(50/200) \approx 14^\circ$

**解答 (b)**：

要向北飞（相对于地面），机头需指向西偏某角度 $\theta$，抵消侧风：

$$
200\sin\theta = 50 \quad\Rightarrow\quad \sin\theta = 0.25 \quad\Rightarrow\quad \theta \approx 14.5^\circ\ \text{（西偏北）}
$$

向北的分速度：$200\cos\theta \approx 200 \times 0.968 \approx 193.6\ \text{km/h}$

> ⚠️ 注意：这是 **渡河问题的完全同构**——空气 = 水，飞机 = 船！

---

### 六、AP Physics C 的微积分深度

#### 6.1 不同参考系下的位置、速度、加速度变换

##### 位置变换（伽利略变换）

假设参考系 $S'$ 相对于参考系 $S$ 以速度 $\vec{V}$ 匀速运动，且 $t=0$ 时两坐标系原点重合：

$$
\boxed{\vec{r}' (t) = \vec{r}(t) - \vec{V}t}
$$

##### 速度变换（伽利略速度变换）

对时间求导：

$$
\boxed{\vec{v}' = \vec{v} - \vec{V}}
$$

这就是我们之前用的相对速度公式！其中 $\vec{v}'$ 是在 $S'$ 系中测得的速度，$\vec{v}$ 是在 $S$ 系中测得的速度。

##### 加速度变换

再对时间求导：

$$
\boxed{\vec{a}' = \vec{a} - \vec{A}}
$$

其中 $\vec{A}$ 是 $S'$ 系相对于 $S$ 系的加速度。

> ⭐ **关键结论**：
> - 如果 $S'$ 系 **匀速运动**（$\vec{A}=0$），则 $\vec{a}' = \vec{a}$ —— **加速度在所有惯性系中相同**！
> - 如果 $S'$ 系 **加速运动**（$\vec{A} \neq 0$），则 $\vec{a}' \neq \vec{a}$ —— 此时需引入虚拟力。

#### 6.2 🧪 AP C 真题风格例题

> Reference frame $S'$ moves with velocity $\vec{V} = 5\hat{i}\ \text{m/s}$ relative to frame $S$.
> A particle's position in frame $S$ is given by $\vec{r}(t) = (3t^2 - 2t)\hat{i} + (4t)\hat{j}$ meters.
>
> (a) Find the particle's velocity $\vec{v}(t)$ in frame $S$.
> (b) Find the particle's velocity $\vec{v}'(t)$ in frame $S'$.
> (c) Find the acceleration in both frames. Are they the same?

**解答**：

**(a)** 在 $S$ 系中求导：

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (6t - 2)\hat{i} + 4\hat{j}\ \text{m/s}
$$

**(b)** 用伽利略速度变换：

$$
\vec{v}'(t) = \vec{v}(t) - \vec{V} = (6t - 2)\hat{i} + 4\hat{j} - 5\hat{i}
$$

$$
\boxed{\vec{v}'(t) = (6t - 7)\hat{i} + 4\hat{j}\ \text{m/s}}
$$

**(c)** 在 $S$ 系中：

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = 6\hat{i}\ \text{m/s}^2
$$

在 $S'$ 系中：

$$
\vec{a}'(t) = \frac{d\vec{v}'}{dt} = 6\hat{i}\ \text{m/s}^2
$$

**它们相同！** ✅ 因为 $S'$ 相对于 $S$ 匀速运动（$\vec{A}=0$），加速度不变。

> ⭐ **AP C 考点**：伽利略变换下，加速度在 **所有惯性系中都是不变的**。这就是为什么牛顿第二定律 $\vec{F}=m\vec{a}$ 在所有惯性系中形式相同！

#### 6.3 匀加速参考系的变换（AP C 进阶）

如果 $S'$ 系相对于 $S$ 系以 **恒定加速度** $\vec{A}$ 运动：

$$
\vec{v}' (t) = \vec{v}(t) - \vec{V}_0 - \vec{A}t
$$

$$
\vec{a}' = \vec{a} - \vec{A}
$$

在这种情况下，牛顿第二定律在 $S'$ 系中的形式变为：

$$
\vec{F} = m\vec{a} = m(\vec{a}' + \vec{A}) \quad\Rightarrow\quad \vec{F} - m\vec{A} = m\vec{a}'
$$

其中 $-m\vec{A}$ 就是 **虚拟力（惯性力）**。

---

### 七、AP 考试难度分级总结

| 层次 | 对应考试 | 核心要求 | 典型题特征 |
|:--|:--|:--|:--|
| **Level 1：基础应用** | 学校期中 | 会用 $\vec{v}_{A/C} = \vec{v}_{A/B} + \vec{v}_{B/C}$ 求一维相对速度 | 人车同行、相向而行等简单场景 |
| **Level 2：二维相对运动** | **AP Physics 1 & 2** 🎯 | 渡河问题（最短时间 vs 最短路径）、飞机侧风问题、雨中运动 | "船头指向对岸 vs 垂直过河"，"风对飞机航线的影响" |
| **Level 3：微积分变换** | **AP Physics C** 🎯 | 伽利略变换 $\vec{r}' = \vec{r} - \vec{V}t$；加速参考系与虚拟力 | 在不同惯性系间变换速度、加速度；在非惯性系中引入 $-m\vec{A}$ |

---

### 八、AP 级别综合练习

#### 🟢 AP Physics 1 风格

> A river flows east at $2\ \text{m/s}$. A swimmer can swim at $1.5\ \text{m/s}$ in still water.
>
> (a) If the swimmer heads directly north (perpendicular to the current), what is her velocity relative to the shore?
> (b) How long will it take her to cross a river that is $60\ \text{m}$ wide?
> (c) How far downstream will she land?
> (d) At what angle should she swim to land directly across from her starting point?

**解答**：

设北为 $+y$，东为 $+x$。

**(a)**

$$
\vec{v}_{S/G} = \vec{v}_{S/W} + \vec{v}_{W/G} = 1.5\hat{j} + 2\hat{i}
$$

大小：$|\vec{v}_{S/G}| = \sqrt{1.5^2 + 2^2} = \sqrt{2.25 + 4} = \sqrt{6.25} = \mathbf{2.5\ m/s}$

方向：北偏东 $\theta = \tan^{-1}\left(\frac{2}{1.5}\right) \approx \mathbf{53^\circ}$ ✅

**(b)** 渡河时间只由垂直河岸的分速度决定：

$$
t = \frac{60}{1.5} = \mathbf{40\ s} ✅
$$

**(c)** 下游漂移：

$$
\Delta x = v_x \times t = 2 \times 40 = \mathbf{80\ m} ✅
$$

**(d)** 要垂直过河（不漂移），需将速度分解：

游泳者 $\vec{v}_{S/W}$ 的 $x$ 分量抵消水流：

$$
1.5\sin\theta = 2 \quad\Rightarrow\quad \sin\theta = \frac{2}{1.5} = \frac{4}{3} > 1
$$

**不可能！** ❌

因为静水速度 $1.5\ \text{m/s}$ 小于水流速度 $2\ \text{m/s}$，无法完全抵消水流！

> ⭐ **AP 陷阱**：当船速（或泳速）小于水流速度时，**无法垂直过河**！

#### 🔵 AP Physics C 风格

> Reference frame $S'$ moves with velocity $\vec{V}(t) = (2t)\hat{i}\ \text{m/s}$ relative to frame $S$.
> A particle's position in frame $S$ is $\vec{r}(t) = (t^3 - 6t)\hat{i} + (4t^2)\hat{j}$ meters.
>
> (a) Find the velocity $\vec{v}(t)$ and acceleration $\vec{a}(t)$ in frame $S$.
> (b) Find the velocity $\vec{v}'(t)$ and acceleration $\vec{a}'(t)$ in frame $S'$.
> (c) Is $S'$ an inertial frame? Explain.
> (d) If a force $\vec{F} = m\vec{a}$ acts on the particle in frame $S$, what additional term is needed to describe the motion in frame $S'$?

**解答**：

**(a)** 在 $S$ 系中：

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (3t^2 - 6)\hat{i} + 8t\hat{j}\ \text{m/s}
$$

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = 6t\hat{i} + 8\hat{j}\ \text{m/s}^2
$$

**(b)** 伽利略速度变换：

$$
\vec{v}'(t) = \vec{v}(t) - \vec{V}(t) = (3t^2 - 6)\hat{i} + 8t\hat{j} - (2t)\hat{i}
$$

$$
\boxed{\vec{v}'(t) = (3t^2 - 2t - 6)\hat{i} + 8t\hat{j}\ \text{m/s}}
$$

对 $t$ 求导得到加速度：

$$
\vec{a}'(t) = \frac{d\vec{v}'}{dt} = (6t - 2)\hat{i} + 8\hat{j}\ \text{m/s}^2
$$

**(c)** $S'$ 不是惯性帧，因为 $\vec{V}(t)$ 不是常数（$\vec{V}(t) = 2t\hat{i}$ 随时间变化）。

$S'$ 的加速度：$\vec{A} = \frac{d\vec{V}}{dt} = 2\hat{i}\ \text{m/s}^2$

验证 $\vec{a}' \neq \vec{a}$：

$$
\vec{a} - \vec{a}' = (6t\hat{i} + 8\hat{j}) - ((6t-2)\hat{i} + 8\hat{j}) = 2\hat{i} = \vec{A} ✅
$$

**(d)** 在非惯性系 $S'$ 中，需要引入虚拟力：

$$
\vec{F}_{fict} = -m\vec{A} = -m(2\hat{i}) = -2m\hat{i}\ \text{N}
$$

所以在 $S'$ 系中，牛顿第二定律的形式为：

$$
\vec{F} + \vec{F}_{fict} = m\vec{a}' \quad\Rightarrow\quad \vec{F} - 2m\hat{i} = m\vec{a}'
$$

> ⭐ **AP C 考点**：非惯性系中必须引入 **惯性力** $-m\vec{A}$，牛顿第二定律才能继续使用！

---

### 九、本节 AP 考点频率统计

| 考点 | AP 1 频率 | AP C 频率 | 说明 |
|:--|:--:|:--:|:--|
| 一维相对速度计算 | ⭐⭐⭐⭐ | ⭐⭐⭐ | 基础技能，代数减法 |
| 二维相对速度矢量合成 | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | 渡河问题、飞机侧风 |
| 渡河最短时间 vs 最短路径 | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | AP 1 FRQ 高频 |
| 船速 < 水流速度的特殊情况 | ⭐⭐⭐ | ⭐⭐ | 概念陷阱 |
| 伽利略变换 $\vec{r}' = \vec{r} - \vec{V}t$ | — | ⭐⭐⭐⭐⭐ | AP C 核心 |
| 加速度在不同惯性系中不变 | — | ⭐⭐⭐⭐ | 证明惯性系等价性 |
| 非惯性系与虚拟力 $-m\vec{A}$ | — | ⭐⭐⭐⭐ | AP C 进阶考点 |

---
---

# 1.5 二维运动（抛体运动）（Two-Dimensional Motion & Projectile Motion）

---

## Part A：基础层（AP Physics 1 & 2 必备）

---

### 一、抛体运动的核心思想——运动的独立性

#### 1.5.1 核心原则

> 抛体运动可以分解为两个 **互相独立** 的一维运动：

$$
\boxed{\text{抛体运动} = \text{水平匀速直线运动} + \text{竖直匀加速运动}}
$$

| 方向 | 加速度 | 速度变化 | 运动类型 |
|:--|:--:|:--|:--|
| **水平（$x$）** | $a_x = 0$ | $v_x$ 恒定不变 | 匀速直线运动 |
| **竖直（$y$）** | $a_y = -g$ | $v_y$ 线性变化 | 匀加速（自由落体） |

> 💡 **伽利略的洞见**：水平运动和竖直运动 **互不干扰**，可以独立分析再合成！

#### 1.5.2 矢量分解——抛出速度

将初速度 $\vec{v}_0$ 分解为水平和竖直分量（设 $\theta$ 为与水平方向的夹角）：
```
    ↑ v₀
    |↗
  v₀y |/ θ
    |/→ v₀x
    └──────→
```


$$
\boxed{v_{0x} = v_0 \cos\theta \quad\quad v_{0y} = v_0 \sin\theta}
$$

---

### 二、平抛运动（水平抛出）

#### 1.5.3 初始条件

物体从高度 $h$ 处以水平初速度 $v_0$ 抛出：

- $v_{0x} = v_0$，$v_{0y} = 0$
- $a_x = 0$，$a_y = -g$
- 设抛出点为原点：$x_0 = 0$，$y_0 = h$

#### 1.5.4 运动方程

| 方向 | 位置方程 | 速度方程 |
|:--|:--|:--|
| **水平** | $x(t) = v_0 t$ | $v_x(t) = v_0$ |
| **竖直** | $y(t) = h - \dfrac{1}{2}gt^2$ | $v_y(t) = -gt$ |

#### 1.5.5 🧪 基础例题

**题目**：从 $80\ \text{m}$ 高的楼顶水平抛出一小球，初速度为 $20\ \text{m/s}$（$g = 10\ \text{m/s}^2$）。
求：(a) 落地时间 (b) 水平射程 (c) 落地时的速度

**解答**：

**(a)** 落地时 $y=0$：

$$0 = 80 - \frac{1}{2} \times 10 \times t^2 \quad\Rightarrow\quad 5t^2 = 80 \quad\Rightarrow\quad t = \mathbf{4\ s}$$

**(b)** 水平射程：

$$x = v_0 t = 20 \times 4 = \mathbf{80\ m}$$

**(c)** 落地时速度分量：

- $v_x = 20\ \text{m/s}$
- $v_y = -gt = -10 \times 4 = -40\ \text{m/s}$

大小：$v = \sqrt{20^2 + 40^2} = \sqrt{2000} \approx 44.7\ \text{m/s}$

方向：与水平方向夹角 $\phi = \tan^{-1}\left(\dfrac{40}{20}\right) \approx 63.4^\circ$ 向下

---

### 三、斜抛运动（以一定角度抛出）

#### 1.5.6 初始条件

物体以初速度 $v_0$、抛射角 $\theta$（与水平夹角）从地面抛出：

- $v_{0x} = v_0\cos\theta$，$v_{0y} = v_0\sin\theta$
- $a_x = 0$，$a_y = -g$
- 设抛出点为原点：$x_0 = 0$，$y_0 = 0$

#### 1.5.7 运动方程

| 方向 | 位置方程 | 速度方程 |
|:--|:--|:--|
| **水平** | $x(t) = (v_0\cos\theta) t$ | $v_x(t) = v_0\cos\theta$ |
| **竖直** | $y(t) = (v_0\sin\theta) t - \dfrac{1}{2}gt^2$ | $v_y(t) = v_0\sin\theta - gt$ |

#### 1.5.8 🧪 基础例题

**题目**：以 $30\ \text{m/s}$ 的初速度、$30^\circ$ 的抛射角斜抛一个小球（$g = 10\ \text{m/s}^2$）。
求：(a) 飞行时间 (b) 水平射程 (c) 最大高度

**解答**：

$v_{0x} = 30\cos30^\circ = 30 \times \frac{\sqrt{3}}{2} \approx 25.98\ \text{m/s}$
$v_{0y} = 30\sin30^\circ = 30 \times \frac{1}{2} = 15\ \text{m/s}$

**(a)** 飞行时间（落地时 $y=0$）：

$$0 = 15t - \frac{1}{2} \times 10 \times t^2 \quad\Rightarrow\quad t(15 - 5t) = 0$$
$$t = 0\ \text{（抛出点）},\quad t = \mathbf{3\ s}$$

**(b)** 水平射程：

$$R = v_{0x} \times t = 25.98 \times 3 \approx \mathbf{77.94\ m}$$

**(c)** 最大高度（最高点时 $v_y = 0$）：

$$0 = 15 - 10t \quad\Rightarrow\quad t_{top} = 1.5\ \text{s}$$

$$H = v_{0y}t_{top} - \frac{1}{2}gt_{top}^2 = 15 \times 1.5 - 5 \times (1.5)^2 = 22.5 - 11.25 = \mathbf{11.25\ m}$$

---

### 四、抛体运动的关键参数

#### 1.5.9 飞行时间（Time of Flight）

从抛出到落回同一水平面的总时间：

$$
\boxed{T = \frac{2v_0\sin\theta}{g}}
$$

> 推导：令 $y=0$，解 $v_0\sin\theta \cdot t - \frac{1}{2}gt^2 = 0$，除 $t=0$ 外得 $t = \frac{2v_0\sin\theta}{g}$。

#### 1.5.10 水平射程（Range）

$$
\boxed{R = \frac{v_0^2\sin 2\theta}{g}}
$$

> 推导：$R = v_{0x} \times T = (v_0\cos\theta) \times \frac{2v_0\sin\theta}{g} = \frac{v_0^2 \cdot 2\sin\theta\cos\theta}{g} = \frac{v_0^2\sin 2\theta}{g}$。

#### 1.5.11 最大高度（Maximum Height）

$$
\boxed{H = \frac{v_0^2\sin^2\theta}{2g}}
$$

> 推导：最高点 $v_y=0$，$0 = v_0\sin\theta - gt_{top}$，$t_{top} = \frac{v_0\sin\theta}{g}$，代入 $y$ 方程。

#### 1.5.12 重要结论

| 结论 | 说明 |
|:--|:--|
| **最大射程角度** $\theta = 45^\circ$ | $\sin 2\theta$ 在 $2\theta = 90^\circ$ 即 $\theta = 45^\circ$ 时取最大值 1 |
| **互补角度等射程** | $\theta$ 和 $90^\circ - \theta$ 有相同射程（因为 $\sin 2\theta = \sin(180^\circ - 2\theta)$） |
| **最高点速度最小** | 最高点 $v_y=0$，只有水平分量 $v_x = v_0\cos\theta$ |

#### 1.5.13 不同抛射角对比

| 抛射角 $\theta$ | 飞行时间 | 水平射程 | 最大高度 | 轨迹形状 |
|:--:|:--:|:--:|:--:|:--:|
| $15^\circ$ | 短 | 中等 | 低 | 低平抛物线 |
| $30^\circ$ | 中等 | 较大 | 中等 | — |
| $45^\circ$ | 中等 | **最大** | 中等 | 对称抛物线 |
| $60^\circ$ | 中等 | 较大（同 $30^\circ$） | 较高 | — |
| $75^\circ$ | 较长 | 中等（同 $15^\circ$） | 很高 | 高陡抛物线 |

---

### 五、轨迹方程

#### 1.5.14 从参数方程消去时间

参数方程：

$$
x = (v_0\cos\theta) t \quad\Rightarrow\quad t = \frac{x}{v_0\cos\theta}
$$

$$
y = (v_0\sin\theta) t - \frac{1}{2}gt^2
$$

代入 $t$：

$$
\boxed{y = x\tan\theta - \frac{g}{2v_0^2\cos^2\theta} x^2}
$$

#### 1.5.15 轨迹形状分析

$$
y = ax^2 + bx + c \quad\text{其中}\quad a = -\frac{g}{2v_0^2\cos^2\theta} < 0
$$

- $a < 0$ ⇒ **开口向下的抛物线**
- 这是 **二次函数**，形状为抛物线

#### 1.5.16 🧪 推导：$45^\circ$ 最大射程的严格证明

**问题**：在给定初速度 $v_0$ 的情况下，抛射角 $\theta$ 为多少时水平射程 $R$ 最大？

**推导**：

由射程公式：

$$
R(\theta) = \frac{v_0^2 \sin 2\theta}{g}
$$

其中 $v_0$ 和 $g$ 是常数。求 $R$ 对 $\theta$ 的一阶导数：

$$
\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \frac{d}{d\theta}(\sin 2\theta) = \frac{v_0^2}{g} \cdot 2\cos 2\theta
$$

令 $\dfrac{dR}{d\theta} = 0$：

$$
\frac{2v_0^2}{g}\cos 2\theta = 0 \quad\Rightarrow\quad \cos 2\theta = 0
$$

$$
2\theta = \frac{\pi}{2} \quad\Rightarrow\quad \theta = \frac{\pi}{4} = 45^\circ
$$

**验证最大值**（二阶导数法）：

$$
\frac{d^2R}{d\theta^2} = \frac{v_0^2}{g} \cdot (-4\sin 2\theta)
$$

代入 $\theta = 45^\circ$（即 $2\theta = 90^\circ$）：

$$
\frac{d^2R}{d\theta^2}\bigg|_{\theta=45^\circ} = \frac{v_0^2}{g} \cdot (-4\sin 90^\circ) = -\frac{4v_0^2}{g} < 0
$$

二阶导数为负 ⇒ **最大值** ✅

**最大射程**：

$$
R_{max} = \frac{v_0^2 \sin(2 \times 45^\circ)}{g} = \frac{v_0^2 \sin 90^\circ}{g} = \boxed{\frac{v_0^2}{g}}
$$

> ⭐ **物理直觉**：$45^\circ$ 时，水平和竖直分速度恰好相等（$v_{0x}=v_{0y}=v_0/\sqrt{2}$），在"飞的够远"和"飞的够久"之间达到最佳平衡！

#### 1.5.17 🧪 例题：斜抛运动的角度选择问题

**题目**：在水平地面上，一个足球运动员想将球踢过一堵高 $3\ \text{m}$、距离 $20\ \text{m}$ 的墙。球被踢出时的初速度为 $20\ \text{m/s}$，重力加速度 $g = 10\ \text{m/s}^2$。

(a) 球能否越过这堵墙？
(b) 如果能，踢出角度应满足什么条件？

**解答**：

**(a)** 先求轨迹方程：

参数方程：$x = (v_0\cos\theta)t$，$y = (v_0\sin\theta)t - \frac{1}{2}gt^2$

消去 $t$：

$$
y = x\tan\theta - \frac{g}{2v_0^2\cos^2\theta} x^2
$$

代入 $v_0 = 20$，$g = 10$，$x = 20$：

$$
y(20) = 20\tan\theta - \frac{10}{2 \times 400 \times \cos^2\theta} \times 400 = 20\tan\theta - \frac{5}{\cos^2\theta}
$$

利用 $\dfrac{1}{\cos^2\theta} = 1 + \tan^2\theta$：

$$
y(20) = 20\tan\theta - 5(1 + \tan^2\theta) = -5\tan^2\theta + 20\tan\theta - 5
$$

**(b)** 令 $y(20) > 3$：

$$
-5\tan^2\theta + 20\tan\theta - 5 > 3
$$

$$
-5\tan^2\theta + 20\tan\theta - 8 > 0
$$

$$
5\tan^2\theta - 20\tan\theta + 8 < 0
$$

解二次方程 $5u^2 - 20u + 8 = 0$（其中 $u = \tan\theta$）：

$$
u = \frac{20 \pm \sqrt{400 - 160}}{10} = \frac{20 \pm \sqrt{240}}{10} = \frac{20 \pm 4\sqrt{15}}{10} = 2 \pm \frac{2\sqrt{15}}{5}
$$

$$
u_1 \approx 2 - 1.55 = 0.45,\quad u_2 \approx 2 + 1.55 = 3.55
$$

所以 $\tan\theta$ 的范围为：

$$
0.45 < \tan\theta < 3.55
$$

即：

$$
\theta_{min} \approx \tan^{-1}(0.45) \approx \mathbf{24.2^\circ},\quad \theta_{max} \approx \tan^{-1}(3.55) \approx \mathbf{74.3^\circ}
$$

> ⭐ **结论**：当踢出角度在 **$24.2^\circ$ 到 $74.3^\circ$** 之间时，球可以越过 $3\ \text{m}$ 高的墙。在此范围之外的角度都会撞到墙！
>
> 注意这里 $\theta = 45^\circ$ 在范围内，但并非唯一的可行角度——抛体运动的 **双解性** 使得较低或较高的角度都能达到同一目标点。

---

## Part B：AP 难度层（概念陷阱 + 深度理解）

---

### 六、AP 考试真正的概念陷阱

#### 🎯 陷阱 1：最高点速度 ≠ 0！

**AP 必考概念**：

> A projectile is launched at an angle. At the highest point of its trajectory:
>
> A) Both $v_x$ and $v_y$ are zero.
> B) $v_y = 0$, $v_x$ is maximum.
> C) **$v_y = 0$, $v_x$ is constant (same as initial $v_x$).**
> D) Both $v_x$ and $v_y$ are constant.

**答案**：C ✅

> ⚠️ **AP 陷阱**：与竖直上抛不同，斜抛在最高点只有 $v_y = 0$，**$v_x$ 仍然不为零**（除非是竖直上抛 $\theta = 90^\circ$）！

#### 🎯 陷阱 2：落地速度大小与抛出速度大小相同吗？

**对称抛体**（落回同一水平面）：

$$v_f = \sqrt{v_x^2 + v_y^2} = \sqrt{(v_0\cos\theta)^2 + (-v_0\sin\theta)^2} = v_0$$

> 落地速度大小 = 抛出速度大小 ✅
>
> 但 **方向不同**——落地速度与水平方向的夹角等于抛出角，但在水平面以下。

#### 🎯 陷阱 3："从地面斜抛" vs "从高处斜抛"——落地时间不同！

**从地面抛**（落回同一高度）：飞行时间 $T = \frac{2v_0\sin\theta}{g}$

**从高处抛**（落回更低高度）：需要用二次方程求 $y=0$ 的解，不是简单公式！

**🧪 示例**：

> 从 $50\ \text{m}$ 高的悬崖以 $20\ \text{m/s}$、$30^\circ$ 向上斜抛，落地时间？

设 $y_0 = 50\ \text{m}$，落地时 $y=0$：

$$0 = 50 + (20\sin30^\circ)t - \frac{1}{2}gt^2$$
$$0 = 50 + 10t - 5t^2 \quad\Rightarrow\quad 5t^2 - 10t - 50 = 0$$
$$t^2 - 2t - 10 = 0 \quad\Rightarrow\quad t = \frac{2 \pm \sqrt{4 + 40}}{2} = \frac{2 \pm \sqrt{44}}{2}$$
$$t \approx \frac{2 + 6.63}{2} = \mathbf{4.32\ s} \quad (t>0)$$

#### 🎯 陷阱 4：$45^\circ$ 一定射程最大吗？

**经典陷阱**：

> ❌ 抛体运动的最大射程角度永远是 $45^\circ$。

**✅ 正确答案**：
- 当 **落回同一水平面** 时，最大射程角度为 $45^\circ$
- 当 **落点低于抛出点** 时，最大射程角度 **小于 $45^\circ$**
- 当 **落点高于抛出点** 时，最大射程角度 **大于 $45^\circ$**

AP 考试可能会给出不同高度的情境，让你判断哪个角度射程最大！

#### 🎯 陷阱 5：空气阻力的影响（AP 概念辨析）

| 参数 | 无空气阻力 | 有空气阻力 |
|:--|:--|:--|
| 轨迹形状 | 对称抛物线 | **不对称**，下降段更陡 |
| 水平射程 | $R = v_0^2\sin 2\theta / g$ | **减小** |
| 最大高度 | $H = v_0^2\sin^2\theta / 2g$ | **减小** |
| 飞行时间 | $T = 2v_0\sin\theta / g$ | **减小** |
| 落地速度 | 等于抛出速度 | **小于** 抛出速度 |

> ⚠️ **AP 1 注意**：除非题目明确说明，否则 **默认忽略空气阻力**。

---

### 七、AP Physics C 的微积分深度

#### 7.1 从牛顿第二定律出发的微积分推导

在抛体运动中，$\vec{F} = m\vec{a}$，且只有重力 $m\vec{g}$ 作用：

$$
\vec{a} = \frac{\vec{F}}{m} = \vec{g} = -g\hat{j}
$$

写成分量形式：

$$
a_x = \frac{d^2x}{dt^2} = 0,\quad a_y = \frac{d^2y}{dt^2} = -g
$$

#### 7.2 积分两次得到运动方程

**水平方向**：

$$
\frac{d^2x}{dt^2} = 0 \quad\Rightarrow\quad \frac{dx}{dt} = C_1
$$

由 $v_x(0) = v_0\cos\theta$ 得 $C_1 = v_0\cos\theta$

$$
\frac{dx}{dt} = v_0\cos\theta \quad\Rightarrow\quad x(t) = (v_0\cos\theta)t + C_2
$$

由 $x(0) = 0$ 得 $C_2 = 0$

$$
\boxed{x(t) = (v_0\cos\theta)t}
$$

**竖直方向**：

$$
\frac{d^2y}{dt^2} = -g \quad\Rightarrow\quad \frac{dy}{dt} = -gt + D_1
$$

由 $v_y(0) = v_0\sin\theta$ 得 $D_1 = v_0\sin\theta$

$$
\frac{dy}{dt} = v_0\sin\theta - gt \quad\Rightarrow\quad y(t) = (v_0\sin\theta)t - \frac{1}{2}gt^2 + D_2
$$

由 $y(0) = 0$ 得 $D_2 = 0$

$$
\boxed{y(t) = (v_0\sin\theta)t - \frac{1}{2}gt^2}
$$

这就是完整的微积分推导！✅

#### 7.3 🧪 AP Physics C 真题难度示例

> A projectile is launched from ground level with initial velocity $\vec{v}_0 = 20\hat{i} + 30\hat{j}\ \text{m/s}$.
> ($g = 10\ \text{m/s}^2$, 忽略空气阻力)
>
> **(a)** Write the position vector $\vec{r}(t)$.
> **(b)** Find the time when the projectile reaches its maximum height.
> **(c)** Find the velocity vector at the maximum height.
> **(d)** Find the speed of the projectile at $t = 2$ s.
> **(e)** Find the angle between the velocity and acceleration vectors at $t = 1$ s.
> **(f)** Derive the equation of the trajectory $y(x)$.

**解答**：

**(a)** $v_{0x} = 20,\ v_{0y} = 30$

$$
\vec{r}(t) = (20t)\hat{i} + \left(30t - \frac{1}{2} \times 10 \times t^2\right)\hat{j} = \boxed{20t\hat{i} + (30t - 5t^2)\hat{j}\ \text{m}}
$$

**(b)** 最高点时 $v_y = 0$：

$$v_y(t) = \frac{dy}{dt} = 30 - 10t = 0 \quad\Rightarrow\quad t = \mathbf{3\ s}$$

**(c)** 最高点：

$$
\vec{v}(3) = 20\hat{i} + (30 - 30)\hat{j} = \boxed{20\hat{i}\ \text{m/s}}
$$

只有水平分量！✅

**(d)** $t = 2$ s：

$$
\vec{v}(2) = 20\hat{i} + (30 - 20)\hat{j} = 20\hat{i} + 10\hat{j}
$$

速度大小（speed）：

$$
|\vec{v}(2)| = \sqrt{20^2 + 10^2} = \sqrt{500} \approx \mathbf{22.36\ \text{m/s}}
$$

**(e)** $t = 1$ s：

$$
\vec{v}(1) = 20\hat{i} + (30 - 10)\hat{j} = 20\hat{i} + 20\hat{j}
$$

$$
\vec{a} = -g\hat{j} = -10\hat{j}
$$

点积：

$$
\vec{v} \cdot \vec{a} = 20 \times 0 + 20 \times (-10) = -200
$$

$$
|\vec{v}| = \sqrt{20^2 + 20^2} = 20\sqrt{2},\quad |\vec{a}| = 10
$$

$$
\cos\theta = \frac{-200}{20\sqrt{2} \times 10} = \frac{-200}{200\sqrt{2}} = -\frac{1}{\sqrt{2}}
$$

$$
\theta = \cos^{-1}\left(-\frac{1}{\sqrt{2}}\right) = \mathbf{135^\circ}
$$

> $\vec{v} \cdot \vec{a} < 0$，所以此时 **物体在减速**（上升阶段）✅

**(f)** 轨迹方程：

$x = 20t \quad\Rightarrow\quad t = \dfrac{x}{20}$

$$
y = 30\left(\frac{x}{20}\right) - 5\left(\frac{x}{20}\right)^2 = \frac{3}{2}x - 5\left(\frac{x^2}{400}\right)
$$

$$
\boxed{y = \frac{3}{2}x - \frac{x^2}{80}}
$$

---

### 八、AP 考试难度分级总结

| 层次 | 对应考试 | 核心要求 | 典型题特征 |
|:--|:--|:--|:--|
| **Level 1：公式代入** | 学校期中 | 用 $T, R, H$ 公式直接计算 | 已知 $v_0, \theta$ 求飞行时间、射程、最大高度 |
| **Level 2：概念辨析与应用** | **AP Physics 1 & 2** 🎯 | 从高处斜抛、落点不同高度、$45^\circ$ 陷阱、空气阻力影响 | "从悬崖抛出的物体何时落地？""考虑空气阻力轨迹如何变化？" |
| **Level 3：微积分推导** | **AP Physics C** 🎯 | 从 $\vec{a} = -g\hat{j}$ 积分两次得到运动方程；求 $\vec{v} \cdot \vec{a}$ 分析加速/减速；推导轨迹方程 | 给 $\vec{v}_0$ 求 $\vec{r}(t)$、速度夹角、轨迹方程 $y(x)$ |

---

### 九、AP 级别综合练习

#### 🟢 AP Physics 1 风格

> A cannonball is fired from ground level with an initial speed of $50\ \text{m/s}$ at an angle of $53^\circ$ above the horizontal. ($g = 10\ \text{m/s}^2$, $\sin53^\circ = 0.8$, $\cos53^\circ = 0.6$)
>
> (a) Calculate the horizontal and vertical components of the initial velocity.
> (b) How long does the cannonball stay in the air?
> (c) What is the maximum height reached?
> (d) What is the horizontal range?
> (e) What is the velocity (magnitude and direction) just before hitting the ground?

**解答**：

**(a)**

$$
v_{0x} = 50 \times 0.6 = 30\ \text{m/s},\quad v_{0y} = 50 \times 0.8 = 40\ \text{m/s}
$$

**(b)**

$$
T = \frac{2v_{0y}}{g} = \frac{2 \times 40}{10} = \mathbf{8\ s}
$$

**(c)**

$$
H = \frac{v_{0y}^2}{2g} = \frac{40^2}{20} = \frac{1600}{20} = \mathbf{80\ m}
$$

**(d)**

$$
R = v_{0x} \times T = 30 \times 8 = \mathbf{240\ m}
$$

**(e)** 落地速度：

- $v_x = 30\ \text{m/s}$（不变）
- $v_y = -40\ \text{m/s}$（对称）

大小：$v = \sqrt{30^2 + 40^2} = \mathbf{50\ m/s}$（与初速度相同！）
方向：与水平方向夹角 $\phi = \tan^{-1}\left(\frac{40}{30}\right) \approx 53^\circ$ 向下 ✅

#### 🔵 AP Physics C 风格

> A projectile is launched from the origin with initial velocity $\vec{v}_0 = (10\hat{i} + 20\hat{j})\ \text{m/s}$.
> The acceleration due to gravity is $\vec{g} = -10\hat{j}\ \text{m/s}^2$.
>
> (a) Find the velocity vector $\vec{v}(t)$ and position vector $\vec{r}(t)$.
> (b) Find the time when $v_y = 0$ and the position at that time.
> (c) Find the speed as a function of time $v(t)$.
> (d) At what time is the speed minimum? What is that minimum speed?
> (e) Find the equation of the trajectory $y(x)$.
> (f) Find the radius of curvature of the trajectory at the highest point.

**解答**：

**(a)** 对加速度积分：

$$
\vec{v}(t) = \int \vec{a}\ dt = \int (-10\hat{j})\ dt = -10t\hat{j} + \vec{C}
$$

代入 $\vec{v}(0) = 10\hat{i} + 20\hat{j}$ 得 $\vec{C} = 10\hat{i} + 20\hat{j}$

$$
\boxed{\vec{v}(t) = 10\hat{i} + (20 - 10t)\hat{j}\ \text{m/s}}
$$

再积分：

$$
\vec{r}(t) = \int \vec{v}(t)\ dt = \int (10\hat{i} + (20-10t)\hat{j})\ dt = 10t\hat{i} + \left(20t - 5t^2\right)\hat{j} + \vec{D}
$$

代入 $\vec{r}(0) = \vec{0}$ 得 $\vec{D} = \vec{0}$

$$
\boxed{\vec{r}(t) = 10t\hat{i} + (20t - 5t^2)\hat{j}\ \text{m}}
$$

**(b)** $v_y = 0$：

$$20 - 10t = 0 \quad\Rightarrow\quad t = \mathbf{2\ s}$$

位置：$\vec{r}(2) = 10(2)\hat{i} + (40 - 20)\hat{j} = \boxed{20\hat{i} + 20\hat{j}\ \text{m}}$

最高点 $(20, 20)\ \text{m}$ ✅

**(c)** 速度大小（speed）：

$$
v(t) = |\vec{v}(t)| = \sqrt{10^2 + (20 - 10t)^2} = \sqrt{100 + (20 - 10t)^2}
$$

$$
\boxed{v(t) = \sqrt{100 + (20 - 10t)^2}\ \text{m/s}}
$$

**(d)** $v(t)$ 取最小值时，根号内的值最小：

$$
f(t) = 100 + (20 - 10t)^2
$$

对 $t$ 求导：$f'(t) = 2(20 - 10t)(-10) = -20(20 - 10t)$

令 $f'(t) = 0$：$20 - 10t = 0 \quad\Rightarrow\quad t = \mathbf{2\ s}$

$$
v_{min} = v(2) = \sqrt{100 + 0} = \mathbf{10\ m/s}
$$

> ⭐ **AP C 重点**：抛体运动的最小速度出现在最高点，大小为 $v_0\cos\theta$（即水平分量）！

**(e)** 轨迹方程：

$x = 10t \quad\Rightarrow\quad t = \dfrac{x}{10}$

$$
y = 20\left(\frac{x}{10}\right) - 5\left(\frac{x}{10}\right)^2 = 2x - 5\left(\frac{x^2}{100}\right)
$$

$$
\boxed{y = 2x - \frac{x^2}{20}}
$$

**(f)** 曲率半径公式（AP C 进阶）：

$$
\rho = \frac{v^2}{a_\perp}
$$

最高点：$v = 10\ \text{m/s}$（水平），$a_\perp = g = 10\ \text{m/s}^2$（向心加速度全部由重力提供）

$$
\rho = \frac{10^2}{10} = \mathbf{10\ m}
$$

---

### 十、本节 AP 考点频率统计

| 考点 | AP 1 频率 | AP C 频率 | 说明 |
|:--|:--:|:--:|:--|
| 矢量分解（$v_{0x}, v_{0y}$） | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | 抛体运动第一步 |
| 飞行时间 $T$ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | 基本计算 |
| 水平射程 $R$ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | 基本计算 |
| 最大高度 $H$ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | 基本计算 |
| 最高点 $v_y=0$ 但 $v_x \neq 0$ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | 概念陷阱，必考 |
| $45^\circ$ 射程最大（同一水平面） | ⭐⭐⭐⭐ | ⭐⭐⭐ | 概念理解 |
| 从高处抛出的落地时间 | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | 需要解二次方程 |
| 空气阻力的定性影响 | ⭐⭐⭐ | ⭐⭐ | 概念辨析 |
| 从 $\vec{a}$ 积分两次求 $\vec{r}(t)$ | — | ⭐⭐⭐⭐⭐ | AP C 核心技能 |
| 速度与加速度点积分析 | — | ⭐⭐⭐⭐ | 分析加速/减速 |
| 轨迹方程 $y(x)$ 推导 | — | ⭐⭐⭐⭐ | AP C FRQ 常考 |
| 曲率半径 | — | ⭐⭐⭐ | AP C 进阶 |

---
