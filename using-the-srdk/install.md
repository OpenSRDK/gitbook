# Install

## How to use in Rust

The following Rust packages are currently published in cargo.

{% hint style="info" %}
Learn more about Cargo, see [why-use-rust.md](../introductions/why-use-rust.md "mention").
{% endhint %}

Linear Algebra RS

{% content-ref url="packages/linear-algebra-rs.md" %}
[linear-algebra-rs.md](packages/linear-algebra-rs.md)
{% endcontent-ref %}

Kernel Method RS

{% content-ref url="packages/kernel-method-rs.md" %}
[kernel-method-rs.md](packages/kernel-method-rs.md)
{% endcontent-ref %}

Probability RS

{% content-ref url="packages/probability-rs.md" %}
[probability-rs.md](packages/probability-rs.md)
{% endcontent-ref %}

Edit your `cargo.toml`.

For Example, how to install opensrdk-linear-algebra 0.8.1.

toml:\*\* \*\*Cargo.toml

```
[dependencies]
opensrdk-linear-algebra = "0.8.1"
blas-src = { version = "0.8", features = ["openblas"] }
lapack-src = { version = "0.8", features = ["openblas"] }
```

Next, do `extern crate` in `main.rs` (or `lib.rs`). It is the same as any other library.

{% hint style="info" %}
**BLAS Libraries**

In `cargo.toml`, edited

> `features = ["openblas"]`

`but, you can change other libraries supported by`[blas-src](https://github.com/blas-lapack-rs/blas-src).

* `accelarate`
* `blis`
* `intel-mkl`
* `netlib`

When you use x86 CPUs(Intel Core, AMD Ryzen, etc.), you can use Intel-MKL and run faster than OpenBLAS.

Note that OpenBLAS and Intel-MKL requires a dependencies.

On the other hand, if you're using an M1 Mac, you can't use OpenBLAS or Intel-MKL, so Accelerate is your only option. Accelerate is developed by Apple and you can use it on macOS or other Apple's OS.
{% endhint %}
