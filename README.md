# Formula-Sheet
MATH 210 Linear Algebra

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

## Projection
The projection of $\vec{u}$ onto $\vec{v}$ is
```math
\mathrm{proj}_{\vec{v}}\,\vec{u}
=
\left(\frac{\vec{u}\cdot\vec{v}}{\vec{v}\cdot\vec{v}}\right)\vec{v}
```
Equivalently,
```math
\operatorname{proj}_{\vec{v}} \vec{u} = \left( \frac{\vec{u} \cdot \vec{v}}{\vec{v} \cdot \vec{v}} \right) \vec{v}
```


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

### 6.4
- **Triple Scalar Product** is used to find if three vectors are coplanar. 
- If the triple scalar product is 0, then the threee vectors are coplanar
- Volume of parallelipiped with Triple Scalar Product

## Formulas & Examples
### Dot Product
For vectors $\vec{u} = (u_1, u_2, \dots, u_n)$ and $\vec{v} = (v_1, v_2, \dots, v_n)$, the dot product is

$$
\vec{u} \cdot \vec{v} = u_1v_1 + u_2v_2 + \cdots + u_nv_n
$$

It can also be written as

$$
\vec{u} \cdot \vec{v} = \|\vec{u}\| \, \|\vec{v}\| \cos\theta
$$

Example:

$$
(1,2,3)\cdot(4,5,6)=1\cdot4+2\cdot5+3\cdot6=32
$$