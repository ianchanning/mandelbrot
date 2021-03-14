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

Fearless concurrency.

# The Mandelbrot set

Complex number $z$

$$
\begin{aligned}
z &= a+bi \\
\end{aligned}
$$

Iterate $z$ from 0, square it and add another complex number $c$

$$
\begin{aligned}
z_0 &= 0 \\
z_{n+1} &= z_n^2+c \\
\end{aligned}
$$

For some values of $c$, $z$ will stay within a distance of 2 from the origin

Those are 'in' the Mandelbrot Set

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

# Fearless concurrency
