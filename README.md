# Ray Tracer

This project uses the Rust programming language to explore the world of Ray
Tracing -- a rendering strategy that simulates individual rays of light to
produce photo-realistic pictures.

Currently the renderer runs on the CPU and thus takes a relatively long time to
render the example scene (~8 minutes, using all 12 cores of my machine). The
image is written to stdout in the PPM image format.

## Getting Started

To render the example scene, run:

```
cargo run --release > image.ppm
```

The image can be viewed with a compatible image viewer. The standard "Preview"
app on macOS is one example:

```
open image.ppm
```

## Attribution

The code of this project is based on the book "Ray Tracing in One Weekend" by
Peter Shirley, Trevor David Black and Steve Hollasch. It can be found
[here](https://raytracing.github.io/). The book provides an implementaiton in
C++, which was ported to Rust by Sheng Chou. His modified version of the book
can be found [here](https://the-ray-tracing-road-to-rust.vercel.app/).
