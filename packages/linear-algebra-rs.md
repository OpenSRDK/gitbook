---
description: Library of Linear Algebra
---

# Linear Algebra RS

{% hint style="info" %}
**GitHub:** [**https://github.com/OpenSRDK/linear-algebra-rs**](https://github.com/OpenSRDK/linear-algebra-rs)
{% endhint %}

Linear Algebra RS provides a library of linear algebra, which is essential for data science.

First, Linear Algebra RS makes it easy to define the matrix. In detail, the matrix is defined using Rust's macro feature.

Linear Algebra RS provides the ability to create the following matrices, which are very easy to use.

## Matrices supported by Linear Algebra RS

### Matrix distinguished by zero location

* Diagonal Matrix（対角行列）
* Bidirectional Matrix（二重対角行列）
* Tridiagonal Matrix（三重対角行列）
* Triangular Matrix（三角行列）

### Matrix distinguished by component replacement

* Symmetric Matrix（対称行列）
* Hermitian Matrix（エルミート行列）
* Symmetric Packed Matrix
* Hermitian Packed Matrix
* Symmetric Tridiagonal Matrix
* Circulant Matrix（巡回行列）
* Toeplitz Matrix（テプリッツ行列）

### Others

* Sparse Matrix（疎行列）
* Kronecker Matrix（クロネッカー行列）

You can generate these matrices, define them by overloading the indexer, and add, subtract, and multiply them easily.

Also, you can perform operations using the LAPACK routine. Linear Algebra RS supports POTRF and POTRS as well as several other LAPACK routines.

For example, POTRF is a Triangular Factorization of a Positive Definite Matrix, which means Cholesky Decomposition, an LU decomposition specializing in symmetric matrices.

These will allow you to perform the calculations necessary for data science faster.
