# 3D Rigid Body Motion - Chapter 2


## Summary
Study the rigid body geometry in three-dimensional space: the rotation matrix, transformation matrix, quaternion, euler angles. How to describe a rigid body's motion in a three-dimensional space. This consists of one rotation and one translation, the part where problems arise is the rotation one.

## Points, Vectors, and Coordinate Systems
The 3D space consists of three axes, however we should now consider a rigid body, which has it's position and orientation. A point is a basic element in space, a vector is an arrow pointing from one point to another. Let us also remind ourselves that we must not confuse a vector with its coordinates

### How do we describe a point in 3D space?

$$
\mathbf{a} = [\mathbf{e}_1, \mathbf{e}_2, \mathbf{e}_3]
\begin{bmatrix} a_1 \\ a_2 \\ a_3 \end{bmatrix}
= a_1 \mathbf{e}_1 + a_2 \mathbf{e}_2 + a_3 \mathbf{e}_3
$$

A base is a set of linearly independent vectos in the space
We have a base of 3 axes, here, the 3 e's can be seen as x,y,z and a's coordinates are how much each a moves each axis in a direction

### The inner product of $ \mathbf {a}, \mathbf {b} \in  \mathbb {R}^ 3 $ can be written as:

$$
\mathbf{a} \cdot \mathbf{b} = \mathbf{a}^T \mathbf{b}
= \sum_{i=1}^{3} a_i b_i
= |\mathbf{a}| \, |\mathbf{b}| \cos\langle \mathbf{a}, \mathbf{b} \rangle
$$

### The outer 

![The result of the outer product can be seen as another vector who is perpendicular to the two vectors](images/cross-product.svg)

