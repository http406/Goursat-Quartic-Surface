# Goursat-Quartic-Surface

### **Goursat Quartic Surface Explanation**
The **Goursat Quartic Surface** is a mathematical surface defined by a quartic (fourth-degree) polynomial equation. It is a type of implicit surface that exhibits complex and symmetrical structures, making it useful in 3D visualization, mathematical modeling, and artistic renderings.

Your code implements a version of this surface using **point cloud rendering**, where the surface is represented by points that satisfy a modified Goursat quartic equation.

---

### **Understanding the Equation**
Your code uses the following equation to generate the surface:

![Image](https://github.com/user-attachments/assets/7186e3e7-e92e-4f9f-8892-9096340db498)

---

### **Breaking Down the Terms**

![Image](https://github.com/user-attachments/assets/bfeec191-0273-479a-a4a2-c16620a73112)


---

### **How This Works in Your Code**
- The equation is **evaluated for many points** in 3D space.
- If a point satisfies the equation **(i.e., its value is close to zero within a threshold like 0.2)**, it is added to the point cloud.
- The result is a **symmetrical, intricate shape** that visually resembles the structure in your reference image.

---

### **Effect of Constants**

![Image](https://github.com/user-attachments/assets/a0baccce-8273-4770-8a81-bd18f9b74e27)

---

### **Summary**
- The **Goursat Quartic** is a fourth-degree algebraic surface.
- The equation defines a **complex, symmetric 3D shape**.
- The **constants \( k_1, k_2, k_3, a \)** allow tuning of its structure.
- Your code **visualizes this shape** using a point cloud in **Three.js**.

Would you like to tweak the parameters to explore different shapes? 🚀
