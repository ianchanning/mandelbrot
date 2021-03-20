# Concurrency in Rust - Mandelbrot set

An introduction to Rust Concurrency using the Mandelbrot set.

Taken from the O'Reilly "Programming Rust" book.

Read the [Slides](./slides.pdf), then compare [`main.rs`](./src/main.rs), [`main-bands.rs`](./src/main-bands.rs) and [`main-task-queue.rs`](./src/main-task-queue.rs).

The code for the concurreny algoithms is from <https://github.com/ProgrammingRust/mandelbrot>.

The main contribution beyond the book is to compare the output of the simpler `z = z * z` vs `z = z * z + c`.

### Unit Circle Set
```rust
let mut z = c;
for i in 0..limit {
    z = z * z;
}
```
![unit-circle](./unit-circle.png)

### Mandelbrot Set
```rust
let mut z = Complex { re: 0.0, im: 0.0 };
for i in 0..limit {
    z = z * z + c;
}
```
![mandelbrot](./mandel.png)
