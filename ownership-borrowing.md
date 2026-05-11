# Ownership and Borrowing for Python Developers

## Python Example

```python
name = "Alice"
another_name = name
print(name)
print(another_name)
```

## Rust Example
let name = String::from("Alice");
let another_name = name;

// println!("{}", name); // this will not compile
In Rust, name was moved to another_name.

This prevents unsafe memory usage.

## Simple Rule

Rust asks:

Who owns this value?

There can be one owner at a time.

## Borrowing 

fn print_name(name: &String) {
println!("{}", name);
}

