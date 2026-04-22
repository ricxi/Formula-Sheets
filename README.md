# Formulas
- Matrices
    - Determinant for 2x2 Matrix
    - Inverse Formula for 2x2 Matrix
    - Algebraic Properties of Matrices
- Vectors
    - Dot Product
    - Projection
    - Cross Product ($\mathbb{R}^3$)
    - Cross Product Magnitude ($\mathbb{R}^3$)
    - Cross Product Algebraic Properties
    - Scalar Triple Product


## Inverse of 2x2 Matrix
The matrix
```math
A
=
\begin{vmatrix}
a & b \\
c & d
\end{vmatrix}
```
is invertible if and only if $ad-bc \neq 0$, in which case the inverse formula is:
```math
A^{-1} 
=
\frac{1}{ad-bc} 
\begin{vmatrix}
d & -b \\
-c & a
\end{vmatrix}
```

## Algebraic Properties of Matrices
If $A$ is an invertible matrix, then $A^{T}$ is an invertible matrix, and:
```math
(A^{T})^{-1} = (A^{-1})^{T} 
```

### Properties of Transposes
```math
(A \pm B)^{T} = A^{T} \pm B^{T}
```
```math
(cA)^{T} = cA^{T}
```
```math
(AB)^{T} = B^{T}A^{T}
```
```math
(A^{T})^{T} = A
```

### Properties of Inverses

1. 
```math
AA^{-1} = A^{-1}A = I
```
2. If $A$ multiplies $B$ equals $I$, then $A$ and $B$ are inverses of each other.
3. If $A$ and $B$ are invertible matrices of the same size, then $AB$ is invertible and:
```math
(AB)^{-1} = B^{-1}A^{-1}
```
Extended to: if $A$, $B$, and $C$ are invertible matrices of the same size, then $ABC$ is invertible and:
```math
(ABC)^{-1} = C^{-1}B^{-1}A^{-1}
```
  
4. If $A$ is invertible and $n$ is a non-negative integer, then:
- $A^{-1}$ is invertible and $(A^{-1})^{-1} = A$
- $A^{n}$ is invertible and $(A^{n})^{-1} = A^{-n} = (A^{-1})^{n}$
- $kA$ is invertible for any scalar $k$ different than zero, and $(kA)^{-1} = k^{-1}A^{-1}$


### Properties of Diagonal Matrices 
- The determinant of a diagonal matrix is the product of all the entries in the diagonal.
1. Find the inverse of a diagonal matrix by replacing all the non-zero entries by their reciprocals.
2. Find the power of a diagonal matrix by replacing the entries by the the corresponding power of each entry.

### Properties of Symmetric Matrices 
1. If $A$ and $B$ are symmetric matrices of the same size, and if $k$ is a scalar, then:
    - $A^{T}$ is symmetric
    - $A+B$ and $A-B$ are symmetric
    - $kA$ is symmetric
2. If $A$ is an invertible symmetric matrix, then $A^{-1}$ is symmetric.
3. The product of a matrix and its transpose is symmetric.
4. If $A$ is a square invertible matrix, then $AA^{T}$ and $A^{T}A$ are also invertible.

### Properties of Determinants
1. $det(kA) = k^{n}det(A)$, where $n$ is the size of the square matrix A.
2. $det(A+B) \neq det(A)+det(B)$
3. A square matrix is invertible if and only if $det(A) \neq 0$
4. If $A$ and $B$ are square matrices of the same size, then $det(AB) = det(A)det(B)$
5. If $A$ is invertible, then:
```math
det(A)^{-1} = \frac{1}{det(A)}
```

## Dot Product

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

## Projection
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

## Cross Product in $\mathbb{R}^3$
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

## Cross Product's Magnitude in $\mathbb{R}^3$ 
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

## Cross Product Algebraic Properties
If $\vec{u}$, $\vec{v}$, and $\vec{w}$ are vectors in a 3-dimensional space and $k$ is a scalar, then the following properties are true:

1) $\vec{u} \times \vec{v} = - (\vec{v} \times \vec{u})$
2) $\vec{u} \times (\vec{v} + \vec{w}) = (\vec{u} \times \vec{v}) + (\vec{u} \times \vec{w})$
3) $k(\vec{u} \times \vec{v}) = (k\vec{u}) \times \vec{v} = \vec{u} \times (k\vec{v})$
4) $\vec{u} \times \vec{0} = \vec{0} \times \vec{u} = \vec{0}$
5) $\vec{u} \times \vec{u} = \vec{0}$
6) $\vec{u} \cdot (\vec{v} \times \vec{w}) = (\vec{u} \times \vec{v}) \cdot \vec{w}$ 
  
Number 6 is related to the scalar triple product.


## Scalar Triple Product
Also known as the Triple Scalar Product

### Volume of a Paralelepiped formed by the vectors $\vec{a}$, $\vec{b}$, and $\vec{c}$.
Method 1:
```math
V = Ah = \|\vec{b} \times \vec{c} \| \| \vec{a} \| \| \cos\theta \| = \|\vec{a} \cdot (\vec{b} \times \vec{c}) \|
```

Method 2 (returns a scalar value):
```math
V 
= 
|\vec{a} \cdot (\vec{b} \times \vec{c})|
=
\begin{vmatrix}
a_1 & a_2 & a_3 \\
b_1 & b_2 & b_3 \\
c_1 & c_2 & c_3
\end{vmatrix}
```
Take the absolute value of the returned scalar.
If the value return is 0, then then all three vectors are coplanar.











# Notes
- Unit 5
- Unit 6


## Unit 1
- Types of Solutions for Linear Systems
    - One unique solution (trivial)
    - No solution (system is inconsistent)
    - Infinitely many solutions (non-trivial; represent with parametric equations)


## Unit X
- A matrix is not invertible if its determinant is 0 ($ad-bc=0$)

## Unit 5
- Component Form
- Linear Combinations?
- Unit Vectors

## Unit 6
### 6.1
- The dot product of two vectors is a **scalar**.
    - Sometimes called the scalar product or the Euclidean inner product
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
- Area of Parallelogram (with cross product):
    1. Calculate the vectors if given vertices.
    2. Get the cross product of the two vectors (determinate formula).
    3. Calculate the norm (magnitude) of the cross product.
    - The magnitude of the cross product equals the area of the parallelogram that the two vectors span: $\|\vec{u} \times \vec{v}\| = \|\vec{u}\| \, \|\vec{v}\| \sin\theta$
- Area of Triangle (with cross product):
    1. Calculate the vectors if given vertices.
    2. Get the cross product of the two vectors (determinate formula).
    3. Calculate the norm (magnitude) of the cross product.
    4. Divide the magnitude by 2 to get the area of the triangle.
    - Same as calculating the area of the parallelogram, but you divide by 2 at the end.


### 6.4
- **Triple Scalar Product** is used to find if three vectors are coplanar. 
- If the triple scalar product is 0, then the three vectors are coplanar
- Volume of parallelipiped with Triple Scalar Product
    1. Calculate the determinate (it should return a scalar)
    2. Take the absolute value of the determinate
