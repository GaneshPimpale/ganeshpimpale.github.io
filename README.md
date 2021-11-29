# My linalg Notes as a test...

# 6.2
## Orthogonal Sets
### Orthogonal Sets
A set of vectors, $\{u_1, ..., u_p\}$, is said to be an **orthogonal set** if each pair of distinct vectors from the set is orthogonal:
> $u_i \cdot u_j = 0$ whenever $i \neq i$

Theorem:
> If $S = \{u_1, ..., u_p\}$ is an orthogonal set of nonzero vectors in $\mathbb{R}^n$, then S is linearly independent and hence a basis for the subspace spanned by S.
> [[4.3 Linearly Independent Sets; Bases]]
> [[1.7 Linear Independence]]
> [[1.3 Vector Equations#Span]]

An **orthogonal basis** for a subspace W of $\mathbb{R}^n$ is a basis for W that is also an orthogonal set

Orthogonal bases are much easier to use since the weights of a linear combination can be computed easily:
> Let $\{u_1, ..., u_p\}$ be an orthogonal basis for a subspace W of $\mathbb{R}^n$. For each y in W, the weights in the linear combination
> $$y = c_1u_1+...+c_pu_p$$
> are given by:
> $$c_j = \frac{y \cdot u_j}{u_j \cdot u_j}, (j = 1, ..., p)$$

#### Example
![[Pasted image 20211031210441.png]]
![[Pasted image 20211028100438.png]]

### An Orthogonal Projection
Given a nonzero vector u in $\mathbb{R}^n$, we want to decompose a vector y in $\mathbb{R}^n$ into the sum of a multiple of u and a vector orthogonal to u:
> $$y = \hat{y} + z$$

To find the orthogonal projection of y onto L:
> $$\hat{y} = proj_Ly = \frac{y \cdot u}{u \cdot u}u$$

Image of the orthogonal projection of y onto W:
![[Pasted image 20211028122227.png]]

To check the calculations above, the result of $\{\hat{y}, y-\hat{y}\}$ will be an orthogonal set:
> $$\hat{y} \cdot (y-\hat{y}) = 0$$

### Geometric Interpretation
This is the geometric understanding of the theorem stating that "Orthogonal bases are much easier to use". 

The theorem decomposes each y in $Span\{u_1, ..., u_p\}$ into the sum of p projections onto one-dimensional subspaces that are all mutually orthogonal. 

$W = \mathbb{R}^2 = Span\{u_1, u_2\}$ with $u_1$ and $u_2$ orthogonal. Any y in $\mathbb{R}^n$ can be written in the form:
> $$y = \frac{y \cdot u_1}{u_1 \cdot u_1}u_1 + \frac{y \cdot u_2}{u_2 \cdot u_2}u_2$$

The first term of the equation above is the projection of y onto the subspace spanned by $u_1$ and the second term is the projection of y onto the subspace spanned by $u_2$. 

Y is expressed as the sum of its projections onto the orthogonal axes determined by $u_1$ and $u_2$:
![[Pasted image 20211028134018.png]]

### Orthonormal Sets
A set $\{u_1, ..., u_p\}$ is an **orthonormal set** if it is an orthogonal set of unit vectors. 

If W is the subspace spanned by such a set, then $\{u_1, ..., u_p\}$ is an orthonormal basis for W since the set will be automatically linearly independent ([[1.7 Linear Independence]])

The following are theorems on orthonormal sets:
> An m x n matrix U has orthonormal columns if and only if $U^TU = I$

> Let U be an m x n matrix with orthonormal columns, and let x and y be in $\mathbb{R}^n$. Then:
> a. $\left\Vert Ux \right\Vert = \left\Vert x \right\Vert$
> b. $(Ux) \cdot (Uy) = x \cdot y$
> c. $(Ux) \cdot (Uy) = 0$ if and only if $x \cdot y = 0$

The theorems above are useful for square matrices. An **orthogonal matrix** is a square invertible matrix U such that $U^{-1} = U^T$.

Any square matrix with orthonormal columns is an orthogonal matrix.