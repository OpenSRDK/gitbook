---
description: >-
  Library for Bayesian modeling that incorporates deep learning kernel Gaussian
  processes.
---

# Probability RS

{% hint style="info" %}
**GitHub:** [**https://github.com/OpenSRDK/probability-rs**](https://github.com/OpenSRDK/probability-rs)
{% endhint %}

Probability RS provides a library of probability distributions. Therefore, Probability RS has the most important role in machine learning.

The features of Probability RS will be explained separately for Bayesian modeling and Gaussian processes.

## Modeling with Bayesian inference

### Advantages

Bayesian inference has advantages over current methods using deep neural networks in that it predicts uncertainty.

Also, The use of Bayesian modeling also makes it possible to use a unified approach to any modeling using any probability distribution.

Therefore, once the combination of likelihood and prior distribution has been modeled, it is possible to reduce it to a unified method where all that is left is to estimate the posterior distribution.

Existing machine learning methods for deep neural networks require separate optimization for different models, such as least squares and support vector machines. On the other hand, using Bayesian modeling eliminates the need for these optimizations and saves time.

## Deep Learning with Gaussian processes

### Theory

First, Probability RS is developed for Bayesian modeling using a Gaussian process with a deep learning kernel.

In the first place, the Gaussian process can be expressed as the limit of an infinite number of neural network units with only one layer of nonlinear transformation. And, the theory can also be extended to a general L-layer model.

In addition, the discovery of a kernel function for Gaussian processes corresponding to deep neural networks (Lee et al., 2018.) has made it possible to use them for Bayesian prediction in deep learning.

### Advantages

The usefulness of representing deep learning as a covariance function and interpreting it as a Gaussian process is as follows

* No overlearning occurs.
* It shows the uncertainty of prediction.
* Covariance functions can be automatically optimized and selected.

Bayesian optimization, which uses a Gaussian process to adjust the super-parameters of existing deep learning, is currently in vogue.

However, it would be faster to use a Gaussian process for deep learning itself.

## Available Probability  Distributions

### Continuous  Probability Distributions

* Beta  distribution
* Gamma distribution
* Exponential distribution
* Elliptical distribution（Normal distribution, **** Cauchy distribution, Student's _t_-distribution）
* F-Distribution (Fisher-Snedecor distribution)
* Continuous uniform distribution

### Discrete Probability Distributions

* Bernoulli distribution
* Categorical distribution (generalized Bernoulli distribution)
* Binomial distribution
* Multinomial distribution (generalized Binomial distribution)
* Geometric distribution
* Poisson distribution
* Discrete uniform distribution

## Available Sampling Algorithm

### Markov Chain Monte Carlo Methods (MCMC)

* Metropolis-Hastings algorithm
* Slice sampling
* Importance sampling

## onparametric method

### Elliptical Process

the elliptical processes -- a family of non-parametric probabilistic models that subsumes the Gaussian process and the Student-t process

* Exact Gaussian Process (,Cauchy process and Student's _t_-process )
* Sparse Gaussian Process (,Cauchy process and Student's _t_-process )
* Gaussian Process Regressor (and Cauchy Process Regressor)
* KISS-GP (Kernel interpolation for scalable structured Gaussian process) and LOVE (LanczOs Variance Estimates)

### Point Process

#### Dirichlet Process

* Stick-Breaking process
* Pitman-Yor process(generalized Chinese restaurant process)
