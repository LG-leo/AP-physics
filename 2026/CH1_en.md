<!-- markdownlint-disable MD033 MD041 -->

<div align="center">

# 📚 AP Physics — Kinematics 1.1: Scalars vs. Vectors

> **Scalars vs. Vectors — Complete Comprehensive Edition**
>
> Covers AP Physics 1 & 2 (Algebra) + AP Physics C (Calculus) — All Difficulty Levels

[![AP Physics](https://img.shields.io/badge/AP-Physics-001845?style=for-the-badge&logo=apache&logoColor=white)](https://ap.collegeboard.org/)
[![Physics 1](https://img.shields.io/badge/AP%20Physics-1-FF6B35?style=flat-square)]()
[![Physics C](https://img.shields.io/badge/AP%20Physics-C-004E89?style=flat-square)]()
[![GitHub](https://img.shields.io/badge/maintained%20with-❤️-ff69b4?style=flat-square)]()

</div>

---

## 📑 Table of Contents

- [Part A: Foundation Layer (AP Physics 1 & 2 Essentials)](#part-a-foundation-layer-ap-physics-1--2-essentials)
  - [I. Core Concepts — Essential Differences Between Scalars and Vectors](#i-core-concepts--essential-differences-between-scalars-and-vectors)
  - [II. Distance vs. Displacement](#ii-distance-vs-displacement)
  - [III. Speed vs. Velocity](#iii-speed-vs-velocity)
  - [IV. Sign Conventions in One-Dimensional Motion](#iv-sign-conventions-in-one-dimensional-motion)
  - [V. Vector Decomposition and Composition](#v-vector-decomposition-and-composition)
- [Part B: AP Difficulty Layer](#part-b-ap-difficulty-layer-conceptual-traps--deep-understanding)
  - [VI. Real Conceptual Traps on the AP Exam](#vi-real-conceptual-traps-on-the-ap-exam)
  - [VII. AP Physics C Calculus Depth](#vii-ap-physics-c-calculus-depth)
  - [VIII. Difficulty Level Summary](#viii-ap-exam-difficulty-level-summary)
  - [IX. AP-Level Practice Problems](#ix-ap-level-practice-problems)
  - [X. Topic Frequency Statistics](#x-topic-frequency-statistics)

---

# Part A: Foundation Layer (AP Physics 1 & 2 Essentials)

---

## I. Core Concepts — Essential Differences Between Scalars and Vectors

### 1.1 Definition Comparison

| Aspect | Scalar | Vector |
|:--|:--|:--|
| **Definition** | A physical quantity with only **magnitude** | A physical quantity with both **magnitude** and **direction** |
| **Mathematical Representation** | A real number (with units) | Arrow notation $\vec{v}$ or bold $\mathbf{v}$, or component form $\langle v_x, v_y \rangle$ |
| **Operation Rules** | Ordinary algebraic operations ($2+3=5$) | Follows **vector addition** (parallelogram law, component addition) |
| **Can be negative?** | ❌ Scalars (e.g., speed, distance) cannot be negative | ✅ In 1D, sign indicates direction |

### 1.2 Common Physical Quantities by Category

| Scalars | Vectors |
|:--|:--|
| Distance, Speed | Displacement, Velocity |
| Time, Mass | Acceleration, Force |
| Energy, Work | Momentum, Impulse |
| Power, Temperature | Electric Field, Magnetic Field |
| Charge, Potential | Gravity, Friction |

---

## II. Distance vs. Displacement

### 2.1 Definition Comparison

| | **Distance** | **Displacement** |
|:--|:--|:--|
| Type | **Scalar** | **Vector** |
| Meaning | **Total length** of the path traveled | **Directed line segment** from start to finish |
| Cares about | "How far" (regardless of direction) | "From where to where, how far + which direction" |
| Can it be zero? | Only if the object doesn't move | Yes — return to starting point, displacement $=0$, but distance $\neq 0$ |
| Notation | $d$ or $s$ (pure number) | $\Delta \vec{x}$ or $\vec{d}$ |
| Unit | meter (m) | meter (m) |

### 2.2 🧪 Classic Basic Example

**Problem**: Xiaoming walks 3 m east from home, then 4 m north.

- **Distance** (total path length) $= 3 + 4 = \mathbf{7\ m}$ ✅
- **Displacement** (straight-line distance from start to finish) $= \sqrt{3^2 + 4^2} = \mathbf{5\ m}$, direction **$53^\circ$ north of east** ($\theta = \tan^{-1}\frac{4}{3}$) ✅

---

## III. Speed vs. Velocity

### 3.1 Definition Comparison

| | **Speed** | **Velocity** |
|:--|:--|:--|
| Type | **Scalar** | **Vector** |
| Meaning | "How fast" (only cares about rate) | "How fast + which direction" |
| Formula | $v = \dfrac{\text{distance}}{\text{time}}$ | $\vec{v} = \dfrac{\Delta \vec{x}}{\Delta t}$ |
| AP Notation | $v$ (no arrow) | $\vec{v}$ or $v_x$ (with sign in 1D) |
| Can be negative? | ❌ Speed is always **non-negative** | ✅ Can be **negative** — indicates opposite direction to the chosen positive direction |

### 3.2 Key Understanding

In one-dimensional motion, we **first choose a positive direction** (e.g., right as positive):

- Object moving **right** → velocity $= +5\ \text{m/s}$
- Object moving **left** → velocity $= -5\ \text{m/s}$

**Speed is $5\ \text{m/s}$ in both cases**, but velocity differs in direction!

---

## IV. Sign Conventions in One-Dimensional Motion

### 4.1 Standard Practice

In one-dimensional (linear) motion, we use **positive and negative signs** to represent direction:

```
          ← Negative direction      Positive direction →
    ─────┼────┼────┼────┼────┼────
         -2   -1    0    1    2
```

- Choose a direction as **positive** (usually right or up)
- Same direction as positive → **positive value**
- Opposite direction → **negative value**

### 4.2 🧪 Basic Example

An object moves from $x=2\ \text{m}$ to $x=-3\ \text{m}$, with positive direction to the right:

- Displacement $\Delta x = x_f - x_i = -3 - 2 = \mathbf{-5\ m}$ (moved 5 m to the left)
- If it takes 2 seconds, average velocity $\bar{v}= \dfrac{-5}{2} = \mathbf{-2.5\ m/s}$

---

## V. Vector Decomposition and Composition

### 5.1 Component Decomposition

Decompose vector $\vec{v}$ into perpendicular components (let $\theta$ be the angle with the positive $x$-axis):

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

### 5.2 Vector Composition

- $v = \sqrt{v_x^2 + v_y^2}$
- $\theta = \tan^{-1}\left(\dfrac{v_y}{v_x}\right)$

### 5.3 One-Dimensional Vector Addition

> Add algebraically, paying attention to signs!

**Example**: An object experiences a force of 5 N to the right and 3 N to the left.

- Let right be positive
- Net force $F_{net} = 5 + (-3) = \mathbf{2\ N}$ (to the right)

### 5.4 🧪 Derivation: Geometric Foundation of Vector Decomposition & Composition

Vector addition has two equivalent methods — the **graphical method** (parallelogram law) and the **analytical method** (component addition). Here we prove their equivalence.

#### Parallelogram Law

For two vectors $\vec{a}$ and $\vec{b}$, their resultant $\vec{c} = \vec{a} + \vec{b}$ is the diagonal of the parallelogram formed by $\vec{a}$ and $\vec{b}$ as adjacent sides.

#### From Parallelogram Law → Component Addition

Let $\vec{a} = a_x\hat{i} + a_y\hat{j}$, $\vec{b} = b_x\hat{i} + b_y\hat{j}$, with angle $\phi$ between them.

According to the parallelogram law, the magnitude of the resultant is:

$$
c = \sqrt{a^2 + b^2 + 2ab\cos\phi}
$$

According to component addition:

$$
\vec{c} = (a_x + b_x)\hat{i} + (a_y + b_y)\hat{j}
$$

Its magnitude is:

$$
|c| = \sqrt{(a_x + b_x)^2 + (a_y + b_y)^2}
$$

Since $a_x = a\cos\theta_a$, $a_y = a\sin\theta_a$, $b_x = b\cos\theta_b$, $b_y = b\sin\theta_b$, substituting and expanding:

$$
|c| = \sqrt{a^2 + b^2 + 2ab(\cos\theta_a\cos\theta_b + \sin\theta_a\sin\theta_b)} = \sqrt{a^2 + b^2 + 2ab\cos(\theta_a - \theta_b)}
$$

where $\phi = \theta_a - \theta_b$ is exactly the angle between the two vectors. Both methods yield the **identical result**! ✅

> 💡 **Core Conclusion**: The parallelogram law and component addition are **completely equivalent** — the analytical method simply converts a geometric problem into algebraic calculations.

### 5.5 🧪 Example: Adding Multiple Vectors

**Problem**: An object is subjected to three forces: $\vec{F}_1 = 3\hat{i} + 4\hat{j}\ \text{N}$, $\vec{F}_2 = -2\hat{i} + \hat{j}\ \text{N}$, $\vec{F}_3 = \hat{i} - 3\hat{j}\ \text{N}$. Find the magnitude and direction of the resultant force.

**Solution**:

**(1)** Add components:

$$
\vec{F}_{net} = \vec{F}_1 + \vec{F}_2 + \vec{F}_3 = (3 - 2 + 1)\hat{i} + (4 + 1 - 3)\hat{j} = 2\hat{i} + 2\hat{j}\ \text{N}
$$

**(2)** Magnitude:

$$
|\vec{F}_{net}| = \sqrt{2^2 + 2^2} = \sqrt{8} = 2\sqrt{2} \approx \mathbf{2.83\ N}
$$

**(3)** Direction (angle from the positive $x$-axis):

$$
\theta = \tan^{-1}\left(\frac{2}{2}\right) = \tan^{-1}(1) = \mathbf{45^\circ}
$$

> ⭐ **No matter how many vectors you add, simply sum their $x$ and $y$ components separately!**

### 5.6 🧪 Derivation: Three Methods for Vector Component Formulas

The vector decomposition formulas $v_x = v\cos\theta$, $v_y = v\sin\theta$ are the most fundamental and important tools in kinematics. Here are three complementary derivation methods to help you understand these formulas from different angles.

#### Method 1: Right Triangle Geometry (Most Intuitive)

The vector $\vec{v}$ and its components $v_x$, $v_y$ form a right triangle. $\vec{v}$ is the hypotenuse, $v_x$ and $v_y$ are the two legs, and $\theta$ is the angle between $\vec{v}$ and the $x$-axis.

In a right triangle, by the definitions of trigonometric functions:
- $\cos\theta = \dfrac{\text{adjacent}}{\text{hypotenuse}} = \dfrac{v_x}{v}$, therefore $v_x = v\cos\theta$
- $\sin\theta = \dfrac{\text{opposite}}{\text{hypotenuse}} = \dfrac{v_y}{v}$, therefore $v_y = v\sin\theta$

> 💡 **Geometric Intuition**: Imagine decomposing a force into two perpendicular directions — the side-length relationships of a right triangle naturally yield the component formulas. When $\theta = 0^\circ$, the entire vector lies along the $x$-axis ($v_x = v$, $v_y = 0$); when $\theta = 90^\circ$, the entire vector lies along the $y$-axis ($v_x = 0$, $v_y = v$).

#### Method 2: Unit Vector Projection (Analytic Geometry)

Express the vector as $\vec{v} = v_x\hat{i} + v_y\hat{j}$. At the same time, the vector can also be expressed as magnitude times a unit direction vector:

$$
\vec{v} = v \cdot \hat{u}
$$

where $\hat{u}$ is the unit vector in the direction of $\vec{v}$, which can be written as $\hat{u} = \cos\theta\hat{i} + \sin\theta\hat{j}$.

Equating the two representations:

$$
v_x\hat{i} + v_y\hat{j} = v(\cos\theta\hat{i} + \sin\theta\hat{j})
$$

Comparing coefficients of $\hat{i}$ and $\hat{j}$:

$$
v_x = v\cos\theta,\quad v_y = v\sin\theta
$$

> 💡 **Key Insight**: The components of a unit vector are exactly the cosine and sine of its direction angle — this is the most elegant bridge between analytic geometry and physical vectors.

#### Method 3: Rotation Matrix (Linear Algebra Perspective)

Starting from the standard position (vector along the $x$-axis, i.e., $(v, 0)$), rotate the coordinate system by angle $-\theta$. The vector's coordinates in the new system are the components.

The 2D rotation matrix is:

$$
\begin{pmatrix} v_x \\ v_y \end{pmatrix} = \begin{pmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{pmatrix}^{-1} \begin{pmatrix} v \\ 0 \end{pmatrix}
$$

Since the inverse of a rotation matrix is its transpose (property of orthogonal matrices), this is equivalent to rotating the vector $(v, 0)$ by angle $\theta$:

$$
\begin{pmatrix} v_x \\ v_y \end{pmatrix} = \begin{pmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{pmatrix} \begin{pmatrix} v \\ 0 \end{pmatrix} = \begin{pmatrix} v\cos\theta \\ v\sin\theta \end{pmatrix}
$$

> 💡 **Advanced Perspective**: The rotation matrix method reveals that vector decomposition is fundamentally just **coordinate rotation**. This idea reappears repeatedly in electromagnetism (e.g., Lorentz force decomposition) and rigid body mechanics.

### 5.7 🧪 Derivation: Three Methods for Vector Composition Formulas

Composing components back into the vector magnitude $v = \sqrt{v_x^2 + v_y^2}$ and direction $\theta = \tan^{-1}(v_y/v_x)$ also has three derivation methods.

#### Method 1: Direct Pythagorean Theorem

The vector $\vec{v}$ and its components $v_x$, $v_y$ form a right triangle. By the Pythagorean theorem:

$$
v^2 = v_x^2 + v_y^2 \quad\Rightarrow\quad v = \sqrt{v_x^2 + v_y^2}
$$

The direction angle follows from the definition of tangent:

$$
\tan\theta = \frac{\text{opposite}}{\text{adjacent}} = \frac{v_y}{v_x} \quad\Rightarrow\quad \theta = \tan^{-1}\left(\frac{v_y}{v_x}\right)
$$

**⚠️ Important Reminder**: $\tan^{-1}$ returns angles in $(-90^\circ, 90^\circ)$. If $v_x < 0$, you must add $180^\circ$ (or $\pi$) to get the correct direction angle. This is frequently used to design multiple-choice traps on the AP exam!

#### Method 2: Vector Dot Product (Self-Product)

The magnitude of a vector can also be defined through the dot product (inner product):

$$
|\vec{v}|^2 = \vec{v} \cdot \vec{v} = (v_x\hat{i} + v_y\hat{j}) \cdot (v_x\hat{i} + v_y\hat{j})
$$

Using the orthogonality properties $\hat{i} \cdot \hat{i} = \hat{j} \cdot \hat{j} = 1$, $\hat{i} \cdot \hat{j} = 0$:

$$
|\vec{v}|^2 = v_x^2(\hat{i}\cdot\hat{i}) + v_x v_y(\hat{i}\cdot\hat{j}) + v_y v_x(\hat{j}\cdot\hat{i}) + v_y^2(\hat{j}\cdot\hat{j}) = v_x^2 + v_y^2
$$

$$
\Rightarrow\quad |\vec{v}| = \sqrt{v_x^2 + v_y^2}
$$

> 💡 **Mathematical Essence**: This is essentially the Euclidean norm ($\ell^2$ norm) of a vector. In more advanced mathematics, this concept generalizes to the **norm in an inner product space**.

#### Method 3: Complex Number Representation (AP C Perspective)

Represent a 2D vector as a complex number: $\vec{v} \leftrightarrow z = v_x + iv_y$ (where $i = \sqrt{-1}$).

The modulus of the complex number is:

$$
|z| = \sqrt{z \cdot \bar{z}} = \sqrt{(v_x + iv_y)(v_x - iv_y)} = \sqrt{v_x^2 + v_y^2}
$$

The argument (phase angle) is:

$$
\arg(z) = \tan^{-1}\left(\frac{v_y}{v_x}\right)
$$

> 💡 **Complex Numbers in Physics**: Complex number representation has wide applications in AC circuit analysis (phasor method) and quantum mechanics (wave functions). Vector composition is essentially a **complex addition** problem!

### 5.8 🧪 Example: Vector Decomposition on an Inclined Plane

**Problem**: A block of mass $m$ rests on a frictionless incline of angle $\theta$. Decompose the gravitational force $\vec{F}_g = mg$ (vertically downward) into components parallel and perpendicular to the incline surface.

**Solution**:

Gravity points vertically downward: $\vec{F}_g = mg(-\hat{j})$ (let upward be $+y$).

**(1) Geometric analysis**: The incline angle is $\theta$, and the angle between gravity and the direction perpendicular to the incline is also $\theta$.

**(2) Component decomposition**:

Parallel to the incline (along the surface):
$$
F_{g,\parallel} = mg\sin\theta \quad (\text{down the incline})
$$

Perpendicular to the incline (normal):
$$
F_{g,\perp} = mg\cos\theta \quad (\text{into the incline})
$$

**(3) Verification**: When $\theta = 0^\circ$ (horizontal surface), $F_{g,\parallel} = 0$ (no sliding tendency), $F_{g,\perp} = mg$ (all weight presses on the surface). When $\theta = 90^\circ$ (vertical surface), $F_{g,\parallel} = mg$ (all weight accelerates along the surface), $F_{g,\perp} = 0$ (no pressure on the surface). ✅

> ⭐ **The inclined plane is the foundation of all mechanics problems** — the parallel component of gravity $mg\sin\theta$ is one of the most frequently used formulas in AP Physics 1!

### 5.9 🧪 Example: Airplane Crosswind Navigation — A Vector Analysis

**Problem**: An airplane has an airspeed (speed in still air) of $250\ \text{km/h}$. It needs to fly due north, but encounters a wind blowing from the northwest ($45^\circ$ north of west) at $50\ \text{km/h}$. Find:
(a) In what direction should the pilot point the aircraft?
(b) What is the airplane's actual ground speed?

**Solution**:

Let north be $+y$, east be $+x$.

The wind blows from the northwest, meaning the wind direction is toward the southeast ($45^\circ$ south of east):

$$
\vec{v}_{W/G} = 50\cos45^\circ\hat{i} + 50(-\sin45^\circ)\hat{j} = 35.36\hat{i} - 35.36\hat{j}
$$

The airplane's velocity relative to the air (magnitude $250\ \text{km/h}$, direction unknown — let the angle from due north be $\phi$):

$$
\vec{v}_{P/A} = 250\sin\phi\hat{i} + 250\cos\phi\hat{j}
$$

**(a)** For the plane to fly due north relative to the ground, $v_{P/G,x} = 0$:

$$
v_{P/G,x} = 250\sin\phi + 35.36 = 0 \quad\Rightarrow\quad \sin\phi = -\frac{35.36}{250} = -0.1414
$$

$$
\phi = \sin^{-1}(-0.1414) \approx -8.13^\circ
$$

The aircraft should point approximately **$8.1^\circ$ west of north**. ✅

**(b)** Actual ground speed:

$$
v_{P/G,y} = 250\cos\phi + (-35.36) = 250\cos(-8.13^\circ) - 35.36
$$

$$
= 250 \times 0.990 - 35.36 \approx 247.5 - 35.36 = 212.1\ \text{km/h}
$$

Ground speed is approximately $\mathbf{212\ \text{km/h}\ \text{due north}}$. ✅

> ⭐ **The essence of navigation problems**: Use vector composition to convert an unknown heading direction into a solvable equation — this is a classic application of relative motion.

---

# Part B: AP Difficulty Layer (Conceptual Traps & Deep Understanding)

---

## VI. Real Conceptual Traps on the AP Exam

### 🎯 Trap 1: Seemingly Simple Situational Analysis

**AP Exam Style**:

> A person walks 10 m east, then 10 m north, then 10 m west.
>
> **Question**: Which of the following is true about the person's motion?
>
> A) Distance = 30 m, Displacement = 10 m north
> B) Distance = 30 m, Displacement = 10 m east
> C) Distance = 10 m, Displacement = 30 m
> D) Distance = 30 m, Displacement = 0 m

**Answer**: A ✅

- Distance $= 10+10+10 = 30$ m
- Displacement $=$ from start $(0,0)$ to finish $(0,10) =$ **10 m north**
- ❌ Common mistake: People think they returned to the starting point, but actually $x=0, y=10$, **not back to origin**!

> 💡 **AP Trick**: They won't just ask about simple back-and-forth along a line — they'll design a path that **makes you think you've returned to the origin** when you haven't!

---

### 🎯 Trap 2: Deep Understanding of Speed vs. Velocity

**AP Physics 1 Must-Know Concept Question**:

> An object moves in a **circular path** at **constant speed**.
>
> Which of the following statements is correct?
>
> A) Both speed and velocity are constant.
> B) Speed is constant, so acceleration is zero.
> C) **Velocity changes because direction changes, so there is acceleration.**
> D) Acceleration is zero because speed is constant.

**Answer**: C ✅

> ⚠️ This is AP's favorite trick — using the word **"constant"** to mislead you! In "uniform circular motion," the "uniform" refers to constant **speed**, but **velocity** changes direction at every instant, so **velocity is NOT constant**, and therefore **there IS acceleration** (centripetal acceleration)!

---

### 🎯 Trap 3: The True Meaning of Signs

AP won't just ask "what does the sign represent" — they'll set a trap in **calculations**:

> A ball is thrown **upward** from the ground with initial speed $v_0$.

**Common AP Student Mistake**:

```
❌ Set upward as positive, gravitational acceleration g = 9.8 m/s² (forgot the negative sign!)
```

**Correct Approach**:

```
✅ Set upward as positive, then a = -g = -9.8 m/s²
   v(t) = v₀ - gt
   y(t) = v₀t - ½gt²
```

**What if we choose differently?**

```
✅ Set downward as positive, then a = +g = +9.8 m/s²
   But now v₀ is negative (thrown upward, opposite to positive direction)
   v(t) = -v₀ + gt
```

> ⭐ **AP C Level Understanding**: The choice of positive direction does not change the physical result — it only changes the sign conventions in the equations. Both approaches yield the **same final answer (magnitude and actual direction)**.

---

### 🎯 Trap 4: Average Speed vs. Average Velocity

AP exam loves testing this distinction!

| | **Average Speed** | **Average Velocity** |
|:--|:--|:--|
| Formula | $\bar{v}_{\text{avg speed}} = \dfrac{\text{total distance}}{\text{total time}}$ | $\vec{\bar{v}} = \dfrac{\text{total displacement}}{\text{total time}}$ |
| Type | **Scalar** | **Vector** |

**🧪 Classic AP Trap Problem**:

> A runner runs 100 m east in 10 s, then turns around and runs 60 m west in 10 s.
>
> (a) Average speed?
> (b) Average velocity?

**Solution**:

- Total distance $= 100 + 60 = 160$ m, total time $= 10 + 10 = 20$ s
- (a) **Average speed** $= \dfrac{160}{20} = \mathbf{8\ m/s}$ ✅
- Total displacement $= 100 - 60 = 40$ m (east)
- (b) **Average velocity** $= \dfrac{40}{20} = \mathbf{2\ m/s\ east}$ ✅

> ⚠️ See that? Average speed is **8 m/s**, but average velocity is only **2 m/s**! These two values can be vastly different!

---

## VII. AP Physics C Calculus Depth

### 7.1 Vectors in the Calculus Framework

AP Physics C requires upgrading from an **algebraic perspective** to a **calculus perspective**:

| Concept | Algebraic Understanding (AP 1) | **Calculus Understanding (AP C)** |
|:--|:--|:--|
| **Position** | A coordinate $x$ | Position vector $\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j} + z(t)\hat{k}$ |
| **Displacement** | $\Delta \vec{x} = \vec{x}_f - \vec{x}_i$ | $\Delta \vec{r} = \displaystyle\int_{t_i}^{t_f} \vec{v}(t)\ dt$ |
| **Velocity** | $\vec{v} = \dfrac{\Delta\vec{x}}{\Delta t}$ | $\vec{v}(t) = \dfrac{d\vec{r}}{dt} = \dot{x}\hat{i} + \dot{y}\hat{j} + \dot{z}\hat{k}$ |
| **Acceleration** | $\vec{a} = \dfrac{\Delta\vec{v}}{\Delta t}$ | $\vec{a}(t) = \dfrac{d\vec{v}}{dt} = \dfrac{d^2\vec{r}}{dt^2}$ |
| **Speed** | $v = \|\vec{v}\|$ (geometric) | $v = \|\vec{v}(t)\| = \sqrt{\dot{x}^2 + \dot{y}^2 + \dot{z}^2}$ (functional magnitude) |

### 7.2 Core Calculus Relationship Diagram

```
Position Vector ──differentiate──▶ Velocity Vector ──differentiate──▶ Acceleration Vector
 →r(t)              →v(t)              →a(t)
   │                   │                   │
   ◀──integrate────    ◀──integrate────
```

### 7.3 🧪 AP Physics C Exam-Style Example

> The position of a particle is given by $\vec{r}(t) = (3t^2 - 2t)\hat{i} + (4t)\hat{j}$ meters.
>
> **(a)** Find the velocity vector $\vec{v}(t)$.
> **(b)** Find the **speed** at $t = 2$ s.
> **(c)** Find the acceleration vector.

**Solution**:

**(a)**

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (6t - 2)\hat{i} + 4\hat{j}\ \text{m/s}
$$

**(b) ⚠️ Important!** speed = |velocity|, not just one component!

$$
\vec{v}(2) = (12-2)\hat{i} + 4\hat{j} = 10\hat{i} + 4\hat{j}
$$

$$
\text{speed} = |\vec{v}(2)| = \sqrt{10^2 + 4^2} = \sqrt{116} \approx 10.77\ \text{m/s}
$$

> ⚠️ **Common AP C Mistake**: When asked for speed, many students give just $10$ or $4$, forgetting to take the magnitude!

**(c)**

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = 6\hat{i} + 0\hat{j} = 6\hat{i}\ \text{m/s}^2
$$

> Note that acceleration is **constant** and only in the $x$ direction! This means although the particle moves in 2D space, the $y$-component of velocity is constant, and only the $x$-component is accelerating.

### 7.4 📐 Dot Product and Angle in Calculus Applications

**In AP Physics C, you often need to find the angle between velocity and acceleration**:

$$
\vec{v} \cdot \vec{a} = |\vec{v}||\vec{a}|\cos\theta \quad\Rightarrow\quad \cos\theta = \frac{\vec{v} \cdot \vec{a}}{|\vec{v}||\vec{a}|}
$$

**🧪 Example**: From the problem above, find the angle between $\vec{v}$ and $\vec{a}$ at $t=1$ s.

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
|\vec{v}| = \sqrt{4^2+4^2} = 4\sqrt{2}, \quad |\vec{a}| = 6
$$
$$
\cos\theta = \frac{24}{4\sqrt{2} \times 6} = \frac{1}{\sqrt{2}}, \quad \theta = 45^\circ
$$

> When $\vec{v} \cdot \vec{a} > 0$ → **speeding up**; $< 0$ → **slowing down**; $= 0$ → constant speed (e.g., uniform circular motion).

---

## VIII. AP Exam Difficulty Level Summary

| Level | Corresponding Exam | Core Requirements | Typical Problem Features |
|:--|:--|:--|:--|
| **Level 1: Basic Recall** | School midterms | Know definitions of scalars/vectors, common categories | "Which of the following is a vector?" |
| **Level 2: Conceptual Analysis** | **AP Physics 1 & 2** 🎯 | Distinguish distance/displacement, speed/velocity in context; identify common traps | Back-and-forth path problems, uniform circular motion, average speed vs. average velocity |
| **Level 3: Calculus Applications** | **AP Physics C** 🎯 | Differentiate/integrate vector functions; analyze motion using dot products | $\vec{r}(t)$ → find $\vec{v}$, $\vec{a}$; find speed as function of time; angle between vectors to determine speeding up/slowing down |

---

## IX. AP-Level Practice Problems

### 🟢 AP Physics 1 Style

> A car travels along a straight road. Its position as a function of time is given by $x(t) = 4t - t^2$ (meters, seconds).
>
> (a) At what time(s) does the car change direction?
> (b) What is the **displacement** of the car from $t=0$ to $t=4$ s?
> (c) What is the **distance traveled** from $t=0$ to $t=4$ s?
> (d) What is the **average speed** and **average velocity** over this interval?

**Solution Outline**:

- (a) $v(t)=dx/dt=4-2t=0$ → $t=2$ s ✅
- (b) Displacement $= x(4) - x(0) = 0 - 0 = \mathbf{0\ m}$ ✅
- (c) $0\rightarrow2$: $x(2)-x(0) = 4$ m; $2\rightarrow4$: $|x(4)-x(2)| = 4$ m; distance $= \mathbf{8\ m}$ ✅
- (d) Average velocity $= \mathbf{0\ m/s}$, average speed $= \mathbf{2\ m/s}$ ✅

> ⚠️ **AP Trap**: Displacement is 0, but distance is not 0! Average velocity is 0, but average speed is not 0!

---

### 🔵 AP Physics C Style

> A particle moves in the $xy$-plane with velocity $\vec{v}(t) = 3\hat{i} + 4t\hat{j}$ m/s.
> At $t=0$, the particle is at the origin.
>
> (a) Find the position vector $\vec{r}(t)$.
> (b) Find the acceleration vector $\vec{a}(t)$.
> (c) Find the magnitude of the acceleration at $t=2$ s.
> (d) Find the angle between the velocity and acceleration vectors at $t=1$ s.
> (e) Is the particle speeding up or slowing down at $t=1$ s? Justify.

**Solution**:

**(a)** $\vec{r}(t) = \displaystyle\int \vec{v}(t)\ dt = 3t\hat{i} + 2t^2\hat{j}\ \text{m}$

**(b)** $\vec{a}(t) = \dfrac{d\vec{v}}{dt} = 4\hat{j}\ \text{m/s}^2$

**(c)** $|\vec{a}| = \mathbf{4\ m/s}^2$

**(d)** At $t=1$: $\vec{v}=3\hat{i}+4\hat{j}$, $\vec{a}=4\hat{j}$, $\cos\theta = \frac{16}{5\times4}=0.8$, $\theta \approx \mathbf{36.9^\circ}$

**(e)** $\vec{v}\cdot\vec{a} = 16 > 0$, therefore **speeding up** ✅

---

## X. Topic Frequency Statistics

| Topic | AP 1 Frequency | AP C Frequency | Notes |
|:--|:--:|:--:|:--|
| Distance vs. Displacement | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | AP 1 favorite MCQ |
| Speed vs. Velocity | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | Uniform circular motion is a must-know |
| Average Speed vs. Average Velocity | ⭐⭐⭐⭐ | ⭐⭐⭐ | May appear in FRQs |
| Sign Conventions | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | Foundation for 1D motion |
| Vector Decomposition & Composition | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | Used throughout all of mechanics |
| Vector Differentiation/Integration | — | ⭐⭐⭐⭐⭐ | AP C core skill |
| Dot Product for Speed Up/Slow Down | — | ⭐⭐⭐⭐ | High-frequency FRQ topic |

---
---

# 1.2 Displacement, Velocity & Acceleration

---

## Part A: Foundation Layer (AP Physics 1 & 2 Essentials)

---

### I. Average Velocity and Instantaneous Velocity

#### 1.2.1 Average Velocity

**Definition**: The ratio of displacement to the time interval over which it occurs.

$$
\boxed{\vec{\bar{v}} = \frac{\Delta \vec{x}}{\Delta t} = \frac{\vec{x}_f - \vec{x}_i}{t_f - t_i}}
$$

| Aspect | Description |
|:--|:--|
| Type | **Vector** — direction is the same as displacement |
| Physical Meaning | Describes the **overall motion speed and direction** over a time interval |
| Unit | m/s (meters per second) |
| Path Independence | Only cares about start and end points, not the path taken in between |

> ⚠️ **Note**: Average velocity is NOT the average of velocities! $\vec{\bar{v}} \neq \dfrac{\vec{v}_i + \vec{v}_f}{2}$ (This equality only holds for **uniformly accelerated linear motion**!)

#### 1.2.2 Instantaneous Velocity

**Definition**: The velocity of an object at a **specific instant** or **specific position**.

$$
\boxed{\vec{v}(t) = \lim_{\Delta t \to 0} \frac{\Delta \vec{x}}{\Delta t}}
$$

| Aspect | Description |
|:--|:--|
| Type | **Vector** — direction is the object's direction of motion at that point |
| Physical Meaning | Describes how fast and in what direction an object is moving at a **given instant** |
| Intuitive Understanding | The speedometer in a car displays instantaneous speed (scalar form) |

#### 1.2.3 Average Speed — Emphasized Again!

$$
\boxed{\bar{v}_{\text{speed}} = \frac{\text{total distance}}{\text{total time}}}
$$

> **Average speed $\neq$ magnitude of average velocity!**
>
> Only when an object moves **in a single direction along a straight line** without turning back does average speed equal the magnitude of average velocity.

**🧪 Example**: Running one lap around a 400 m track in 80 s
- Average speed $= 400 / 80 = 5\ \text{m/s}$
- Average velocity $= 0 / 80 = 0\ \text{m/s}$ (returns to start, displacement is 0)
- Magnitude of average velocity $= 0 \neq 5$ ✅

---

### II. Average Acceleration and Instantaneous Acceleration

#### 2.1 Average Acceleration

**Definition**: The ratio of the change in velocity to the time interval over which it occurs.

$$
\boxed{\vec{\bar{a}} = \frac{\Delta \vec{v}}{\Delta t} = \frac{\vec{v}_f - \vec{v}_i}{t_f - t_i}}
$$

| Aspect | Description |
|:--|:--|
| Type | **Vector** — direction is the same as the change in velocity $\Delta \vec{v}$ |
| Physical Meaning | Describes the **average rate of change of velocity** over a time interval |
| Unit | m/s² (meters per second squared) |

> ⚠️ **Note**: The direction of acceleration is **not necessarily** the same as the direction of velocity! When speeding up, $\vec{a}$ is in the same direction as $\vec{v}$; when slowing down, they are opposite.

#### 2.2 Instantaneous Acceleration

**Definition**: The acceleration of an object at a **specific instant**.

$$
\boxed{\vec{a}(t) = \lim_{\Delta t \to 0} \frac{\Delta \vec{v}}{\Delta t}}
$$

| Aspect | Description |
|:--|:--|
| Type | **Vector** |
| Physical Meaning | Describes the **instantaneous rate of change of velocity** |

#### 2.3 Key Understanding: Direction of Acceleration

The direction of acceleration is **determined by $\Delta \vec{v}$**, not by $\vec{v}$ itself!

| Motion State | $\vec{v}$ Direction | $\vec{a}$ Direction | $\Delta \vec{v}$ Direction |
|:--|:--|:--|:--|
| Speeding up east | → East | → East | → East |
| Slowing down east | → East | ← West | ← West |
| Speeding up west | ← West | ← West | ← West |
| Slowing down west | ← West | → East | → East |

> 💡 **Memory Aid**: When speeding up, $\vec{a}$ and $\vec{v}$ are in the **same direction**; when slowing down, $\vec{a}$ and $\vec{v}$ are in **opposite directions**.

---

### III. The Three Big Equations of Uniformly Accelerated Linear Motion

#### 3.1 Conditions for Use

> The object moves along a **straight line**, and **acceleration is constant** (both magnitude and direction are unchanging).

#### 3.2 The Three Core Equations

Let $t=0$ have initial velocity $v_0$, initial position $x_0$, and constant acceleration $a$:

| # | Equation | Meaning | Missing Variable |
|:--:|:--|:--|:--:|
| **①** | $v = v_0 + at$ | **Velocity-Time Relation** | $\Delta x$ |
| **②** | $\Delta x = v_0 t + \dfrac{1}{2}at^2$ | **Position-Time Relation** | $v$ |
| **③** | $v^2 = v_0^2 + 2a\Delta x$ | **Velocity-Displacement Relation** | $t$ |

Where $\Delta x = x - x_0$.

#### 3.3 🧪 Classic Basic Example

**Problem**: A car starts from rest and accelerates uniformly at $2\ \text{m/s}^2$ for 5 seconds. Find:
(a) The velocity at the end of the 5th second
(b) The displacement during the first 5 seconds

**Solution**:

Given $v_0 = 0$, $a = 2\ \text{m/s}^2$, $t = 5\ \text{s}$

**(a)** Using equation ①:
$$v = v_0 + at = 0 + 2 \times 5 = \mathbf{10\ m/s}$$

**(b)** Using equation ②:
$$\Delta x = v_0 t + \frac{1}{2}at^2 = 0 + \frac{1}{2} \times 2 \times 5^2 = \mathbf{25\ m}$$

#### 3.4 Strategy for Choosing the Right Equation 🎯

| Given | Wanted | Which Equation |
|:--|:--|:--:|
| $v_0,\ a,\ t$ | $v$ | ① $v = v_0 + at$ |
| $v_0,\ a,\ t$ | $\Delta x$ | ② $\Delta x = v_0 t + \frac{1}{2}at^2$ |
| $v_0,\ a,\ \Delta x$ | $v$ | ③ $v^2 = v_0^2 + 2a\Delta x$ |
| $v_0,\ v,\ a$ | $\Delta x$ | ③ rearranged: $\Delta x = \dfrac{v^2-v_0^2}{2a}$ |
| $v_0,\ v,\ t$ | $\Delta x$ | $\Delta x = \dfrac{v_0+v}{2}\cdot t$ (derived from ① and ②) |

#### 3.5 🧪 Derivation: Mutual Relationships Among the Three Big Equations

The three equations are not independent — they can be derived sequentially from the definition of uniform acceleration.

> **Starting point**: Acceleration is constant $a = \text{constant}$, and $a = \dfrac{dv}{dt}$ (calculus definition).

##### Deriving Equation ① (Velocity-Time Relation) from the Definition

From $a = \dfrac{dv}{dt}$, integrate with respect to time:

$$
\int_{v_0}^{v} dv = \int_{0}^{t} a\ dt = a \int_{0}^{t} dt
$$

$$
v - v_0 = at \quad\Rightarrow\quad \boxed{v = v_0 + at}
$$

✅ This is Equation ①.

##### Deriving Equation ② (Position-Time Relation) from Equation ①

From $v = \dfrac{dx}{dt}$, substitute Equation ①:

$$
\frac{dx}{dt} = v_0 + at
$$

Integrate with respect to time:

$$
\int_{x_0}^{x} dx = \int_{0}^{t} (v_0 + at)\ dt
$$

$$
x - x_0 = v_0 t + \frac{1}{2}at^2 \quad\Rightarrow\quad \boxed{\Delta x = v_0 t + \frac{1}{2}at^2}
$$

✅ This is Equation ②.

##### Deriving Equation ③ (Velocity-Displacement Relation) from Equations ① and ②

From Equation ①, solve for $t = \dfrac{v - v_0}{a}$ and substitute into Equation ②:

$$
\Delta x = v_0\left(\frac{v - v_0}{a}\right) + \frac{1}{2}a\left(\frac{v - v_0}{a}\right)^2
$$

$$
\Delta x = \frac{v_0(v - v_0)}{a} + \frac{(v - v_0)^2}{2a}
$$

Combine terms:

$$
\Delta x = \frac{2v_0(v - v_0) + (v - v_0)^2}{2a} = \frac{(v - v_0)(2v_0 + v - v_0)}{2a}
$$

$$
\Delta x = \frac{(v - v_0)(v + v_0)}{2a} = \frac{v^2 - v_0^2}{2a}
$$

Rearranging:

$$
\boxed{v^2 = v_0^2 + 2a\Delta x}
$$

✅ This is Equation ③.

> ⭐ **You only need to memorize any two equations (usually ① and ②); the third can always be derived algebraically!**

#### 3.5.2 🧪 Derivation: Two More Ways to Derive Equation ①

Equation $v = v_0 + at$ is the cornerstone of the three big equations. Besides the calculus derivation above, here are two more methods.

##### Method 2: From the Definition of Average Acceleration

For uniformly accelerated motion, the average acceleration equals the constant acceleration $a$:

$$
a = \frac{\Delta v}{\Delta t} = \frac{v - v_0}{t - 0}
$$

Cross-multiply:

$$
a \cdot t = v - v_0 \quad\Rightarrow\quad v = v_0 + at
$$

> 💡 **Physical Intuition**: Acceleration times time equals the change in velocity. Every second that passes, the velocity increases by $a$. This is a **linear accumulation** perspective — final velocity = initial velocity + velocity change accumulated each second.

##### Method 3: From the Geometric Meaning of the v-t Graph

On a v-t graph, uniformly accelerated motion is a straight line with slope $a$, starting at $(0, v_0)$. The vertical coordinate at time $t$ is $v(t)$.

The point-slope equation of the line:

$$
v(t) - v_0 = a \cdot (t - 0)
$$

Rearranging:

$$
v(t) = v_0 + at
$$

> 💡 **Geometric Intuition**: The equation of a straight line on a v-t graph IS the velocity formula! Slope = acceleration, vertical intercept = initial velocity. This is more intuitive than algebraic symbols — graphs are always the best way to understand formulas.

#### 3.5.3 🧪 Derivation: Two More Ways to Derive Equation ②

Equation $\Delta x = v_0 t + \frac{1}{2}at^2$ reveals the relationship between displacement and time in uniformly accelerated motion.

##### Method 2: From Average Velocity

In uniformly accelerated linear motion, velocity changes linearly with time, so the average velocity equals the arithmetic mean of the initial and final velocities:

$$
\bar{v} = \frac{v_0 + v}{2}
$$

Substitute Equation ① $v = v_0 + at$:

$$
\bar{v} = \frac{v_0 + (v_0 + at)}{2} = v_0 + \frac{1}{2}at
$$

Displacement = average velocity × time:

$$
\Delta x = \bar{v} \cdot t = \left(v_0 + \frac{1}{2}at\right) \cdot t = v_0 t + \frac{1}{2}at^2
$$

> ⭐ **Key Understanding**: Only in **uniformly accelerated linear motion** does the average velocity equal the arithmetic mean of initial and final velocities! The elegance of this method lies in bypassing integration, but the prerequisite is that acceleration is constant.

##### Method 3: From the Area Under a v-t Graph

On a v-t graph, $v(t) = v_0 + at$ is a straight line. The area under the curve from $t=0$ to $t$ is a trapezoid.

The trapezoid's top base is $v_0$, bottom base is $v_0 + at$, and height is $t$:

$$
\text{Area} = \frac{(v_0) + (v_0 + at)}{2} \cdot t = v_0 t + \frac{1}{2}at^2
$$

> 💡 **Geometric Insight**: Decompose the trapezoid into a rectangle (area $v_0 t$, corresponding to displacement from uniform motion) and a triangle (area $\frac{1}{2} \cdot at \cdot t = \frac{1}{2}at^2$, the extra displacement contributed by acceleration). So $\Delta x = v_0 t + \frac{1}{2}at^2$ is simply **the sum of rectangle + triangle areas**!

#### 3.5.4 🧪 Derivation: Two More Ways to Derive Equation ③

Equation $v^2 = v_0^2 + 2a\Delta x$ does not contain the time variable, making it very useful for problems where time is not of interest.

##### Method 2: From Energy Conservation (Physics Perspective)

Under a constant force $F = ma$, the work done by the force equals the change in kinetic energy (work-energy principle):

$$
W = F \cdot \Delta x = ma \cdot \Delta x
$$

Change in kinetic energy:

$$
\Delta K = \frac{1}{2}mv^2 - \frac{1}{2}mv_0^2
$$

By the work-energy principle $W = \Delta K$:

$$
ma \cdot \Delta x = \frac{1}{2}mv^2 - \frac{1}{2}mv_0^2
$$

Cancel $m$ and rearrange:

$$
v^2 = v_0^2 + 2a\Delta x
$$

> ⭐ **Physical Essence**: Equation ③ is fundamentally the **energy conservation equation under a constant force**! $\frac{1}{2}mv^2 = \frac{1}{2}mv_0^2 + F \cdot \Delta x$ is a more fundamental physical law than the kinematic equations. This derivation also naturally explains why the sign handling of $v$ and $a$ in Equation ③ is different from energy (a scalar!) — work can be positive or negative.

##### Method 3: Eliminating Time from the v-t Graph

On a v-t graph, displacement $\Delta x$ is the trapezoid area, and time $t = \dfrac{v - v_0}{a}$ (from Equation ①).

Trapezoid area formula:

$$
\Delta x = \frac{v_0 + v}{2} \cdot t = \frac{v_0 + v}{2} \cdot \frac{v - v_0}{a}
$$

Simplify:

$$
\Delta x = \frac{(v_0 + v)(v - v_0)}{2a} = \frac{v^2 - v_0^2}{2a}
$$

Rearrange:

$$
v^2 = v_0^2 + 2a\Delta x
$$

> 💡 **Purely Geometric Method**: No calculus, no energy — just trapezoid area + algebraic elimination. This method could have been used in Galileo's era!

### 3.6 The Unified View of the Three Big Equations: Understanding Everything from the v-t Graph

The most profound way to understand the three big equations is to recognize that they all come from **the same v-t graph**:

```
v (m/s)
↑
│        ╱
│      ╱ |        v-t line: v(t) = v₀ + at
│    ╱   |
│  ╱     | Triangle area = ½at²
│╱_______| Rectangle area = v₀t
└──────────→ t    Total displacement = v₀t + ½at²
```

| What You Read from the Graph | The Formula You Get |
|:--|:--|
| The **vertical coordinate** of a point on the line | $v = v_0 + at$ (Equation ①) |
| The **total area** under the line | $\Delta x = v_0 t + \frac{1}{2}at^2$ (Equation ②) |
| **Eliminate $t$** from the area and coordinates | $v^2 = v_0^2 + 2a\Delta x$ (Equation ③) |

> ⭐ **Ultimate Understanding**: The three big equations are not three isolated formulas — they are **three different ways of reading the same v-t line**. Once you grasp this, you've truly understood uniformly accelerated motion.

#### 3.7 🧪 Example: The Pursuit Problem

**Problem**: A car travels at a constant speed of $20\ \text{m/s}$. The driver notices a truck $80\ \text{m}$ ahead traveling at $10\ \text{m/s}$ in the same direction. The driver immediately applies the brakes, producing a constant deceleration of $2\ \text{m/s}^2$.

(a) Will the car collide with the truck?
(b) If yes, how many seconds after braking does the collision occur?
(c) If no, what is the minimum distance between them?

**Solution**:

Let the car's initial position be $x=0$ and the truck's initial position be $x=80\ \text{m}$.

Car: $x_C(t) = 20t - \frac{1}{2} \times 2 \times t^2 = 20t - t^2$ (decelerating)
Truck: $x_T(t) = 80 + 10t$ (constant speed)

**(a)** A collision occurs when positions are equal:

$$
20t - t^2 = 80 + 10t
$$

$$
-t^2 + 10t - 80 = 0 \quad\Rightarrow\quad t^2 - 10t + 80 = 0
$$

Discriminant $\Delta = 100 - 320 = -220 < 0$, **no real solution** → **no collision** ✅

**(b)** No real solution means no collision.

**(c)** The distance between them is $d(t) = x_T(t) - x_C(t) = (80 + 10t) - (20t - t^2) = t^2 - 10t + 80$

This is an upward-opening quadratic. The minimum occurs at $t = -\frac{b}{2a} = \frac{10}{2} = 5\ \text{s}$:

$$
d_{min} = 5^2 - 10 \times 5 + 80 = 25 - 50 + 80 = \mathbf{55\ m}
$$

The minimum distance is **55 m** — no collision. ✅

> ⭐ **Key Strategy**: Set position equations equal to check for collisions. If there's no real solution, they don't collide. Find the minimum distance using quadratic optimization or the condition of zero relative velocity.

---

### IV. Free Fall Motion

#### 4.1 Key Points

> In the **absence of air resistance**, all objects at the **same location** fall with the **same gravitational acceleration** $g$.

- $g \approx 9.8\ \text{m/s}^2$ (near Earth's surface, directed vertically downward)
- Free fall is uniformly accelerated linear motion with **initial velocity 0** and **acceleration $g$ downward**

#### 4.2 Free Fall Equations

Let downward be positive, $v_0 = 0$, $a = g$:

| General Equation | Free Fall Form |
|:--|:--|
| $v = v_0 + at$ | $v = gt$ |
| $\Delta x = v_0 t + \frac{1}{2}at^2$ | $h = \frac{1}{2}gt^2$ |
| $v^2 = v_0^2 + 2a\Delta x$ | $v^2 = 2gh$ |

#### 4.3 🧪 Basic Example

**Problem**: A small ball is dropped from the top of a 45 m tall tower ($g = 10\ \text{m/s}^2$). Find:
(a) The time to reach the ground
(b) The velocity just before hitting the ground

**Solution**:

**(a)** Using $h = \frac{1}{2}gt^2$:
$$45 = \frac{1}{2} \times 10 \times t^2 \quad\Rightarrow\quad t^2 = 9 \quad\Rightarrow\quad t = \mathbf{3\ s}$$

**(b)** Using $v = gt$:
$$v = 10 \times 3 = \mathbf{30\ m/s}\ (\text{downward})$$

#### 4.4 🧪 Derivation: Free Fall Equations from Calculus

Starting from Newton's second law, free fall involves only gravity $F = mg$:

$$
a = \frac{F}{m} = g \quad (\text{directed downward})
$$

Let downward be positive. Integrate the acceleration to find velocity:

$$
v(t) = \int a\ dt = \int g\ dt = gt + C
$$

Using the initial condition $v(0) = 0$, we get $C = 0$, so:

$$
\boxed{v = gt}
$$

Integrate velocity to find position:

$$
y(t) = \int v(t)\ dt = \int gt\ dt = \frac{1}{2}gt^2 + D
$$

Using $y(0) = 0$, we get $D = 0$, so:

$$
\boxed{h = \frac{1}{2}gt^2}
$$

The equation $v^2 = 2gh$ can also be obtained by eliminating $t$ from $v = gt$ and $h = \frac{1}{2}gt^2$:

$$
t = \frac{v}{g} \quad\Rightarrow\quad h = \frac{1}{2}g\left(\frac{v}{g}\right)^2 = \frac{v^2}{2g} \quad\Rightarrow\quad \boxed{v^2 = 2gh}
$$

> 💡 **Advantage of Calculus**: If gravitational acceleration varies with height (e.g., $g(y)$ is not constant), the algebraic method fails, but the calculus method still works!

#### 4.5 🧪 Example: Complete Analysis of Vertical Projectile Motion

**Problem**: A ball is thrown straight upward with an initial speed of $30\ \text{m/s}$ ($g = 10\ \text{m/s}^2$, neglect air resistance).
Find:
(a) The time to reach the highest point
(b) The maximum height
(c) The total time from launch to return to the starting point
(d) The velocity just before returning to the starting point
(e) The velocity and position at $t = 2\ \text{s}$ and $t = 5\ \text{s}$

**Solution**:

Let upward be the positive direction, $v_0 = +30\ \text{m/s}$, $a = -g = -10\ \text{m/s}^2$.

**(a)** At the highest point, $v = 0$:

$$0 = 30 - 10t \quad\Rightarrow\quad t_{up} = \mathbf{3\ s}$$

**(b)** Maximum height:

$$H = v_0 t_{up} - \frac{1}{2}gt_{up}^2 = 30 \times 3 - 5 \times 9 = 90 - 45 = \mathbf{45\ m}$$

**(c)** Return to start when $y=0$:

$$0 = 30t - 5t^2 \quad\Rightarrow\quad t(30 - 5t) = 0$$
$$t = 0\ (\text{launch}),\quad t = \mathbf{6\ s}\ (\text{return})$$

> ⭐ Note that $t_{total} = 2 \times t_{up} = 6\ \text{s}$ — the ascent time equals the descent time (symmetry).

**(d)** Velocity upon return:

$$v = v_0 - gt = 30 - 10 \times 6 = -30\ \text{m/s}$$

The speed is $30\ \text{m/s}$, directed **downward** (opposite to the initial velocity). ✅

**(e)** At $t=2\ \text{s}$ (ascending):

$$v(2) = 30 - 20 = 10\ \text{m/s}\ (\text{upward})$$
$$y(2) = 30 \times 2 - 5 \times 4 = 60 - 20 = \mathbf{40\ m}\ (\text{still rising})$$

At $t=5\ \text{s}$ (descending):

$$v(5) = 30 - 50 = -20\ \text{m/s}\ (\text{downward})$$
$$y(5) = 30 \times 5 - 5 \times 25 = 150 - 125 = \mathbf{25\ m}\ (\text{past the highest point, falling})$$

> ⚠️ **Common AP Mistake**: Many students think the ball is still rising at $t=5\ \text{s}$, but it actually passed the highest point at $t=3\ \text{s}$ and is already on its way down!

---

## Part B: AP Difficulty Layer (Conceptual Traps & Deep Understanding)

---

### V. Real Conceptual Traps on the AP Exam

#### 🎯 Trap 1: Average Speed vs. Average Velocity — Values Can Differ Greatly

**AP Classic Problem**:

> A particle moves along a line with velocity $v(t) = 3t^2 - 12t + 9$ m/s for $0 \leq t \leq 4$ s.
> Find the **average speed** and **average velocity** over $[0, 4]$.

**Key**: First determine whether the object changes direction! Set $v(t)=0$:
$$3t^2 - 12t + 9 = 0 \quad\Rightarrow\quad t^2 - 4t + 3 = 0 \quad\Rightarrow\quad (t-1)(t-3)=0$$
Direction changes at $t=1$ and $t=3$.

Then calculate the path length in segments (requires integration) and divide by total time.

> ⚠️ **AP 1 doesn't test integration for path length** (that's AP C), but they will give you piecewise constant velocities to calculate manually!

#### 🎯 Trap 2: Negative Acceleration = Slowing Down? — ❌ Completely Wrong!

**AP Favorite Concept Question**:

> An object moves along the $x$-axis with velocity $v_x = -10\ \text{m/s}$ and acceleration $a_x = -2\ \text{m/s}^2$.
> Is the object speeding up or slowing down?

**Analysis**:
- $v_x = -10$ (moving left)
- $a_x = -2$ (acceleration is also to the left)
- Velocity and acceleration are in the **same direction** (both negative)

**Answer**: **Speeding up** ✅

> ⭐ **Core Understanding**:
> - **$\vec{v}$ and $\vec{a}$ in same direction** → **speeding up** (regardless of sign)
> - **$\vec{v}$ and $\vec{a}$ in opposite directions** → **slowing down**
>
> "Negative acceleration" only means the direction is opposite to the positive direction — it does **NOT mean slowing down**!

#### 🎯 Trap 3: The Mass Myth in Free Fall

**AP Classic Misconception**:

> ❌ "Heavier objects fall faster."

**Correct Answer**: In the absence of air resistance, **all objects**, regardless of mass, fall with the same acceleration $g$.

**Galileo's Leaning Tower of Pisa Experiment** (legendary) and modern verification:
- In a vacuum, a feather and a steel ball hit the ground at the same time ✅
- On Earth's surface, air resistance affects lighter objects, but **gravitational acceleration itself is independent of mass**

> 💡 **AP Exam Tip**: If the problem states "neglect air resistance," then all objects have the same downward acceleration $g$, regardless of mass!

#### 🎯 Trap 4: Braking Problems — Don't Forget to Check the Stopping Time! ⚠️

**AP Classic Trap**:

> A car is traveling at $20\ \text{m/s}$ when the driver applies brakes, causing a constant deceleration of $4\ \text{m/s}^2$.
> How far does the car travel before stopping?

**Wrong approach**: Directly substitute $t=5$ s into equation ②... 

Wait! Where does $t=5$ s come from? Using $v = v_0 + at$:
$$0 = 20 - 4t \quad\Rightarrow\quad t = 5\ \text{s}$$

This **5 s is the stopping time**. Correctly substitute into equation ③:
$$v^2 = v_0^2 + 2a\Delta x \quad\Rightarrow\quad 0 = 20^2 + 2(-4)\Delta x$$
$$\Delta x = \frac{400}{8} = \mathbf{50\ m}$$

**But** — what if the problem asks for the **displacement at $t = 7$ s**?

> ⚠️ **AP Super Trap**: The car stops at $t=5$ s! At $t=7$ s, the car has been stopped for 2 seconds, and the displacement is **still 50 m**, NOT the value you'd get by plugging $t=7$ into the equation!
>
> **Essential Check**: In braking problems, always calculate the **stopping time** first: $t_{stop} = \dfrac{v_0}{|a|}$!

#### 🎯 Trap 5: Projectile Motion — At the Highest Point, v=0, but a≠0!

**AP Physics 1 Must-Know Concept**:

> A ball is thrown straight upward. At the highest point of its motion:
>
> A) Both velocity and acceleration are zero.
> B) Velocity is zero, acceleration is zero.
> C) **Velocity is zero, acceleration is $g$ downward.**
> D) Velocity is maximum, acceleration is zero.

**Answer**: C ✅

> ⭐ **Key Understanding**:
> - At the highest point: $v = 0$ (instantaneously at rest)
> - At the highest point: $a = g$ downward **≠ 0** (gravity is always acting!)
>
> AP exam LOVES testing this — never choose B!

---

### VI. AP Physics C Calculus Depth

#### 6.1 From Algebra to Calculus: The Complete Framework

**Differentiation (from position to velocity to acceleration)**

$$
\vec{r}(t) \xrightarrow{\ \dfrac{d}{dt}\ } \vec{v}(t) = \frac{d\vec{r}}{dt} \xrightarrow{\ \dfrac{d}{dt}\ } \vec{a}(t) = \frac{d\vec{v}}{dt} = \frac{d^2\vec{r}}{dt^2}
$$

**Integration (from acceleration to velocity to position)**

$$
\vec{a}(t) \xrightarrow{\ \displaystyle\int dt\ } \vec{v}(t) = \vec{v}_0 + \int_{0}^{t} \vec{a}(\tau)\ d\tau \xrightarrow{\ \displaystyle\int dt\ } \vec{r}(t) = \vec{r}_0 + \int_{0}^{t} \vec{v}(\tau)\ d\tau
$$

#### 6.2 Uniform Acceleration as a Special Case of the Calculus Framework

When $\vec{a} = \text{constant}$:

$$
\vec{v}(t) = \vec{v}_0 + \int_0^t \vec{a}\ d\tau = \vec{v}_0 + \vec{a}t
$$

$$
\vec{r}(t) = \vec{r}_0 + \int_0^t (\vec{v}_0 + \vec{a}\tau)\ d\tau = \vec{r}_0 + \vec{v}_0 t + \frac{1}{2}\vec{a}t^2
$$

**See! The first two of the three big equations are obtained by integrating in the calculus framework!** ✅

#### 6.3 🧪 AP Physics C Exam-Style Example

> The acceleration of a particle moving along the $x$-axis is given by $a(t) = 6t - 4\ \text{m/s}^2$.
> At $t = 0$, the particle is at $x = 2\ \text{m}$ with velocity $v = 3\ \text{m/s}$.
>
> **(a)** Find the velocity function $v(t)$.
> **(b)** Find the position function $x(t)$.
> **(c)** Find the velocity at $t = 2$ s.
> **(d)** Find the displacement from $t = 0$ to $t = 3$ s.

**Solution**:

**(a)** Integrate the acceleration:

$$
v(t) = \int a(t)\ dt = \int (6t - 4)\ dt = 3t^2 - 4t + C
$$

Substitute $v(0) = 3$:
$$3 = 0 - 0 + C \quad\Rightarrow\quad C = 3$$

$$
\boxed{v(t) = 3t^2 - 4t + 3\ \text{m/s}}
$$

**(b)** Integrate the velocity:

$$
x(t) = \int v(t)\ dt = \int (3t^2 - 4t + 3)\ dt = t^3 - 2t^2 + 3t + D
$$

Substitute $x(0) = 2$:
$$2 = 0 - 0 + 0 + D \quad\Rightarrow\quad D = 2$$

$$
\boxed{x(t) = t^3 - 2t^2 + 3t + 2\ \text{m}}
$$

**(c)** Substitute $t=2$:

$$
v(2) = 3(4) - 4(2) + 3 = 12 - 8 + 3 = \mathbf{7\ m/s}
$$

**(d)** Displacement $\Delta x = x(3) - x(0)$:

$$
x(3) = 27 - 18 + 9 + 2 = 20
$$
$$
x(0) = 2
$$
$$
\Delta x = 20 - 2 = \mathbf{18\ m}
$$

#### 6.4 Connection to Variable Forces and Newton's Second Law (AP C Advanced)

In AP Physics C, acceleration is often linked to force:

$$
\vec{F}_{net} = m\vec{a} = m\frac{d\vec{v}}{dt} = m\frac{d^2\vec{r}}{dt^2}
$$

When force varies with time:

$$
\vec{F}(t) = m\vec{a}(t) \quad\Rightarrow\quad \vec{a}(t) = \frac{\vec{F}(t)}{m}
$$

Then integrate to find velocity and position:

$$
\vec{v}(t) = \vec{v}_0 + \int_0^t \frac{\vec{F}(\tau)}{m}\ d\tau
$$

$$
\vec{r}(t) = \vec{r}_0 + \int_0^t \vec{v}(\tau)\ d\tau
$$

#### 6.5 Dot Product for Speeding Up / Slowing Down (AP C 2D Motion)

In two-dimensional motion, use the **dot product of velocity and acceleration** to determine whether the object is speeding up or slowing down:

$$
\vec{v} \cdot \vec{a} \; \begin{cases}
> 0 & \text{speeding up} \\
< 0 & \text{slowing down} \\
= 0 & \text{constant speed (e.g., uniform circular motion)}
\end{cases}
$$

> This is the **practical application** of the dot product method introduced in Section 1.1!

---

### VII. AP Exam Difficulty Level Summary

| Level | Corresponding Exam | Core Requirements | Typical Problem Features |
|:--|:--|:--|:--|
| **Level 1: Formula Application** | School midterms | Memorize the three big equations, substitute values | Given $v_0, a, t$, find $v$ or $\Delta x$ |
| **Level 2: Conceptual Analysis** | **AP Physics 1 & 2** 🎯 | Distinguish average vs. instantaneous, speeding up vs. slowing down, braking check, highest point analysis | Highest point v=0 but a≠0, braking stopping time, sign of acceleration ≠ speeding up/slowing down |
| **Level 3: Calculus Applications** | **AP Physics C** 🎯 | Integrate $a(t)$ to find $v(t)$, integrate again to find $x(t)$; differentiate in reverse | $a(t)=6t-4$ with initial conditions → find $x(t)$; differentiate $x(t)$ to get $v(t)$ and $a(t)$ |

---

### VIII. AP-Level Practice Problems

#### 🟢 AP Physics 1 Style

> A ball is thrown **downward** from a cliff with initial speed $5\ \text{m/s}$.
> The cliff is $60\ \text{m}$ high. ($g = 10\ \text{m/s}^2$)
>
> (a) How long does it take to reach the ground?
> (b) What is the velocity just before hitting the ground?
> (c) How far does it fall in the last second of its motion?

**Solution**:

Set downward as positive, $v_0 = +5\ \text{m/s}$, $a = +g = 10\ \text{m/s}^2$, $\Delta y = 60\ \text{m}$

**(a)** Using $\Delta y = v_0 t + \frac{1}{2}gt^2$:
$$60 = 5t + 5t^2 \quad\Rightarrow\quad t^2 + t - 12 = 0$$
$$(t+4)(t-3)=0 \quad\Rightarrow\quad t = \mathbf{3\ s} \quad (t=-4\ \text{rejected})$$

**(b)** Using $v = v_0 + gt$:
$$v = 5 + 10(3) = \mathbf{35\ m/s}\ (\text{downward})$$

**(c)** "Last second" = from $t=2$ s to $t=3$ s:
- $y(2) = 5(2) + \frac{1}{2}(10)(4) = 10 + 20 = 30\ \text{m}$
- $y(3) = 60\ \text{m}$ (ground)
- Distance fallen in last second $= 60 - 30 = \mathbf{30\ m}$ ✅

> ⚠️ **AP Trap**: Don't just use the formula with $v_0=5$ to calculate the displacement in 1 second — that gives the first second, not the last second!

#### 🔵 AP Physics C Style

> A particle moves along the $x$-axis with acceleration $a(t) = 12t^2 - 6\ \text{m/s}^2$.
> At $t = 0$, $x = 1\ \text{m}$ and $v = -4\ \text{m/s}$.
>
> (a) Find $v(t)$ and $x(t)$.
> (b) At what time(s) does the particle come to rest?
> (c) Find the displacement from $t = 0$ to $t = 2$ s.
> (d) Find the total distance traveled from $t = 0$ to $t = 2$ s.

**Solution**:

**(a)** Integrate $a(t)$ to find $v(t)$:

$$
v(t) = \int (12t^2 - 6)\ dt = 4t^3 - 6t + C
$$

Substitute $v(0) = -4$:
$$-4 = 0 - 0 + C \quad\Rightarrow\quad C = -4$$

$$
\boxed{v(t) = 4t^3 - 6t - 4\ \text{m/s}}
$$

Integrate $v(t)$ to find $x(t)$:

$$
x(t) = \int (4t^3 - 6t - 4)\ dt = t^4 - 3t^2 - 4t + D
$$

Substitute $x(0) = 1$:
$$1 = 0 - 0 - 0 + D \quad\Rightarrow\quad D = 1$$

$$
\boxed{x(t) = t^4 - 3t^2 - 4t + 1\ \text{m}}
$$

**(b)** "Come to rest" means $v(t) = 0$:

$$4t^3 - 6t - 4 = 0 \quad\Rightarrow\quad 2t^3 - 3t - 2 = 0$$

Use a calculator to find the root: $t \approx 1.46$ s (only one real root since $4t^3 - 6t - 4$ is an increasing function)

**(c)** Displacement $\Delta x = x(2) - x(0)$:

$$
x(2) = 16 - 12 - 8 + 1 = -3
$$
$$
x(0) = 1
$$
$$
\Delta x = -3 - 1 = \mathbf{-4\ m}
$$

**(d)** Total distance requires two segments (turning point at $t \approx 1.46$):

From $t=0$ to $t=1.46$ (moving left): $\Delta x_1 = x(1.46) - x(0) \approx -6.69 - 1 = -7.69$, distance $d_1 = 7.69$ m

From $t=1.46$ to $t=2$ (moving right): $\Delta x_2 = x(2) - x(1.46) \approx -3 - (-6.69) = 3.69$, distance $d_2 = 3.69$ m

Total distance $d = 7.69 + 3.69 \approx \mathbf{11.38\ m}$ ✅

> ⭐ **AP C Grading Emphasis**: As long as your approach is correct — find the turning points, separate into intervals, take absolute values — you'll get most of the credit even with approximate numerical values!

---

### IX. Topic Frequency Statistics

| Topic | AP 1 Frequency | AP C Frequency | Notes |
|:--|:--:|:--:|:--|
| Average Velocity Formula | ⭐⭐⭐⭐ | ⭐⭐⭐ | Basic calculation |
| Three Big Equations | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | AP 1 core tool |
| Free Fall / Vertical Projectile Motion | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | AP 1 must-know scenario |
| Braking Stopping Time Check | ⭐⭐⭐⭐ | ⭐⭐⭐ | High-frequency trap |
| Highest Point $v=0,\ a\neq0$ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | Must-know concept |
| Sign of $a$ vs. Speeding Up/Slowing Down | ⭐⭐⭐⭐ | ⭐⭐⭐ | Conceptual distinction |
| Integrate $a(t)$ to find $v(t), x(t)$ | — | ⭐⭐⭐⭐⭐ | AP C core skill |
| Differentiate $x(t)$ to find $v(t), a(t)$ | — | ⭐⭐⭐⭐⭐ | AP C core skill |
| Path Length with Turning Points | — | ⭐⭐⭐⭐ | FRQ essential |
| Variable Force $F=ma$ Integration | — | ⭐⭐⭐⭐ | AP C integrated problems |

---
---


# 1.3 Kinematics Graph Analysis

---

## Part A: Foundation Layer (AP Physics 1 & 2 Essentials)

---

### I. Position-Time Graphs (x-t Graphs)

#### 1.3.1 Core Concepts

> **The slope of an x-t graph at any point = the instantaneous velocity at that time**

$$
\boxed{v(t) = \text{slope of } x(t) \text{ at time } t = \frac{dx}{dt}}
$$

#### 1.3.2 Meaning of Different Shapes

| x-t Graph Feature | Corresponding Motion | Velocity |
|:--|:--|:--|
| ✅ Straight line (positive slope) | Uniform motion to the right | $v$ = positive constant |
| ✅ Straight line (negative slope) | Uniform motion to the left | $v$ = negative constant |
| ✅ Straight line (zero slope / horizontal) | At rest | $v = 0$ |
| 🔼 Curve bending upward (convex up) | Speeding up | $v$ increasing |
| 🔽 Curve bending downward (concave down) | Slowing down | $v$ decreasing |
| 🔄 Parabolic shape | Uniformly accelerated / decelerated motion | $v$ changing linearly |

#### 1.3.3 🧪 Basic Example: Reading Velocity from an x-t Graph

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

This is a straight line through the origin, slope $= \frac{6-0}{3-0} = 2\ \text{m/s}$

So the object is moving to the right at a **constant velocity of $2\ \text{m/s}$**.

#### 1.3.4 Geometric Meaning of Average Velocity on an x-t Graph

$$
\bar{v} = \frac{\Delta x}{\Delta t} = \text{slope of the secant line connecting start and end points}
$$

- Instantaneous velocity $v(t)$ = slope of the **tangent line** at that point
- Average velocity $\bar{v}$ = slope of the **secant line** from start to end

> 💡 **The Difference**: A secant looks at the whole picture; a tangent looks at a single instant.

---

### II. Velocity-Time Graphs (v-t Graphs)

#### 2.1 Core Concepts

The v-t graph is **the most important graph in AP Physics** because it contains two types of information:

$$
\boxed{\text{slope} = \text{acceleration} \quad\quad \text{area} = \text{displacement}}
$$

##### Slope ⇒ Acceleration

$$
a(t) = \text{slope of } v(t) \text{ at time } t = \frac{dv}{dt}
$$

##### Area ⇒ Displacement

$$
\Delta x = \text{area under } v(t) \text{ curve} = \int_{t_i}^{t_f} v(t)\ dt
$$

> ⚠️ **Note**:
> - Area **above** the $t$-axis → **positive displacement** (to the right)
> - Area **below** the $t$-axis → **negative displacement** (to the left)
> - **Net displacement** = total area above − total area below
> - **Total distance** = total area above + total area below (both taken as absolute values)

#### 2.2 Meaning of Different Shapes

| v-t Graph Feature | Corresponding Motion | Acceleration |
|:--|:--|:--|
| ✅ Horizontal line ($v \neq 0$) | Uniform linear motion | $a = 0$ |
| ✅ Horizontal line ($v = 0$) | At rest | $a = 0$ |
| ✅ Slanted line (positive slope) | Uniformly accelerating | $a$ = positive constant |
| ✅ Slanted line (negative slope) | Uniformly decelerating | $a$ = negative constant |
| 🔼 Curve bending upward | Acceleration increasing | $a$ increasing |
| 🔽 Curve bending downward | Acceleration decreasing | $a$ decreasing |

#### 2.3 🧪 Basic Example

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

- **Slope** $= \frac{6-0}{3-0} = 2\ \text{m/s}^2$ → acceleration is $2\ \text{m/s}^2$
- **Area** (triangle) $= \frac{1}{2} \times 3 \times 6 = 9\ \text{m}$ → displacement is $9\ \text{m}$

---

### III. Acceleration-Time Graphs (a-t Graphs)

#### 3.1 Core Concepts

$$
\boxed{\text{area} = \text{change in velocity}}
$$

$$
\Delta v = \text{area under } a(t) \text{ curve} = \int_{t_i}^{t_f} a(t)\ dt
$$

#### 3.2 Meaning of Different Shapes

| a-t Graph Feature | Corresponding Motion | Velocity Behavior |
|:--|:--|:--|
| ✅ Horizontal line ($a \neq 0$) | Uniform acceleration/deceleration | $v$ changing linearly |
| ✅ Horizontal line ($a = 0$) | Uniform motion or at rest | $v$ constant |
| 🔼 Slanted line | Acceleration changing uniformly | $v$ changing quadratically |

#### 3.3 🧪 Basic Example

```
a (m/s²)
↑
3 ┤╱╱╱╱╱╱╱╱╱
2 ┤╱╱╱╱╱╱╱╱╱
1 ┤╱╱╱╱╱╱╱╱╱
0 ┼──────────────────→ t (s)
   0  1  2  3  4  5
```

**Area** from $t=0$ to $t=4$ s $= 3 \times 4 = 12$ → change in velocity $\Delta v = 12\ \text{m/s}$

If $v_0 = 0$, then $v(4) = 12\ \text{m/s}$

---

### IV. Converting Between the Three Types of Graphs

#### 4.1 Conversion Relationship Diagram

```
  x-t Graph
    │
    │ Differentiate (slope)
    ▼
  v-t Graph ──── Differentiate (slope) ────▶ a-t Graph
    │                                         │
    │ Integrate (area)                         │ Integrate (area)
    ▼                                         ▼
  Δx (displacement)                         Δv (change in velocity)
```

#### 4.2 Given x-t Graph → Draw v-t Graph

| Step | Operation |
|:--|:--|
| **1** | Identify key points on the x-t graph (turning points, inflection points) |
| **2** | Find the **slope** of each segment (= velocity) |
| **3** | Plot those slope values on the v-t graph for the corresponding time intervals |

**🧪 Example**:

```
x-t:                      v-t:
x ↑                       v ↑
  |     ╱╲                  |    ╱╲
  |   ╱   ╲    ╱            |  ╱   ╲    ╱
  | ╱      ╲  ╱             |╱      ╲  ╱
  |╱        ╲╱              |        ╲╱
  └───────→ t               └─────────→ t
```

- x-t slope decreasing from positive to 0 → v-t decreasing from positive to 0
- x-t slope becomes negative with increasing magnitude → v-t increasing in negative direction

#### 4.3 Given v-t Graph → Draw a-t Graph

| Step | Operation |
|:--|:--|
| **1** | Find the **slope** of each segment on the v-t graph (= acceleration) |
| **2** | Plot those slope values on the a-t graph |

#### 4.4 Given v-t Graph → Draw x-t Graph

| Step | Operation |
|:--|:--|
| **1** | Choose a starting position $x_0$ |
| **2** | Calculate the **area** under each segment of the v-t graph (= displacement) |
| **3** | Plot cumulative displacements on the x-t graph |

#### 4.5 🧪 Comprehensive Conversion Example

**Problem**: Given the following v-t graph, draw the corresponding a-t graph and x-t graph (let $x_0 = 0$).

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

**Solution**:

**a-t graph**: v-t slopes are constant (straight segments) ⇒ a is piecewise constant

- $0 \leq t \leq 2$: slope $= \frac{4-0}{2-0} = 2$ ⇒ $a = 2\ \text{m/s}^2$
- $2 \leq t \leq 4$: slope $= \frac{0-4}{4-2} = -2$ ⇒ $a = -2\ \text{m/s}^2$
- $t > 4$: slope $= 0$ ⇒ $a = 0$

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

**x-t graph**: Calculate the area under the v-t graph (cumulative displacement)

- $t=2$: area $= \frac{1}{2} \times 2 \times 4 = 4$ m
- $t=4$: area $= 4 + \frac{1}{2} \times 2 \times 4 = 8$ m
- $t=5$: area $= 8 + 0 = 8$ m (at rest afterward)

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

#### 4.6 🧪 Derivation: Mathematical Proof that v-t Area = Displacement

**Core idea**: Divide the time axis into many infinitesimally small intervals $\Delta t_i$. During each $\Delta t_i$, the velocity is approximately constant (uniform motion), so the displacement $\Delta x_i \approx v(t_i) \Delta t_i$.

As $\Delta t_i \to 0$, the approximation becomes exact:

$$
\Delta x = \lim_{\Delta t_i \to 0} \sum_i v(t_i) \Delta t_i = \int_{t_i}^{t_f} v(t)\ dt
$$

This is precisely the **Riemann sum → definite integral** process:

```
v(t)
↑
│    ╱╲
│  ╱   ╲     Each small rectangle area ≈ v(tᵢ)·Δtᵢ
│╱      ╲    Total area → displacement
└─────────→ t
  Δtᵢ
```

**Geometric meaning**: The area bounded by the v-t curve and the $t$-axis equals the displacement.

> 💡 **Analogy**: Just like approximating the area under a curve with many tiny rectangles — as the rectangle width approaches 0, the total area equals the definite integral.

#### 4.6.2 🧪 Derivation: Three Validations of the Fundamental Theorem of Calculus in Kinematics

In Section 1.3, the core of graph analysis rests on three relationships:
1. **x-t slope = velocity**: $v = dx/dt$
2. **v-t slope = acceleration**: $a = dv/dt = d^2x/dt^2$
3. **v-t area = displacement**: $\Delta x = \int v\ dt$

These three relationships can be understood and verified using three complementary approaches.

##### Validation 1: Verify the Slope-Area Relationship Using Uniformly Accelerated Motion

Take the displacement function for uniformly accelerated motion $x(t) = v_0 t + \frac{1}{2}at^2$:

Differentiate to get velocity: $v(t) = \frac{dx}{dt} = v_0 + at$ ✓ (x-t slope = velocity)

Differentiate again to get acceleration: $a(t) = \frac{dv}{dt} = a$ ✓ (v-t slope = acceleration)

Conversely, integrate $v(t)$: $\int_0^t (v_0 + a\tau)\ d\tau = v_0 t + \frac{1}{2}at^2 = x(t) - x(0)$ ✓ (v-t area = change in displacement)

> 💡 **Essence of the Fundamental Theorem of Calculus**: Differentiation (slope) and integration (area) are **inverse operations**. This is precisely Newton and Leibniz's greatest discovery.

##### Validation 2: Understanding Slope via Numerical Differences

When $\Delta t$ is very small, the derivative can be approximated by a difference quotient:

$$
v(t) = \frac{dx}{dt} \approx \frac{x(t+\Delta t) - x(t)}{\Delta t}
$$

This is the foundation of numerical methods for solving differential equations and the mathematical essence of finding tangent slopes on an x-t graph. As $\Delta t \to 0$, the secant becomes the tangent, and the average velocity becomes the instantaneous velocity.

##### Validation 3: Approximating Area via Riemann Sums

The area under a v-t graph can be approximated by summing rectangles. Divide the interval $[0, t]$ into $n$ equal parts, each of width $\Delta t = t/n$:

$$
\Delta x \approx \sum_{i=1}^{n} v(t_i) \Delta t
$$

Taking the limit $n \to \infty$ (i.e., $\Delta t \to 0$), the approximation becomes exact:

$$
\Delta x = \lim_{n \to \infty} \sum_{i=1}^{n} v(t_i) \Delta t = \int_0^t v(\tau)\ d\tau
$$

> ⭐ **Practical application on AP C**: If you're given a nonlinear $v(t)$ function, you cannot use the trapezoid formula — you must use a definite integral! But if you're given a piecewise linear graph, you can use the trapezoid formula to find the area — this is very common in AP Physics 1.

#### 4.6.3 Deep Understanding: Why the Area Under a v-t Graph Equals Displacement

We can build an intuitive understanding using a simple physical scenario.

Suppose an object moves with a changing speed. We slice time into extremely thin segments $\Delta t$. Within each tiny time segment, the velocity is almost constant (because velocity doesn't change significantly over an extremely short time interval).

For the $i$-th time segment, the object travels approximately $v(t_i) \cdot \Delta t$. Summing the displacements from all segments:

$$
\text{Total displacement} \approx \sum_{i} v(t_i) \cdot \Delta t
$$

On a v-t graph, each $v(t_i) \cdot \Delta t$ is the area of a thin rectangle. As $\Delta t$ approaches zero, the total area of all rectangles precisely equals the area under the curve:

$$
\text{Displacement} = \lim_{\Delta t \to 0} \sum_i v(t_i) \cdot \Delta t = \int_{t_i}^{t_f} v(t)\ dt
$$

> ⭐ **In one sentence**: **Velocity is the rate at which displacement accumulates** — the faster you move at any given instant, the more displacement you accumulate per unit time. The area under the v-t graph is the geometric manifestation of this "accumulation effect."

#### 4.7 🧪 Example: Drawing Motion Graphs from a Verbal Description

**Problem**: An object moves along the $x$-axis with the following motion:
- $0 \to 2\ \text{s}$: Starts at the origin, moves right at a constant $3\ \text{m/s}$
- $2 \to 4\ \text{s}$: Decelerates uniformly at $-2\ \text{m/s}^2$
- $4 \to 6\ \text{s}$: Moves left at a constant $1\ \text{m/s}$

Draw (a) the x-t graph, (b) the v-t graph, and (c) the a-t graph.

**Solution**:

**Step 1: Write the piecewise functions**

Let the positive $x$-direction be to the right.

$0 \to 2\ \text{s}$: constant velocity $v = 3\ \text{m/s}$, $x(t) = 3t$

$2 \to 4\ \text{s}$: uniformly decelerating, $v_0 = 3\ \text{m/s}$, $a = -2\ \text{m/s}^2$
- $v(t) = 3 - 2(t-2) = 7 - 2t$
- $x(2) = 6\ \text{m}$, $x(t) = 6 + 3(t-2) - (t-2)^2$

$4 \to 6\ \text{s}$: constant velocity left, $v = -1\ \text{m/s}$, $x(4) = 6 + 3(2) - 4 = 8\ \text{m}$
- $x(t) = 8 - (t-4)$

**Step 2: The v-t graph**

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

- $0 \to 2$: horizontal line at $v=3$
- $2 \to 4$: slanted line, $v$ decreasing from $3$ to $-1$
- $4 \to 6$: horizontal line at $v=-1$

**Step 3: The a-t graph**

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

- $0 \to 2$: $a = 0$
- $2 \to 4$: $a = -2\ \text{m/s}^2$
- $4 \to 6$: $a = 0$

**Step 4: The x-t graph**

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

- $0 \to 2$: straight line with slope $3$
- $2 \to 4$: downward-opening parabola (slope decreasing from positive to negative)
- $4 \to 6$: straight line with slope $-1$, position decreasing from $8\ \text{m}$ to $6\ \text{m}$

> ⭐ **Key Skill**: Being able to work backwards from a verbal description to construct motion graphs is an advanced AP Physics 1 graph skill!

---

## Part B: AP Difficulty Layer (Conceptual Traps & Deep Understanding)

---

### V. Real Conceptual Traps on the AP Exam

#### 🎯 Trap 1: The Area Under a v-t Graph is Displacement, NOT Distance!

> Many students know "area = displacement," but AP asks about distance — that's when you need to take absolute values!

**🧪 Classic Problem**:

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

**Find**: (a) Displacement and (b) Distance from $t=0$ to $t=4$.

- Displacement $= \text{positive area} - \text{negative area} = \frac{1}{2}\times 3 \times 3 - \frac{1}{2} \times 1 \times 1 = 4.5 - 0.5 = \mathbf{4\ m}$
- Distance $= \text{positive area} + |\text{negative area}| = 4.5 + 0.5 = \mathbf{5\ m}$

> ⚠️ **AP Trap**: If the problem asks "total distance traveled," that's distance! If it asks "displacement," that's displacement!

#### 🎯 Trap 2: Slope of x-t Graph is Velocity, But What Does the Curvature Mean?

| x-t Curve Shape | Meaning |
|:--|:--|
| Convex up (bending upward) | $v$ is increasing (speeding up) |
| Concave down (bending downward) | $v$ is decreasing (slowing down) |

But this is just **first-order information**. AP C goes further and asks about **second-order information**:

- Convex up ⇒ $v$ increasing ⇒ $a > 0$
- Concave down ⇒ $v$ decreasing ⇒ $a < 0$

> 💡 This is determined by the **second derivative**: when x-t is convex up, $\frac{d^2x}{dt^2} = a > 0$!

#### 🎯 Trap 3: The Slope of x-t is Velocity — But Know the Difference Between Tangent and Secant!

**AP Must-Know Multiple Choice**:

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

**Analysis**: The slope (tangent) of the x-t curve decreases as $t$ increases ⇒ velocity is decreasing ⇒ answer is C.

> ⭐ **AP Point**: It's not about the curve itself, but about **how the slope of the curve changes**!

#### 🎯 Trap 4: The Area Under an a-t Graph is $\Delta v$, NOT $v$!

**AP Classic Mistake**:

> Students see the area under an a-t graph and say, "That's the velocity."

**Correct Answer**:
$$v(t) = v_0 + \text{area under } a(t) \text{ from } 0 \text{ to } t$$

> ⚠️ The area gives the **change in velocity $\Delta v$**, and you must add the initial velocity $v_0$ to get $v(t)$!

#### 🎯 Trap 5: Identifying "Turning Points" in Graph Conversions

AP exams often give you one graph and ask you to draw another — **knowing how turning points correspond** is crucial!

| Original Graph | Key Feature | Corresponds to in Target Graph |
|:--|:--|:--|
| x-t inflection point (slope changes) | Turning point in v-t |
| x-t horizontal tangent ($v=0$) | v-t intersects t-axis |
| v-t inflection point (slope changes) | Turning point in a-t |
| v-t intersects t-axis ($v=0$) | Object changes direction |
| v-t extremum (slope = 0) | a-t intersects t-axis ($a=0$) |

#### 🎯 Trap 6: AP Classic — Which Set of Graphs Cannot Represent the Same Motion?

**AP Physics 1 Exam Style**:

> Which of the following sets of graphs could **NOT** represent the motion of the same object?

This type of question tests **consistency between graphs**:

- If x-t is a parabola opening upward ⇒ v-t should be a straight line with positive slope ⇒ a-t should be a horizontal line at a positive constant
- If v-t is a horizontal line ⇒ a-t should be a horizontal line at 0, and x-t should be a straight slanted line

> ⚠️ **AP Trap**: One set of graphs in the options may look almost right, but the slope/area relationships don't match!

---

### VI. AP Physics C Calculus Depth

#### 6.1 The Fundamental Theorem of Calculus Unified in Kinematics

AP Physics C requires you to truly understand that **slope = derivative, area = integral**:

##### Differential Perspective (Slope)

$$
v(t) = \frac{dx}{dt} \quad\longleftrightarrow\quad \text{tangent slope of x-t graph}
$$

$$
a(t) = \frac{dv}{dt} = \frac{d^2x}{dt^2} \quad\longleftrightarrow\quad \text{tangent slope of v-t graph}
$$

##### Integral Perspective (Area)

$$
\Delta x = \int_{t_i}^{t_f} v(t)\ dt \quad\longleftrightarrow\quad \text{area under v-t curve}
$$

$$
\Delta v = \int_{t_i}^{t_f} a(t)\ dt \quad\longleftrightarrow\quad \text{area under a-t curve}
$$

#### 6.2 Fundamental Theorem of Calculus in Kinematics

$$
\boxed{\frac{d}{dt} \int_{a}^{t} f(\tau)\ d\tau = f(t)}
$$

In kinematics:

$$
\frac{d}{dt} \left[ \int_{0}^{t} v(\tau)\ d\tau \right] = v(t)
$$

This means: **The derivative of the area function = the original function** — this is the mathematical essence of graph conversion!

#### 6.3 🧪 AP Physics C Exam-Style Example

> The velocity of a particle moving along the $x$-axis is given by $v(t) = 3t^2 - 12t + 9$ m/s for $t \geq 0$.
>
> **(a)** Find the acceleration function $a(t)$.
> **(b)** At what time(s) does the particle change direction?
> **(c)** Find the displacement from $t = 0$ to $t = 4$ s.
> **(d)** Find the total distance traveled from $t = 0$ to $t = 4$ s.
> **(e)** Sketch $v(t)$ and $a(t)$ on the same axes for $0 \leq t \leq 4$.

**Solution**：

**(a)** Differentiate:

$$
a(t) = \frac{dv}{dt} = 6t - 12\ \text{m/s}^2
$$

**(b)** Change direction when $v(t) = 0$:

$$3t^2 - 12t + 9 = 0 \quad\Rightarrow\quad t^2 - 4t + 3 = 0$$
$$(t-1)(t-3) = 0 \quad\Rightarrow\quad t = \mathbf{1\ s, \ 3\ s}$$

**(c)** Displacement = net area under v-t curve (integral):

$$
\Delta x = \int_{0}^{4} (3t^2 - 12t + 9)\ dt
$$

$$
= \left[ t^3 - 6t^2 + 9t \right]_{0}^{4}
$$

$$
= (64 - 96 + 36) - (0) = \mathbf{4\ m}
$$

**(d)** Total distance requires three segments ($0 \to 1$, $1 \to 3$, $3 \to 4$), taking absolute values of each:

**Interval [$0$, $1$]: $v \geq 0$**

$$
d_1 = \int_{0}^{1} (3t^2 - 12t + 9)\ dt = \left[ t^3 - 6t^2 + 9t \right]_{0}^{1} = 1 - 6 + 9 = 4\ \text{m}
$$

**Interval [$1$, $3$]: $v \leq 0$**

$$
d_2 = \left| \int_{1}^{3} (3t^2 - 12t + 9)\ dt \right| = \left| \left[ t^3 - 6t^2 + 9t \right]_{1}^{3} \right|
$$

$$
= |(27 - 54 + 27) - (1 - 6 + 9)| = |0 - 4| = 4\ \text{m}
$$

**Interval [$3$, $4$]: $v \geq 0$**

$$
d_3 = \int_{3}^{4} (3t^2 - 12t + 9)\ dt = \left[ t^3 - 6t^2 + 9t \right]_{3}^{4}
$$

$$
= (64 - 96 + 36) - (27 - 54 + 27) = 4 - 0 = 4\ \text{m}
$$

**Total distance**:

$$
d = d_1 + d_2 + d_3 = 4 + 4 + 4 = \mathbf{12\ m}
$$

> ⭐ **AP C Core Point**: The difference between displacement and distance — displacement is the algebraic sum of integrals, while distance is the sum of absolute values!

**(e)** Sketch:

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

- $v(t)$ is an upward-opening parabola, minimum at $t=2$: $v(2) = -3$ m/s
- $a(t)$ is a straight line with positive slope, $a=0$ at $t=2$
- When $t < 2$: $a < 0$ (slowing down), when $t > 2$: $a > 0$ (speeding up)

#### 6.4 Advanced Application: Determining Acceleration Direction from x-t Curvature (AP C)

AP C requires you to determine acceleration direction directly from the **curvature (second derivative)** of an x-t graph:

| x-t Curve | 1st Derivative $v$ | 2nd Derivative $a$ | Motion State |
|:--|:--:|:--:|:--|
| Convex up (bending upward) | $v > 0$ | $a > 0$ | Speeding up in positive direction |
| Convex up (bending upward) | $v < 0$ | $a > 0$ | Slowing down in negative direction |
| Concave down (bending downward) | $v > 0$ | $a < 0$ | Slowing down in positive direction |
| Concave down (bending downward) | $v < 0$ | $a < 0$ | Speeding up in negative direction |

> 💡 **Memory Aid**: Convex up = positive acceleration (like a smile 😊), concave down = negative acceleration (like a frown 😞)

---

### VII. AP Exam Difficulty Level Summary

| Level | Corresponding Exam | Core Requirements | Typical Problem Features |
|:--|:--|:--|:--|
| **Level 1: Reading Values** | School midterms | Read slope from x-t for velocity; read slope from v-t for acceleration, area for displacement | "Find the velocity at $t=2$" |
| **Level 2: Graph Conversion** | **AP Physics 1 & 2** 🎯 | Convert between x-t → v-t → a-t; identify which set of graphs cannot represent the same motion | "Which set could NOT represent the same motion?" |
| **Level 3: Calculus Analysis** | **AP Physics C** 🎯 | Use integration for exact area, differentiation for exact slope; find total distance from $v(t)$ function (piecewise integration) | $v(t)=3t^2-12t+9$ — find total distance |

---

### VIII. AP-Level Practice Problems

#### 🟢 AP Physics 1 Style

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

**Solution**:

**(a)** $0 \to 2$ s: slope $= \frac{4-0}{2-0} = \mathbf{2\ m/s^2}$ ✅

**(b)** Displacement = net area under v-t:

- $0 \to 2$: triangle area $= \frac{1}{2} \times 2 \times 4 = 4$ m
- $2 \to 3$: triangle area $= \frac{1}{2} \times 1 \times 4 = 2$ m (positive)
- $3 \to 4$: triangle area $= \frac{1}{2} \times 1 \times (-2) = -1$ m (negative)

Net displacement $= 4 + 2 + (-1) = \mathbf{5\ m}$ ✅

**(c)** Total distance $= 4 + 2 + 1 = \mathbf{7\ m}$ ✅

**(d)** The object changes direction at $t=3$ s (when $v=0$), and is farthest from start at that point: $x(3) = 4 + 2 = \mathbf{6\ m}$ ✅

#### 🔵 AP Physics C Style

> A particle moves along the $x$-axis with acceleration $a(t) = 4t - 6\ \text{m/s}^2$.
> At $t = 0$, $x = 0$ and $v = 8\ \text{m/s}$.
>
> (a) Find $v(t)$ and $x(t)$.
> (b) At what time(s) is the particle at rest?
> (c) Find the displacement and total distance for $0 \leq t \leq 4$.
> (d) Sketch $v(t)$ and indicate on the graph the area that represents displacement.

**Solution**:

**(a)** Integrate to find $v(t)$:

$$
v(t) = \int (4t - 6)\ dt = 2t^2 - 6t + C
$$

Substitute $v(0) = 8$:

$$
8 = 0 - 0 + C \quad\Rightarrow\quad C = 8
$$

$$
\boxed{v(t) = 2t^2 - 6t + 8\ \text{m/s}}
$$

Integrate again to find $x(t)$:

$$
x(t) = \int (2t^2 - 6t + 8)\ dt = \frac{2}{3}t^3 - 3t^2 + 8t + D
$$

Substitute $x(0) = 0$:

$$
0 = 0 + D \quad\Rightarrow\quad D = 0
$$

$$
\boxed{x(t) = \frac{2}{3}t^3 - 3t^2 + 8t\ \text{m}}
$$

**(b)** At rest means $v(t) = 0$:

$$2t^2 - 6t + 8 = 0 \quad\Rightarrow\quad t^2 - 3t + 4 = 0$$

Discriminant $\Delta = 9 - 16 = -7 < 0$, **no real solutions**!

This means the particle **never stops** — velocity is always positive. ✅

**(c)** Displacement $\Delta x = x(4) - x(0)$:

$$
x(4) = \frac{2}{3}(64) - 3(16) + 8(4) = \frac{128}{3} - 48 + 32 = \frac{80}{3} \approx 26.67\ \text{m}
$$

$$
\Delta x = \frac{80}{3} - 0 = \mathbf{\frac{80}{3}\ \text{m} \approx 26.67\ \text{m}}
$$

Since $v(t) > 0$ for all $t \geq 0$ (discriminant < 0, opens upward), the particle never turns around, so **total distance = displacement**:

$$
\text{Total distance} = \mathbf{\frac{80}{3}\ \text{m} \approx 26.67\ \text{m}}
$$

**(d)** Graph:

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

$v(t) = 2t^2 - 6t + 8$ is an upward-opening parabola. The entire curve lies above the $t$-axis ⇒ displacement = distance.

> ⭐ **AP C Important Check**: Is $v(t)$ always positive? Check discriminant + direction of opening + $v(0)$!

---

### IX. Topic Frequency Statistics

| Topic | AP 1 Frequency | AP C Frequency | Notes |
|:--|:--:|:--:|:--|
| Read slope from x-t for velocity | ⭐⭐⭐⭐ | ⭐⭐⭐ | Basic skill |
| Read slope from v-t for acceleration | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | Basic skill |
| Area under v-t for displacement | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | AP 1 core skill |
| Area under v-t for distance (absolute values) | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | High-frequency trap |
| Area under a-t for $\Delta v$ | ⭐⭐⭐ | ⭐⭐⭐⭐ | Must add initial velocity |
| Graph conversion (x-t ↔ v-t ↔ a-t) | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | AP 1 MCQ/FRQ staple |
| "Which set cannot represent same motion" | ⭐⭐⭐⭐ | ⭐⭐⭐ | AP 1 classic MCQ |
| Total distance from $v(t)$ (piecewise integration) | — | ⭐⭐⭐⭐⭐ | AP C FRQ essential |
| Second derivative for acceleration direction | — | ⭐⭐⭐⭐ | Direct from x-t curvature |
| Discriminant to check if $v(t)$ is always positive | — | ⭐⭐⭐ | AP C problem-solving technique |

---
---

# 1.4 Reference Frames & Relative Motion

---

## Part A: Foundation Layer (AP Physics 1 & 2 Essentials)

---

### I. What is a Reference Frame?

#### 1.4.1 Core Concept

> A **reference frame** is a **coordinate system + time measurement** used to describe the position and motion of objects.

The same physical motion can appear **completely different** when observed from different reference frames!

**Classic Example**:

| Scenario | Observed from Ground Frame | Observed from Train Frame |
|:--|:--|:--|
| Person standing still on the train | Moving forward at $v_{train}$ | **At rest** |
| Person walking forward on the train | Moving forward at $v_{train} + v_{walk}$ | Moving forward at $v_{walk}$ |
| Ball dropped from the train | **Parabolic** motion | **Free fall** (straight down) |

> 💡 **Core Idea**: Motion is **relative** — there is no such thing as an absolutely stationary reference frame.

#### 1.4.2 Inertial vs. Non-Inertial Reference Frames

| Type | Definition | Characteristics |
|:--|:--|:--|
| **Inertial Frame** | Frame where Newton's laws hold (at rest or constant velocity) | No fictitious forces |
| **Non-Inertial Frame** | Frame that is accelerating | Requires fictitious forces (e.g., centrifugal force, Coriolis force) |

> ⚠️ **AP Physics 1 only covers transformations between inertial frames**. Non-inertial frames are AP Physics C content.

---

### II. Basic Concepts of Relative Velocity

#### 1.4.3 Notation Conventions

We use subscript notation to clearly describe relative motion:

| Notation | Meaning | Read as |
|:--|:--|:--|
| $\vec{v}_{A/B}$ | Velocity of A **relative to** B | "A with respect to B" |
| $\vec{v}_{A/G}$ | Velocity of A relative to the Ground | "A relative to Ground" |

#### 1.4.4 Vector Addition of Relative Velocities — The Core Formula

$$
\boxed{\vec{v}_{A/C} = \vec{v}_{A/B} + \vec{v}_{B/C}}
$$

> **Interpretation**: Velocity of A relative to C = velocity of A relative to B + velocity of B relative to C.

**Important Corollary**:

$$
\boxed{\vec{v}_{A/B} = -\vec{v}_{B/A}}
$$

> The velocity of A relative to B and the velocity of B relative to A have the same magnitude but opposite directions.

#### 1.4.5 🧪 Basic Example

**Problem**: Xiaoming walks east at $2\ \text{m/s}$ on a train that is traveling east at $10\ \text{m/s}$. Find Xiaoming's velocity relative to the ground.

**Solution**:

Let east be the positive direction:

$$
v_{\text{Xiaoming/ground}} = v_{\text{Xiaoming/train}} + v_{\text{train/ground}} = 2 + 10 = \mathbf{12\ m/s\ (east)}
$$

---

### III. One-Dimensional Relative Motion

#### 1.4.6 Motion Along the Same Line

When two objects move along the same straight line, the relative velocity is an **algebraic difference**:

$$
\boxed{v_{A/B} = v_A - v_B}
$$

(Here $v_A$ and $v_B$ are algebraic values with signs)

| Scenario | $v_A$ | $v_B$ | $v_{A/B}$ | Interpretation |
|:--|:--:|:--:|:--:|:--|
| Same direction, A faster | $+10$ | $+6$ | $+4$ | A approaches B at 4 |
| Same direction, B faster | $+6$ | $+10$ | $-4$ | A falls behind B at 4 |
| Moving toward each other | $+10$ | $-6$ | $+16$ | A approaches B rapidly at 16 |
| Moving away from each other | $-10$ | $+6$ | $-16$ | A moves away from B at 16 |

#### 1.4.7 🧪 One-Dimensional Relative Motion Example

**Problem**: A car travels east at $25\ \text{m/s}$, and a truck travels west at $15\ \text{m/s}$. Find the velocity of the car relative to the truck.

**Solution**:

Let east be positive:

- Car: $v_{car} = +25\ \text{m/s}$
- Truck: $v_{truck} = -15\ \text{m/s}$

$$
v_{car/truck} = v_{car} - v_{truck} = (+25) - (-15) = \mathbf{+40\ m/s\ (east)}
$$

> 💡 **Intuitive Understanding**: From the truck driver's perspective, the car is rushing toward them at $40\ \text{m/s}$ to the east!

---

### IV. Two-Dimensional Relative Motion

#### 1.4.8 Vector Addition in 2D

When the motions of two objects are not along the same line, we need **vector addition** (parallelogram law or component method) to find the relative velocity.

$$
\boxed{\vec{v}_{A/C} = \vec{v}_{A/B} + \vec{v}_{B/C}}
$$

This formula holds for 2D as well — it's just **vector addition** now.

#### 1.4.9 Problem-Solving Steps

| Step | Operation |
|:--|:--|
| **1** | Identify all known velocities (magnitude and direction) |
| **2** | Write the vector relationship: $\vec{v}_{A/C} = \vec{v}_{A/B} + \vec{v}_{B/C}$ |
| **3** | Decompose each vector into $x$ and $y$ components |
| **4** | Add the components algebraically |
| **5** | Combine to find the magnitude and direction of the resultant vector |

#### 1.4.10 🧪 Classic 2D Relative Motion: Crossing a River

**Problem**: A boat's speed in still water is $4\ \text{m/s}$ (pointed directly across the river). The river flows east at $3\ \text{m/s}$. The river is $200\ \text{m}$ wide. Find:

(a) The boat's velocity relative to the shore (magnitude and direction)
(b) The time to cross the river
(c) How far downstream the boat lands

**Solution**:

Let $y$ be the positive direction across the river, and $x$ be the positive downstream direction.

**(a)** Boat relative to water: $\vec{v}_{B/W} = 4\ \hat{j}\ \text{m/s}$
Water relative to ground: $\vec{v}_{W/G} = 3\ \hat{i}\ \text{m/s}$

$$
\vec{v}_{B/G} = \vec{v}_{B/W} + \vec{v}_{W/G} = 4\hat{j} + 3\hat{i} = 3\hat{i} + 4\hat{j}\ \text{m/s}
$$

**Magnitude**:

$$
|\vec{v}_{B/G}| = \sqrt{3^2 + 4^2} = \mathbf{5\ m/s}
$$

**Direction** (angle from downstream):

$$
\theta = \tan^{-1}\left(\frac{4}{3}\right) \approx \mathbf{53^\circ}\ \text{(toward the opposite bank, angled upstream)}
$$

**(b)** Crossing time depends only on the **velocity component perpendicular to the river**:

$$
t = \frac{\text{river width}}{v_y} = \frac{200}{4} = \mathbf{50\ s}
$$

**(c)** Downstream drift:

$$
\Delta x = v_x \times t = 3 \times 50 = \mathbf{150\ m\ (downstream)}
$$

> ⭐ **Core Conclusion**: Crossing time is determined only by the **velocity component perpendicular to the river bank** — it is independent of the current speed!

#### 1.4.11 🧪 Derivation: Invariance of Acceleration Under the Galilean Transformation

**Core idea**: In two inertial frames moving at constant velocity relative to each other, **acceleration is invariant**.

**Mathematical proof**:

Let frame $S'$ move with constant velocity $\vec{V}$ relative to frame $S$, with their origins coinciding at $t=0$.

**Position transformation**:

$$
\vec{r}'(t) = \vec{r}(t) - \vec{V}t
$$

**Velocity transformation** (differentiate with respect to time):

$$
\vec{v}'(t) = \frac{d\vec{r}'}{dt} = \frac{d\vec{r}}{dt} - \vec{V} = \vec{v}(t) - \vec{V}
$$

**Acceleration transformation** (differentiate again):

$$
\vec{a}'(t) = \frac{d\vec{v}'}{dt} = \frac{d\vec{v}}{dt} - \frac{d\vec{V}}{dt} = \vec{a}(t) - 0 = \vec{a}(t)
$$

Since $\vec{V}$ is constant, $\dfrac{d\vec{V}}{dt} = 0$. ✅

> ⭐ **Important Corollary**: Since $\vec{a}' = \vec{a}$ and mass $m$ is invariant in classical mechanics, $\vec{F} = m\vec{a}$ takes the same form in all inertial frames — this is **Galilean relativity**!

#### 1.4.11.2 🧪 Derivation: Three Validations of the Completeness of the Galilean Transformation

##### Validation 1: Verify Galilean Transformation Using Projectile Motion

**Scenario**: Perform a projectile experiment on a uniformly moving train.

**Ground frame $S$**: The train moves at constant velocity $\vec{V} = V\hat{i}$. A person on the train throws an object with initial velocity $\vec{v}_0'$ (relative to the train).

As seen in the ground frame $S$:
- Initial velocity $\vec{v}_0 = \vec{v}_0' + \vec{V}$
- Position $\vec{r}(t) = (\vec{v}_0' + \vec{V})t - \frac{1}{2}gt^2\hat{j}$

As seen in the train frame $S'$:
- $\vec{r}'(t) = \vec{r}(t) - \vec{V}t = \vec{v}_0' t - \frac{1}{2}gt^2\hat{j}$

In the train frame, the observer sees a **standard projectile motion with initial velocity $\vec{v}_0'$** — there is no sign whatsoever that the train is moving! This is precisely the manifestation of Galilean relativity: **in a uniformly moving reference frame, all mechanical experiments yield the same results as in a stationary reference frame**.

##### Validation 2: Verify Reference Frame Equivalence Using Momentum Conservation

In frame $S$, two objects collide and satisfy momentum conservation: $m_1\vec{v}_1 + m_2\vec{v}_2 = m_1\vec{u}_1 + m_2\vec{u}_2$ (before and after collision).

In frame $S'$ ($\vec{v}_i' = \vec{v}_i - \vec{V}$), momentum conservation becomes:
$$m_1(\vec{v}_1 - \vec{V}) + m_2(\vec{v}_2 - \vec{V}) = m_1(\vec{u}_1 - \vec{V}) + m_2(\vec{u}_2 - \vec{V})$$

Simplifying reveals that the $-\vec{V}(m_1 + m_2)$ term cancels out on both sides — momentum conservation holds equally in frame $S'$. ✅

##### Validation 3: Prove Invariance of Newton's Second Law

In frame $S$: $\vec{F} = m\vec{a}$

In frame $S'$ ($\vec{V}$ is constant): $\vec{F}' = m\vec{a}' = m\vec{a} = \vec{F}$

Since both acceleration and force are invariant under the Galilean transformation, Newton's second law takes the same form in all inertial frames.

> ⭐ **AP C Core: Galilean Invariance** — "The laws of mechanics have the same form in all inertial reference frames" — this is the cornerstone of Newtonian mechanics, and also the starting point from which Einstein developed special relativity (replacing the Galilean transformation with the Lorentz transformation).

#### 1.4.12 🧪 Example: Multi-Reference Frame Problem

**Problem**: A train travels east at $20\ \text{m/s}$. A person on the train walks east at $2\ \text{m/s}$ (relative to the train). Meanwhile, a person on the ground rides a bicycle east at $5\ \text{m/s}$. Find:

(a) The velocity of the person on the train relative to the ground
(b) The velocity of the person on the train relative to the cyclist
(c) The velocity of the cyclist relative to the person on the train

**Solution**:

Let east be the positive direction.

**(a)** Given $v_{person/train} = +2\ \text{m/s}$, $v_{train/ground} = +20\ \text{m/s}$

$$
v_{person/ground} = v_{person/train} + v_{train/ground} = 2 + 20 = \mathbf{+22\ \text{m/s}\ (east)}
$$

**(b)** Find $v_{person/bike}$:

Given $v_{bike/ground} = +5\ \text{m/s}$

$$
v_{person/bike} = v_{person/ground} - v_{bike/ground} = 22 - 5 = \mathbf{+17\ \text{m/s}\ (east)}
$$

Alternatively, using the chain rule:

$$
v_{person/bike} = v_{person/train} + v_{train/ground} + v_{ground/bike}
$$

Note that $v_{ground/bike} = -v_{bike/ground} = -5\ \text{m/s}$:

$$
v_{person/bike} = 2 + 20 + (-5) = \mathbf{+17\ \text{m/s}\ (east)}
$$

**(c)** By symmetry:

$$
v_{bike/person} = -v_{person/bike} = \mathbf{-17\ \text{m/s}\ (west)}
$$

> ⭐ **Chain Rule Technique**: Relative velocities can be chained through any number of intermediate reference frames:
>
> $$
> \vec{v}_{A/Z} = \vec{v}_{A/B} + \vec{v}_{B/C} + \vec{v}_{C/D} + \cdots + \vec{v}_{Y/Z}
> $$
>
> As long as consecutive subscripts "connect end-to-end"!

---

## Part B: AP Difficulty Layer (Conceptual Traps & Deep Understanding)

---

### V. Real Conceptual Traps on the AP Exam

#### 🎯 Trap 1: Forgetting Vector Addition When Changing Reference Frames

**AP Classic Mistake**:

> ❌ Simply adding magnitudes algebraically, ignoring direction.

**✅ Correct Approach**: The relative velocity formula is a **vector equation** — direction must always be accounted for!

**🧪 Example**:

> A boat heading north at $5\ \text{m/s}$ in still water crosses a river flowing east at $3\ \text{m/s}$.

**Wrong answer**: $5 + 3 = 8\ \text{m/s}$ ❌

**Correct answer**: $\sqrt{5^2 + 3^2} = \sqrt{34} \approx 5.83\ \text{m/s}$, direction **$31^\circ$ north of east** ✅

#### 🎯 Trap 2: River Crossing — Shortest Time vs. Shortest Path

The AP exam frequently tests two different crossing strategies!

| Strategy | Condition | Boat Heading | Result |
|:--|:--|:--|:--|
| **Shortest Time** | Point directly across | Perpendicular to the bank | Shortest time, but drifts downstream |
| **Shortest Path** | Point upstream at an angle | Cancel the current | Crosses straight across, no drift, but takes longer |

**🧪 Example**:

> River width $120\ \text{m}$, current $4\ \text{m/s}$ east, boat speed in still water $5\ \text{m/s}$.
>
> (a) What is the shortest crossing time?
> (b) For the shortest path (no drift), at what angle should the boat be aimed?

**Solution (a)**:

Point directly across, $v_y = 5\ \text{m/s}$

$$
t_{min} = \frac{120}{5} = \mathbf{24\ s}
$$

**Solution (b)**:

To cross straight across (no drift), aim upstream at an angle $\theta$ such that the $x$-component cancels the current:

$$
v_{B/W}\sin\theta = v_{current} \quad\Rightarrow\quad 5\sin\theta = 4
$$

$$
\sin\theta = \frac{4}{5} = 0.8 \quad\Rightarrow\quad \theta = \sin^{-1}(0.8) \approx \mathbf{53^\circ}\ \text{(upstream)}
$$

The perpendicular component of velocity:

$$
v_y = 5\cos\theta = 5 \times 0.6 = 3\ \text{m/s}
$$

Crossing time:

$$
t = \frac{120}{3} = \mathbf{40\ s}
$$

> ⚠️ **AP Trap**: Shortest time (24 s) $\neq$ shortest path (40 s) — read the question carefully to see which one is being asked!

#### 🎯 Trap 3: Walking/Running in the Rain

**Classic AP Scenario**:

> Rain is falling vertically. Does a person get less wet by walking slowly or running fast?

**Analysis**:

- From the **ground frame**: rain falls vertically, the person moves horizontally
- From the **person's frame**: the rain has both a vertical downward velocity and a **horizontal component** (equal to the person's speed, but opposite in direction)

**Relative velocity diagram** (from the person's frame):

```
         ↑ v_rain (vertical)
         |
         |  ↗ v_rain/person (resultant)
         | /
         |/
  ←──────┼
  v_person
  (horizontal backward)
```

> ⭐ **AP Conclusion**: The faster you run, the **less rain you get per unit time** (and since you spend less time in the rain, you get even less total rain)!

#### 🎯 Trap 4: Wind and Airplanes — Isomorphic to River Crossing

**AP Physics 1 Common Problem**:

> An airplane's airspeed (relative to the air) is $200\ \text{km/h}$ north. Wind blows from west to east at $50\ \text{km/h}$.
>
> (a) What is the plane's velocity relative to the ground?
> (b) If the plane wants to fly north (relative to the ground), which direction should it point?

**Solution (a)**:

$$
\vec{v}_{P/G} = \vec{v}_{P/A} + \vec{v}_{A/G} = 200\hat{j} + 50\hat{i}
$$

Magnitude: $\sqrt{200^2 + 50^2} \approx 206\ \text{km/h}$
Direction: $14^\circ$ east of north

**Solution (b)**:

To fly north (relative to the ground), point the nose west of north at angle $\theta$ to cancel the crosswind:

$$
200\sin\theta = 50 \quad\Rightarrow\quad \sin\theta = 0.25 \quad\Rightarrow\quad \theta \approx 14.5^\circ\ \text{(west of north)}
$$

Northward component: $200\cos\theta \approx 200 \times 0.968 \approx 193.6\ \text{km/h}$

> ⚠️ Note: This is **completely isomorphic** to the river crossing problem — air = water, airplane = boat!

#### 🎯 Trap 5: Analyzing Problems in an Accelerating Frame (AP C Only)

**AP Physics C Content**:

> In an **accelerating reference frame**, Newton's second law no longer holds without modification — we must introduce **fictitious forces** (also called **inertial forces**).

$$
\vec{F}_{\text{fictitious}} = -m\vec{a}_{\text{frame}}
$$

where $\vec{a}_{\text{frame}}$ is the acceleration of the reference frame.

**🧪 Example**:

> A bus accelerates forward at $2\ \text{m/s}^2$. Inside the bus, a box of mass $5\ \text{kg}$ sits on a frictionless floor.
> Analyze the box's motion from (a) the ground frame and (b) the bus frame.

**Ground frame (inertial)**:

- No horizontal forces on the box (frictionless floor), so $a_{box} = 0$
- The box remains **at rest** (or continues at constant velocity) relative to the ground

**Bus frame (non-inertial)**:

- The box accelerates **backward** at $2\ \text{m/s}^2$ relative to the bus
- To explain this acceleration, introduce a fictitious force:

$$
F_{fict} = -m a_{bus} = -5 \times 2 = -10\ \text{N}\ \text{(backward)}
$$

> 💡 **AP C Understanding**: Fictitious forces are not real forces — they are a **product of the frame's acceleration**.

---

### VI. AP Physics C Calculus Depth

#### 6.1 Position, Velocity, and Acceleration Transformations Between Frames

##### Position Transformation (Galilean Transformation)

Suppose frame $S'$ moves with constant velocity $\vec{V}$ relative to frame $S$, and the origins coincide at $t=0$:

$$
\boxed{\vec{r}' (t) = \vec{r}(t) - \vec{V}t}
$$

##### Velocity Transformation (Galilean Velocity Transformation)

Differentiate with respect to time:

$$
\boxed{\vec{v}' = \vec{v} - \vec{V}}
$$

This is exactly the relative velocity formula we've been using! Here $\vec{v}'$ is the velocity measured in $S'$, and $\vec{v}$ is the velocity measured in $S$.

##### Acceleration Transformation

Differentiate again:

$$
\boxed{\vec{a}' = \vec{a} - \vec{A}}
$$

where $\vec{A}$ is the acceleration of $S'$ relative to $S$.

> ⭐ **Key Conclusions**:
> - If $S'$ moves at **constant velocity** ($\vec{A}=0$), then $\vec{a}' = \vec{a}$ — **acceleration is the same in all inertial frames!**
> - If $S'$ is **accelerating** ($\vec{A} \neq 0$), then $\vec{a}' \neq \vec{a}$ — we need to introduce fictitious forces.

#### 6.2 🧪 AP C Exam-Style Example

> Reference frame $S'$ moves with velocity $\vec{V} = 5\hat{i}\ \text{m/s}$ relative to frame $S$.
> A particle's position in frame $S$ is given by $\vec{r}(t) = (3t^2 - 2t)\hat{i} + (4t)\hat{j}$ meters.
>
> (a) Find the particle's velocity $\vec{v}(t)$ in frame $S$.
> (b) Find the particle's velocity $\vec{v}'(t)$ in frame $S'$.
> (c) Find the acceleration in both frames. Are they the same?

**Solution**:

**(a)** Differentiate in frame $S$:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (6t - 2)\hat{i} + 4\hat{j}\ \text{m/s}
$$

**(b)** Apply the Galilean velocity transformation:

$$
\vec{v}'(t) = \vec{v}(t) - \vec{V} = (6t - 2)\hat{i} + 4\hat{j} - 5\hat{i}
$$

$$
\boxed{\vec{v}'(t) = (6t - 7)\hat{i} + 4\hat{j}\ \text{m/s}}
$$

**(c)** In frame $S$:

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = 6\hat{i}\ \text{m/s}^2
$$

In frame $S'$:

$$
\vec{a}'(t) = \frac{d\vec{v}'}{dt} = 6\hat{i}\ \text{m/s}^2
$$

**They are the same!** ✅ Because $S'$ moves at constant velocity relative to $S$ ($\vec{A}=0$), acceleration is invariant.

> ⭐ **AP C Point**: Under the Galilean transformation, acceleration is **invariant in all inertial frames**. This is why Newton's second law $\vec{F}=m\vec{a}$ takes the same form in every inertial frame!

#### 6.3 Transformation for Uniformly Accelerating Frames (AP C Advanced)

If $S'$ moves with **constant acceleration** $\vec{A}$ relative to $S$:

$$
\vec{v}' (t) = \vec{v}(t) - \vec{V}_0 - \vec{A}t
$$

$$
\vec{a}' = \vec{a} - \vec{A}
$$

In this case, Newton's second law in frame $S'$ becomes:

$$
\vec{F} = m\vec{a} = m(\vec{a}' + \vec{A}) \quad\Rightarrow\quad \vec{F} - m\vec{A} = m\vec{a}'
$$

where $-m\vec{A}$ is the **fictitious force** (inertial force).

---

### VII. AP Exam Difficulty Level Summary

| Level | Corresponding Exam | Core Requirements | Typical Problem Features |
|:--|:--|:--|:--|
| **Level 1: Basic Application** | School midterms | Use $\vec{v}_{A/C} = \vec{v}_{A/B} + \vec{v}_{B/C}$ for 1D relative motion | Simple scenarios: person on train, cars approaching |
| **Level 2: 2D Relative Motion** | **AP Physics 1 & 2** 🎯 | River crossing (shortest time vs. shortest path), airplane crosswind, rain problems | "Boat pointed across vs. straight across," "wind affecting flight path" |
| **Level 3: Calculus Transformations** | **AP Physics C** 🎯 | Galilean transformation $\vec{r}' = \vec{r} - \vec{V}t$; accelerating frames and fictitious forces | Transform velocity/acceleration between inertial frames; introduce $-m\vec{A}$ in non-inertial frames |

---

### VIII. AP-Level Practice Problems

#### 🟢 AP Physics 1 Style

> A river flows east at $2\ \text{m/s}$. A swimmer can swim at $1.5\ \text{m/s}$ in still water.
>
> (a) If the swimmer heads directly north (perpendicular to the current), what is her velocity relative to the shore?
> (b) How long will it take her to cross a river that is $60\ \text{m}$ wide?
> (c) How far downstream will she land?
> (d) At what angle should she swim to land directly across from her starting point?

**Solution**:

Let north be $+y$, east be $+x$.

**(a)**

$$
\vec{v}_{S/G} = \vec{v}_{S/W} + \vec{v}_{W/G} = 1.5\hat{j} + 2\hat{i}
$$

Magnitude: $|\vec{v}_{S/G}| = \sqrt{1.5^2 + 2^2} = \sqrt{2.25 + 4} = \sqrt{6.25} = \mathbf{2.5\ m/s}$

Direction: $\theta = \tan^{-1}\left(\frac{2}{1.5}\right) \approx \mathbf{53^\circ}$ north of east ✅

**(b)** Crossing time depends only on the perpendicular component:

$$
t = \frac{60}{1.5} = \mathbf{40\ s} ✅
$$

**(c)** Downstream drift:

$$
\Delta x = v_x \times t = 2 \times 40 = \mathbf{80\ m} ✅
$$

**(d)** To land directly across (no drift), the swimmer's $x$-component must cancel the current:

$$
1.5\sin\theta = 2 \quad\Rightarrow\quad \sin\theta = \frac{2}{1.5} = \frac{4}{3} > 1
$$

**Impossible!** ❌

Since the swimmer's speed ($1.5\ \text{m/s}$) is less than the current speed ($2\ \text{m/s}$), she **cannot completely cancel the drift**.

> ⭐ **AP Trap**: When the boat/swimmer speed is less than the current speed, **it is impossible to cross straight across**!

#### 🔵 AP Physics C Style

> Reference frame $S'$ moves with velocity $\vec{V}(t) = (2t)\hat{i}\ \text{m/s}$ relative to frame $S$.
> A particle's position in frame $S$ is $\vec{r}(t) = (t^3 - 6t)\hat{i} + (4t^2)\hat{j}$ meters.
>
> (a) Find the velocity $\vec{v}(t)$ and acceleration $\vec{a}(t)$ in frame $S$.
> (b) Find the velocity $\vec{v}'(t)$ and acceleration $\vec{a}'(t)$ in frame $S'$.
> (c) Is $S'$ an inertial frame? Explain.
> (d) If a force $\vec{F} = m\vec{a}$ acts on the particle in frame $S$, what additional term is needed to describe the motion in frame $S'$?

**Solution**:

**(a)** In frame $S$:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (3t^2 - 6)\hat{i} + 8t\hat{j}\ \text{m/s}
$$

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = 6t\hat{i} + 8\hat{j}\ \text{m/s}^2
$$

**(b)** Galilean velocity transformation:

$$
\vec{v}'(t) = \vec{v}(t) - \vec{V}(t) = (3t^2 - 6)\hat{i} + 8t\hat{j} - (2t)\hat{i}
$$

$$
\boxed{\vec{v}'(t) = (3t^2 - 2t - 6)\hat{i} + 8t\hat{j}\ \text{m/s}}
$$

Differentiate to get acceleration:

$$
\vec{a}'(t) = \frac{d\vec{v}'}{dt} = (6t - 2)\hat{i} + 8\hat{j}\ \text{m/s}^2
$$

**(c)** $S'$ is **not** an inertial frame because $\vec{V}(t)$ is not constant ($\vec{V}(t) = 2t\hat{i}$ changes with time).

Acceleration of $S'$: $\vec{A} = \frac{d\vec{V}}{dt} = 2\hat{i}\ \text{m/s}^2$

Verify that $\vec{a}' \neq \vec{a}$:

$$
\vec{a} - \vec{a}' = (6t\hat{i} + 8\hat{j}) - ((6t-2)\hat{i} + 8\hat{j}) = 2\hat{i} = \vec{A} ✅
$$

**(d)** In the non-inertial frame $S'$, we need a fictitious force:

$$
\vec{F}_{fict} = -m\vec{A} = -m(2\hat{i}) = -2m\hat{i}\ \text{N}
$$

So in frame $S'$, Newton's second law becomes:

$$
\vec{F} + \vec{F}_{fict} = m\vec{a}' \quad\Rightarrow\quad \vec{F} - 2m\hat{i} = m\vec{a}'
$$

> ⭐ **AP C Point**: In a non-inertial frame, we must introduce the **inertial force** $-m\vec{A}$ for Newton's second law to remain valid!

---

### IX. Topic Frequency Statistics

| Topic | AP 1 Frequency | AP C Frequency | Notes |
|:--|:--:|:--:|:--|
| 1D relative velocity | ⭐⭐⭐⭐ | ⭐⭐⭐ | Basic skill, algebraic subtraction |
| 2D relative velocity vector addition | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | River crossing, airplane crosswind |
| Shortest time vs. shortest path crossing | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | AP 1 FRQ high-frequency |
| Boat speed < current speed special case | ⭐⭐⭐ | ⭐⭐ | Conceptual trap |
| Galilean transformation $\vec{r}' = \vec{r} - \vec{V}t$ | — | ⭐⭐⭐⭐⭐ | AP C core |
| Acceleration invariant in inertial frames | — | ⭐⭐⭐⭐ | Proof of inertial frame equivalence |
| Non-inertial frames & fictitious force $-m\vec{A}$ | — | ⭐⭐⭐⭐ | AP C advanced topic |

---
---

#1.5 Two-Dimensional Motion (Projectile Motion)

---

## Part A: Foundation Layer (AP Physics1 &2 Essentials)

---

### I. The Core Idea of Projectile Motion — Independence of Motion

#### 1.5.1 Core Principle> Projectile motion can be decomposed into two **mutually independent** one-dimensional motions:

$$
\boxed{\text{Projectile Motion} = \text{Horizontal Uniform Motion} + \text{Vertical Uniformly Accelerated Motion}}
$$

| Direction | Acceleration | Velocity Change | Type of Motion |
|:--|:--:|:--|:--|
| **Horizontal ($x$)** | $a_x =0$ | $v_x$ constant | Uniform linear motion |
| **Vertical ($y$)** | $a_y = -g$ | $v_y$ changes linearly | Uniformly accelerated (free fall) |

> 💡 **Galileo's Insight**: Horizontal and vertical motions are **completely independent** — analyze them separately and then combine!

#### 1.5.2 Vector Decomposition — Initial Velocity

Decompose the initial velocity $\vec{v}_0$ into horizontal and vertical components (let $\theta$ be the angle with the horizontal):

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

### II. Horizontal Projectile Motion#### 1.5.3 Initial Conditions

An object is launched horizontally from a height $h$ with initial speed $v_0$:

- $v_{0x} = v_0$, $v_{0y} =0$
- $a_x =0$, $a_y = -g$
- Let the launch point be the origin: $x_0 =0$, $y_0 = h$

#### 1.5.4 Equations of Motion

| Direction | Position Equation | Velocity Equation |
|:--|:--|:--|
| **Horizontal** | $x(t) = v_0 t$ | $v_x(t) = v_0$ |
| **Vertical** | $y(t) = h - \dfrac{1}{2}gt^2$ | $v_y(t) = -gt$ |

#### 1.5.5 🧪 Basic Example

**Problem**： A small ball is thrown horizontally from the top of an $80\ \text{m}$ tall building with an initial speed of $20\ \text{m/s}$ ($g =10\ \text{m/s}^2$). Find:
(a) Time to reach the ground(b) Horizontal range(c) Velocity just before hitting the ground**Solution**:

**(a)** When it hits the ground, $y=0$:

$$0 =80 - \frac{1}{2} \times10 \times t^2 \quad\Rightarrow\quad5t^2 =80 \quad\Rightarrow\quad t = \mathbf{4\ s}$$

**(b)** Horizontal range:

$$x = v_0 t =20 \times4 = \mathbf{80\ m}$$

**(c)** Velocity components at impact:

- $v_x =20\ \text{m/s}$
- $v_y = -gt = -10 \times4 = -40\ \text{m/s}$

Magnitude: $v = \sqrt{20^2 +40^2} = \sqrt{2000} \approx44.7\ \text{m/s}$

Direction: $\phi = \tan^{-1}\left(\dfrac{40}{20}\right) \approx63.4^\circ$ below the horizontal---

### III. Projectile Motion at an Angle#### 1.5.6 Initial Conditions

An object is launched from ground level with initial speed $v_0$ at angle $\theta$ above the horizontal:

- $v_{0x} = v_0\cos\theta$, $v_{0y} = v_0\sin\theta$
- $a_x =0$, $a_y = -g$
- Let the launch point be the origin: $x_0 =0$, $y_0 =0$

#### 1.5.7 Equations of Motion

| Direction | Position Equation | Velocity Equation |
|:--|:--|:--|
| **Horizontal** | $x(t) = (v_0\cos\theta) t$ | $v_x(t) = v_0\cos\theta$ |
| **Vertical** | $y(t) = (v_0\sin\theta) t - \dfrac{1}{2}gt^2$ | $v_y(t) = v_0\sin\theta - gt$ |

#### 1.5.8 🧪 Basic Example

**Problem**： A ball is launched at $30\ \text{m/s}$ at an angle of $30^\circ$ above the horizontal ($g =10\ \text{m/s}^2$). Find:
(a) Time of flight(b) Horizontal range(c) Maximum height**Solution**:

$v_{0x} =30\cos30^\circ =30 \times \frac{\sqrt{3}}{2} \approx25.98\ \text{m/s}$
$v_{0y} =30\sin30^\circ =30 \times \frac{1}{2} =15\ \text{m/s}$

**(a)** Time of flight (when $y=0$ again):

$$0 =15t - \frac{1}{2} \times10 \times t^2 \quad\Rightarrow\quad t(15 -5t) =0$$
$$t =0\ \text{(launch)},\quad t = \mathbf{3\ s}$$

**(b)** Horizontal range:

$$R = v_{0x} \times t =25.98 \times3 \approx \mathbf{77.94\ m}$$

**(c)** Maximum height (when $v_y =0$):

$$0 =15 -10t \quad\Rightarrow\quad t_{top} =1.5\ \text{s}$$

$$H = v_{0y}t_{top} - \frac{1}{2}gt_{top}^2 =15 \times1.5 -5 \times (1.5)^2 =22.5 -11.25 = \mathbf{11.25\ m}$$

---

### IV. Key Parameters of Projectile Motion#### 1.5.9 Time of Flight

Total time from launch to landing at the same height:

$$
\boxed{T = \frac{2v_0\sin\theta}{g}}
$$

> Derivation: Set $y=0$, solve $v_0\sin\theta \cdot t - \frac{1}{2}gt^2 =0$. Other than $t=0$, $t = \frac{2v_0\sin\theta}{g}$.

#### 1.5.10 Horizontal Range

$$
\boxed{R = \frac{v_0^2\sin2\theta}{g}}
$$

> Derivation: $R = v_{0x} \times T = (v_0\cos\theta) \times \frac{2v_0\sin\theta}{g} = \frac{v_0^2 \cdot2\sin\theta\cos\theta}{g} = \frac{v_0^2\sin2\theta}{g}$.

#### 1.5.11 Maximum Height

$$
\boxed{H = \frac{v_0^2\sin^2\theta}{2g}}
$$

> Derivation: At max height $v_y=0$, $0 = v_0\sin\theta - gt_{top}$, $t_{top} = \frac{v_0\sin\theta}{g}$, substitute into $y$ equation.

#### 1.5.12 Important Conclusions

| Conclusion | Explanation |
|:--|:--|
| **Maximum range at $\theta =45^\circ$** | $\sin2\theta$ reaches its maximum value of1 when $2\theta =90^\circ$, i.e., $\theta =45^\circ$ |
| **Complementary angles have equal range** | $\theta$ and $90^\circ - \theta$ yield the same range (since $\sin2\theta = \sin(180^\circ -2\theta)$) |
| **Minimum speed at the highest point** | At the top, $v_y=0$, only the horizontal component remains: $v_x = v_0\cos\theta$ |

#### 1.5.13 Comparison of Different Launch Angles

| Launch Angle $\theta$ | Time of Flight | Horizontal Range | Maximum Height | Trajectory Shape |
|:--:|:--:|:--:|:--:|:--:|
| $15^\circ$ | Short | Medium | Low | Low, flat parabola |
| $30^\circ$ | Medium | Large | Medium | — |
| $45^\circ$ | Medium | **Maximum** | Medium | Symmetric parabola |
| $60^\circ$ | Medium | Large (same as $30^\circ$) | High | — |
| $75^\circ$ | Long | Medium (same as $15^\circ$) | Very high | High, steep parabola |

---

### V. Equation of the Trajectory#### 1.5.14 Eliminating Time from Parametric Equations

Parametric equations:

$$
x = (v_0\cos\theta) t \quad\Rightarrow\quad t = \frac{x}{v_0\cos\theta}
$$

$$
y = (v_0\sin\theta) t - \frac{1}{2}gt^2$$

Substitute $t$:

$$
\boxed{y = x\tan\theta - \frac{g}{2v_0^2\cos^2\theta} x^2}
$$

#### 1.5.15 Shape Analysis

$$
y = ax^2 + bx + c \quad\text{where}\quad a = -\frac{g}{2v_0^2\cos^2\theta} <0$$

- $a <0$ ⇒ **downward-opening parabola**
- This is a **quadratic function** — the trajectory is a parabola

#### 1.5.16 🧪 Derivation: Rigorous Proof that $45^\circ$ Maximizes Range

**Problem**: For a given initial speed $v_0$, which launch angle $\theta$ gives the maximum horizontal range $R$?

**Derivation**:

Starting from the range formula:

$$
R(\theta) = \frac{v_0^2 \sin 2\theta}{g}
$$

where $v_0$ and $g$ are constants. Take the first derivative of $R$ with respect to $\theta$:

$$
\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \frac{d}{d\theta}(\sin 2\theta) = \frac{v_0^2}{g} \cdot 2\cos 2\theta
$$

Set $\dfrac{dR}{d\theta} = 0$:

$$
\frac{2v_0^2}{g}\cos 2\theta = 0 \quad\Rightarrow\quad \cos 2\theta = 0
$$

$$
2\theta = \frac{\pi}{2} \quad\Rightarrow\quad \theta = \frac{\pi}{4} = 45^\circ
$$

**Verify it's a maximum** (second derivative test):

$$
\frac{d^2R}{d\theta^2} = \frac{v_0^2}{g} \cdot (-4\sin 2\theta)
$$

Substitute $\theta = 45^\circ$ (so $2\theta = 90^\circ$):

$$
\frac{d^2R}{d\theta^2}\bigg|_{\theta=45^\circ} = \frac{v_0^2}{g} \cdot (-4\sin 90^\circ) = -\frac{4v_0^2}{g} < 0
$$

The second derivative is negative ⇒ **maximum** ✅

**Maximum range**:

$$
R_{max} = \frac{v_0^2 \sin(2 \times 45^\circ)}{g} = \frac{v_0^2 \sin 90^\circ}{g} = \boxed{\frac{v_0^2}{g}}
$$

> ⭐ **Physical Intuition**: At $45^\circ$, the horizontal and vertical components of velocity are equal ($v_{0x}=v_{0y}=v_0/\sqrt{2}$), striking the perfect balance between "flying far enough" and "staying in the air long enough"!

#### 1.5.16.2 🧪 Derivation: Three Methods for the Time of Flight Formula

The formula $T = \dfrac{2v_0\sin\theta}{g}$ describes the total time a projectile launched from the ground spends in the air before returning to the same level.

##### Method 1: Symmetry (Physical Intuition)

In the absence of air resistance, the ascent and descent of projectile motion are completely symmetric.

Ascent phase: from launch to the highest point, $v_y$ decreases uniformly from $v_0\sin\theta$ to $0$:
$$
0 = v_0\sin\theta - g t_{up} \quad\Rightarrow\quad t_{up} = \frac{v_0\sin\theta}{g}
$$

By symmetry, descent time = ascent time, therefore:
$$
T = t_{up} + t_{down} = 2 \times \frac{v_0\sin\theta}{g} = \frac{2v_0\sin\theta}{g}
$$

> 💡 **Prerequisite for Symmetry**: The launch and landing points must be at the same height. If the landing point is above or below the launch point (e.g., launching from a cliff), symmetry no longer holds!

##### Method 2: Direct Quadratic Equation Solving (Algebraic)

Set the launch point as the origin. Landing occurs when $y = 0$:

$$
0 = (v_0\sin\theta) t - \frac{1}{2}gt^2 = t\left(v_0\sin\theta - \frac{1}{2}gt\right)
$$

The solutions are $t = 0$ (launch instant, discarded) or:
$$
t = \frac{2v_0\sin\theta}{g}
$$

> 💡 **Factorization** is the fastest way to solve this. Note that if you don't factor and instead use the quadratic formula, it takes an extra step — factorization exploits the fact that $t=0$ is already a known root.

##### Method 3: From the $v_y$-$t$ Graph (Graphical)

On a $v_y$-$t$ graph, $v_y(t) = v_0\sin\theta - gt$ is a straight line with slope $-g$.

The line intersects the $t$-axis at $t_{up} = v_0\sin\theta/g$. By symmetry, the two triangles formed by the line and the $t$-axis are congruent, so the total time $T = 2t_{up} = 2v_0\sin\theta/g$.

```
v_y
↑
│   ╲
│    ╲  at t_up: v_y = 0
│     ╲
│      ╲────→ t
│       ╲  ╱
│        ╲╱  at t=T: v_y = -v₀sinθ
│         ╲
```

> 💡 **Graphical Insight**: On the $v_y$-$t$ graph, at landing $v_y = -v_0\sin\theta$ (same magnitude as the initial vertical component, but pointing downward). This is the key signature of "same-level landing."

#### 1.5.16.3 🧪 Derivation: Three Methods for the Horizontal Range Formula

The formula $R = \dfrac{v_0^2\sin 2\theta}{g}$ is one of the most elegant results in projectile motion.

##### Method 1: Direct Combination (Algebraic Derivation)

Range $R$ = horizontal velocity × time of flight (because horizontal motion is uniform):

$$
R = v_{0x} \cdot T = (v_0\cos\theta) \cdot \frac{2v_0\sin\theta}{g}
$$

$$
= \frac{v_0^2 \cdot 2\sin\theta\cos\theta}{g} = \frac{v_0^2 \sin 2\theta}{g}
$$

where we've used the trig identity $\sin 2\theta = 2\sin\theta\cos\theta$.

> ⭐ **$R \propto v_0^2$**: Doubling the initial speed quadruples the range! This is why golfers and baseball pitchers need such tremendous power.

##### Method 2: From the Trajectory Equation (Analytic Geometry)

The trajectory equation is:
$$
y = x\tan\theta - \frac{g}{2v_0^2\cos^2\theta} x^2
$$

Landing occurs at $y = 0$ (excluding $x=0$):
$$
0 = x\tan\theta - \frac{g}{2v_0^2\cos^2\theta} x^2
$$

Factor (since $x \neq 0$):
$$
\tan\theta = \frac{g}{2v_0^2\cos^2\theta} x \quad\Rightarrow\quad x = \frac{2v_0^2 \sin\theta\cos\theta}{g} = \frac{v_0^2\sin 2\theta}{g}
$$

> 💡 **Advantage of the Trajectory Equation Method**: When the landing point is NOT at the same level (e.g., $y = -h$), simply replace $y$ with $-h$ and solve the quadratic equation to get the range.

##### Method 3: Dimensional Analysis (A Scaling Perspective)

Range $R$ depends on three parameters: $v_0$, $\theta$, and $g$.

The dimension of $R$ is $[L]$, $v_0$ has dimension $[L/T]$, and $g$ has dimension $[L/T^2]$.

The only dimensionless combination is $\theta$ (angles are inherently dimensionless). To construct $[L]$, we need $v_0^2/g$ ($[L^2/T^2] / [L/T^2] = [L]$).

Therefore $R$ must be proportional to $v_0^2/g$, multiplied by some function of $\theta$:
$$
R = \frac{v_0^2}{g} \cdot f(\theta)
$$

The specific $f(\theta) = \sin 2\theta$ must be determined through dynamical derivation, but dimensional analysis already tells us:
- $R \propto v_0^2$ (the effect of initial speed)
- $R \propto 1/g$ (on the Moon, where $g$ is smaller, the range is greater!)

> ⭐ **Dimensional Analysis** is one of the most powerful tools in physics — even without fully understanding the mechanism, you can infer relationships between physical quantities!

#### 1.5.16.4 🧪 Derivation: Three Methods for the Maximum Height Formula

The formula $H = \dfrac{v_0^2\sin^2\theta}{2g}$ describes the highest point of projectile motion.

##### Method 1: From Vertical Motion Directly (Most Direct)

In the vertical direction, the hallmark of the highest point is $v_y = 0$. Use Equation ③ ($v_y^2 = v_{0y}^2 + 2a_y\Delta y$):

$$
0 = (v_0\sin\theta)^2 + 2(-g)H
$$

$$
H = \frac{v_0^2\sin^2\theta}{2g}
$$

> 💡 **Physical Intuition**: Maximum height depends only on the **initial value of the vertical component of velocity**. The horizontal component does not affect height — horizontal and vertical motions are completely independent!

##### Method 2: From the Time to the Highest Point

First find the time to reach the highest point: $t_{top} = \dfrac{v_0\sin\theta}{g}$

Substitute into the vertical displacement formula:
$$
H = (v_0\sin\theta) \cdot t_{top} - \frac{1}{2}g t_{top}^2
$$

$$
= (v_0\sin\theta)\frac{v_0\sin\theta}{g} - \frac{1}{2}g\left(\frac{v_0\sin\theta}{g}\right)^2
$$

$$
= \frac{v_0^2\sin^2\theta}{g} - \frac{v_0^2\sin^2\theta}{2g} = \frac{v_0^2\sin^2\theta}{2g}
$$

##### Method 3: From Energy Conservation

At the highest point, all vertical kinetic energy has been converted to gravitational potential energy (taking the launch point as reference):

$$
\frac{1}{2}m(v_0\sin\theta)^2 = mgH
$$

$$
H = \frac{v_0^2\sin^2\theta}{2g}
$$

> ⭐ **The Power of the Energy Perspective**: Using energy conservation, you can find the maximum height in a single line — no time variable needed at all! This is why the energy method is such an important problem-solving tool in AP Physics 1 FRQs.

#### 1.5.16.5 Deep Relationships Between Projectile Parameters

| Parameter | Formula | Dependence on $\theta$ | Maximum Value |
|:--|:--|:--|:--|
| Time of flight $T$ | $\dfrac{2v_0\sin\theta}{g}$ | $\propto \sin\theta$ | $\theta = 90^\circ$ (straight up) |
| Horizontal range $R$ | $\dfrac{v_0^2\sin 2\theta}{g}$ | $\propto \sin 2\theta$ | $\theta = 45^\circ$ |
| Maximum height $H$ | $\dfrac{v_0^2\sin^2\theta}{2g}$ | $\propto \sin^2\theta$ | $\theta = 90^\circ$ |
| $H/R$ ratio | $\dfrac{\tan\theta}{4}$ | $\propto \tan\theta$ | — |

> 💡 **An Interesting Relationship**: $H/R = \tan\theta/4$. This means at $\theta = 45^\circ$, $H = R/4$; at $\theta = 76^\circ$, $H = R$ (height equals range); for $\theta > 76^\circ$, the projectile flies higher than it goes far!

#### 1.5.17 🧪 Example: Choosing the Right Launch Angle

**Problem**: A soccer player wants to kick a ball over a wall that is $3\ \text{m}$ high and $20\ \text{m}$ away. The ball is kicked with an initial speed of $20\ \text{m/s}$ from ground level. ($g = 10\ \text{m/s}^2$)

(a) Can the ball clear the wall?
(b) If so, what range of launch angles will work?

**Solution**:

**(a)** First, find the trajectory equation:

Parametric equations: $x = (v_0\cos\theta)t$, $y = (v_0\sin\theta)t - \frac{1}{2}gt^2$

Eliminate $t$:

$$
y = x\tan\theta - \frac{g}{2v_0^2\cos^2\theta} x^2
$$

Substitute $v_0 = 20$, $g = 10$, $x = 20$:

$$
y(20) = 20\tan\theta - \frac{10}{2 \times 400 \times \cos^2\theta} \times 400 = 20\tan\theta - \frac{5}{\cos^2\theta}
$$

Using $\dfrac{1}{\cos^2\theta} = 1 + \tan^2\theta$:

$$
y(20) = 20\tan\theta - 5(1 + \tan^2\theta) = -5\tan^2\theta + 20\tan\theta - 5
$$

**(b)** Set $y(20) > 3$:

$$
-5\tan^2\theta + 20\tan\theta - 5 > 3
$$

$$
-5\tan^2\theta + 20\tan\theta - 8 > 0
$$

$$
5\tan^2\theta - 20\tan\theta + 8 < 0
$$

Solve $5u^2 - 20u + 8 = 0$ (where $u = \tan\theta$):

$$
u = \frac{20 \pm \sqrt{400 - 160}}{10} = \frac{20 \pm \sqrt{240}}{10} = \frac{20 \pm 4\sqrt{15}}{10} = 2 \pm \frac{2\sqrt{15}}{5}
$$

$$
u_1 \approx 2 - 1.55 = 0.45,\quad u_2 \approx 2 + 1.55 = 3.55
$$

So the range of $\tan\theta$ is:

$$
0.45 < \tan\theta < 3.55
$$

Therefore:

$$
\theta_{min} \approx \tan^{-1}(0.45) \approx \mathbf{24.2^\circ},\quad \theta_{max} \approx \tan^{-1}(3.55) \approx \mathbf{74.3^\circ}
$$

> ⭐ **Conclusion**: When the launch angle is between **$24.2^\circ$ and $74.3^\circ$**, the ball can clear the $3\ \text{m}$ wall. Angles outside this range will hit the wall!
>
> Note that $\theta = 45^\circ$ is within this range, but it's not the only feasible angle — projectile motion has a **dual solution** property where both lower and higher angles can reach the same target point.

---

## Part B: AP Difficulty Layer (Conceptual Traps & Deep Understanding)

---

### VI. Real Conceptual Traps on the AP Exam

#### 🎯 Trap 1: Velocity at the Highest Point is NOT Zero!

**AP Must-Know Concept**:

> A projectile is launched at an angle. At the highest point of its trajectory:
>
> A) Both $v_x$ and $v_y$ are zero.
> B) $v_y =0$, $v_x$ is maximum.
> C) **$v_y =0$, $v_x$ is constant (same as initial $v_x$).**
> D) Both $v_x$ and $v_y$ are constant.

**Answer**: C ✅> ⚠️ **AP Trap**: Unlike straight-up projectile motion (θ =90°), in angled projectile motion, only $v_y =0$ at the highest point — **$v_x$ is still non-zero**!

#### 🎯 Trap2: Is the Landing Speed the Same as the Launch Speed?

**Symmetric projectile** (lands at same height):

$$v_f = \sqrt{v_x^2 + v_y^2} = \sqrt{(v_0\cos\theta)^2 + (-v_0\sin\theta)^2} = v_0$$

> Landing speed = launch speed ✅>
> But **direction differs** — the angle with the horizontal is the same magnitude, but below the horizontal instead of above.

#### 🎯 Trap3: Launch from Ground vs. Launch from a Height — Different Landing Times!

**Launch from ground** (lands at same height): $T = \frac{2v_0\sin\theta}{g}$

**Launch from a height** (lands at a lower elevation): Must solve a quadratic equation for $y=0$ — not a simple formula!

**🧪 Example**:

> A projectile is launched at $20\ \text{m/s}$, $30^\circ$ above horizontal, from a $50\ \text{m}$ high cliff. When does it hit the ground?

Let $y_0 =50\ \text{m}$, ground at $y=0$:

$$0 =50 + (20\sin30^\circ)t - \frac{1}{2}gt^2$$
$$0 =50 +10t -5t^2 \quad\Rightarrow\quad5t^2 -10t -50 =0$$
$$t^2 -2t -10 =0 \quad\Rightarrow\quad t = \frac{2 \pm \sqrt{4 +40}}{2} = \frac{2 \pm \sqrt{44}}{2}$$
$$t \approx \frac{2 +6.63}{2} = \mathbf{4.32\ s} \quad (t>0)$$

#### 🎯 Trap4: Is $45^\circ$ Always the Angle for Maximum Range?

**Classic Trap**:

> ❌ The angle for maximum range in projectile motion is always $45^\circ$.

**✅ Correct Answer**:
- When **landing at the same height** as launch: maximum range at $45^\circ$
- When **landing below** the launch height: maximum range angle is **less than $45^\circ$**
- When **landing above** the launch height: maximum range angle is **greater than $45^\circ$**

The AP exam may give you a scenario with different landing heights and ask you to determine which angle gives the maximum range!

#### 🎯 Trap5: Effect of Air Resistance (AP Conceptual Analysis)

| Parameter | Without Air Resistance | With Air Resistance |
|:--|:--|:--|
| Trajectory shape | Symmetric parabola | **Asymmetric**, steeper descent |
| Horizontal range | $R = v_0^2\sin2\theta / g$ | **Decreases** |
| Maximum height | $H = v_0^2\sin^2\theta /2g$ | **Decreases** |
| Time of flight | $T =2v_0\sin\theta / g$ | **Decreases** |
| Landing speed | Equal to launch speed | **Less than** launch speed |

> ⚠️ **AP1 Note**: Unless explicitly stated, **air resistance is neglected by default**.

---

### VII. AP Physics C Calculus Depth

#### 7.1 Derivation from Newton's Second Law Using Calculus

In projectile motion, $\vec{F} = m\vec{a}$, and only gravity $m\vec{g}$ acts:

$$
\vec{a} = \frac{\vec{F}}{m} = \vec{g} = -g\hat{j}
$$

In component form:

$$
a_x = \frac{d^2x}{dt^2} =0,\quad a_y = \frac{d^2y}{dt^2} = -g$$

#### 7.2 Integrate Twice to Get the Equations of Motion

**Horizontal direction**:

$$
\frac{d^2x}{dt^2} =0 \quad\Rightarrow\quad \frac{dx}{dt} = C_1$$

From $v_x(0) = v_0\cos\theta$, we get $C_1 = v_0\cos\theta$

$$
\frac{dx}{dt} = v_0\cos\theta \quad\Rightarrow\quad x(t) = (v_0\cos\theta)t + C_2$$

From $x(0) =0$, we get $C_2 =0$

$$
\boxed{x(t) = (v_0\cos\theta)t}
$$

**Vertical direction**:

$$
\frac{d^2y}{dt^2} = -g \quad\Rightarrow\quad \frac{dy}{dt} = -gt + D_1$$

From $v_y(0) = v_0\sin\theta$, we get $D_1 = v_0\sin\theta$

$$
\frac{dy}{dt} = v_0\sin\theta - gt \quad\Rightarrow\quad y(t) = (v_0\sin\theta)t - \frac{1}{2}gt^2 + D_2$$

From $y(0) =0$, we get $D_2 =0$

$$
\boxed{y(t) = (v_0\sin\theta)t - \frac{1}{2}gt^2}
$$

This is the complete calculus derivation! ✅

#### 7.3 🧪 AP Physics C Exam-Style Example

> A projectile is launched from ground level with initial velocity $\vec{v}_0 =20\hat{i} +30\hat{j}\ \text{m/s}$.
> ($g =10\ \text{m/s}^2$, neglect air resistance)
>
> **(a)** Write the position vector $\vec{r}(t)$.
> **(b)** Find the time when the projectile reaches its maximum height.
> **(c)** Find the velocity vector at the maximum height.
> **(d)** Find the speed of the projectile at $t =2$ s.
> **(e)** Find the angle between the velocity and acceleration vectors at $t =1$ s.
> **(f)** Derive the equation of the trajectory $y(x)$.

**Solution**:

**(a)** $v_{0x} =20$, $v_{0y} =30$

$$
\vec{r}(t) = (20t)\hat{i} + \left(30t - \frac{1}{2} \times10 \times t^2\right)\hat{j} = \boxed{20t\hat{i} + (30t -5t^2)\hat{j}\ \text{m}}
$$

**(b)** At maximum height, $v_y =0$:

$$v_y(t) = \frac{dy}{dt} =30 -10t =0 \quad\Rightarrow\quad t = \mathbf{3\ s}$$

**(c)** At maximum height:

$$
\vec{v}(3) =20\hat{i} + (30 -30)\hat{j} = \boxed{20\hat{i}\ \text{m/s}}
$$

Only the horizontal component remains! ✅**(d)** At $t =2$ s:

$$
\vec{v}(2) =20\hat{i} + (30 -20)\hat{j} =20\hat{i} +10\hat{j}
$$

Speed:

$$
|\vec{v}(2)| = \sqrt{20^2 +10^2} = \sqrt{500} \approx \mathbf{22.36\ \text{m/s}}
$$

**(e)** At $t =1$ s:

$$
\vec{v}(1) =20\hat{i} + (30 -10)\hat{j} =20\hat{i} +20\hat{j}
$$

$$
\vec{a} = -g\hat{j} = -10\hat{j}
$$

Dot product:

$$
\vec{v} \cdot \vec{a} =20 \times0 +20 \times (-10) = -200$$

$$
|\vec{v}| = \sqrt{20^2 +20^2} =20\sqrt{2},\quad |\vec{a}| =10$$

$$
\cos\theta = \frac{-200}{20\sqrt{2} \times10} = \frac{-200}{200\sqrt{2}} = -\frac{1}{\sqrt{2}}
$$

$$
\theta = \cos^{-1}\left(-\frac{1}{\sqrt{2}}\right) = \mathbf{135^\circ}
$$

> $\vec{v} \cdot \vec{a} <0$, so the projectile is **slowing down** (ascending) ✅**(f)** Trajectory equation:

$x =20t \quad\Rightarrow\quad t = \dfrac{x}{20}$

$$
y =30\left(\frac{x}{20}\right) -5\left(\frac{x}{20}\right)^2 = \frac{3}{2}x -5\left(\frac{x^2}{400}\right)
$$

$$
\boxed{y = \frac{3}{2}x - \frac{x^2}{80}}
$$

---

### VIII. AP Exam Difficulty Level Summary| Level | Corresponding Exam | Core Requirements | Typical Problem Features |
|:--|:--|:--|:--|
| **Level1: Formula Substitution** | School midterms | Use $T, R, H$ formulas directly | Given $v_0, \theta$, find time of flight, range, max height |
| **Level2: Conceptual Analysis & Applications** | **AP Physics1 &2** 🎯 | Launch from height, different landing levels, $45^\circ$ trap, air resistance effects | "When does it hit the ground from a cliff?" "How does air resistance change the trajectory?" |
| **Level3: Calculus Derivation** | **AP Physics C** 🎯 | Integrate twice from $\vec{a} = -g\hat{j}$ to get equations of motion; use $\vec{v} \cdot \vec{a}$ to analyze speeding up/slowing down; derive trajectory equation | Given $\vec{v}_0$, find $\vec{r}(t)$, angle between vectors, trajectory $y(x)$ |

---

### IX. AP-Level Practice Problems#### 🟢 AP Physics1 Style> A cannonball is fired from ground level with an initial speed of $50\ \text{m/s}$ at an angle of $53^\circ$ above the horizontal. ($g =10\ \text{m/s}^2$, $\sin53^\circ =0.8$, $\cos53^\circ =0.6$)
>
> (a) Calculate the horizontal and vertical components of the initial velocity.
> (b) How long does the cannonball stay in the air?
> (c) What is the maximum height reached?
> (d) What is the horizontal range?
> (e) What is the velocity (magnitude and direction) just before hitting the ground?

**Solution**:

**(a)**

$$
v_{0x} =50 \times0.6 =30\ \text{m/s},\quad v_{0y} =50 \times0.8 =40\ \text{m/s}
$$

**(b)**

$$
T = \frac{2v_{0y}}{g} = \frac{2 \times40}{10} = \mathbf{8\ s}
$$

**(c)**

$$
H = \frac{v_{0y}^2}{2g} = \frac{40^2}{20} = \frac{1600}{20} = \mathbf{80\ m}
$$

**(d)**

$$
R = v_{0x} \times T =30 \times8 = \mathbf{240\ m}
$$

**(e)** Landing velocity:

- $v_x =30\ \text{m/s}$ (unchanged)
- $v_y = -40\ \text{m/s}$ (symmetric)

Magnitude: $v = \sqrt{30^2 +40^2} = \mathbf{50\ m/s}$ (same as launch speed!)
Direction: $\phi = \tan^{-1}\left(\frac{40}{30}\right) \approx53^\circ$ below horizontal ✅#### 🔵 AP Physics C Style> A projectile is launched from the origin with initial velocity $\vec{v}_0 = (10\hat{i} +20\hat{j})\ \text{m/s}$.
> The acceleration due to gravity is $\vec{g} = -10\hat{j}\ \text{m/s}^2$.
>
> (a) Find the velocity vector $\vec{v}(t)$ and position vector $\vec{r}(t)$.
> (b) Find the time when $v_y =0$ and the position at that time.
> (c) Find the speed as a function of time $v(t)$.
> (d) At what time is the speed minimum? What is that minimum speed?
> (e) Find the equation of the trajectory $y(x)$.
> (f) Find the radius of curvature of the trajectory at the highest point.

**Solution**:

**(a)** Integrate the acceleration:

$$
\vec{v}(t) = \int \vec{a}\ dt = \int (-10\hat{j})\ dt = -10t\hat{j} + \vec{C}
$$

From $\vec{v}(0) =10\hat{i} +20\hat{j}$, we get $\vec{C} =10\hat{i} +20\hat{j}$

$$
\boxed{\vec{v}(t) =10\hat{i} + (20 -10t)\hat{j}\ \text{m/s}}
$$

Integrate again:

$$
\vec{r}(t) = \int \vec{v}(t)\ dt = \int (10\hat{i} + (20-10t)\hat{j})\ dt =10t\hat{i} + \left(20t -5t^2\right)\hat{j} + \vec{D}
$$

From $\vec{r}(0) = \vec{0}$, we get $\vec{D} = \vec{0}$

$$
\boxed{\vec{r}(t) =10t\hat{i} + (20t -5t^2)\hat{j}\ \text{m}}
$$

**(b)** $v_y =0$:

$$20 -10t =0 \quad\Rightarrow\quad t = \mathbf{2\ s}$$

Position: $\vec{r}(2) =10(2)\hat{i} + (40 -20)\hat{j} = \boxed{20\hat{i} +20\hat{j}\ \text{m}}$

Highest point at $(20,20)\ \text{m}$ ✅**(c)** Speed (magnitude of velocity):

$$
v(t) = |\vec{v}(t)| = \sqrt{10^2 + (20 -10t)^2} = \sqrt{100 + (20 -10t)^2}
$$

$$
\boxed{v(t) = \sqrt{100 + (20 -10t)^2}\ \text{m/s}}
$$

**(d)** $v(t)$ is minimized when the expression under the square root is minimized:

$$
f(t) =100 + (20 -10t)^2$$

Differentiate: $f'(t) =2(20 -10t)(-10) = -20(20 -10t)$Set $f'(t) =0$: $20 -10t =0 \quad\Rightarrow\quad t = \mathbf{2\ s}$

$$
v_{min} = v(2) = \sqrt{100 +0} = \mathbf{10\ m/s}
$$

> ⭐ **AP C Point**: The minimum speed in projectile motion occurs at the highest point, and its value is $v_0\cos\theta$ (the horizontal component)!

**(e)** Trajectory equation:

$x =10t \quad\Rightarrow\quad t = \dfrac{x}{10}$

$$
y =20\left(\frac{x}{10}\right) -5\left(\frac{x}{10}\right)^2 =2x -5\left(\frac{x^2}{100}\right)
$$

$$
\boxed{y =2x - \frac{x^2}{20}}
$$

**(f)** Radius of curvature (AP C Advanced):

$$
\rho = \frac{v^2}{a_\perp}
$$

At the highest point: $v =10\ \text{m/s}$ (horizontal), $a_\perp = g =10\ \text{m/s}^2$ (centripetal acceleration is entirely due to gravity)

$$
\rho = \frac{10^2}{10} = \mathbf{10\ m}
$$

> 💡 The radius of curvature can also be found from the second derivative of the trajectory: $\rho = \frac{(1 + (y')^2)^{3/2}}{|y''|}$

---

### X. Topic Frequency Statistics| Topic | AP1 Frequency | AP C Frequency | Notes |
|:--|:--:|:--:|:--|
| Vector decomposition ($v_{0x}, v_{0y}$) | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | First step in any projectile problem |
| Time of flight $T$ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | Basic calculation |
| Horizontal range $R$ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | Basic calculation |
| Maximum height $H$ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | Basic calculation |
| Highest point: $v_y=0$ but $v_x \neq0$ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | Conceptual trap, must-know |
| $45^\circ$ for maximum range (same level) | ⭐⭐⭐⭐ | ⭐⭐⭐ | Conceptual understanding |
| Landing time from elevated launch | ⭐⭐⭐⭐ | ⭐⭐⭐⭐ | Requires solving a quadratic |
| Qualitative effect of air resistance | ⭐⭐⭐ | ⭐⭐ | Conceptual analysis |
| Integrate $\vec{a}$ twice to get $\vec{r}(t)$ | — | ⭐⭐⭐⭐⭐ | AP C core skill |
| Dot product of velocity & acceleration | — | ⭐⭐⭐⭐ | Analyze speeding up/slowing down |
| Derive trajectory equation $y(x)$ | — | ⭐⭐⭐⭐ | AP C FRQ staple |
| Radius of curvature | — | ⭐⭐⭐ | AP C advanced |

---

