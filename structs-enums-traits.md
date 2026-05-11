# Structs, Enums, and Traits

## Are Rust Structs and Enums an Alternative to OOP?

Partly, yes.

Rust does not use classes like Python or TypeScript.

Instead, Rust commonly uses:

- structs for data
- impl blocks for behavior
- enums for variants
- traits for shared behavior

## Python Class Example

```python
class User:
    def __init__(self, name):
        self.name = name

    def greet(self):
        print(f"Hello, {self.name}")
```

## Rust Struct + Impl Example

    struct User {
      name: String,
    }
    
    impl User {
        fn greet(&self) {
        println!("Hello, {}", self.name);
        }
    }
## Traits Instead of Interfaces
    
    trait Speak {
       fn speak(&self);
    }