# Rust for Python Developers — Recommended Resources

This page contains a curated list of resources for Python and web developers who want to learn Rust.

The goal is not to collect hundreds of links.

The goal is to follow a practical path:

1. Understand what Python hides from you
2. Learn the Rust mental model
3. Practice ownership and borrowing
4. Build small projects
5. Move toward production-level Rust

---

## 1. Start Here: Official Rust Resources

### The Rust Programming Language Book

Best for learning Rust from first principles.

Link: https://doc.rust-lang.org/book/

Recommended chapters:

- Getting Started
- Common Programming Concepts
- Understanding Ownership
- Structs
- Enums and Pattern Matching
- Error Handling
- Generic Types, Traits, and Lifetimes
- Smart Pointers
- Fearless Concurrency

Why this is useful for Python developers:

Python hides memory ownership, references, and many runtime details. The Rust Book helps you understand why Rust asks you to think about ownership, borrowing, and lifetimes.

---

### Rust by Example

Best for learning through small runnable examples.

Link: https://doc.rust-lang.org/rust-by-example/

Use this when you want to see Rust concepts in code quickly.

Good topics to practice:

- structs
- enums
- match
- error handling
- traits
- generics
- lifetimes
- modules
- standard library examples

---

### Rustlings

Best for hands-on beginner exercises.

Link: https://github.com/rust-lang/rustlings

Rustlings gives you small exercises where you fix code and learn by reading compiler messages.

This is very useful because Rust beginners often learn a lot from compiler errors.

Recommended usage:

Read one chapter from the Rust Book, then solve related Rustlings exercises.

---

## 2. Python-to-Rust Mental Model

If you come from Python, do not learn Rust as “Python with different syntax.”

Rust has a different mental model.

Important differences:

| Concept | Python | Rust |
|---|---|---|
| Memory management | Automatic | Ownership and borrowing |
| Type checking | Runtime / optional type hints | Compile-time |
| Errors | Exceptions | Result<T, E> |
| Null values | None | Option<T> |
| Data modeling | Classes, dicts | Structs, enums |
| Shared behavior | Duck typing / ABCs | Traits |
| Mutation | Flexible | Controlled |
| Performance | Runtime overhead | Systems-level performance |

Questions Rust asks you to think about:

- Who owns this value?
- Is this value borrowed or moved?
- Can this value be mutated?
- How long does this reference live?
- What happens if this operation fails?
- Can this code run safely across threads?

---

## 3. Memory Concepts to Learn

Before Rust ownership fully makes sense, learn these concepts:

- CPU
- RAM
- stack
- heap
- pointer
- reference
- allocation
- deallocation
- copy
- move
- mutable state
- shared state
- process
- thread

You do not need to become a C or operating systems expert first.

But you should understand the basic idea that memory must be allocated, used, and freed safely.

Python does most of this automatically.

Rust makes these rules visible and checks many of them at compile time.

---

## 4. Ownership and Borrowing Resources

Focus heavily on these topics:

- ownership
- borrowing
- mutable borrowing
- move semantics
- references
- lifetimes
- clone vs copy
- stack vs heap
- String vs &str
- Vec<T>
- Option<T>
- Result<T, E>

Suggested learning order:

1. Learn `String` and `&str`
2. Learn move vs copy
3. Learn function parameters with ownership
4. Learn immutable borrowing
5. Learn mutable borrowing
6. Learn basic lifetimes
7. Learn structs with owned and borrowed fields

---

## 5. Structs, Enums, Traits, and OOP Comparison

Rust does not use classes like Python.

Instead, Rust commonly uses:

- `struct` for data
- `impl` for behavior
- `enum` for variants
- `trait` for shared behavior
- `match` for pattern matching

Python example:

```python
class Dog:
    def speak(self):
        return "woof"