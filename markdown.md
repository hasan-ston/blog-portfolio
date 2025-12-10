# Physics 1D03: Comprehensive Performance Review & Study Guide

Based on a detailed analysis of your uploaded notes and practice papers, this document outlines specific mistakes found in your work, explains the concepts you missed, and provides strategies to answer these questions correctly in the future.

---

## 1. Vector Math & Cross Products

**The Mistake:**
In your notes, you attempted to calculate torque using the cross product $\vec{\tau} = \vec{r} \times \vec{F}$. You correctly set up the matrix, but you made a sign/order error in the calculation. You wrote: "Order matters here. By flipping the rows, the sign changes." While true, your manual calculation resulted in an incorrect vector because of the expansion method.

**How to Avoid It:**
* **The Determinant Method:** When calculating $\vec{r} \times \vec{F}$, set it up strictly as:
    $$
    \begin{vmatrix} 
    \hat{i} & \hat{j} & \hat{k} \\ 
    r_x & r_y & r_z \\ 
    F_x & F_y & F_z 
    \end{vmatrix}
    $$
    * **$\hat{i}$ component:** $(r_y F_z - r_z F_y)$
    * **$\hat{j}$ component:** $-(r_x F_z - r_z F_x)$ **<-- Do not forget this negative sign!**
    * **$\hat{k}$ component:** $(r_x F_y - r_y F_x)$

* **Order is Critical:** Always put position ($\vec{r}$) in the middle row and Force ($\vec{F}$) in the bottom row. Remember: $\vec{r} \times \vec{F} = - (\vec{F} \times \vec{r})$.

---

## 2. Rotational Dynamics & Moment of Inertia

**The Mistake:**
You noted the Parallel Axis Theorem ($I_{new} = I_{cm} + Md^2$) but wrote "system also has to be symmetric".
* **Correction:** The system does **not** need to be symmetric. The Parallel Axis Theorem applies to *any* rigid body, provided the two axes are parallel and one passes through the Center of Mass (COM).

**The Mistake:**
Calculating the Moment of Inertia ($I$) for discrete masses. You summed them up but seemingly confused the radius for different masses or the axis of rotation.
* **Correction:** $I = \sum m_i r_i^2$. Here, $r_i$ is the perpendicular distance from the *axis of rotation*, not necessarily the distance from the origin.

**Key Concept to Lock In:**
* **Hollow vs. Solid:** You correctly identified that for the same mass and radius, a hollow pipe has higher rotational kinetic energy ($I \approx MR^2$) than a solid cylinder ($I = \frac{1}{2}MR^2$).
* *Reasoning:* Mass further from the center = harder to rotate = higher $I$.

---

## 3. Static Equilibrium (Torque & Forces)

**The Mistake:**
Solving for tension in a wire holding a beam. You initially tried to solve it using only forces ($\sum F_y = 0 \Rightarrow T - 24 = 0$), which yielded 24N. This is incorrect because the hinge also exerts a vertical force that you didn't account for.
* **Correction:** You correctly fixed this later by using Torque ($\sum \tau = 0$).

**Strategy for These Questions:**
1.  **Pick a Pivot:** Always choose the pivot point where the *unknown forces are greatest* (usually the hinge/pin). This eliminates those forces from the torque equation because their lever arm is zero.
2.  **Sum of Torques:** $\sum \tau = 0$. Be careful with signs (Counter-Clockwise is positive, Clockwise is negative).
3.  **Sum of Forces:** Only use $\sum F_x = 0$ and $\sum F_y = 0$ *after* finding unknowns via torque, usually to find the reaction forces at the hinge.

---

## 4. Work & Energy

**The Mistake:**
Confusion regarding the signs for work.
* **Work by Friction:** Always negative (kinetic friction acts opposite to displacement).
* **Work by Gravity:**
    * Moving UP: Gravity does **negative** work.
    * Moving DOWN: Gravity does **positive** work.
* **Potential Energy ($U$):**
    * Moving UP: $\Delta U$ is positive.
    * Moving DOWN: $\Delta U$ is negative.
* **Relation:** $W_{grav} = -\Delta U_{grav}$.

**The Mistake:**
Calculating work done by gravity on a skier. You noted "remember force down is positive".
* **Clarification:** Work depends on the *change in height* only, not the path taken.
    $$W_g = mg(h_{initial} - h_{final})$$
    If $h_{initial} > h_{final}$ (going down), Work is positive.

---

## 5. Simple Harmonic Motion (SHM)

**The Mistake:**
Calculating the phase angle $\phi$. You wrote $\cos(1) = \pi t$, which indicates confusion on how to extract the phase constant from initial conditions.
* **The Trap:** Many students assume $\phi = 0$ or guess.

**How to Answer:**
1.  Use the displacement equation: $x(t) = A \cos(\omega t + \phi)$.
2.  At $t=0$, $x_0 = A \cos(\phi) \implies \cos(\phi) = x_0/A$.
3.  **CRITICAL STEP:** Check velocity. $v(t) = -A\omega \sin(\omega t + \phi)$.
4.  At $t=0$, $v_0 = -A\omega \sin(\phi)$.
5.  The sign of $v_0$ tells you which quadrant $\phi$ is in (since your calculator's $\arccos$ function only gives values in Q1 or Q2).

---

## 6. Rolling Motion & Friction

**The Mistake:**
Determining the direction of friction on a rolling spool. You marked "A" (left) for a string pulling to the left.
* **Concept:** Static friction opposes the tendency to slip.
* **Correction:** If you pull the top of a wheel to the *left*, the wheel wants to rotate counter-clockwise, but the Center of Mass also accelerates left.
    * **Rule of Thumb:** If the pulling force provides "too much" torque (pulling the top), friction acts in the direction of motion to prevent spinning out. If the pulling force provides "too much" linear acceleration (pulling the center), friction acts opposite to motion.

---

## 7. Summary of Formulas & Concepts to "Lock In"

Based on your notes, these are the concepts you circled or highlighted, meaning they are high-priority for you to memorize:

1.  **RPM to Rad/s:** You noted "This is velocity, not time! LOCK IN."
    * **Conversion:** $1 \text{ rpm} = \frac{2\pi}{60} \text{ rad/s}$. Always convert immediately.
2.  **Power:**
    * Rotational: $P = \tau \omega$
    * Linear: $P = \vec{F} \cdot \vec{v}$
3.  **Impulse:** $J = \Delta p = F_{avg} \Delta t$.
4.  **Parallel Axis Theorem:** $I = I_{cm} + Md^2$.
5.  **Dot Product vs Cross Product:**
    * Work = Dot Product ($W = \vec{F} \cdot \vec{d}$) $\rightarrow$ Scalar result.
    * Torque = Cross Product ($\vec{\tau} = \vec{r} \times \vec{F}$) $\rightarrow$ Vector result.

---

## 8. Action Plan

1.  **Redo the "Truss" Questions:** You struggled with specific truss diagrams. Practice the "Method of Joints" specifically. Look for zero-force members (T-joints with no external load).
2.  **Practice Phase Angles:** Pick 3 SHM problems where $t=0$ is *not* at max amplitude and calculate $\phi$ carefully.
3.  **Torque Signs:** When setting up $\sum \tau = 0$, draw the pivot, draw the force vector, and use the Right Hand Rule or standard convention (CCW +, CW -) strictly. Do not skip this step.
