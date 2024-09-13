# Lecture Notes: Stresses on Inclined Sections

### 1. Introduction to Axial Loading

- **Axial Loading** occurs when forces are applied along the longitudinal axis of a bar, generating **normal stresses** on sections perpendicular to the axis.

  **Normal Stress Formula**: 
  $$\sigma_x = \frac{P}{A}$$

  ![Axial Stress Diagram](/Figures/2024-09-13-12-07-01.png)

---

### 2. Stress on Inclined Sections

- When a bar is subjected to axial force **P**, stresses also act on **inclined sections** (not just on perpendicular sections). These stresses consist of:
  - **Normal force (N)** perpendicular to the inclined plane.
  - **Shear force (V)** parallel to the inclined plane.

#### Equations of Forces:
- Normal force:
  $$N = P \cos(\theta)$$
- Shear force:
  $$V = P \sin(\theta)$$

  ![](/Figures/2024-09-13-12-09-49.png)

  ![](/Figures/2024-09-13-12-10-40.png)

---

### 3. Calculating Normal and Shear Stresses

- The normal and shear stresses on the inclined plane are derived from the forces acting on it. Since the inclined plane has a larger area than the cross-section perpendicular to the axis, we calculate its area as:
  $$A_1 = \frac{A}{\cos(\theta)}$$

    ![](/Figures/2024-09-13-12-30-46.png)

#### Normal and Shear Stress Equations:
1. **Normal Stress**:
  $$\sigma_\theta = \sigma_x \cos^2(\theta) = \frac{1}{2} \sigma_x (1 + \cos 2\theta)$$
2. **Shear Stress**:
  $$\tau_\theta = - \sigma_x \sin(\theta) \cos(\theta) = \frac{1}{2} \sigma_x \sin 2\theta$$

    Where $\theta$ is the inclination of the plane and $\sigma_x$ is the normal stress on the perpendicular cross-section.

    ![](/Figures/2024-09-13-13-07-32.png)

3. **Maximum normal stress** occurs when $\theta=0$:
   $$\sigma_\text{max} = \sigma_x$$
4. **Maximum shear stress** occurs at $\theta=45 ^ \circ$:
   $$\tau_\text{max} = \frac{\sigma_x}{2}$$

  These maximum stress points are critical for analyzing failure in materials.

  ![](/Figures/2024-09-13-13-08-27.png)

---

### 4. Example Problem

#### Example: Stress on an Inclined Plane at 30°
- A bar is subjected to axial load **P**, and we want to calculate the normal and shear stresses on an inclined section at $\theta = 30^\circ$.
- Given: $\sigma_x = 50 \text{ MPa}$.

1. **Normal Stress**:
  $$\sigma_{30} = 50 \times \cos^2(30^\circ) = 37.5 \ \text{MPa}$$
2. **Shear Stress**:
  $$\tau_{30} = 50 \times \sin(30^\circ) \cos(30^\circ) = 21.7 \ \text{MPa}$$

---

### 5. Summary

- Stresses on inclined sections are a combination of **normal** and **shear stresses**.
- **Maximum normal stress** occurs when \( \theta = 0^\circ \), and **maximum shear stress** occurs when \( \theta = 45^\circ \).
- Understanding these stress distributions is essential for predicting material failure, especially in **shear failure** scenarios.


