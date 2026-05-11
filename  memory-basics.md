
# Memory Basics Before Learning Rust

To understand Rust, you should understand these ideas:

## Stack

The stack stores simple values with known size.

Examples:

- integers
- booleans
- small fixed-size data

## Heap

The heap stores data that can grow or has unknown size at compile time.

Examples:

- String
- Vec
- dynamic data

## Why This Matters

Rust ownership becomes easier when you understand that memory must be allocated, used, and freed safely.

Python handles this automatically.

Rust makes this explicit and checks it at compile time.