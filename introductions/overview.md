# Overview

## What is Open SRDK?

OpenSRDK (Open Science Research and Development Kit) is a Rust library for data science.

The goal of the Open SRDK is to socially implement Bayesian modeling that incorporates deep learning kernel Gaussian processes. This will create a new future.

Also on the roadmap is the creation of methods that will be easier to implement with this libraries, such as combining world model reinforcement learning with principal component analysis using deep learning kernel Gaussian process latent variable models.

## SRDK Packages

OpenSRDK consists of the following three packages.&#x20;

The most important library for machine learning is Probability RS, and the other two are the libraries needed to use it.

* Linear Algebra RS
* Kernel Method RS
* Probability RS

{% hint style="info" %}
[install.md](../using-the-srdk/install.md "mention") is required to use these.
{% endhint %}

### Linear Algebra RS

{% content-ref url="../packages/linear-algebra-rs.md" %}
[linear-algebra-rs.md](../packages/linear-algebra-rs.md)
{% endcontent-ref %}

This is a library of linear algebra. Since linear algebra is an integral part of data science, it is responsible for that part.

### Kernel Method RS

{% content-ref url="../packages/kernel-method-rs.md" %}
[kernel-method-rs.md](../packages/kernel-method-rs.md)
{% endcontent-ref %}

This is a library of kernel method. It has no value on its own. It is more valuable when used in combination with Probability RS.

### Probability RS

{% content-ref url="../packages/probability-rs.md" %}
[probability-rs.md](../packages/probability-rs.md)
{% endcontent-ref %}

Probability RS is most important library in OpenSRDK. This is a library of probability distribution.&#x20;
