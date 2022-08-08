# bits-util

A utility library to operate bits for [Zig](https://ziglang.org/).

## Synopsis

```Zig
// rotate 2 bits to left for u8 bits
try testing.expect(rotateLeft8(0b00001111, 2) == 0b00111100);
// rotate 2 bits to right for u8 bits
try testing.expect(rotateLeft8(0b00001111, -2) == 0b11000011);

// Also `rotateLeft16`, `rotateLeft32`, and `rotateLeft64` work as well.
```

## Notes

This code is based on the Golang's `math/bits` implementation: https://cs.opensource.google/go/go/+/refs/tags/go1.19:src/math/bits/bits.go

