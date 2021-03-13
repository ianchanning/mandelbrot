% Rust Concurrency - Generating the Mandelbrot Set
% Ian Channing <https://github.com/ianchanning/mandelbrot>
% March 10, 2021

# Taken from the Rust Book

Based on the Concurrency section of Chapter 2 (A Tour of Rust)

from the O'Reilly "Programming Rust" book.

# Introduction

The Mandelbrot set.

Complex numbers and iterating complex numbers.

Generating the Mandelbrot set with one processor.

The required changes to use multiple processors.

# The Mandelbrot set

$z=a+bi$

$z=z^2+c$

# Complex numbers and iterating complex numbers

Addition

$(a+bi)+(c+di)=(a+c)+(b+d)i$

Multiplication

$$
\begin{aligned}
(a+bi)\times(c+di) &= ac+(ad+bc)i+bdi^2 \\
& = (ac-bd)+(ad+bc)i \\
\end{aligned}
$$

# Generating the Mandelbrot set with one processor

# The required changes to use multiple processors
