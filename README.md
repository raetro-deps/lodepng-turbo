# lodepng-turbo
lodepng-turbo is a PNG image codec that uses SIMD instructions (MMX, SSE2, AVX2, NEON) to accelerate baseline PNG decompression on x86, x86-64, ARM systems.

## Background
lodepng-turbo is a PNG image codec that uses SIMD instructions (MMX, SSE2, AVX2, NEON) 
to accelerate baseline PNG decompression on x86, x86-64, ARM systems. 
On x86 and x86-64 or ARM systems, lodepng-turbo is twice as fast as libpng, but it may be slower elsewhere. 
With lodepng-turbo, its highly optimized libdeflate and depng prediction routines perform significantly better than lodepng(origin) and libpng.

lodepng-turbo implements both the traditional lodepng API and the less powerful but more direct TurboPNG API.

## How to build

Build lodepng-turbo with gcc/clang and GNU make.

```shell
$ make
```
## Acknowledgments

lodepng is a very easy-to-understand png library, which is the foundation of this library.

libdeflate is a very fast zlib compatible codec, and substantial decode processing is realized with this library.

SimdTests is a public domain to test SIMD optimized functions related mostly to 2D computer graphics.

## License

zlib

## Copyright

Copyright 2019 KATO Kanryu <k.kanryu@gmail.com>
