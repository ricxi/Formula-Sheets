# Formula Sheet
Formulas and Notes

## Formulas

### Dot Product
The dot product can be written in two ways for vectors $\vec{u} = (u_1, u_2, \dots, u_n)$ and $\vec{v} = (v_1, v_2, \dots, v_n)$ :
  
Method 1: 
```math
\vec{u} \cdot \vec{v} = u_1v_1 + u_2v_2 + \cdots + u_nv_n
```

Method 2:
```math
\vec{u} \cdot \vec{v} = \|\vec{u}\| \, \|\vec{v}\| \cos\theta
```
```math
\cos\theta = \frac{\vec{u} \cdot \vec{v}}{\|\vec{u}\| \, \|\vec{v}\|}
```

### Projection
The projection of $\vec{u}$ onto $\vec{v}$ is

```math
\mathrm{proj}_{\vec{v}}\,\vec{u}
=
\left(\frac{\vec{u}\cdot\vec{v}}{\|\vec{v}\|^2}\right)\vec{v}
```
Equivalently,
```math
\mathrm{proj}_{\vec{v}}\,\vec{u}
=
\left(\frac{\vec{u}\cdot\vec{v}}{\vec{v}\cdot\vec{v}}\right)\vec{v}
```

### Cross Product in $\mathbb{R}^3$
For vectors $\vec{u} = (u_1, u_2, u_3)$ and $\vec{v} = (v_1, v_2, v_3)$ in $\mathbb{R}^3$, the cross product is

```math
\vec{u} \times \vec{v}
=
\begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3
\end{vmatrix}
```

```math
\vec{u} \times \vec{v}
=
\begin{vmatrix}
u_2 & u_3 \\
v_2 & v_3
\end{vmatrix}
\hat{i}
-
\begin{vmatrix}
u_1 & u_3 \\
v_1 & v_3
\end{vmatrix}
\hat{j}
+
\begin{vmatrix}
u_1 & u_2 \\
v_1 & v_2
\end{vmatrix}
\hat{k}
```

```math
\vec{u} \times \vec{v}
=
\bigl(u_2v_3 - u_3v_2,\; u_3v_1 - u_1v_3,\; u_1v_2 - u_2v_1\bigr)
```

### Cross Product's Magnitude in $\mathbb{R}^3$ 
For $\vec{u}, \vec{v} \in \mathbb{R}^3$, this is the magnitude of the cross product, where $\theta$ is the angle between the vectors.
```math
\|\vec{u} \times \vec{v}\|
=
\sqrt{
(u_2v_3-u_3v_2)^2
+
(u_3v_1-u_1v_3)^2
+
(u_1v_2-u_2v_1)^2
}
```

Geometric Version:
```math
\|\vec{u} \times \vec{v}\| = \|\vec{u}\| \, \|\vec{v}\| \sin\theta
```
## Notes
- Unit 5
- Unit 6

## Unit 5
- Component Form
- Linear Combinations?
- Unit Vectors

## Unit 6
### 6.1
- The dot product of two vectors is a **scalar**.
- Two vectors are **perpendicular** to one another if the dot product is **0**.
- **Algebraic Properties of the Dot Product** (see page 59; 60 in pdf)

### 6.2
- In vectory geometry, perpendicular vectors are known as **orthogonal vectors**.
- **Mutually Orthogonal**: all the vectors are perpendicular to each other (e.g.: for a,b,c ab=0, bc=0, and ac=0)
- When all pairs of distinct vectors in a set of vectors are orthogonal, the set of vectors is known as an **orthogonal set**.
- An **orthonormal set** of vectors is an orthogonal set that contains only unit vectors. This means that not only are pairs of distinct vectors in the set orthogonal, they also each has a
magnitude of 1. Get the magnitudes, and then get the dot products.
- **Projection** of u onto v

### 6.3
- For vectors in R3, the **cross product** provides a systematic way to determine a vector that is mutually orthogonal to two other vectors.
- The result of the **cross product** is a vector.
- Area of Triangle with cross product
- Area of parallelogram with cross product
    - The magnitude of the cross product equals the area of the parallelogram that the initial two vectors span.

### 6.4
- **Triple Scalar Product** is used to find if three vectors are coplanar. 
- If the triple scalar product is 0, then the threee vectors are coplanar
- Volume of parallelipiped with Triple Scalar Product
