# Lecture Notes: Torsion in Circular Shafts

## 1. Introduction to Torsion

- **Definition:** Torsion refers to the twisting of a straight bar when it is loaded by moments (torques) about its longitudinal axis.
  
  **Examples:**
  - Turning a screwdriver
  - Drive shafts in automobiles
  - Axles, propeller shafts, and drill bits

---

## 2. Torque and Moment of a Couple

- **Torque (T):** The moment produced by two equal and opposite forces acting at a distance.
  
  **Formula:**  

    $$T = F \times d$$

  where:
  - $F$ is the applied force
  - $d$ is the perpendicular distance between forces.

- **Units of Torque:**
  - SI: Newton-meter (N·m)
  - USCS: Pound-foot (lb·ft), Pound-inch (lb·in)

- **Representation:**  
  Torques can be represented as vectors or curved arrows depending on preference.

![](/Figures/2024-09-13-15-25-04.png)

---

## 3. Distinguishing Torque and Bending Moment

- **Torque (Torsion):** A moment that twists an object around its longitudinal axis. It produces **shear stresses** and results in **twisting deformation**.
  
- **Bending Moment:** A moment that bends an object, creating **tensile and compressive stresses** across the cross-section. It results in **bending deformation**.

#### **Key Point:**  
- Torque causes twisting, while bending moments cause flexure. Both involve moments but act in fundamentally different ways on materials.

---

## 4. Torsional Deformation of Circular Bars

- **Deformation:** Consider a circular bar subjected to a torque $T$ applied at both ends.
  - Each cross-section rotates relative to the fixed end.
  - Cross sections remain plane, circular, all radii remain straight.
  - If angle of rotation is small, lenght of the bar and its radius remain unchanged.

- **Angle of Twist $\phi$:**  
  The angular displacement between two sections.

![](/Figures/2024-09-13-15-26-34.png)



- **Shear Strain $\gamma$:**  
  
  ![](/Figures/2024-09-13-15-28-41.png)

  - **At the Surface:** Maximum shear strain occurs at the outer surface. The shear strain on the surface of the bar is related to the angle of twist as:
  
    $$\gamma_{\text{max}} = \frac{bb'}{ab} = \frac{rd\phi}{dx}$$ 

    where:
    - $r$ is the radius of the bar
    - $\frac{d\phi}{dx}$ is the rate of change of twist along the bar’s length

    if $\theta = \frac{d\phi}{dx}$ is a constant, then
    $$\gamma_\text{max} = r\theta = r \frac{\phi}{L}$$

    where:
    - $L$ is the length of the bar
  - **Strain varies linearly** with radial distance from the center, reaching zero at the center.

    $$\gamma = \rho \frac{d\phi}{dx} = \frac{\rho}{r} \gamma_\text{max}$$ 

---

## 5. Shear Strain in Circular Tubes

- For a **circular tube** with inner radius $r_1$ and outer radius $r_2$, shear strain also varies linearly from the inner to the outer surface.
  
  **Shear strain at inner and outer surfaces:**
  
  $$\gamma_{\text{max}} = \frac{r_2}{L} \cdot \phi$$

  
  $$\gamma_{\text{min}} = \frac{r_1}{r_2} \gamma_\text{max} = \frac{r_1}{L} \cdot \phi$$
  
![](/Figures/2024-09-13-17-02-31.png)

---

## 6. Conclusion

- Torsion creates a state of pure shear.
- Shear strain and stress vary linearly with radial distance from the center of a circular bar, reaching a maximum at the outer surface.
- The equations for shear strain are applicable to both solid bars and hollow tubes.
- the concept of shear strain is a **geometric concept**, valid for any mater but $\phi$ and $\theta$ should be **small**.

---
