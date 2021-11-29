# Install

## How to use in Rust

The following Rust packages are currently published in cargo.

{% hint style="info" %}
**[What is cargo](../introductions/why-use-rust.md)**
{% endhint %}

{% content-ref url="packages/linear-algebra-rs.md" %}
[linear-algebra-rs.md](../packages/linear-algebra-rs.md)
{% endcontent-ref %}

{% content-ref url="packages/kernel-method-rs.md" %}
[kernel-method-rs.md](../packages/kernel-method-rs.md)
{% endcontent-ref %}

{% content-ref url="packages/probability-rs.md" %}
[probability-rs.md](../packages/probability-rs.md)
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
