# Mathematical model
Neural networks can be represented as **function approximators**
$$
	f_\theta(x) = W_L\sigma\left(W_{L-1}\ldots\sigma(W_1x+b_1) + b_{L-1}\right)
$$

where
- $W_i$ weight matrices
- $b_i$ biases
- $\sigma$  activation functions
# Linear algebra
## Numerical structures

| data type | space                        | example          |
| --------- | ---------------------------- | ---------------- |
| scalar    | $x\in R$                     | 9.81             |
| vector    | $x\in R^n$                   | 1d signals       |
| matrix    | $x\in R^{m\times n}$         | grayscale images |
| tensor    | $x \in R^{d_1, \ldots, d_n}$ | color image      |
## Tensors
linear arrangement of a set of K matrices

---
$$X = \begin{pmatrix}X_R & \ X_G & \ X_B\end{pmatrix}$$

![[Pasted image 20260430004104.png]]
## Vectors
- addition $c_i = a_{i} + b_{}$
- scalar prod $(\lambda a)_{i} = \lambda a_{i}$
- dot prod $a \cdot b = \sum_{i=1}^na_{i}b_{i}$
## Matrices
addition $c_{ij} = a_{ij} + b_{ij}$
multiplication $c_{ij} = \sum^P_{k=1}a_{ik}b_{kj}$
### Hadamard product
element-wise multiplication of 2 matrices $A, B \in R^{N\times M}$
$$
(A \circ B)_{ij} = a_{ij}b_{ij} \ \forall i,j
$$
i -> N e j -> M
Use cases
- element-wise normalization
- feature-wise multiplication in attention mechanisms
### Kroneker product
$A \in (R, C)^{P\times Q}$ and $B \in (R, C)^{N\times M}$
$$
A \otimes B = \begin{pmatrix}
a_{11}B & \dots & a_{1Q}B \\
\vdots & \ddots & \vdots \\ \\
a_{P1}B & \ldots & a_{PQ}B
\end{pmatrix} \in (R, C)^{PN\times QM}
$$
### Hermitian matrix
$A \in C^{N\times M}$ (complex domain)
$A^H = [a^*_{ji}]$
Real domain -> $A^H = A^T$
### Reshaping
### Diagonal
### Toeplitz matrix
### Positive semidefinite matrix
### Inverse matrix
#### Matrix inversion lemma
#### Properties
### Pseudoinverse matrix
#### Properties
### Rank and determinant
#### Low-rank approximation

## Algebraic structures
- groups
- rings
- fields
# Geometric interpretation of Linear Transformations
# Metrics and Norms
# Unconstrained Convex Optimization
