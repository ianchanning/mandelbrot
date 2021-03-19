# Concurrency in Rust - Mandelbrot set

An introduction to Rust Concurrency using the Mandelbrot set.

Taken from the O'Reilly "Programming Rust" book.

### [Slides](./slides.pdf)

```rust
let mut z = c;
for i in 0..limit {
    z = z * z;
}
```

![unit-circle](./unit-circle.png)

```rust
let mut z = Complex { re: 0.0, im: 0.0 };
for i in 0..limit {
    z = z * z + c;
}
```

![mandelbrot](./mandel.png)
