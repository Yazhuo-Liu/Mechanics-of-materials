# Speech Script: Thermal Strain and Static Indeterminate Problems

## 1. Introduction to Thermal Effects

**Good morning everyone, today we'll be diving into the effects of temperature changes on materials and how thermal expansion can affect structures, particularly in statically indeterminate systems.**

Let’s start with thermal strain. Thermal strain occurs when a material experiences a change in temperature. This strain is independent of any external forces and arises purely from the temperature difference.

The formula for thermal strain is given by:

$$\epsilon_T = \alpha \Delta T$$

Where:
- $\alpha$ is the **coefficient of thermal expansion**,
- $\Delta T$ is the **change in temperature**,
- $\epsilon_T$ is the **thermal strain** (positive for expansion, negative for contraction).

### Units for $\alpha$:
In SI units, $\alpha$ is expressed as $1/\text{K}$ or $1/^\circ C$. In USCS units, it's $1/^\circ F$.

### Sign Convention for Thermal Strain:
- If the temperature increases, the thermal strain is positive, meaning the material expands.
- If the temperature decreases, the thermal strain is negative, meaning the material contracts.

### Example Calculation:

Let’s take a stainless steel bar with:
- $E = 30 \times 10^6 \ 	ext{psi}$ (modulus of elasticity),
- $\alpha = 9.6 \times 10^{-6} \ / \ ^\circ F$ (coefficient of thermal expansion).

For a temperature increase of $\Delta T = 100^\circ F$, the stress can be calculated as:

$$
\sigma = E \alpha \Delta T = (30 \times 10^6) \times (9.6 \times 10^{-6}) \times 100 = 29,000 \ 	ext{psi}
$$

This shows that even a modest temperature change can induce significant stresses in the material.

### Difference between Thermal Strain and Mechanical Strain:
- **Thermal strain** results from temperature changes, not external forces.
- **Mechanical strain** arises from applied loads.

---

## 2. Thermal Expansion in Structures

Now, moving on to **thermal expansion in structures**. When an object, such as a block, expands freely without restraint, no stresses develop.

### Thermal Displacement Formula:

$$\delta_T = L \alpha \Delta T$$

Where:
- $L$ is the original length,
- $\alpha$ is the coefficient of thermal expansion,
- $\Delta T$ is the change in temperature,
- $\delta_T$ is the elongation.

### Example:

For a bar with:
- $L = 1 \ 	ext{m}$,
- $\alpha = 12 \times 10^{-6} \ / \ ^\circ C$,
- $\Delta T = 50^\circ C$,

The expansion is:

$$
\delta_T = (1) \times (12 \times 10^{-6}) \times 50 = 0.6 \ 	ext{mm}
$$

So, a modest temperature change can cause a visible elongation in a material.

---

## 3. Thermal Stresses in Restrained Structures

Let’s talk about **statically determinate structures**. If expansion is unrestrained, thermal expansion does not generate stresses. A good example is a two-bar truss heated uniformly—it will elongate but won’t develop stresses.

**However**, in **statically indeterminate structures**, thermal stresses arise when expansion is restrained. If only some parts of the structure are heated, the structure's constraints prevent free expansion, causing thermal stresses.

---

## 4. Example: Statically Indeterminate Bar with Uniform Temperature Increase

Now, let’s walk through an example of a **statically indeterminate bar** with both ends fixed and heated uniformly.

- A bar $AB$ with length $L$, modulus $E$, and coefficient of thermal expansion $\alpha$, is fixed at both ends.

- The temperature increase $\Delta T$ induces **thermal stress** in the bar, as the rigid supports prevent free expansion.

### Step-by-Step Thermal Stress Derivation:

1. **Equation of Equilibrium**:
   $$R_A + R_B = 0$$
   Since this is a statically indeterminate problem, we have more unknowns than equilibrium equations.

2. **Compatibility Equation**:
   The total elongation of the bar is zero due to the fixed ends:

   $$\delta_{AB} = \delta_T + \delta_B = 0$$

   Where:
   - $\delta_B$ is the displacement due to external forces: 
   $$\delta_B = \frac{R_B L}{EA}$$
   - $\delta_T$ is the thermal displacement:
   $$\delta_T = \alpha \Delta T L$$

3. **Solving for Reaction Forces**:
   $$R_A = -R_B = E A \alpha \Delta T$$

4. **Thermal Stress**:
   $$\sigma_T = \frac{R_A}{A} = E \alpha \Delta T$$

   This stress develops because the bar cannot expand freely. If $\Delta T > 0$, the bar tends to expand, but the supports create compressive stresses.

---

## Conclusion:
- **Key Takeaways**:
  - Thermal expansion can cause significant strain and stress, especially when structures are restrained.
  - Understanding statically indeterminate structures is essential for designing systems that can handle thermal stresses without failure.

---

**Thank you! Let’s move on to the next topic or feel free to ask questions on anything we’ve discussed.**
