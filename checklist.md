# Rust for Python Developers

A practical learning roadmap for Python and web developers who want to understand Rust, ownership, borrowing, memory, structs, enums, traits, and systems programming fundamentals.

If you come from Python, JavaScript, TypeScript, or web development, Rust can feel strange at first.

You may understand the syntax, but still struggle to internalize:

- ownership
- borrowing
- lifetimes
- stack vs heap
- copying vs moving
- structs and enums
- traits
- `Option<T>` and `Result<T, E>`
- how Rust is different from Python

This repository is designed to help you build the right mental model step by step.

---

## Who This Is For

This roadmap is for you if:

- You know Python and want to learn Rust
- You come from web development and want to understand lower-level programming
- You have tried Rust but ownership and borrowing did not fully click
- You want to understand memory, processes, stack, heap, and references
- You want to compare Rust concepts with Python or TypeScript
- You want to build small practical Rust projects

---

## Why Rust Feels Difficult for Python Developers

Python hides many low-level details from you.

In Python, you usually do not think deeply about:

- who owns memory
- when memory is freed
- whether a value is copied or referenced
- whether two parts of your program are mutating the same data
- how long a reference is valid

Rust makes these rules explicit.

That can feel difficult in the beginning, but it is also what makes Rust powerful.

Rust teaches you to ask:

- Who owns this value?
- Is this value borrowed or moved?
- Can this value be changed?
- How long does this reference live?
- What happens if this operation fails?

---

## Recommended Learning Checklist

Use this checklist if you are coming from Python and want to learn Rust step by step.

The goal is not just to learn Rust syntax.

The goal is to understand the Rust mental model:

- memory
- ownership
- borrowing
- structs
- enums
- traits
- error handling
- small practical projects

---

## Phase 1: Memory Basics

Before Rust ownership fully makes sense, you should understand basic memory concepts.

- [ ] Understand what RAM is
- [ ] Understand what the stack is
- [ ] Understand what the heap is
- [ ] Understand stack vs heap
- [ ] Understand values vs references
- [ ] Understand pointers at a basic level
- [ ] Understand copying vs moving
- [ ] Understand allocation and deallocation

---

## Phase 2: Rust Ownership

Ownership is one of the most important Rust concepts.

- [ ] Understand that every value has one owner
- [ ] Understand what happens when a value is moved
- [ ] Understand why some types are copied and some are moved
- [ ] Understand `String` vs `&str`
- [ ] Understand ownership in function parameters
- [ ] Understand ownership in function return values
- [ ] Understand when to use `.clone()`

---

## Phase 3: Borrowing

Borrowing allows you to use a value without taking ownership.

- [ ] Understand immutable borrowing
- [ ] Understand mutable borrowing
- [ ] Understand the rule: many immutable references or one mutable reference
- [ ] Understand why Rust prevents data races
- [ ] Understand references with `&`
- [ ] Understand mutable references with `&mut`
- [ ] Understand lifetimes at a basic level

---

## Phase 4: Rust Data Modeling

Rust does not use classes like Python.

Instead, Rust commonly uses structs, enums, traits, and pattern matching.

- [ ] Understand structs
- [ ] Understand `impl` blocks
- [ ] Understand enums
- [ ] Understand pattern matching with `match`
- [ ] Understand traits
- [ ] Understand how traits compare to Python interfaces or duck typing
- [ ] Understand when to use structs
- [ ] Understand when to use enums
- [ ] Understand when to use traits

---

## Phase 5: Error Handling

Rust handles errors differently from Python.

Python often uses exceptions.

Rust commonly uses `Option<T>` and `Result<T, E>`.

- [ ] Understand `Option<T>`
- [ ] Understand `Some`
- [ ] Understand `None`
- [ ] Understand `Result<T, E>`
- [ ] Understand `Ok`
- [ ] Understand `Err`
- [ ] Understand the `?` operator
- [ ] Understand basic custom error handling

---

## Phase 6: Practice Projects

Do not only read Rust.

Build small projects.

- [ ] Build a CLI calculator
- [ ] Build a file word counter
- [ ] Build a command-line todo app
- [ ] Build a file parser
- [ ] Build a CSV reader
- [ ] Build a JSON reader using `serde`
- [ ] Build a small HTTP API
- [ ] Build a project using structs, enums, traits, and error handling

---

## Phase 7: Final Confidence Check

You are becoming comfortable with Rust when you can explain:

- [ ] Why ownership exists
- [ ] Why borrowing exists
- [ ] Why Rust does not need a garbage collector
- [ ] Why Rust prevents many memory bugs at compile time
- [ ] How structs and enums replace many class-based patterns
- [ ] How traits provide shared behavior
- [ ] How `Option<T>` replaces many null-style patterns
- [ ] How `Result<T, E>` replaces many exception-style patterns

---

## Suggested Next Step

After finishing this checklist, build one complete small project.

Good project idea:

> A command-line log file analyzer that reads a file, parses lines, counts errors, groups results, and prints a summary.

This project will help you practice:

- file handling
- strings
- vectors
- structs
- enums
- error handling
- ownership
- borrowing

---

## Additional Resource

This repository is free.

I also created a paid Rust for Python Developers Bundle for people who want a more structured learning path.

It is designed for Python and web developers who want to understand Rust step by step, especially:

- ownership
- borrowing
- memory basics
- structs
- enums
- traits
- error handling
- Rust mental models
- practical beginner projects

You can find it here:

https://tobiweissmann.gumroad.com/l/wcylm

You do not need to buy the bundle to use this free roadmap.