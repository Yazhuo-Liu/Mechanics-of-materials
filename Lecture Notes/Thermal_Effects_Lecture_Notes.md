
# Lecture Topic: Thermal Effects and Statically Indeterminate Problems

---

### 1. Introduction to Thermal Effects

- **Thermal Strain:**
  - When a material experiences a change in temperature, it undergoes **thermal strain**, which is independent of any external forces. If the material is allowed to expand freely, no internal stresses will develop.
  - **Thermal Strain Formula**:
    $$\epsilon_T = \alpha \Delta T$$
    - $\alpha$ is the **coefficient of thermal expansion**, which varies by material.
    - $\Delta T$ is the **change in temperature**.
    - $\epsilon_T$ is the **thermal strain** (positive for expansion, negative for contraction).

- **Units for $\alpha$**:
  - In SI units: $\alpha$ is expressed in $1/\text{K}$ or $1/^\circ C$.
  - In USCS units: $\alpha$ is in $1/^\circ F$.
  - **Sign Convention for Thermal Strain**: 
    - If the temperature **increases**, the thermal strain $\epsilon_T$ is **positive** (expansion).
    - If the temperature **decreases**, the thermal strain $\epsilon_T$ is **negative** (contraction).

- **Example Calculation**: 
  - Let’s consider a **stainless steel** bar where:
    - $E = 30 \times 10^6 \ 	ext{psi}$ (modulus of elasticity),
    - $\alpha = 9.6 \times 10^{-6} \ /\ ^\circ F$ (coefficient of thermal expansion).
  - A temperature increase of $\Delta T = 100^\circ F$ produces the same strain as a stress:
    $$
    \sigma = E \alpha \Delta T = (30 \times 10^6) \times (9.6 \times 10^{-6}) \times 100 = 29,000 \ 	ext{psi}
    $$
    This shows how even a **modest change in temperature** can induce significant stresses.

- Difference between ***thermal strain*** and ***mechanical strain***:
  - Thermal strain arises from temperature changes, not external forces.
  - Mechanical strain results from applied loads.

- **Isotropic** vs. **Anisotropic** Materials:
  - Isotropic materials have uniform thermal expansion in all directions.
  - Anisotropic materials exhibit different expansions depending on the direction.

---

### 2. Thermal Expansion in Structures

- **Free Thermal Expansion**: 
  - For a **free object** (like a block), thermal expansion occurs without developing stresses

    ![](/Figures/2024-09-13-01-09-31.png)
  
  
  - **Thermal Displacement Formula**:
    $$\delta_T = L \alpha \Delta T$$
    - $L$ is the original **length of the object**.
    - $\alpha$ is the coefficient of thermal expansion.
    - $\Delta T$ is the change in temperature.
    - $\delta_T$ is the **elongation** (displacement) due to thermal expansion.

  - Example:
    - For a bar of length $L = 1 \ 	ext{m}$, $\alpha = 12 \times 10^{-6} \ /\ ^\circ C$, and $\Delta T = 50^\circ C$, the expansion is:
      $$
      \delta_T = (1) \times (12 \times 10^{-6}) \times (50) = 0.6 \ 	ext{mm}
      $$

- **Thermal Strain in a Bar**:
  - In a prismatic bar (Figure 2-38), thermal expansion is uniform along the bar, and the increase in length is given by:
    $$\delta_T = L \alpha \Delta T$$

    ![](/Figures/2024-09-13-01-12-54.png)

---

### 3. Thermal Stresses in Restrained Structures

- **Statically Determinate Structures**:
  - In **statically determinate structures**, if expansion is **unrestrained**, no thermal stresses develop.
  - **Example**: A two-bar truss (Figure 2-39) heated uniformly will elongate, but no stresses are created because the structure is free to expand.

    ![](/Figures/2024-09-13-01-12-02.png)

- **Statically Indeterminate Structures**:
  - When thermal expansion is **restrained** in a statically indeterminate structure, **thermal stresses** develop.
  - If only some parts of the structure are heated, thermal stresses occur because the structure prevents free expansion.

    ![](/Figures/2024-09-13-01-14-23.png)

---

### 4. Example Problems

---

#### Example: Statically Indeterminate Bar with Uniform Temperature Increase

- **Setup**:
  - A bar (AB) of length $L$, modulus $E$, and thermal expansion coefficient $\alpha$, is **fixed at both ends**.

    ![](/Figures/2024-09-13-01-35-03.png)

  - Temperature increase: $\Delta T$.
  - Find the thermal stress $\sigma_T$

- **Thermal Stress Derivation**:
  1. **Equation of equilibrium**:
      $$R_A + R_B = 0$$
      - Two unknowns, 1 equation -- Statically indeterminate structure.

  2. **Compatibility Equation**: 

      ![](/Figures/2024-09-13-01-35-38.png)

     - The total elongation is zero due to the fixed ends, so:
       $$\delta_{AB} = \delta_T + \delta_B = 0$$
     - $\delta_R$ is the displacement due to external forces:
       $$\delta_B = \frac{R_B L}{EA}$$
     - $\delta_T$ is the displacement due to thermal expension:
       $$\delta_T = \alpha (\Delta T) L$$
  
  3. **Solving for Reaction Forces**:
     $$R_A = - R_B = E A \alpha \Delta T$$

  4. **Thermal Stress**:
     $$\sigma_T = \frac{R_A}{A} = E \alpha \Delta T$$
     - This stress develops because the bar cannot expand freely.
     - If $\Delta T>0$, the bar **tends to expand**, but the rigid supports prevent this expansion, leading to the development of **compressive stresses**

- Notes:
  - $R_A$, $R_B$ are independent of $L$
  - $\sigma$ is independent of $L$ and $A$
  - Zero axial strains everywhere, non-zero transverse strains.
  - Longitudinal stress without longitudinal strains

---

### Conclusion
- **Key Takeaways**:
  - Thermal expansion can cause significant strain and stress, especially when structures are restrained.
  - Understanding statically indeterminate structures is essential for designing systems that can handle thermal stresses without failure.
