# Lecture Notes: Circular Bars of Linearly Elastic Materials

## 1. Review of tortional deformation

![](/Figures/2024-09-13-15-28-41.png)

**Shear strain ($\gamma$) in Torsion** is defined as the angular displacement between two lines that were initially perpendicular to each other on a cross-sectional plane of the bar.
  
In a bar subjected to torsion, the ends twist relative to each other, causing 

- shear deformation in the surface.

    $$\gamma_\text{max} = \frac{r d\phi}{dx} = r\theta$$

    where $\theta = \frac{d\phi}{dx}$ is the rate of twist.

  - In pure torsion,
      $$\theta = \frac{\phi}{L}$$
      therefore
      $$\gamma_\text{max} = r\theta = r\frac{\phi}{L}$$

- shear deformation in the bar

    $$\gamma = \rho \theta = \frac{\rho}{r} \gamma_\text{max}$$

- For a **circular tube** with inner radius $r_1$ and outer radius $r_2$, shear strain also varies linearly from the inner to the outer surface.
  
    $$\gamma_{\text{max}} = \frac{r_2}{L} \cdot \phi$$

    
    $$\gamma_{\text{min}} = \frac{r_1}{r_2} \gamma_\text{max} = \frac{r_1}{L} \cdot \phi$$
  
    ![](/Figures/2024-09-13-17-02-31.png)

---

## 2. Shear Stress in Circular Bars

![](/Figures/2024-09-13-21-07-25.png)

Remember that stress elements are actually three-dimensional objects with a thickness perpendicular to the plane of the figure.

### **2.1 Hooke’s Law for Shear**
- For a **linearly elastic material**, the shear stress $\tau$ is proportional to the shear strain $\gamma$ according to **Hooke’s Law**:

  $$\tau = G \gamma$$

  where:
  - $\tau$ is the shear stress,
  - $G$ is the **shear modulus** (material property),
  - $\gamma$ is the shear strain.
  -  The maximum shear stress:
    $$\tau_\text{max} = G\gamma_\text{max} = G r \theta $$

- Combining this with the expression for shear strain, we get the shear stress at a distance $\rho$ from the center of the bar:

  $$\tau(\rho) = G \rho \theta = \frac{\rho}{r} \tau_\text{max}$$

  - This shows that shear stress also varies **linearly** with the radial distance $r$, just like shear strain.



- **Longitudinal** and transverse shear stresses in a circular bar subjected to torsion:

    ![](/Figures/2024-09-13-21-10-49.png)

  - Refer to **Equality of Shear Stresses on Perpendicular Planes**: shear stresses on mutually perpendicular planes of an element are equal
    ![](/Figures/2024-09-13-21-18-22.png)


### 2.2 The Torsion Formula

The **Torsion Formula** allows us to determine the relationship between shear stress and the applied torque $T$. Once this formula is established, it can be used to calculate the stresses and strains in a bar due to any set of applied torques.

- **Shear stress distribution:** The shear stresses acting on a cross-section of a bar act continuously around the section and have a resultant that forms a moment, equal to the applied torque $T$.

#### Derivation:

- **Elemental moment:**  

    ![](/Figures/2024-09-13-21-41-13.png)

  Consider an element of area $dA$ located at a radial distance $\rho$ from the axis of the bar (Figure 3-9). The shear force acting on this element is equal to 

  $$\tau dA$$
  
  where $\tau$ is the shear stress at radius $\rho$. The moment of this force about the axis of the bar is:

  $$dM = \rho \cdot \tau dA$$

  Substituting for $\tau$ from:

  $$\tau = \frac{\rho}{r} \tau_\text{max}$$

  The elemental moment becomes:

  $$dM = \frac{\tau_{\text{max}}}{r} \cdot \rho^2 dA$$

- **Total Torque:**

  To find the total torque, we sum the elemental moments over the entire cross-sectional area:

  $$T = \int_A dM = \frac{\tau_{\text{max}}}{r} \int_A \rho^2 dA
    $$

  The **polar moment of inertia** $I_p$ of the cross-section:

  $$I_p = \int_A \rho^2 dA$$

  then
  
  $$T = \frac{\tau_{\text{max}}}{r} \cdot I_p$$

- **Shear Stress:**

  Rearranging the equation for $T$:

  $$\tau_{\text{max}} = \frac{T \cdot r}{I_p}$$

  Generalized torsion formula:

  $$\tau(\rho) = \frac{\rho}{r} \tau_\text{max} = \frac{T\cdot\rho}{I_p}$$

  - Units:
    - Torque $T$: $N\cdot m$ or $lb\cdot in$
    - Radius $r$: $m$ or $in$
    - Polar moment of inertia $I_p$: $m^4$ or $in^4$
    - Shear stress $\tau$: $Pa$ or $psi$



## 3. Polar Moment of Inertia:

The **polar moment of inertia** ($I_p$) is a property of the cross-sectional shape that quantifies how material is distributed around the axis of twist. It plays a key role in determining the resistance of the bar to torsion.

- For a **solid circular bar** of radius $r$:
    $$I_p = \frac{\pi r^4}{2} = \frac{\pi d^4}{32}$$

    - The maximum shear stress:

    $$\tau_{\text{max}} = \frac{16T}{\pi d^3}$$

- For a **hollow circular tube** with inner radius $r_1$ and outer radius $r_2$:

    $$I_p = \frac{\pi (r_2^4 - r_1^4)}{2}$$



---

## 4. Shear deformation

### 4.1 Rate of twist
The **rate of twist** of a bar made of linearly elastic material can be related to the applied torque $T$. 

If we know $T$, $G$ and geometry, from the torsion formula, we can express the **rate of twist** $\theta$ as:

$$\theta = \frac{\tau_\text{max}}{Gr} = \frac{T}{G I_p}$$

Where:
- $T$ is the applied torque,
- $G$ is the shear modulus of elasticity,
- $I_p$ is the polar moment of inertia of the bar’s cross-section.

- The **rate of twist** $\theta$ is measured in radians per unit length and shows how fast the bar twists per unit length.
- The quantity $G I_p$ is known as the **torsional rigidity** of the bar.

### 4.2 Total Angle of Twist

For a bar in **pure torsion**, the **total angle of twist** $\phi$, which is the rotation angle of one end relative to the other, is given by:

$$\phi = \theta L = \frac{T L}{G I_p}$$

Where:
- $\phi$ is the total angle of twist in radians,
- $L$ is the length of the bar.

This equation shows that the total angle of twist is proportional to the applied torque $T$ and the length of the bar $L$, but inversely proportional to the **torsional rigidity** $G I_p$.

### 4.3 Torsional Stiffness and Flexibility

- Recall in pure tension, the tensile deformation

    $$\delta = \frac{PL}{EA}$$

    - the **axial stiffness**:

        $$k = \frac{EA}{L}$$

    - the **axial flexibility**:

        $$f = \frac{L}{EA}$$

- Similarly, we have the **torsional stiffness** of the bar, which represents the torque required to produce a unit angle of twist:

    $$k_T = \frac{G I_p}{L}$$

- The **torsional flexibility** $f_T$ is the reciprocal of the torsional stiffness, which measures the angle of twist produced by a unit torque:

    $$f_T = \frac{L}{G I_p}$$






## 5. Shear Strain and Stress in Circular Tubes

The same principles apply to **hollow circular tubes**. However, the inner radius $r_1$ and outer radius $r_2$ need to be considered.

The **maximum shear stress** occurs at the outer surface, while the minimum shear stress occurs at the inner surface.

- **Maximum shear stress** at $r = r_2$:

    $$\tau_{\text{max}} = \frac{T \cdot r_2}{I_p}$$

- **Shear stress at the inner radius**:

    $$\tau_{\text{min}} = \frac{T \cdot r_1}{I_p}$$


## 5. Conclusion

- Shear strain and shear stress in circular bars vary **linearly** with the radial distance from the center of the bar.
- The **maximum shear stress** occurs at the outer surface and can be calculated using the **torsion formula**.
- The shear strain and stress in **hollow tubes** follow similar principles, but both inner and outer radii must be considered.