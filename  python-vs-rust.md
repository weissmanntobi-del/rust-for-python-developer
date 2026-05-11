# Python vs Rust Mental Model

| Concept           | Python                       | Rust                       |
|-------------------|------------------------------|----------------------------|
| Memory management | Automatic garbage collection | Ownership and borrowing    |
| Type system       | Dynamic                      | Static                     |
| Errors            | Exceptions                   | Result<T, E>               |
| Null values       | None                         | Option<T>                  |
| Classes           | Common                       | Not class-based            |
| Interfaces        | Duck typing / ABCs           | Traits                     |
| Mutation          | Flexible                     | Controlled                 |
| Performance       | Slower runtime               | Systems-level performance  |
| Concurrency       | Limited by GIL in many cases | Strong compile-time safety |

Rust is not just Python with different syntax.

Rust requires a different mental model.

In Python, you often think:

"Can I make this work?"

In Rust, you also think:

"Who owns this value?"
"Can this value be changed?"
"How long does this reference live?"
"Can this fail?"
"Is this safe across threads?"