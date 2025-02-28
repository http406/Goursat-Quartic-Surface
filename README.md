# Goursat-Quartic-Surface

### **Goursat Quartic Surface Explanation**
The **Goursat Quartic Surface** is a mathematical surface defined by a quartic (fourth-degree) polynomial equation. It is a type of implicit surface that exhibits complex and symmetrical structures, making it useful in 3D visualization, mathematical modeling, and artistic renderings.

Your code implements a version of this surface using **point cloud rendering**, where the surface is represented by points that satisfy a modified Goursat quartic equation.

---

### **Understanding the Equation**
Your code uses the following equation to generate the surface:

\[
x^4 + y^4 + z^4 + k_1 (x^2 + y^2 + z^2)^2 + k_2 a^2 (x^2 + y^2 + z^2) + k_3 a^4 = 0
\]

Where:
- \( x, y, z \) are the 3D coordinates.
- \( k_1, k_2, k_3 \) are constants that shape the surface.
- \( a \) is a scaling factor affecting the overall structure.
- \( (x^2 + y^2 + z^2) \) represents the squared radius from the origin.
- \( (x^2 + y^2 + z^2)^2 \) represents the fourth power of the radius, influencing higher-order surface curvatures.

---

### **Breaking Down the Terms**
1. **\( x^4 + y^4 + z^4 \)**
   - These terms ensure the quartic nature of the equation, leading to symmetric curved structures.

2. **\( k_1 (x^2 + y^2 + z^2)^2 \)**
   - This term introduces a dependence on the squared radius, affecting the overall smoothness and shape of the surface.

3. **\( k_2 a^2 (x^2 + y^2 + z^2) \)**
   - It scales the influence of quadratic terms, modifying the curvature and size of the shape.

4. **\( k_3 a^4 \)**
   - This is an additive constant that shifts the equation, changing the density of valid points.

---

### **How This Works in Your Code**
- The equation is **evaluated for many points** in 3D space.
- If a point satisfies the equation **(i.e., its value is close to zero within a threshold like 0.2)**, it is added to the point cloud.
- The result is a **symmetrical, intricate shape** that visually resembles the structure in your reference image.

---

### **Effect of Constants**
- **\( k_1 \) (-0.5)**: Controls how the squared radius term affects curvature.
- **\( k_2 \) (1)**: Affects the balance between different power terms.
- **\( k_3 \) (-1.5)**: Modifies the overall size and distribution.
- **\( a \) (2)**: Scales the impact of quadratic and quartic terms.

---

### **Summary**
- The **Goursat Quartic** is a fourth-degree algebraic surface.
- The equation defines a **complex, symmetric 3D shape**.
- The **constants \( k_1, k_2, k_3, a \)** allow tuning of its structure.
- Your code **visualizes this shape** using a point cloud in **Three.js**.

Would you like to tweak the parameters to explore different shapes? 🚀
