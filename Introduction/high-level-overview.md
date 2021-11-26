# High-level Overview

## What is Open SRDK?

OpenSRDK (Open Science Research and Development Kit) is a Rust library for data science.

The goal of the Open SRDK is to socially implement Bayesian modeling that incorporates deep learning kernel Gaussian processes. This will create a new future.

Also on the roadmap is the creation of methods that will be easier to implement with this libraries, such as combining world model reinforcement learning with principal component analysis using deep learning kernel Gaussian process latent variable models.

### SRDK Packages

The following Rust packages are currently published in cargo.

{% content-ref url="packages/linear-algebra-rs.md" %}
[linear-algebra-rs.md](../packages/linear-algebra-rs.md)
{% endcontent-ref %}

{% content-ref url="packages/kernel-method-rs.md" %}
[kernel-method-rs.md](../packages/kernel-method-rs.md)
{% endcontent-ref %}

{% content-ref url="packages/probability-rs.md" %}
[probability-rs.md](../packages/probability-rs.md)
{% endcontent-ref %}

{% hint style="info" %}
**How to Install:**

toml:\*\* \*\*Cargo.toml

```
[dependencies]
opensrdk-linear-algebra = "0.8.1"
blas-src = { version = "0.8", features = ["openblas"] }
lapack-src = { version = "0.8", features = ["openblas"] }
```

Next, do `extern crate` in `main.rs` (or `lib.rs`). It is the same as any other library.
{% endhint %}

{% hint style="info" %}
**BLAS Libraries**

In `cargo.toml`, edited&#x20;

> `features = ["openblas"]`

`but, you can change other libraries supported by`[blas-src](https://github.com/blas-lapack-rs/blas-src).

- `accelarate`
- `blis`
- `intel-mkl`
- `netlib`

When you use x86 CPUs(Intel Core, AMD Ryzen, etc.), you can use Intel-MKL and run faster than OpenBLAS.

Note that OpenBLAS and Intel-MKL requires a dependencies.

On the other hand, if you're using an M1 Mac, you can't use OpenBLAS or Intel-MKL, so Accelerate is your only option. Accelerate is developed by Apple and you can use it on macOS or other Apple's OS.
{% endhint %}

### Fundamentals: Dive a little deeper

Learn the fundamentals of MyProduct to get a deeper understanding of our main features:

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

{% hint style="info" %}
**Good to know:** Splitting your product into fundamental concepts, objects, or areas can be a great way to let readers deep dive into the concepts that matter most to them. Combine guides with this approach to 'fundamentals' and you're well on your way to great documentation!
{% endhint %}
