# Why use Rust?

## Why develop OpenSRDK in Rust?

First, Rust is superior to Python and other languages in terms of processing performance.

The reason why the Python ecosystem has been able to develop without any performance problems is that the actual linear algebra is left to other routines.
For example, numpy calls OpenBLAS routine.

In Python, tensor calculations are done by GPUs. Python does not do any tensor calculations in the Python for loop.

However, in OpenSRDK design, the responsibility of the processing before throwing everything at the GPU increases more than with conventional methods.

To avoid degradation of processing performance in this area, OpenSRDK uses Rust.
The design philosophy of OpenSRDK is discussed in another section.

## About Rust

In an yearly survey conducted by Stack Overflow between 2016 and 2020, Rust was voted "the programming language developers love the most". Technology leaders are willing to adopt Rust.

For example, Rust is used in Google's Android development, for example in the Bluetooth module. And, Facebook uses Rust to drive its web, mobile, and API services.

Rust has a high enough productivity.

## Features of RUST

One of the features of Rust is that unauthorized data access can be prevented at compile time.
Therefore, Rust provides a guarantee that the program will be memory safe without increasing the runtime cost of the program.

Rust also has some other advantages over other languages, which can be roughly summarized as follows

- Processing performance
- Parallelism
- Memory efficiency

### Processing performance

Rust provides all the performance available in a computer.

Cache-friendly data structures are provided by default, usually using arrays to store data rather than deeply nested tree structures with pointers.

A modern package manager (cargo) is provided. This makes it easy to use many open source packages. This makes it easy to build large projects with many dependencies.

Also, methods are usually statically dispatched. This allows the compiler to aggressively optimize the code, sometimes to the point of removing the cost of function calls altogether.

### Parallelism

It is said that it is difficult for a software engineer to make a single computer "do multiple jobs simultaneously". Two independent threads of execution on a single computer can be unwieldy and sometimes lead to serious errors.

However, Rust allows you to easily create programs with concurrency. By taking advantage of ownership and type checking, many concurrency errors become compile-time errors instead of run-time errors.

### Memory efficiency

It is easy to create programs with minimal memory requirements.

You can use fixed-length structures when needed, and you know how individual bytes will be managed. Higher-level structures such as iterations and generic types also have minimal runtime overhead.
