---
description: Library for kernel methods
---

# Kernel Method RS

{% hint style="info" %}
**GitHub:** [**https://github.com/OpenSRDK/kernel-method-rs**](https://github.com/OpenSRDK/kernel-method-rs)
{% endhint %}

Kernel Method RS provides a library of kernel method. This is used in combination with Probability RS.

The Kernel Method RS maps data onto a high-dimensional feature space to find and study the structure of the data.

## What is the kernel method?

The kernel method is one of the methods used in pattern recognition, and it is used in combination with algorithms such as discrimination. A well-known method is to use it in combination with a support vector machine, which is one of the pattern recognition models that use supervised learning.

Pattern recognition is generally used to find and study the structure of data (e.g. clusters, rankings, principal components, correlations, classifications). For this reason, the kernel method maps the data onto a higher dimensional feature space.

A wide variety of mappings can be used as feature maps (generally nonlinear mappings), and correspondingly, a wide variety of data structures can be found.

## Kernel Function

The name "kernel method" comes from the use of kernel functions. Kernel functions provide a means of computing the inner product in feature space directly from the data, without going through the explicit computation of the coordinates of the data in feature space.

The advantage of using kernel functions to evaluate the inner product is that it is less computationally intensive than going through explicit coordinate calculations.

The following kernel functions are supported by Kernel Method RS.

### Supported Kernel Functions

* Linear Kernel（線形カーネル）
* Constant Kernel（定数カーネル）
* Exponential Kernel（指数カーネル）
* Periodic Kernel（周期カーネル）
* ARD Kernel (Automatic Relevance Determination Kernel)
* RBF Kernel (Radial Basis Function Kernel)
* Spectral Mixture Kernel (invented and discussed in Wilson et al., 2013.)

When the matrix created by these kernel functions is a positive definite matrix, its kernel function has the following properties.

* A linear combination of kernel functions is a kernel function.
* The product of two kernel functions is a kernel function.

Kernel Method RS uses these properties and Rust's operator overloading to make it easy to create a kernel function that is a linear combination of the different kernel functions described above.
