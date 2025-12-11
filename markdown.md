# Physics 1D03: Comprehensive Study Guide & Error Analysis

This document compiles a detailed review of your notes, practice papers, and specific annotations ("Red Ink") to help you prepare for your exam.

---

## 1. The "Red Ink" Revelations (Critical Annotations)
These are specific, high-value corrections you wrote down in your notes. **Memorize these.**

### **"Velocity, not time! LOCK IN"**
* [cite_start]**Context:** Question 8, 2003 Supplement [cite: 2343-2344].
* **The Mistake:** Interpreting the x-axis of a Power curve as time.
* **The Concept:** The graph shows **Torque vs. Speed (RPM)**.
    * Power is defined as $P = \tau \omega$.
    * It is the **product** of the axes values, not the slope.
    * **Lock In:** $1 \text{ rpm} = \frac{2\pi}{60} \text{ rad/s}$. Always convert immediately.

### **Elastic Collisions & Conservation**
* [cite_start]**Your Note:** "Momentum always conserved if no external force... meaning energy is conserved" [cite: 2394-2399].
* **Clarification:**
    * **Momentum ($\vec{p}$):** Conserved in *all* collisions (elastic and inelastic) if net external force is zero.
    * **Kinetic Energy ($K$):** Conserved **ONLY** in elastic collisions.
    * *Correction:* In inelastic collisions, total energy is conserved, but mechanical/kinetic energy is lost to heat/sound.

### **Work & Path Independence**
* [cite_start]**Your Note:** "Work doesn't depend on path, only endpoints" [cite: 90-93].
* **The Concept:** For conservative forces (Gravity, Springs):
    $$W = -\Delta U$$
    * **Gravity:** $W_g = mg(h_{initial} - h_{final})$. If you end up lower than you started, gravity did positive work, regardless of the loops you took to get there.

### **Force as Derivative of Potential**
* [cite_start]**Your Note:** "Force is negative derivative of potential"[cite: 1900].
* **The Math:** $F(x) = -\frac{dU}{dx}$.
* **Application:** If Potential Energy $U = \frac{1}{2}kx^2$, then $F = -kx$. This proves Simple Harmonic Motion (SHM) because the restoring force is proportional to negative displacement.

### **Free Fall Acceleration**
* [cite_start]**Your Note:** "Assume free fall unless stated otherwise"[cite: 2556].
* [cite_start]**The Concept:** When drawing an acceleration graph for a bouncing ball[cite: 2583]:
    * While in the air (rising OR falling): $a = -9.81 \, \text{m/s}^2$ (constant, negative).
    * During contact with the floor: $a$ is a massive positive spike.

---

## 2. Graph Analysis: Deep Dive

### **Graph 1: Angular Position ($\theta$) vs. Time**
* [cite_start]**Scenario:** A curve that starts steep positive, flattens out, then goes negative[cite: 2212].
* **Analysis:**
    * Slope of Position ($\theta$) = Velocity ($\omega$).
    * Slope of Velocity ($\omega$) = Acceleration ($\alpha$).
    * **Region 1:** Slope is positive but flattening $\rightarrow$ Velocity is decreasing $\rightarrow$ **$\alpha$ is negative**.
    * **Region 2:** Slope is negative and getting steeper $\rightarrow$ Velocity is becoming more negative $\rightarrow$ **$\alpha$ is negative**.
* **Result:** The curve is concave down the entire time, so angular acceleration is negative throughout.

### **Graph 2: SHM Position vs. Time (Finding Phase $\phi$)**
* [cite_start]**Scenario:** A sine wave starting at $x=0$ but moving downwards (negative velocity) at $t=0$[cite: 2774].
* **How to Solve:**
    1.  **Displacement:** $x(0) = A \cos(\phi) = 0 \rightarrow \phi = \pm \frac{\pi}{2}$.
    2.  **Velocity:** $v(t) = -A\omega \sin(\omega t + \phi)$.
    3.  **Check Sign:** At $t=0$, $v(0) = -A\omega \sin(\phi)$.
        * If $\phi = -\frac{\pi}{2}$: $v(0) \propto -(-1) = \text{positive}$ (Incorrect).
        * If $\phi = +\frac{\pi}{2}$: $v(0) \propto -(1) = \text{negative}$ (Correct).
    * **Answer:** $\phi = +\frac{\pi}{2}$.

### **Graph 3: Force vs. Position (Work)**
* [cite_start]**Scenario:** A triangular force graph[cite: 1441].
* [cite_start]**Your Note:** "W = Area under curve"[cite: 1283].
* **Calculation:** Do not integrate manually. Use geometry.
    * Area = $\frac{1}{2} \times \text{base} \times \text{height}$.
    * Set $W = \Delta K = \frac{1}{2}m(v_f^2 - v_i^2)$ to find final velocity.

---

## 3. Core Concept Mistakes & Fixes

### **Vector Math: The Cross Product**
* [cite_start]**The Mistake:** Incorrectly expanding the cross product manually[cite: 361].
* **The Fix:** Use the Determinant Method strictly for Torque ($\vec{\tau} = \vec{r} \times \vec{F}$).
    $$
    \begin{vmatrix} 
    \hat{i} & \hat{j} & \hat{k} \\ 
    r_x & r_y & r_z \\ 
    F_x & F_y & F_z 
    \end{vmatrix} = \hat{i}(r_y F_z - r_z F_y) - \hat{j}(r_x F_z - r_z F_x) + \hat{k}(r_x F_y - r_y F_x)
    $$
    * **Note:** The middle term ($\hat{j}$) must have a **negative** sign.

### **Rotational Dynamics**
* [cite_start]**The Mistake:** Thinking the Parallel Axis Theorem ($I = I_{cm} + Md^2$) only applies to symmetric systems[cite: 43].
* **The Fix:** It applies to **any** rigid body, as long as the axes are parallel.
* **Comparison:** Hollow objects have higher Moment of Inertia ($I \approx MR^2$) than solid objects ($I \approx \frac{1}{2}MR^2$). [cite_start]This means hollow objects are **harder** to spin and store more energy at the same speed[cite: 1330].

### **Static Equilibrium**
* [cite_start]**The Mistake:** Solving for tension using only $\sum F_y = 0$ and ignoring the hinge force[cite: 369].
* **The Strategy:**
    1.  **Pivot:** Place the pivot at the Hinge/Pin to eliminate unknown hinge forces.
    2.  **Torque:** Solve $\sum \tau = 0$ first to find Tension.
    3.  [cite_start]**Forces:** Use $\sum F_x = 0$ and $\sum F_y = 0$ *after* to find the horizontal and vertical hinge reaction forces[cite: 1403].

### **Rolling Friction**
* [cite_start]**The Mistake:** Guessing friction direction based on rotation alone[cite: 2405].
* **The Fix:**
    * If pulling the **top** of the wheel: Torque is high, angular acceleration is high. Friction points **forward** (direction of motion) to prevent spinning out.
    * If pulling the **center** (axle): Linear acceleration is high. Friction points **backward** to generate the torque needed to rotate.

---

## 4. Action Plan for Exam

1.  **Truss Analysis:** Practice the "Method of Joints". [cite_start]Identify **Zero-Force Members** (T-joints with no external load) to save time[cite: 1740].
2.  **Hinge Forces:** Practice calculating the X and Y components of a hinge force explicitly using Newton's laws. [cite_start]Do not assume it points along the beam[cite: 1403].
3.  **Phase Angles:** Practice finding $\phi$ for SHM when $x(0) \neq A$ and $v(0) \neq 0$.
